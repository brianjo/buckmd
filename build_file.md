/\* \* Copyright (c) Facebook, Inc. and its affiliates. \* \* Licensed
under the Apache License, Version 2.0 (the \"License\"); \* you may not
use this file except in compliance with the License. \* You may obtain a
copy of the License at \* \* http://www.apache.org/licenses/LICENSE-2.0
\* \* Unless required by applicable law or agreed to in writing,
software \* distributed under the License is distributed on an \"AS IS\"
BASIS, \* WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
or implied. \* See the License for the specific language governing
permissions and \* limitations under the License. \*/ {namespace
buck.build_file} /\*\*\*/ {template .soyweb} {call buck.page} {param
title: \'Build File\' /} {param navid: \'concept_build_file\' /} {param
prettify: true /} {param description} Any file, typically named BUCK,
that defines one or more build rules. {/param} {param content}

A *build file* is a file, typically named `BUCK`, that defines one or
more {call buck.build_rule /}s.

Note that you can change the name that Buck uses for the build file in
the `buildfile` section of {call buck.buckconfig_link /}.

A source file in your project can only be referenced by rules in its
\"nearest\" build file, where \"nearest\" means its closest direct
ancestor in your project\'s file tree. (If a source file has a build
file as a sibling, then that is its nearest ancestor.) For example, if
your project had the following `BUCK` files:

{literal}

    java/com/facebook/base/BUCK
    java/com/facebook/common/BUCK
    java/com/facebook/common/collect/BUCK

{/literal}

Then your build rules would have the following constraints:

-   Rules in `java/com/facebook/base/BUCK` can reference any file under
    `java/com/facebook/base/`.
-   Rules in `java/com/facebook/common/` can reference any files under
    that directory, except for those under
    {sp}`java/com/facebook/common/collect/`, as those \"belong\" to the
    `BUCK` file in the {sp}`collect` directory.

The set of source files accessible to a build file is also known as its
*build package*.

The way to refer to code across build packages is to create build rules
and use `deps` to refer to that code. Going back to the previous
example, suppose code in `java/com/facebook/common/concurrent/` wants to
depend on code in `java/com/facebook/common/collect/`. Presumably
{sp}`java/com/facebook/common/collect/BUCK` has a build rule like:

{literal}

``` {.prettyprint .lang-py}
java_library(
  name = 'collect',
  srcs = glob(['*.java']),
  deps = [
    '//java/com/facebook/base:base',
  ],
)
```

{/literal}

Then `java/com/facebook/common/BUCK` could have a rule like:

{literal}

``` {.prettyprint .lang-py}
java_library(
  name = 'concurrent',
  srcs = glob(['concurrent/*.java']),
  deps = [
    '//java/com/facebook/base:base',
    '//java/com/facebook/common/collect:collect',
  ],
)
```

{/literal} whereas the following **would be invalid** because
{sp}`java/com/facebook/common/collect/` has its own build file, so
`//java/com/facebook/common/collect:concurrent` cannot list
{sp}`java/com/facebook/common/collect/*.java` in its `srcs`. {literal}

``` {.prettyprint .lang-py}
java_library(
  name = 'concurrent',
  srcs = glob(['collect/*.java', 'concurrent/*.java']),
  deps = [
    '//java/com/facebook/base:base',
  ],
)
```

{/literal} {/param} {/call} {/template}
