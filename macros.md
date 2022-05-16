/\* \* Copyright (c) Facebook, Inc. and its affiliates. \* \* Licensed
under the Apache License, Version 2.0 (the \"License\"); \* you may not
use this file except in compliance with the License. \* You may obtain a
copy of the License at \* \* http://www.apache.org/licenses/LICENSE-2.0
\* \* Unless required by applicable law or agreed to in writing,
software \* distributed under the License is distributed on an \"AS IS\"
BASIS, \* WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
or implied. \* See the License for the specific language governing
permissions and \* limitations under the License. \*/ {namespace
buck.macros} /\*\* \* \@param title \* \@param navid \*/ {template
.section}

### {\$title} {#{$navid}}

{/template} /\*\* \* \@param title \*/ {template .code_title}
`{$title}`{style="
      font-weight: bold;
      background: #F0F8FF;
      border: 1px solid #ccc;
      border-radius: 2px;
      padding: 0.5em 0.5em"} {/template} /\*\*\*/ {template .soyweb}
{call buck.page} {param title: \'Macros\' /} {param navid:
\'extending_macros\' /} {param prettify: true /} {param description}
Macros let you define custom rules that map to Buck\'s built-in build
rules. {/param} {param content}

Because build files accept valid Python code, it is possible to define
Python functions that have the side-effect of creating build rules. Such
functions are called *macros*.

**Warning:** Although build files are evaluated as Python and can
therefore perform arbitrary computation---such as writing files and
accessing the network---doing so may cause Buck to fail in peculiar
ways. Therefore, we recommend that you be conservative when using Python
functionality within Buck macros.

{call .section } {param title: \'On this page\' /} {param navid: \'toc\'
/} {/call}

-   [How to define a macro](#defining)
-   [Compound build rules: macros that expand to multiple
    rules](#compound-rules)
-   [How to view expanded macros](#viewing)
-   [Use naming conventions to distinguish macros](#naming)

{call .section } {param title: \'How to define a macro\' /} {param
navid: \'defining\' /} {/call}

We recommend that you define and maintain your macros in files that are
external to your build files. These files must have an extension; we
recommend that you use the extension, `.bzl` (Build
[Zebeline](https://en.wikipedia.org/wiki/Sable#Etymology) Language).

To make your macros accessible to a build file, import them using the
{call buck.fn_load /} function.

In the following example, the macro `java_library_using_guava`, defined
in the file `java_macros.bzl`, creates a build rule named `java_library`
that depends on the Google Guava libraries.

{call .code_title} {param title: \'java_macros.bzl\' /} {/call}
{literal}

``` {.prettyprint .lang-py}
def java_library_using_guava(
    name,
    srcs=[],
    resources=[],
    deps=[],
    visibility=[]):
  java_library(
    name = name,
    srcs = srcs,
    resources = resources,
    deps = [
      # This assumes this is where Guava is in your project.
      '//third_party/java/guava:guava',
    ] + deps,
    visibility = visibility,
  )
```

{/literal}

Instantiating this macro looks the same as defining a built-in build
rule. In the following code, we assume that `java_macros.bzl` is stored
in the subdirectory `libs/java_libs/team_macros`.

{literal}

``` {.prettyprint .lang-py}
#
# load the macro from the external file
#
load("//libs/java_libs/team_macros:java_macros.bzl", "java_library_using_guava")

#
# Calling this function has the side-effect of creating
# a java_library() rule named 'util' that depends on Guava.
#
java_library_using_guava(
  name = 'util',
  # Source code that depends on Guava.
  srcs = glob(['*.java']),
)
```

{/literal}

**Note:** Although, macros can be written in the build file itself, or
imported from separate files using {call buck.fn_include_defs /} or
{sp}{call buckconfig.buildfile_includes /}, we do not recommend any of
these approaches. These approaches make macros more difficult to
maintain and debug---*and they will be deprecated in future versions of
Buck*.

{call .section } {param title: \'Compound build rules: macros that
expand to multiple rules\' /} {param navid: \'compound-rules\' /}
{/call}

You can also create more sophisticated macros that expand into multiple
build rules. For example, you could create a macro that produces rules
for both debug and release versions of an APK:

{literal}

``` {.prettyprint .lang-py}
def create_apks(
    name,
    manifest,
    debug_keystore,
    release_keystore,
    proguard_config,
    deps):

  # This loop will create two android_binary rules.
  for type in [ 'debug', 'release' ]:
    # Select the appropriate keystore.
    if type == 'debug':
      keystore = debug_keystore
    else:
      keystore = release_keystore

    android_binary(
      # Note how we must parameterize the name of the
      # build rule so that we avoid creating two build
      # rules with the same name.
      name = '%s_%s' % (name, type),
      manifest = manifest,
      keystore = keystore,
      package_type = type,
      proguard_config = proguard_config,
      deps = deps,
      visibility = [
        'PUBLIC',
      ],
    )
```

{/literal}

As in the previous example, instantiating this macro *looks* the same as
specifying a single built-in build rule:

{literal}

``` {.prettyprint .lang-py}
create_apks(
  name = 'messenger',
  manifest = 'AndroidManifest.xml',
  debug_keystore = '//keystores:debug',
  release_keystore = '//keystores:prod',
  proguard_config = 'proguard.cfg',
  deps = [
    # ...
  ],
)
{/literal}
```

However, instantiating this macro actually creates *two* build rules.
For example, if you instantiated this macro in the build file,
`apps/messenger/BUCK`, it would create the following rules:

{literal}

    //apps/messenger:messenger_debug
    //apps/messenger:messenger_release

{/literal}

Note, though, that in this scenario, the following is **NOT** a build
rule:

    {literal}
    //apps/messenger:messenger              # MACRO, NOT A RULE
    {/literal}

Therefore, the following commands do not not work, which could be
confusing for developers who don\'t realize that `messenger` is a macro
rather than a rule.

{literal}

    buck build //apps/messenger:messenger    # FAILS
    buck targets --type create_apks          # FAILS

{/literal} {call .section } {param title: \'How to view expanded
macros\' /} {param navid: \'viewing\' /} {/call}

To view a build file with all macros expanded, use {call
buck.cmd_link}{param name: \'audit\' /}{/call}. The following invocation
of `buck audit` would show the debug and release rules from the
preceding example, but not the macro that created them.

    {literal}
    buck audit rules //apps/messenger
    {/literal}

{call .section } {param title: \'Use naming conventions to distinguish
macros\' /} {param navid: \'naming\' /} {/call}

You can create naming conventions for your macros to help your
developers distinguish them from built-in rules. For example, you could
prefix your macros with the name of your company. On the other hand,
part of the beauty of macros is that they are as familiar to use as
built-in rules. How you communicate macros to your team is up to you.

{/param} {/call} {/template}
