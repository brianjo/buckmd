/\* \* Copyright (c) Facebook, Inc. and its affiliates. \* \* Licensed
under the Apache License, Version 2.0 (the \"License\"); \* you may not
use this file except in compliance with the License. \* You may obtain a
copy of the License at \* \* http://www.apache.org/licenses/LICENSE-2.0
\* \* Unless required by applicable law or agreed to in writing,
software \* distributed under the License is distributed on an \"AS IS\"
BASIS, \* WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
or implied. \* See the License for the specific language governing
permissions and \* limitations under the License. \*/ {namespace
buck.glob} /\*\*\*/ {template .soyweb} {call buck.page} {param title:
\'glob()\' /} {param navid: \'function_glob\' /} {param prettify: true
/} {param description} The glob() function is used to specify a set of
files using patterns. {/param} {param content} {call buck.function}
{param status: \'FROZEN\' /} {param overview}

The `glob()` function specifies a set of files using patterns.

A pattern is structured as a *relative* path with no repeated or
trailing path separators, such as the forward slash (`/`).

Patterns may contain shell-like wildcards, such as `*` , `?` , or
`[charset]`.

Additionally, the path element, `**` , matches any subpath. For instance

    {literal}
    foo/**/bar
    {/literal}

is equivalent to

    {literal}
    ["foo/bar", "foo/*/bar", "foo/*/*/bar", ...]
    {/literal}

The patterns that specify the set of files to include---as well as the
patterns that specify the files to *exclude* (see the `exclude`
parameter below)---must both be statically defined; you cannot generate
these patterns dynamically at build time.

{/param} {param args} {call buck.functionArg} {param desc} The first
parameter is unnamed and is a list of patterns that match files under
the current directory. {/param} {/call} {call buck.functionArg} {param
name : \'exclude\' /} {param default : \'\[\]\' /} {param desc} A list
of patterns that identify files that should be removed from the set
specified by the first parameter. You cannot specify both the `exclude`
parameter and the `excludes` parameter because they serve the same
purpose. {/param} {/call} {call buck.functionArg} {param name :
\'include_dotfiles\' /} {param default : \'False\' /} {param desc}
Specifies whether `*` and `**` patterns should capture file and
directory names that start with a dot (`.`). By default, this parameter
is false, which indicates that files that start with a dot are
automatically excluded. {/param} {/call} {call buck.functionArg} {param
name : \'excludes\' /} {param default : \'\[\]\' /} {param desc}
DEPRECATED\
This parameter is deprecated; use the `exclude` parameter instead of
`excludes`.\
A list of patterns that identify files that should be removed from the
set specified by the first argument. {/param} {/call} {/param} {param
examples}

For the purposes of these examples, a *regular* file is one that is not
a *dotfile*; a file is a dotfile if its path---relative to the current
directory---includes at least one path element that starts with a dot.

All the regular `.java` files in the current directory:

``` {.prettyprint .lang-py}
{literal}
glob(['*.java'])
{/literal}
```

All the `.java` files in the current directory---including dotfiles:

``` {.prettyprint .lang-py}
{literal}
glob(['*.java'], include_dotfiles=True)
{/literal}
```

All the files under the current directory:

``` {.prettyprint .lang-py}
{literal}
glob(['**/'], include_dotfiles=True)
{/literal}
```

All the regular files under the directory `.git`:

``` {.prettyprint .lang-py}
{literal}
glob(['.git/**/'])
{/literal}
```

All the files starting with `'.'` under regular (non-dot) directories:

``` {.prettyprint .lang-py}
{literal}
glob(['**/.*'])
{/literal}
```

All the regular `.java` and `.aidl` files in the current directory:

``` {.prettyprint .lang-py}
{literal}
glob(['*.java', '*.aidl'])
{/literal}
```

All the regular `.java` files under current directory:

``` {.prettyprint .lang-py}
{literal}
glob(['**/*.java'])
{/literal}
```

All of regular files under the current directory that end in
`Test.java`:

``` {.prettyprint .lang-py}
{literal}
glob(['**/*Test.java'])
{/literal}
```

All the regular files under the current directory that end in
`Test.java`, as well as `StringTests.java`:

``` {.prettyprint .lang-py}
{literal}
glob(['**/*Test.java', 'StringTests.java'])
{/literal}
```

All the regular files under the current directory that end in
`Test.java`, *except* for `HaltingProblemTest.java`:

``` {.prettyprint .lang-py}
{literal}
glob(['**/*Test.java'], exclude = ['HaltingProblemTest.java'])
{/literal}
```

All the regular `.java` files under the current directory, *except* for
those that end in `Test.java`:

``` {.prettyprint .lang-py}
{literal}
glob(['**/*.java'], exclude = ['**/*Test.java'])
{/literal}
```

{/param} {/call} // buck.function {/param} // content {/call}
{/template}
