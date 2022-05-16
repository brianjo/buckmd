/\* \* Copyright (c) Facebook, Inc. and its affiliates. \* \* Licensed
under the Apache License, Version 2.0 (the \"License\"); \* you may not
use this file except in compliance with the License. \* You may obtain a
copy of the License at \* \* http://www.apache.org/licenses/LICENSE-2.0
\* \* Unless required by applicable law or agreed to in writing,
software \* distributed under the License is distributed on an \"AS IS\"
BASIS, \* WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
or implied. \* See the License for the specific language governing
permissions and \* limitations under the License. \*/ {namespace
buck.query_cheat_sheet} /\*\* \* \@param id attribute for this blob of
HTML so users can link to an individual FAQ. We should make \* an effort
to keep these identifiers stable to avoid breaking links. Therefore,
when choosing \* an id, try to make it generic enough so that it is
forward-compatible. \* \@param question Question. \* \@param shortAnswer
Try to keep this to a one-liner. \* \@param? longAnswer This portion of
the answer can include more detail. \*/ {template .faq}

::: {#{$id|id} .{css .faq}}
::: {.{css .faq_q}}
{\$question\|noAutoescape}
:::

::: {.{css .faq_a}}
{\$shortAnswer\|noAutoescape} {if \$longAnswer}

{\$longAnswer\|noAutoescape}

{/if}
:::
:::

{/template} /\*\*\*/ {template .soyweb} {call buck.page} {param title:
\'Buck Cheat Sheet\' /} {param navid: \'article_query_cheat_sheet\' /}
{param prettify: true /} {param description} Most common use cases of
buck query. {/param} {param content}

This section provides example command lines that you can use to obtain
information about Buck and about your build. These techniques can help
you to understand how your build works and to troubleshoot issues with
your build.

Most of these examples use the {call buck.cmd_query /}, {call
buck.cmd_targets /}, and {call buck.cmd_audit /} commands. For more
information and examples, see the reference pages for those commands.

------------------------------------------------------------------------

-   [How do I get a list of all the rules that Buck supports from the
    command line?](#list-all-rules)
-   [How do I see the arguments for a given rule from the command
    line?](#list-args-for-rule)
-   [How do I find all the targets for a
    package?](#find-existing-targets)
-   [How do I specify more than one target to
    `buck query`?](#query-multiple-targets)
-   [How do I get the attribute names and values for the targets that
    result from a query?](#output-target-attributes)
-   [How do I perform a query *inside* of a rule?](#queries-in-rules)
-   [How do I find the dependencies for a target, that is, the targets
    on which a specified target depends?](#find-dependencies)
-   [How do I find the reverse-dependencies for a target, that is, the
    targets that *depend on* a specified
    target?](#find-reverse-dependencies)
-   [How do I find the build file that contains the target that owns a
    source file?](#find-buildfile-owner)

------------------------------------------------------------------------

\
{call .faq} {param id: \'list-all-rules\' /} {param question}

How do I get a list of all the rules that Buck supports, *from the
command line*, so that I can process them with `grep`, `sed`, etc?

{/param} {param shortAnswer}

Use {call buck.cmd_audit /} with the `ruletypes` (plural) subcommand,
which returns an alphabetized list of all the rules that Buck supports.

{call buckaudit.example_ruletypes /} {/param} {/call} {call .faq} {param
id: \'list-args-for-rule\' /} {param question}

How do I see the arguments for a rule from the command line?

{/param} {param shortAnswer}

Use {call buck.cmd_audit /} with the `ruletype` (singular) subcommand
followed by the name of the rule.

{call buckaudit.example_ruletype /} {/param} {/call} {call .faq} {param
id: \'find-existing-targets\' /} {param question}

How do I find all the targets for a package?

{/param} {param shortAnswer}

Specify a *build target pattern* that represents the targets in the
package.

``` {.prettyprint .lang-js}
{literal}
buck query //path/to/dir/...
{/literal}
```

{/param} {param longAnswer}

The `buck query` command can accept a {call buck.build_target_pattern /}
as a parameter. If you specify a build target pattern, Buck evaluates
this pattern and shows all the build targets that match it.

{/param} {/call} {call .faq} {param id: \'query-multiple-targets\' /}
{param question}

How do I specify more than one target to `buck query`?

{/param} {param shortAnswer} Use the {call buckquery.set /} operator.
{call buckquery.example_multiple_targets /} {/param} {/call} {call .faq}
{param id: \'output-target-attributes\' /} {param question}

How do I get the attribute names and values for the targets returned by
a query?

{/param} {param shortAnswer}

Add the `--output-attributes` option to the command line, followed by
regular expressions that represent the attributes of interest.

``` {.prettyprint .lang-js}
{literal}
buck query "deps(//foo:bar)" --output-attributes 'name' 'exported_headers'
{/literal}
```

{/param} {param longAnswer}

The `--output-attributes` option enables you to specify which attributes
Buck should return. Instead of returning the names of the targets that
match the query expression, Buck returns the names and values of the
specified attributes for those targets in JSON format. Attributes are
specified as regular expressions. For example, `'.*'` matches all
attributes. See the {sp} [buck query
page](%7BROOT%7Dcommand/query.html#output-attributes) {sp}for more
details. The output for the example query above might look something
like the following.

``` {.prettyprint .lang-js}
{literal}
{
  "//foo/bar/lib:lib" : {
    "exported_headers" : [ "App/util.h" ],
    "name" : "lib"
  },
  "//foo/bar:app" : {
    "exported_headers" : [ "App/lib.h" ],
    "name" : "app"
  }
}
{/literal}
```

{/param} {/call} {call .faq} {param id: \'queries-in-rules\' /} {param
question}

How do I perform a query *inside* of a rule?

{/param} {param shortAnswer}

Use **{call buck.string_parameter_macros /}**, specifically, the *query*
macros:

    {literal}
    $(query_targets "queryfunction(//:foo)")
    $(query_outputs "queryfunction(//:foo)")
    $(query_targets_and_outputs [SEPARATOR] "queryfunction(//:foo)")
    {/literal}

Note, however, that the query macros are supported only for {call
buck.genrule /} and {call buck.apk_genrule /}.

{/param} {/call} {call .faq} {param id: \'find-dependencies\' /} {param
question}

How do I find the dependencies for a target?

{/param} {param shortAnswer}

Use the `deps()` operator.

``` {.prettyprint .lang-js}
{literal}
buck query "deps('//foo:bar')"
buck query "deps('//foo:bar', 1, first_order_deps())"
buck query "deps(set('//foo:bar' '//foo:lib' '//foo/baz:util'))"
{/literal}
```

{/param} {param longAnswer}

The [deps](%7BROOT%7Dcommand/query.html#deps) operator finds the
dependencies of the specified targets. The first argument represents the
targets of interest. This can be a single {call buck.build_target /} or
{call buck.build_target_pattern /}, or a set of these.

The optional second argument is the *depth* of the search for
dependencies from the specified targets. For example, `1`, as shown in
the example above, returns only the direct dependencies. If you do not
provide this argument, the output is the complete set of transitive
dependencies.

{/param} {/call} {call .faq} {param id: \'find-reverse-dependencies\' /}
{param question}

How do I find the reverse-dependencies for a target, that is, the
targets that *depend on* a specified target?

{/param} {param shortAnswer}

Use the `buck query` {call buck.cmd_link}{param name: \'query\' /}{param
section: \'rdeps\'/}{/call}{sp} (reverse dependencies) operator.

{call buckquery.example_rdeps /} {/param} {/call} {call .faq} {param id:
\'find-buildfile-owner\' /} {param question}

How do I find the buildfile that contains the target that owns a source
file?

{/param} {param shortAnswer} {call buckquery.example_buildfile_owner /}
{/param} {/call} {/param} {/call} {/template}
