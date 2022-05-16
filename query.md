/\* \* Copyright (c) Facebook, Inc. and its affiliates. \* \* Licensed
under the Apache License, Version 2.0 (the \"License\"); \* you may not
use this file except in compliance with the License. \* You may obtain a
copy of the License at \* \* http://www.apache.org/licenses/LICENSE-2.0
\* \* Unless required by applicable law or agreed to in writing,
software \* distributed under the License is distributed on an \"AS IS\"
BASIS, \* WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
or implied. \* See the License for the specific language governing
permissions and \* limitations under the License. \*/ {namespace
buck.query} /\*\* \* \@param anchor \* \@param title \*/ {template
.section}

#### {\$title} {#{$anchor}}

{/template} /\*\*\*/ {template .soyweb} {call buck.page} {param title:
\'buck query\' /} {param navid: \'command_query\' /} {param prettify:
true /} {param description} Provide facilities to query information
about the target-nodes graph. {/param} {param content} {call
buck.command} {param overview}

The `buck query` command provides functionality to query the
*target-nodes* graph (\"target graph\") and return the build targets
that satisfy the query expression.

The query language enables you to combine multiple operators in a single
command. For example, to retrieve a list of all the tests for a build
target, you can combine the `deps()` and `testsof()` operators into a
single call to `buck query`.

    {literal}
    buck query "testsof(deps('//java/com/example/app:amazing'))"
    {/literal}

## Query Language

The Buck query language was inspired by the [Bazel Query
Language](http://bazel.io/docs/query.html). Buck\'s query language uses
the same parser, so the lexical syntax is similar. Buck\'s query
language supports a *subset* of Bazel\'s query functionality but also
adds a few operators, such as `attrfilter`, `inputs`, and `owner`.

### Operators

Buck\'s query language supports the following operators. The name of the
operator below is linked to a section that provides more detail about
that operator\'s functionality and syntax.

-   [`allpaths`](#allpaths): All dependency paths
-   [`attrfilter`](#attrfilter): Rule attribute filtering
-   [`attrregexfilter`](#attrregexfilter): Rule attribute filtering with
    regex
-   [`buildfile`](#buildfile): Build files of targets
-   [`deps and first-order-deps`](#deps): Transitive closure of
    dependencies
-   [`except`](#set-operations): Set difference
-   [`filter`](#filter): Filter targets by name
-   [`inputs`](#inputs): Direct input files
-   [`intersect`](#set-operations): Set intersection
-   [`kind`](#kind): Filter targets by rule type
-   [`labels`](#labels): Extract content of rule attributes
-   [`owner`](#owner): Find targets that own specified files
-   [`rdeps`](#rdeps): Transitive closure of reverse dependencies
-   [`set`](#set): Group targets
-   [`testsof`](#testsof): List the tests of the specified targets
-   [`union`](#set-operations): Set union

### Parameters to operators

The most common parameter for a Buck query operator is an expression
that evaluates to a build target or collection of build targets. Such an
expression could be an explicit {call buck.build_target /}, a {call
buck.build_target_pattern /}, an {call buckconfig.alias /}, or *the set
of targets returned by another Buck query operator*.

**Tip:** You can pass an alias directly to the `buck query` command line
to see what it resolves to. For example:

    {literal}
    $ buck query app
    //apps/myapp:app
    {/literal}

#### Non-target parameters

In addition to target parameters, some Buck query operators take string
parameters such as filenames ([`owner()`](#owner)) or regular
expressions ([`filter()`](#filter)).

**Note:** You can hover over the parameters in the syntax blocks for the
query operators (later in this topic) to obtain short tool-tip
descriptions of the parameters.

#### Quoting of arguments

It is not necessary to quote arguments if they adhere to certain
conditions. That is, they comprise sequences of characters drawn from
the alphabet, numerals, forward slash (`/`), colon (`:`), period (`.`),
hyphen (`-`), underscore (`_`), or asterisk (`*`)---and they do not
start with a hyphen or period. For example, quoting `java_test` is
unnecessary.

All that said, we *do* recommend that you quote arguments as a best
practice even when Buck doesn\'t require it.

You should always use quotes when writing scripts that construct
`buck query` expressions *from user-supplied values*.

Note that argument quoting for `buck query` is in addition to any
quoting that your shell requires. In the following example,
double-quotes are used for the shell and single-quotes are used for the
`build target` expression.

    {literal}
    buck query "'//foo:bar=wiz'"
    {/literal}

{call .section} {param anchor: \'set-operations\' /} {param title:
\'Algebraic set operations: intersection, union, set difference\'/}
{/call}

  Nominal                         Symbolic
  -------------------------- ------------------
  `intersect`{.not-inline}    `^`{.not-inline}
  `union`{.not-inline}        `+`{.not-inline}
  `except`{.not-inline}       `-`{.not-inline}

These three operators compute the corresponding set operations over
their arguments. Each operator has two forms, a nominal form, such as
`intersect`, and a symbolic form, such as `^`. the two forms are
equivalent; the symbolic forms are just faster to type. For example,

    buck query "deps('//foo:bar') intersect deps('//baz:lib')"

and

    buck query "deps('//foo:bar') ^ deps('//baz:lib')"

both return the targets that appear in the {sp}[transitive
closure](https://en.wikipedia.org/wiki/Transitive_closure){sp} of
`//foo:bar` and `//baz:lib`.

The `intersect` (`^`) and `union` (`+`) operators are commutative. The
`except` (`-`) operator is not commutative.

The parser treats all three operators as left-associative and of equal
precedence, so we recommend that you use parentheses if you need to
ensure a specific order of evaluation. A parenthesized expression
resolves to the value of the expression it encloses. For example, the
first two expressions are equivalent, but the third is not:

    {literal}
    x intersect y union z
    (x intersect y) union z
    x intersect (y union z)
    {/literal}

{call .section} {param anchor: \'set\' /} {param title: \'Group targets:
set\'/} {/call}

**Syntax**

    {literal}
    set(a:expr b:expr c:expr ...)
    {/literal}

The `set(a b c ...)` operator computes the union of a set of zero or
more target expressions. Separate the targets with white space (not
commas). Quote the targets to ensure that they are parsed correctly.

If you want to invoke `buck query` on a list of targets, then `set()` is
a way to group this list in a query.

**Example:**

{call buckquery.example_multiple_targets /}

**Example:**

The following command line returns the merged set (union) of
dependencies for the targets: `main` and `subs` in the build file in the
root of the Buck project.

    {literal}
    buck query "deps( set( '//:main' '//:subs' ) )"
    {/literal}

{call .section} {param anchor: \'allpaths\' /} {param title: \'All
dependency paths: allpaths\'/} {/call}

**Syntax**

    {literal}
    allpaths(from:expr, to:expr)
    {/literal}

The `allpaths(from, to)` operator evaluates to the graph formed by paths
between the target expressions `from` and `to`, following the
dependencies between nodes. For example, the value of

    {literal}
    buck query "allpaths('//foo:bar', '//foo/bar/lib:baz')"
    {/literal}

is the dependency graph rooted at the single target node `//foo:bar`,
that includes all target nodes that depend on `//foo/bar/lib:baz`.

The two arguments to `allpaths()` can themselves be expressions. For
example, the command:

    {literal}
    buck query "allpaths(kind(java_library, '//...'), '//foo:bar')"
    {/literal}

shows all the paths between any `java_library` in the repository and the
target `//foo:bar`.

We recommend using `allpaths()` with the
`--output-format dot`{sp}parameter to generate a graphviz file that can
then be rendered as an image. For example:

``` {.prettyprint .lang-py}
{literal}
$ buck query "allpaths('//foo:bar', '//foo/bar/lib:baz')" --output-format dot --output-file result.dot
$ dot -Tpng result.dot -o image.png
{/literal}
```

*Graphviz* is an open-source graph-visualization software tool. Graphviz
uses the *dot* language to describe graphs.

{call .section} {param anchor: \'attrfilter\' /} {param title: \'Rule
attribute filtering: attrfilter\'/} {/call}

**Syntax**

    {literal}
    attrfilter(attribute, value, expr)
    {/literal}

The `attrfilter(attribute, value, expr)` operator evaluates the given
target expression and filters the resulting build targets to those where
the specified `attribute` contains the specified `value`.

In this context, the term `attribute` refers to an argument in a build
rule, such as `name`, `headers`, `srcs`, or `deps`.

If the attribute is a single value, say `name`, it is compared to the
specified `value`, and the target is returned if they match. If the
attribute is a list, the target is returned if that list contains the
specified `value`. If the attribute is a dictionary, the target is
returned if the `value` exists in either the keys or the values of the
dictionary.

For example,

    {literal}
    buck query "attrfilter(deps, '//foo:bar', '//...')"
    {/literal}

returns the build targets in the repository that depend on
`//foo:bar`---or more precisely: those build targets that include
`//foo:bar` in their `deps` argument list.

The match performed by `attrfilter()` is semantic rather than textual.
So, for example, if you have the following `deps` argument in your build
file:

    {literal}
    cxx_binary(
      name = 'main',
      srcs = [
        'main.cpp'
      ],
      deps = [
        ':myclass',
      ],
    )
    {/literal}

Your `attrfilter()` clause should be:

    {literal}
    buck query "attrfilter( deps, '//:myclass', '//...' )"
    {/literal}

Note the double forward slash (`//`) before the second argument to
`attrfilter()`.

{call .section} {param anchor: \'attrregexfilter\' /} {param title:
\'Rule attribute filtering with regex: attrregexfilter\'/} {/call}

**Syntax**

    {literal}
    attrregexfilter(attribute, pattern, expr)
    {/literal}

The `attrregexfilter(attribute, pattern, expr)` operator is identical to
the `attrfilter(attribute, value, expr)` operator except that it takes a
regular expression as the second argument. It evaluates the given target
expression and filters the resulting build targets to those where the
specified `attribute` matches the specified `pattern`.

In this context, the term `attribute` refers to an argument in a build
rule, such as `name`, `headers`, `srcs`, or `deps`.

If the attribute is a single value, say `name`, it is matched against
the specified `pattern`, and the target is returned if they match. If
the attribute is a list, the target is returned if that list contains a
value that matches the specified `pattern`. If the attribute is a
dictionary, the target is returned if the `pattern` match is found in
either the keys or the values of the dictionary.

{call .section} {param anchor: \'buildfile\' /} {param title: \'Build
files of targets: buildfile\'/} {/call}

**Syntax**

    {literal}
    buildfile(expr)
    {/literal}

The `buildfile(expr)` operator evaluates to those build files that
define the targets that result from the evaluation of the target
expression, `expr`.

{call buckquery.example_buildfile_owner /} {call .section} {param
anchor: \'deps\' /} {param title: \'Transitive closure of dependencies:
deps and first-order-deps\'/} {/call}

**Syntax**

    {literal}
    deps(argset:expr)
    deps(argset:expr, depth:int)
    deps(argset:expr, depth:int, filter:expr)
    deps(argset:expr, depth:int, first_order_deps())
    {/literal}

The `deps(x)` operator evaluates to the graph formed by the
{sp}[transitive
closure](https://en.wikipedia.org/wiki/Transitive_closure){sp} of the
dependencies of its argument set, *x*, including the nodes from the
argument set itself. For example, the value of

    {literal}
    buck query "deps('//foo:bar')"
    {/literal}

is the dependency graph rooted at the target node `//foo:bar`. It
includes all of the dependencies of `//foo:bar`. It also includes
`//foo:bar` itself.

The `deps` operator accepts an optional second argument, which is an
integer literal specifying an upper bound on the depth of the search.
So,

    {literal}
    deps('//foo:bar', 1)
    {/literal}

evaluates to the direct dependencies of the target `//foo:bar`, and

    {literal}
    deps('//foo:bar', 2)
    {/literal}

further includes the nodes directly reachable from the nodes in
`deps('//foo:bar', 1)`, and so on. If the depth parameter is omitted,
the search is unbounded, that is, it computes the entire transitive
closure of dependencies.

#### Filter expressions and first_order_deps()

The `deps()` operator also accepts an optional third argument, which is
a filter expression that is evaluated for each node and returns the
child nodes to recurse on when collecting transitive dependencies.

This filter expression can use the `first_order_deps()` operator which
returns a set that contains the first-order dependencies of the current
node---which is equivalent to `deps(<node>, 1)`. For example, the query,

    {literal}
    buck query "deps('//foo:bar', 1, first_order_deps())"
    {/literal}

is equivalent to

    {literal}
    buck query "deps('//foo:bar', 1)"
    {/literal}

The `first_order_deps()` operator can be used only as an argument passed
to `deps()`.

Note that because `deps()` uses positional parameters, you must specify
the second argument in order to specify the third. In this scenario, if
you want the search to be unbounded, we recommend that you use
`2147483647` which corresponds to Java\'s `Integer.MAX_VALUE`.

{call .section} {param anchor: \'filter\' /} {param title: \'Filter
targets by name: filter\'/} {/call}

**Syntax**

    {literal}
    filter(regex, expr)
    {/literal}

The `filter(regex, expr)` operator evaluates the specified target
expression, `expr`, and returns the targets that have a name attribute
that matches the specified regular expression `regex`. For example,

    {literal}
    buck query "filter('library', deps('//foo:bar'))"
    {/literal}

returns the targets in the transitive closure of `//foo:bar` that
contain the string {sp}`library` in their name attribute.

The `filter()` operator performs a *partial* match. So, both of the
following clauses would match a target with the name `main`.

    {literal}
    buck query "filter( 'main', '//...' )"
    {/literal}

    {literal}
    buck query "filter( 'mai', '//...' )"
    {/literal}

Another example:

    {literal}
    buck query "filter('.*\.java$', labels(srcs, '//foo:bar'))"
    {/literal}

returns the `java` files used to build {sp}`//foo:bar`.

You often need to quote the pattern to ensure that regular expressions,
such as `.*xpto`, are parsed correctly.

{call .section} {param anchor: \'inputs\' /} {param title: \'Direct
input files: inputs\'/} {/call}

**Syntax**

    {literal}
    inputs(expr)
    {/literal}

The `inputs(expr)` operator returns the files that are inputs to the
target expression, `expr`, ignoring all dependencies. Note that it does
not include any files required for parsing, such as the BUCK file.
Rather, it returns only the files required to actually run the build
after parsing has been performed.

Note also that `inputs()` returns only those input files indicated by
the *target graph*. Input files that are present in the *action graph*
but not in the target graph are not returned by `inputs()`.

You could consider the `inputs()` and `owner()` operators to be inverses
of each other.

{call .section} {param anchor: \'kind\' /} {param title: \'Filter
targets by rule type: kind\'/} {/call}

**Syntax**

    {literal}
    kind(regex, expr)
    {/literal}

The `kind(regex, expr)` operator evaluates the specified target
expression, `expr`, and returns the targets where the rule type matches
the specified `regex`. For example,

    {literal}
    buck query "kind('java_library', deps('//foo:bar'))"
    {/literal}

returns all `java_library` targets in the transitive dependencies of
`//foo:bar`.

The specified `pattern` can be a regular expression. For example,

    {literal}
    buck query "kind('.*_test', '//...')"
    {/literal}

returns all targets in the repository with a rule type that ends with
`_test`, such as `java_test` and `cxx_test`.

You often need to quote the pattern to ensure that regular expressions,
such as `.*xpto`, are parsed correctly.

To get a list of the available rule types in a given set of targets, you
could use a command such as the following:

    {literal}
    buck query : --output-attribute buck.type
    {/literal}

which prints all the rule types in the build file in the current
directory (`:`)---in JSON format. See `--output-attribute` described in
the **Parameters** section below for more information.

{call .section} {param anchor: \'labels\' /} {param title: \'Extract
content of rule attributes: labels\'/} {/call}

**Syntax**

    {literal}
    labels(attribute, expr)
    {/literal}

The `labels(attribute, expr)` operator returns the set of build targets
and file paths listed in the attribute specified by the `attribute`
parameter, in the targets that result from the evaluation of target
expression, `expr`. Valid values for *attribute* include `srcs`,
`headers`, and `deps`.

**Example**: Get all build targets and file paths specified in the
`srcs` attribute for *all the rules* in the build file in the current
directory.

    {literal}
    buck query "labels( 'srcs', ':' )"
    {/literal}

In performing this operation, Buck validates that any source files
referenced in these attributes do, in fact, exist; Buck generates an
error if they do not.

**Example**: Get all the build targets and file paths specified in the
`deps` arguments in the *tests of* the target `//foo:bar`.

    {literal}
    buck query "labels('deps', testsof('//foo:bar'))"
    {/literal}

Note that `deps` must be quoted because, in addition to being a
build-file attribute, it is itself a reserved keyword of the query
language.

{call .section} {param anchor: \'owner\' /} {param title: \'Find targets
that own specified files: owner\'/} {/call}

**Syntax**

    {literal}
    owner(inputfile)
    {/literal}

The `owner(inputfile)` operator returns the targets that own the
specified `inputfile`. In this context, *own* means that the target has
the specified file as an input. You could consider the `owner()` and
`inputs()` operators to be inverses of each other.

**Example**:

    {literal}
    buck query "owner('examples/1.txt')"
    {/literal}

returns the targets that owns the file `examples/1.txt`, which could be
a value such as `//examples:one`.

It is possible for the specified file to have multiple owners, in which
case, `owner()` returns a set of targets.

If no owner for the file is found, `owner()` outputs the message:

    {literal}
    No owner was found for <file>
    {/literal}

{call .section} {param anchor: \'rdeps\' /} {param title: \'Transitive
closure of reverse dependencies: rdeps\'/} {/call}

**Syntax**

    {literal}
    rdeps(universe:expr, argset:expr)
    rdeps(universe:expr, argset:expr, depth:int)
    {/literal}

The `rdeps(universe, argset)` operator returns the reverse dependencies
of the argument set `argset` within the {sp}[transitive
closure](https://en.wikipedia.org/wiki/Transitive_closure){sp} of the
set `universe` (the *universe*). The returned values include the nodes
from the argument set `argset` itself.

The `rdeps` operator accepts an optional third argument, which is an
integer literal specifying an upper bound on the depth of the search. A
value of one (`1`) specifies that `buck query` should return only direct
dependencies. If the `depth` parameter is omitted, the search is
unbounded.

**Example** {call buckquery.example_rdeps /} **Example**

The *universe:expr* parameter includes the *entire* transitive closure
of the target pattern specified. So some of these targets might be
outside the directory structure indicated by that target pattern. For
example, the result set of

    {literal}
    buck query "rdeps('//foo/bar/...', '//fuga:baz', 1)"
    {/literal}

might contain targets outside the directory structure beneath

    {literal}
    foo/bar/
    {/literal}

To say it another way, if a target in `//foo/bar/...` depends on, say,
`//hoge,` which in turn depends on {sp}`//fuga:baz,` *then `//hoge`
would show up in the result set*.

If you wanted to constrain the result set to only those targets beneath
{sp}`foo/bar`, you could use the [`intersect`](#set-operations)
operator:

    {literal}
    buck query "rdeps('//foo/bar/...', '//fuga:baz', 1) ^ '//foo/bar/...'"
    {/literal}

The caret (`^`) is a succinct synonym for `intersect`.

{call .section} {param anchor: \'testsof\' /} {param title: \'List the
tests of the specified targets: testsof\'/} {/call}

**Syntax**

    {literal}
    testsof(expr)
    {/literal}

The `testsof(expr)` operator returns the tests associated with the
targets specified by the target expression, `expr`. For example,

    {literal}
    buck query "testsof(set('//foo:bar' '//baz:app+lib')"
    {/literal}

returns the tests associated with `//foo:bar` and `//baz:app+lib`.

To obtain all the tests associated with the target and its dependencies,
you can combine the `testsof()` operator with the `deps()` operator. For
example,

    {literal}
    buck query "testsof(deps('//foo:bar'))"
    {/literal}

first finds the transitive closure of `//foo:bar`, and then lists all
the tests associated with the targets in this transitive closure.

## Executing multiple queries at once

Suppose you want to know the tests associated with a set of targets.
This can be done by combining the `testsof`, `deps` and `set` operators.
For example,

    {literal}
    buck query "testsof(deps(set('target1' 'target2' 'target3')))"
    {/literal}

Suppose you now want to know the tests for *each* of these targets; the
above command returns the union of the tests. Instead of executing one
query for the entire set of targets, `buck query` provides a way to
repeat a query with different targets using a single command. To do
this, first define the query expression format and then list the input
targets, separated by spaces. For example,

    {literal}
    buck query "testsof(deps( %s ))" target1 target2 target3
    {/literal}

The `%s` in the query expression is replaced by each of the listed
targets, and for each target, the resulting query expression is
evaluated. If you add the `--output-format json` parameter, the result
of the command is grouped by input target; otherwise, as in the previous
example using `set()`, the command merges the results and returns the
union of the queries.

This syntax is also useful for subcommands that take arguments that are
not targets, such as `owner()`. Recall that the `set()` operator works
only with targets, but the `owner()` operator takes a filename as its
argument.

    {literal}
    buck query "owner( %s )" main.cpp myclass.cpp myclass.h
    {/literal}

## Referencing Args Files

When running queries, arguments can be stored in external files, one
argument per line, and referenced with the `@` symbol. This is
convenient when the number of arguments is long or when you want to
persist the query input in source control.

    buck query "testsof(deps(%s))" @/path/to/args-file

If you want to include all the targets in the `@`-file in a single query
execution, you can use the following alternative syntax. Note the
addition of the capital \"`S`\" in \"`%Ss`\".

    buck query "testsof(deps(%Ss))" @/path/to/args-file

In the example above, the lines of the file are converted to a set and
substituted for the `%Ss`. In addition, each line\'s contents are singly
quoted. In the example above, if the args file contains the following:

    {literal}
    //foo:bar
    //foo:baz
    {/literal}

Then the query expression is equivalent to:

    {literal}
    buck query "testsof(deps(set('//foo:bar' '//foo:baz')))"
    {/literal}

If you use multiple `%Ss` operators in a single query, you can specify
which lines in the `@`-file should be used for each instance of `%Ss` in
the query expression: use `--` to separate elements that go in different
sets. For example:

    buck query "testsof(deps(%Ss)) union deps(%Ss)" @path/to/args-file

    {literal}
    //foo:foo
    --
    //bar:bar
    {/literal}

is equivalent to running the following:

    buck query "testsof(deps(set('//foo:foo'))) union deps(set('//bar:bar'))"

{/param} {param params} {call buck.param} {param name: \'output-format
dot\' /} {param desc}

Outputs the digraph representing the query results in [dot
format](https://en.wikipedia.org/wiki/DOT_(graph_description_language)#Directed_graphs).
The nodes will be colored according to their type. See
[graphviz.org](http://www.graphviz.org/doc/info/colors.html) for color
definitions.

``` {.prettyprint .lang-py}
{literal}
android_aar          : springgreen2
android_library      : springgreen3
android_resource     : springgreen1
android_prebuilt_aar : olivedrab3
java_library         : indianred1
prebuilt_jar         : mediumpurple1
{/literal}
```

Example usage:

``` {.prettyprint .lang-py}
{literal}
$ buck query "allpaths('//foo:bar', '//path/to:other')" --output-format dot --output-file graph.dot
$ dot -Tpng graph.dot -o graph.png
{/literal}
```

Then, open `graph.png` to visualize the graph.

{/param} {/call} {call buck.param} {param name: \'output-format
dot_bfs\' /} {param desc}

Outputs the digraph representing the query results in [dot
format](https://en.wikipedia.org/wiki/DOT_(graph_description_language)#Directed_graphs)
in bfs order. The nodes will be colored according to their type.

Example usage:

``` {.prettyprint .lang-py}
          {literal}
$ buck query "allpaths('//foo:bar', '//path/to:other')" --output-format dot_bfs --output-file graph.dot
$ dot -Tpng graph.dot -o graph.png
          {/literal}
      
```

Then, open `graph.png` to visualize the graph.

{/param} {/call} {call buck.param} {param name: \'output-format json\'
/} {param desc}

Outputs the results as JSON.

{/param} {/call} {call buck.param} {param name: \'output-format thrift\'
/} {param desc}

Outputs the results as thrift binary.

{/param} {/call} {call buck.param} {param name: \'output-file\' /}
{param desc}

Outputs the results into file path specified.

Example usage:

``` {.prettyprint .lang-py}
          {literal}
$ buck query "allpaths('//foo:bar', '//path/to:other')" --output-format dot --output-file graph.dot
$ dot -Tpng graph.dot -o graph.png
          {/literal}
      
```

{/param} {/call} {call buck.param} {param name: \'output-attributes \'
/} {param desc}

::: {#output-attributes}
Outputs the results as a JSON dictionary
{sp}`build target -> attributes map`. The attributes map is a dictionary
mapping the specified attributes to their values for the build target.
Attributes are regular expressions (e.g. \'.\*\' matches all
attributes). If an attribute (e.g. `srcs`) is not defined for a build
target, it is not present in the output.\
\
NOTE: There is ambiguity when using this option with \'%s\' style
queries. It is suggested to use `--output-attribute` instead. Example:

``` {.prettyprint .lang-py}
{literal}
$ buck query '//example/...' --output-attributes buck.type name srcs
{
  "//example/foo:bar" : {
    "buck.type" : "cxx_library",
    "name" : "foobar",
    "srcs" : [ "example/foo/bar.cc", "example/foo/lib/lib.cc" ]
  }
  "//example/foo:main" : {
    "buck.type" : "cxx_binary",
    "name" : "main"
  }
}
{/literal}
```
:::

{/param} {/call} {call buck.param} {param name: \'output-attribute \' /}
{param desc}

::: {#output-attributes}
Outputs the results as a JSON dictionary
{sp}`build target -> attributes map`. The attributes map is a dictionary
mapping the specified attributes to their values for the build target.
Attributes are regular expressions (e.g. \'.\*\' matches all
attributes). If an attribute (e.g. `srcs`) is not defined for a build
target, it is not present in the output.\
\
Multiple attributes may be specified by providing the
\--output-attribute option multiple times.\
\
NOTE: The primary difference between this and \--output-attributes is
that \--output-attribute works correctly with other multiple-argument
queries. Example:

``` {.prettyprint .lang-py}
{literal}
$ buck query '//example/...' --output-attribute buck.type --output-attribute name --output-attribute srcs
{
  "//example/foo:bar" : {
    "buck.type" : "cxx_library",
    "name" : "foobar",
    "srcs" : [ "example/foo/bar.cc", "example/foo/lib/lib.cc" ]
  }
  "//example/foo:main" : {
    "buck.type" : "cxx_binary",
    "name" : "main"
  }
}
{/literal}
```
:::

{/param} {/call} {/param} {param examples}

``` {.prettyprint .lang-py}
{literal}
#
# For the following examples, assume this BUCK file exists in
# the `examples` directory.
#
cxx_library(
  name = 'one',
  srcs = [ '1.cpp' ],
  deps = [
    ':two',
    ':three',
  ],
)

cxx_library(
  name = 'two',
  srcs = [ '2.cpp' ],
  deps = [
    ':four',
  ],
  tests = [ ':two-tests' ]
)

cxx_library(
  name = 'three',
  srcs = [ '3.cpp' ],
  deps = [
    ':four',
    ':five',
  ],
  tests = [ ':three-tests' ],
)

cxx_library(
  name = 'four',
  srcs = [ '4.cpp' ],
  deps = [
    ':five',
  ]
)

cxx_library(
  name = 'five',
  srcs = [ '5.cpp' ],
)

cxx_test(
  name = 'two-tests',
  srcs = [ '2-test.cpp' ],
  deps = [ ':two' ],
)

cxx_test(
  name = 'three-tests',
  srcs = [ '3-test.cpp' ],
  deps = [ ':three' ],
)
{/literal}
```

**Example**: List *all* the targets in the repository.

    buck query "//..."

    {literal}
    //examples:five
    //examples:four
    //examples:one
    //examples:three
    //examples:three-tests
    //examples:two
    //examples:two-tests
    {/literal}

**Example**: Resolve multiple aliases.

Suppose `.buckconfig` contains the following aliases:

    {literal}
    app = //apps/myapp:app
    lib = //libraries/mylib:lib
    {/literal}

Then the following query

    {literal}
    buck query "%s" app lib --output-format json
    {/literal}

returns

``` {.prettyprint .lang-js}
{literal}
{
  "app": ["//apps/myapp:app"],
  "lib": ["//libraries/mylib:lib"]
}
{/literal}
```

**Example**: List all of the targets on which the `one` library
*directly* depends.

    {literal}
    $ buck query "deps(//examples:one, 1)"
    //examples:one
    //examples:three
    //examples:two
    {/literal}

**Example**: Display a JSON representation of the transitive closure of
the targets on which the `one` library depends.

    {literal}
    $ buck query --output-format json "deps(//examples:one)"
    [
      "//examples:five",
      "//examples:four",
      "//examples:one",
      "//examples:three",
      "//examples:two"
    ]
    {/literal}

**Example**: Display a JSON representation of the tests associated with
the{sp} `one` and `three` libraries.

    {literal}
    $ buck query --output-format json "testsof(deps('%s'))" //examples:one //examples:three
    {
      "//examples:one": ["//examples:two-tests"],
      "//examples:three": ["//examples:three-tests"]
    }
    {/literal}

**Example**: Display the build file that contains the target which is
the owner of the source file, `examples/1.cpp`.

    {literal}
    $ buck query "buildfile(owner('examples/1.cpp'))"
    example/BUCK
    {/literal}

{/param} {/call} {/param} // content {/call} // buck.page {/template}
