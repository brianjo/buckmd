/\* \* Copyright (c) Facebook, Inc. and its affiliates. \* \* Licensed
under the Apache License, Version 2.0 (the \"License\"); \* you may not
use this file except in compliance with the License. \* You may obtain a
copy of the License at \* \* http://www.apache.org/licenses/LICENSE-2.0
\* \* Unless required by applicable law or agreed to in writing,
software \* distributed under the License is distributed on an \"AS IS\"
BASIS, \* WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
or implied. \* See the License for the specific language governing
permissions and \* limitations under the License. \*/ {namespace
buck.visibility} /\*\*\*/ {template .soyweb} {call buck.page} {param
title: \'Visibility\' /} {param navid: \'concept_visibility\' /} {param
prettify: true /} {param description} Determines whether a build rule
can include a build target in its list of dependencies. {/param} {param
content}

Visibility determines whether a build rule can include a build target in
its list of `deps`. In a large project, you may want to prevent
developers from \"reaching across\" the project and pulling in
additional code. Reducing the visibility of build rules can help prevent
that type of behavior.

There are two types of visibility attributes available, each of which
takes a list of {sp}[build target
patterns](%7BROOT%7Dconcept/build_target_pattern.html): `visibility`,
which determines what other targets can depend on a target, and
`within_view`, which determines what other targets a target can depend
on.

Both attributes act as allowlists, with some exceptions. In general, if
a target is not listed, there may be no dependency relationship. If the
`within_view` list is empty or unset, however, its check is bypassed.
Similarly, targets defined in the same build file always act as if they
were members of their siblings\' `visibility` lists.

There is also a special value, `'PUBLIC'`, which makes a build rule
visible to all other rules. `'PUBLIC'` is valid in `visibility` but not
`within_view`.

In case of logically-conflicting lists, `within_view` takes precedence
over `visibility`. If `//foo:bar` defines `//hello:world` in its
`visibility` list, but `//hello:world` does not define `//foo:bar` in
its `within_view` list, then `//hello:world` may not depend on
`//foo:bar`.

## Examples

A common library like Guava should be able to be included by any build
rule:

{literal}

``` {.prettyprint .lang-py}
prebuilt_jar(
  name = 'guava',
  binary_jar = 'guava-14.0.1.jar',
  visibility = [
    'PUBLIC',
  ],
)
```

{/literal}

It is common to restrict the visibility of Android resources to the Java
code that uses it:

{literal}

``` {.prettyprint .lang-py}
android_resource(
  name = 'ui_res',
  res = 'res',
  package = 'com.example',
  visibility = [
    '//java/com/example/ui:ui',
  ],
)
```

{/literal}

Or it may be simpler to make it visible to the entire directory in case
additional build rules are added to `java/com/example/ui/BUCK`:

{literal}

``` {.prettyprint .lang-py}
android_resource(
  name = 'ui_res',
  res = 'res',
  package = 'com.example',
  visibility = [
    '//java/com/example/ui:',
  ],
)
```

{/literal}

Also, it is common to limit code for testing to be visible only to
tests. If you define all of your Java unit tests in a folder named
{sp}`javatests/` in the root of your project, then you could define the
following rule to ensure that only allow build rules under `javatests/`
can depend on JUnit:

{literal}

``` {.prettyprint .lang-py}
prebuilt_jar(
  name = 'junit',
  binary_jar = 'junit-4.11.jar',
  visibility = [
    '//javatests/...',
  ],
)
```

{/literal}

Finally, restricting the view of a target can be useful for preventing
dependency creep:

{literal}

``` {.prettyprint .lang-py}
java_library(
  name = 'example',
  visibility = [
    'PUBLIC',
  ],
  within_view = [
    '//foo:bar',
    '//hello:world',
  ],
)
```

{/literal} {/param} {/call} {/template}
