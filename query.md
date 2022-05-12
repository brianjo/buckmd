::: {#fb-root}
:::

::: topbar
[](http://buck.build/)

# Buck

-   
-   [Docs](/setup/getting_started.html)
-   [Issues](https://github.com/facebook/buck/issues)
-   [GitHub](https://github.com/facebook/buck)
:::

::: socialBanner
Support Ukraine. [Help Provide Humanitarian Aid to
Ukraine](https://opensource.fb.com/support-ukraine).
:::

::: {.section .content}
::: width
# buck query

::: overview
The `buck query` command provides functionality to query the
*target-nodes* graph (\"target graph\") and return the build targets
that satisfy the query expression.

The query language enables you to combine multiple operators in a single
command. For example, to retrieve a list of all the tests for a build
target, you can combine the `deps()` and `testsof()` operators into a
single call to `buck query`.

    buck query "testsof(deps('//java/com/example/app:amazing'))"

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
expression could be an explicit [build
target](/concept/build_target.html), a [build target
pattern](/concept/build_target_pattern.html), an
[`[alias]`](/files-and-dirs/buckconfig.html#alias), or *the set of
targets returned by another Buck query operator*.

**Tip:** You can pass an alias directly to the `buck query` command line
to see what it resolves to. For example:

    $ buck query app
    //apps/myapp:app

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

    buck query "'//foo:bar=wiz'"

#### Algebraic set operations: intersection, union, set difference {#set-operations}

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

both return the targets that appear in the [transitive
closure](https://en.wikipedia.org/wiki/Transitive_closure) of
`//foo:bar` and `//baz:lib`.

The `intersect` (`^`) and `union` (`+`) operators are commutative. The
`except` (`-`) operator is not commutative.

The parser treats all three operators as left-associative and of equal
precedence, so we recommend that you use parentheses if you need to
ensure a specific order of evaluation. A parenthesized expression
resolves to the value of the expression it encloses. For example, the
first two expressions are equivalent, but the third is not:

    x intersect y union z
    (x intersect y) union z
    x intersect (y union z)

#### Group targets: set {#set}

**Syntax**

    set(a:expr b:expr c:expr ...)

The `set(a b c ...)` operator computes the union of a set of zero or
more target expressions. Separate the targets with white space (not
commas). Quote the targets to ensure that they are parsed correctly.

If you want to invoke `buck query` on a list of targets, then `set()` is
a way to group this list in a query.

**Example:**

The following command line returns the target `main` in the build file
in the root of the Buck project and all the targets from the build file
in the `myclass` subdirectory of the root.

    buck query "set( '//:main' '//myclass:' )"

**Example:**

The following command line returns the merged set (union) of
dependencies for the targets: `main` and `subs` in the build file in the
root of the Buck project.

    buck query "deps( set( '//:main' '//:subs' ) )"

#### All dependency paths: allpaths {#allpaths}

**Syntax**

    allpaths(from:expr, to:expr)

The `allpaths(from, to)` operator evaluates to the graph formed by paths
between the target expressions `from` and `to`, following the
dependencies between nodes. For example, the value of

    buck query "allpaths('//foo:bar', '//foo/bar/lib:baz')"

is the dependency graph rooted at the single target node `//foo:bar`,
that includes all target nodes that depend on `//foo/bar/lib:baz`.

The two arguments to `allpaths()` can themselves be expressions. For
example, the command:

    buck query "allpaths(kind(java_library, '//...'), '//foo:bar')"

shows all the paths between any `java_library` in the repository and the
target `//foo:bar`.

We recommend using `allpaths()` with the `--output-format dot` parameter
to generate a graphviz file that can then be rendered as an image. For
example:

``` {.prettyprint .lang-py}
$ buck query "allpaths('//foo:bar', '//foo/bar/lib:baz')" --output-format dot --output-file result.dot
$ dot -Tpng result.dot -o image.png
```

*Graphviz* is an open-source graph-visualization software tool. Graphviz
uses the *dot* language to describe graphs.

#### Rule attribute filtering: attrfilter {#attrfilter}

**Syntax**

    attrfilter(attribute, value, expr)

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

    buck query "attrfilter(deps, '//foo:bar', '//...')"

returns the build targets in the repository that depend on
`//foo:bar`---or more precisely: those build targets that include
`//foo:bar` in their `deps` argument list.

The match performed by `attrfilter()` is semantic rather than textual.
So, for example, if you have the following `deps` argument in your build
file:

    cxx_binary(
      name = 'main',
      srcs = [
        'main.cpp'
      ],
      deps = [
        ':myclass',
      ],
    )

Your `attrfilter()` clause should be:

    buck query "attrfilter( deps, '//:myclass', '//...' )"

Note the double forward slash (`//`) before the second argument to
`attrfilter()`.

#### Rule attribute filtering with regex: attrregexfilter {#attrregexfilter}

**Syntax**

    attrregexfilter(attribute, pattern, expr)

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

#### Build files of targets: buildfile {#buildfile}

**Syntax**

    buildfile(expr)

The `buildfile(expr)` operator evaluates to those build files that
define the targets that result from the evaluation of the target
expression, `expr`.

In order to find the build file associated with a source file, combine
the `owner` operator with `buildfile`. For example,

    buck query "buildfile(owner('foo/bar/main.cpp'))" 

first finds the targets that *own* `foo/bar/main.cpp` and then returns
the build files, such as `foo/bar/BUCK`, that define those targets.

#### Transitive closure of dependencies: deps and first-order-deps {#deps}

**Syntax**

    deps(argset:expr)
    deps(argset:expr, depth:int)
    deps(argset:expr, depth:int, filter:expr)
    deps(argset:expr, depth:int, first_order_deps())

The `deps(x)` operator evaluates to the graph formed by the [transitive
closure](https://en.wikipedia.org/wiki/Transitive_closure) of the
dependencies of its argument set, *x*, including the nodes from the
argument set itself. For example, the value of

    buck query "deps('//foo:bar')"

is the dependency graph rooted at the target node `//foo:bar`. It
includes all of the dependencies of `//foo:bar`. It also includes
`//foo:bar` itself.

The `deps` operator accepts an optional second argument, which is an
integer literal specifying an upper bound on the depth of the search.
So,

    deps('//foo:bar', 1)

evaluates to the direct dependencies of the target `//foo:bar`, and

    deps('//foo:bar', 2)

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

    buck query "deps('//foo:bar', 1, first_order_deps())"

is equivalent to

    buck query "deps('//foo:bar', 1)"

The `first_order_deps()` operator can be used only as an argument passed
to `deps()`.

Note that because `deps()` uses positional parameters, you must specify
the second argument in order to specify the third. In this scenario, if
you want the search to be unbounded, we recommend that you use
`2147483647` which corresponds to Java\'s `Integer.MAX_VALUE`.

#### Filter targets by name: filter {#filter}

**Syntax**

    filter(regex, expr)

The `filter(regex, expr)` operator evaluates the specified target
expression, `expr`, and returns the targets that have a name attribute
that matches the specified regular expression `regex`. For example,

    buck query "filter('library', deps('//foo:bar'))"

returns the targets in the transitive closure of `//foo:bar`that contain
the string `library` in their name attribute.

The `filter()` operator performs a *partial* match. So, both of the
following clauses would match a target with the name `main`.

    buck query "filter( 'main', '//...' )"

    buck query "filter( 'mai', '//...' )"

Another example:

    buck query "filter('.*\.java$', labels(srcs, '//foo:bar'))"

returns the `java` files used to build `//foo:bar`.

You often need to quote the pattern to ensure that regular expressions,
such as `.*xpto`, are parsed correctly.

#### Direct input files: inputs {#inputs}

**Syntax**

    inputs(expr)

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

#### Filter targets by rule type: kind {#kind}

**Syntax**

    kind(regex, expr)

The `kind(regex, expr)` operator evaluates the specified target
expression, `expr`, and returns the targets where the rule type matches
the specified `regex`. For example,

    buck query "kind('java_library', deps('//foo:bar'))"

returns all `java_library` targets in the transitive dependencies of
`//foo:bar`.

The specified `pattern` can be a regular expression. For example,

    buck query "kind('.*_test', '//...')"

returns all targets in the repository with a rule type that ends with
`_test`, such as `java_test` and `cxx_test`.

You often need to quote the pattern to ensure that regular expressions,
such as `.*xpto`, are parsed correctly.

To get a list of the available rule types in a given set of targets, you
could use a command such as the following:

    buck query : --output-attribute buck.type

which prints all the rule types in the build file in the current
directory (`:`)---in JSON format. See `--output-attribute` described in
the **Parameters** section below for more information.

#### Extract content of rule attributes: labels {#labels}

**Syntax**

    labels(attribute, expr)

The `labels(attribute, expr)` operator returns the set of build targets
and file paths listed in the attribute specified by the `attribute`
parameter, in the targets that result from the evaluation of target
expression, `expr`. Valid values for *attribute* include `srcs`,
`headers`, and `deps`.

**Example**: Get all build targets and file paths specified in the
`srcs` attribute for *all the rules* in the build file in the current
directory.

    buck query "labels( 'srcs', ':' )"

In performing this operation, Buck validates that any source files
referenced in these attributes do, in fact, exist; Buck generates an
error if they do not.

**Example**: Get all the build targets and file paths specified in the
`deps` arguments in the *tests of* the target `//foo:bar`.

    buck query "labels('deps', testsof('//foo:bar'))"

Note that `deps` must be quoted because, in addition to being a
build-file attribute, it is itself a reserved keyword of the query
language.

#### Find targets that own specified files: owner {#owner}

**Syntax**

    owner(inputfile)

The `owner(inputfile)` operator returns the targets that own the
specified `inputfile`. In this context, *own* means that the target has
the specified file as an input. You could consider the `owner()` and
`inputs()` operators to be inverses of each other.

**Example**:

    buck query "owner('examples/1.txt')"

returns the targets that owns the file `examples/1.txt`, which could be
a value such as `//examples:one`.

It is possible for the specified file to have multiple owners, in which
case, `owner()` returns a set of targets.

If no owner for the file is found, `owner()` outputs the message:

    No owner was found for <file>

#### Transitive closure of reverse dependencies: rdeps {#rdeps}

**Syntax**

    rdeps(universe:expr, argset:expr)
    rdeps(universe:expr, argset:expr, depth:int)

The `rdeps(universe, argset)` operator returns the reverse dependencies
of the argument set `argset` within the [transitive
closure](https://en.wikipedia.org/wiki/Transitive_closure) of the set
`universe` (the *universe*). The returned values include the nodes from
the argument set `argset` itself.

The `rdeps` operator accepts an optional third argument, which is an
integer literal specifying an upper bound on the depth of the search. A
value of one (`1`) specifies that `buck query` should return only direct
dependencies. If the `depth` parameter is omitted, the search is
unbounded.

**Example**

The following example, returns the targets in the [transitive
closure](https://en.wikipedia.org/wiki/Transitive_closure) of
`//foo:bar` that depend directly on `//example:baz`.

    buck query "rdeps('//foo:bar', '//example:baz', 1)"

**Example**

The *universe:expr* parameter includes the *entire* transitive closure
of the target pattern specified. So some of these targets might be
outside the directory structure indicated by that target pattern. For
example, the result set of

    buck query "rdeps('//foo/bar/...', '//fuga:baz', 1)"

might contain targets outside the directory structure beneath

    foo/bar/

To say it another way, if a target in `//foo/bar/...` depends on, say,
`//hoge,` which in turn depends on `//fuga:baz,` *then `//hoge` would
show up in the result set*.

If you wanted to constrain the result set to only those targets beneath
`foo/bar`, you could use the [`intersect`](#set-operations) operator:

    buck query "rdeps('//foo/bar/...', '//fuga:baz', 1) ^ '//foo/bar/...'"

The caret (`^`) is a succinct synonym for `intersect`.

#### List the tests of the specified targets: testsof {#testsof}

**Syntax**

    testsof(expr)

The `testsof(expr)` operator returns the tests associated with the
targets specified by the target expression, `expr`. For example,

    buck query "testsof(set('//foo:bar' '//baz:app+lib')"

returns the tests associated with `//foo:bar` and `//baz:app+lib`.

To obtain all the tests associated with the target and its dependencies,
you can combine the `testsof()` operator with the `deps()` operator. For
example,

    buck query "testsof(deps('//foo:bar'))"

first finds the transitive closure of `//foo:bar`, and then lists all
the tests associated with the targets in this transitive closure.

## Executing multiple queries at once

Suppose you want to know the tests associated with a set of targets.
This can be done by combining the `testsof`, `deps` and `set` operators.
For example,

    buck query "testsof(deps(set('target1' 'target2' 'target3')))"

Suppose you now want to know the tests for *each* of these targets; the
above command returns the union of the tests. Instead of executing one
query for the entire set of targets, `buck query` provides a way to
repeat a query with different targets using a single command. To do
this, first define the query expression format and then list the input
targets, separated by spaces. For example,

    buck query "testsof(deps( %s ))" target1 target2 target3

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

    buck query "owner( %s )" main.cpp myclass.cpp myclass.h

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

    //foo:bar
    //foo:baz

Then the query expression is equivalent to:

    buck query "testsof(deps(set('//foo:bar' '//foo:baz')))"

If you use multiple `%Ss` operators in a single query, you can specify
which lines in the `@`-file should be used for each instance of `%Ss` in
the query expression: use `--` to separate elements that go in different
sets. For example:

    buck query "testsof(deps(%Ss)) union deps(%Ss)" @path/to/args-file

    //foo:foo
    --
    //bar:bar

is equivalent to running the following:

    buck query "testsof(deps(set('//foo:foo'))) union deps(set('//bar:bar'))"

## Parameters

-   `--output-format dot`

    Outputs the digraph representing the query results in [dot
    format](https://en.wikipedia.org/wiki/DOT_(graph_description_language)#Directed_graphs).
    The nodes will be colored according to their type. See
    [graphviz.org](http://www.graphviz.org/doc/info/colors.html) for
    color definitions.

    ``` {.prettyprint .lang-py}
    android_aar          : springgreen2
    android_library      : springgreen3
    android_resource     : springgreen1
    android_prebuilt_aar : olivedrab3
    java_library         : indianred1
    prebuilt_jar         : mediumpurple1
    ```

    Example usage:

    ``` {.prettyprint .lang-py}
    $ buck query "allpaths('//foo:bar', '//path/to:other')" --output-format dot --output-file graph.dot
    $ dot -Tpng graph.dot -o graph.png
    ```

    Then, open `graph.png` to visualize the graph.

-   `--output-format dot_bfs`

    Outputs the digraph representing the query results in [dot
    format](https://en.wikipedia.org/wiki/DOT_(graph_description_language)#Directed_graphs)
    in bfs order. The nodes will be colored according to their type.

    Example usage:

    ``` {.prettyprint .lang-py}
    $ buck query "allpaths('//foo:bar', '//path/to:other')" --output-format dot_bfs --output-file graph.dot
    $ dot -Tpng graph.dot -o graph.png
              
    ```

    Then, open `graph.png` to visualize the graph.

-   `--output-format json`

    Outputs the results as JSON.

-   `--output-format thrift`

    Outputs the results as thrift binary.

-   `--output-file`

    Outputs the results into file path specified.

    Example usage:

    ``` {.prettyprint .lang-py}
    $ buck query "allpaths('//foo:bar', '//path/to:other')" --output-format dot --output-file graph.dot
    $ dot -Tpng graph.dot -o graph.png
              
    ```

-   `--output-attributes <attributes>`

    ::: {#output-attributes}
    Outputs the results as a JSON dictionary
    `build target -> attributes map`. The attributes map is a dictionary
    mapping the specified attributes to their values for the build
    target. Attributes are regular expressions (e.g. \'.\*\' matches all
    attributes). If an attribute (e.g. `srcs`) is not defined for a
    build target, it is not present in the output.\
    \
    NOTE: There is ambiguity when using this option with \'%s\' style
    queries. It is suggested to use `--output-attribute` instead.
    Example:

    ``` {.prettyprint .lang-py}
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
    ```
    :::

-   `--output-attribute <attribute>`

    ::: {#output-attributes}
    Outputs the results as a JSON dictionary
    `build target -> attributes map`. The attributes map is a dictionary
    mapping the specified attributes to their values for the build
    target. Attributes are regular expressions (e.g. \'.\*\' matches all
    attributes). If an attribute (e.g. `srcs`) is not defined for a
    build target, it is not present in the output.\
    \
    Multiple attributes may be specified by providing the
    \--output-attribute option multiple times.\
    \
    NOTE: The primary difference between this and \--output-attributes
    is that \--output-attribute works correctly with other
    multiple-argument queries. Example:

    ``` {.prettyprint .lang-py}
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
    ```
    :::

## Examples

``` {.prettyprint .lang-py}
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
```

**Example**: List *all* the targets in the repository.

    buck query "//..."

    //examples:five
    //examples:four
    //examples:one
    //examples:three
    //examples:three-tests
    //examples:two
    //examples:two-tests

**Example**: Resolve multiple aliases.

Suppose `.buckconfig` contains the following aliases:

    app = //apps/myapp:app
    lib = //libraries/mylib:lib

Then the following query

    buck query "%s" app lib --output-format json

returns

``` {.prettyprint .lang-js}
{
  "app": ["//apps/myapp:app"],
  "lib": ["//libraries/mylib:lib"]
}
```

**Example**: List all of the targets on which the `one` library
*directly* depends.

    $ buck query "deps(//examples:one, 1)"
    //examples:one
    //examples:three
    //examples:two

**Example**: Display a JSON representation of the transitive closure of
the targets on which the `one` library depends.

    $ buck query --output-format json "deps(//examples:one)"
    [
      "//examples:five",
      "//examples:four",
      "//examples:one",
      "//examples:three",
      "//examples:two"
    ]

**Example**: Display a JSON representation of the tests associated with
the `one` and `three` libraries.

    $ buck query --output-format json "testsof(deps('%s'))" //examples:one //examples:three
    {
      "//examples:one": ["//examples:two-tests"],
      "//examples:three": ["//examples:three-tests"]
    }

**Example**: Display the build file that contains the target which is
the owner of the source file, `examples/1.cpp`.

    $ buck query "buildfile(owner('examples/1.cpp'))"
    example/BUCK
:::

### The Basics

-   [Getting Started](/setup/getting_started.html)
-   [Key Concepts](/about/overview.html)
-   [Tutorial](/learning/tutorial.html)
-   [Installing the IntelliJ
    Plugin](/setup/intellij_plugin_install.html)
-   [Exopackage](/article/exopackage.html)
-   [Buck Cheat Sheet](/article/query_cheat_sheet.html)

### About

-   [What Makes Buck so Fast?](/concept/what_makes_buck_so_fast.html)
-   [Showcase](/about/showcase.html)
-   [Troubleshooting](/concept/troubleshooting.html)
-   [Performance Tuning](/about/performance_tuning.html)
-   [FAQ](/concept/faq.html)
-   [Learn More (Buck Presentations)](/presentations/index.html)

### Concepts

-   [Build Rule](/concept/build_rule.html)
-   [Build File](/concept/build_file.html)
-   [Build Target](/concept/build_target.html)
-   [Build Target Pattern](/concept/build_target_pattern.html)
-   [Buck Daemon (buckd)](/concept/buckd.html)
-   [Visibility](/concept/visibility.html)
-   [Flavors](/concept/flavors.html)
-   [HTTP Cache API](/concept/http_cache_api.html)
-   [Rule Keys](/concept/rule_keys.html)
-   [Java ABIs](/concept/java_abis.html)
-   [Skylark](/concept/skylark.html)

### Files and Directories

-   [.buckconfig](/files-and-dirs/buckconfig.html)
-   [.buckjavaargs](/files-and-dirs/buckjavaargs.html)
-   [buck-out](/files-and-dirs/buck-out.html)

### Commands

-   [Common Parameters](/command/common_parameters.html)
-   [buck audit](/command/audit.html)
-   [buck build](/command/build.html)
-   [buck clean](/command/clean.html)
-   [buck doctor](/command/doctor.html)
-   [buck fetch](/command/fetch.html)
-   [buck fix](/command/fix.html)
-   [buck install](/command/install.html)
-   [buck kill](/command/kill.html)
-   [buck killall](/command/killall.html)
-   [buck project](/command/project.html)
-   [buck publish](/command/publish.html)
-   [buck query](/command/query.html)
-   [buck run](/command/run.html)
-   [buck root](/command/root.html)
-   [buck server](/command/server.html)
-   [buck targets](/command/targets.html)
-   [buck test](/command/test.html)
-   [buck uninstall](/command/uninstall.html)
-   [Exit Codes](/command/exit_codes.html)

### Build Rules

-   **Core**
-   [command_alias()](/rule/command_alias.html)
-   [export_file()](/rule/export_file.html)
-   [filegroup()](/rule/filegroup.html)
-   [genrule()](/rule/genrule.html)
-   [http_archive()](/rule/http_archive.html)
-   [http_file()](/rule/http_file.html)
-   [remote_file()](/rule/remote_file.html)
-   [test_suite()](/rule/test_suite.html)
-   [worker_tool()](/rule/worker_tool.html)
-   [zip_file()](/rule/zip_file.html)
-   **Android**
-   [android_aar()](/rule/android_aar.html)
-   [android_binary()](/rule/android_binary.html)
-   [android_build_config()](/rule/android_build_config.html)
-   [android_instrumentation_apk()](/rule/android_instrumentation_apk.html)
-   [android_instrumentation_test()](/rule/android_instrumentation_test.html)
-   [android_library()](/rule/android_library.html)
-   [android_manifest()](/rule/android_manifest.html)
-   [android_prebuilt_aar()](/rule/android_prebuilt_aar.html)
-   [android_resource()](/rule/android_resource.html)
-   [apk_genrule()](/rule/apk_genrule.html)
-   [gen_aidl()](/rule/gen_aidl.html)
-   [keystore()](/rule/keystore.html)
-   [ndk_library()](/rule/ndk_library.html)
-   [prebuilt_jar()](/rule/prebuilt_jar.html)
-   [prebuilt_native_library()](/rule/prebuilt_native_library.html)
-   [robolectric_test()](/rule/robolectric_test.html)
-   **CXX**
-   [cxx_binary()](/rule/cxx_binary.html)
-   [cxx_library()](/rule/cxx_library.html)
-   [cxx_genrule()](/rule/cxx_genrule.html)
-   [cxx_precompiled_header()](/rule/cxx_precompiled_header.html)
-   [cxx_test()](/rule/cxx_test.html)
-   [prebuilt_cxx_library()](/rule/prebuilt_cxx_library.html)
-   [prebuilt_cxx_library_group()](/rule/prebuilt_cxx_library_group.html)
-   **D**
-   [d_binary()](/rule/d_binary.html)
-   [d_library()](/rule/d_library.html)
-   [d_test()](/rule/d_test.html)
-   **Go**
-   [go_binary()](/rule/go_binary.html)
-   [go_library()](/rule/go_library.html)
-   [go_test()](/rule/go_test.html)
-   [cgo_library()](/rule/cgo_library.html)
-   **Groovy**
-   [groovy_library()](/rule/groovy_library.html)
-   **Halide**
-   [halide_library()](/rule/halide_library.html)
-   **Haskell**
-   [haskell_binary()](/rule/haskell_binary.html)
-   [haskell_library()](/rule/haskell_library.html)
-   [prebuilt_haskell_library()](/rule/prebuilt_haskell_library.html)
-   **iOS**
-   [apple_asset_catalog()](/rule/apple_asset_catalog.html)
-   [apple_binary()](/rule/apple_binary.html)
-   [apple_bundle()](/rule/apple_bundle.html)
-   [apple_library()](/rule/apple_library.html)
-   [apple_package()](/rule/apple_package.html)
-   [apple_resource()](/rule/apple_resource.html)
-   [apple_test()](/rule/apple_test.html)
-   [core_data_model()](/rule/core_data_model.html)
-   [prebuilt_apple_framework()](/rule/prebuilt_apple_framework.html)
-   **Java**
-   [java_binary()](/rule/java_binary.html)
-   [java_library()](/rule/java_library.html)
-   [java_test()](/rule/java_test.html)
-   [prebuilt_jar()](/rule/prebuilt_jar.html)
-   [prebuilt_native_library()](/rule/prebuilt_native_library.html)
-   **Kotlin**
-   [kotlin_library()](/rule/kotlin_library.html)
-   [kotlin_test()](/rule/kotlin_test.html)
-   **Lua**
-   [cxx_lua_extension()](/rule/cxx_lua_extension.html)
-   [lua_binary()](/rule/lua_binary.html)
-   [lua_library()](/rule/lua_library.html)
-   **OCaml**
-   [ocaml_binary()](/rule/ocaml_binary.html)
-   [ocaml_library()](/rule/ocaml_library.html)
-   **Python**
-   [prebuilt_python_library()](/rule/prebuilt_python_library.html)
-   [python_binary()](/rule/python_binary.html)
-   [python_library()](/rule/python_library.html)
-   [python_test()](/rule/python_test.html)
-   **Rust**
-   [rust_binary()](/rule/rust_binary.html)
-   [rust_library()](/rule/rust_library.html)
-   [rust_test()](/rule/rust_test.html)
-   [prebuilt_rust_library()](/rule/prebuilt_rust_library.html)
-   **Shell**
-   [sh_binary()](/rule/sh_binary.html)
-   [sh_test()](/rule/sh_test.html)
-   **.NET**
-   [csharp_library()](/rule/csharp_library.html)
-   [prebuilt_dotnet_library()](/rule/prebuilt_dotnet_library.html)

### Functions

-   **Python DSL**
-   [add_build_file_dep()](/function/add_build_file_dep.html)
-   [allow_unsafe_import()](/function/allow_unsafe_import.html)
-   [flatten_dicts()](/function/flatten_dicts.html)
-   [glob()](/function/glob.html)
-   [get_base_path()](/function/get_base_path.html)
-   [get_cell_name()](/function/get_cell_name.html)
-   [host_info()](/function/host_info.html)
-   [include_defs()](/function/include_defs.html)
-   [load()](/function/load.html)
-   [read_config()](/function/read_config.html)
-   [subdir_glob()](/function/subdir_glob.html)
-   [String Parameter Macros](/function/string_parameter_macros.html)

```{=html}
<!-- -->
```
-   **Skylark**
-   [glob()](/skylark/generated/glob.html)
-   [host_info()](/skylark/generated/host_info.html)
-   [package_name()](/skylark/generated/package_name.html)
-   [provider()](/skylark/generated/provider.html)
-   [read_config()](/skylark/generated/read_config.html)
-   [repository_name()](/skylark/generated/repository_name.html)
-   [rule_exists()](/skylark/generated/rule_exists.html)

### Extending Buck

-   [Custom Macros](/extending/macros.html)
-   [Custom Rules](/extending/rules.html)
-   [Building E2E Tests for Buck](/extending/e2e_tests.html)
:::
:::

::: width
© Copyright Facebook, 2013 - 2020
:::
