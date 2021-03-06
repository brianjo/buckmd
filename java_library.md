/\* \* Copyright (c) Facebook, Inc. and its affiliates. \* \* Licensed
under the Apache License, Version 2.0 (the \"License\"); \* you may not
use this file except in compliance with the License. \* You may obtain a
copy of the License at \* \* http://www.apache.org/licenses/LICENSE-2.0
\* \* Unless required by applicable law or agreed to in writing,
software \* distributed under the License is distributed on an \"AS IS\"
BASIS, \* WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
or implied. \* See the License for the specific language governing
permissions and \* limitations under the License. \*/ {namespace
java_library} /\*\*\*/ {template .soyweb} {call buck.page} {param title:
\'java_library()\' /} {param navid: \'rule_java_library\' /} {param
prettify: true /} {param description} A rule that is used to define a
set of Java files that can be compiled together. {/param} {param
content} {call buck.rule} {param status: \'FROZEN\' /} {param overview}
A `java_library()` rule defines a set of Java files that can be compiled
together. The main output of a {sp}`java_library()` rule is a single JAR
file containing all of the compiled class files, as well as the static
files specified in the `resources` argument. {/param} {param args} {call
buck.name_arg /} {call buck.arg} {param name: \'srcs\' /} {param
default: \'\[\]\' /} {param desc} The set of `.java` files to compile
for this rule. If any of the files in this list end in `.src.zip`, then
the entries in the ZIP file that end in `.java` will be included as
ordinary inputs to compilation. This is common when using a {call
buck.genrule /} to auto-generate some Java source code that needs to be
compiled with some hand-written Java code. {/param} {/call} {call
jvm_common.resources_arg /} {call buck.arg} {param name: \'deps\' /}
{param default: \'\[\]\' /} {param desc} Rules (usually other
`java_library` rules) that are used to generate the classpath required
to compile this `java_library`. {/param} {/call} {call buck.arg} {param
name: \'source\' /} {param default: \'\' /} {param desc} Specifies the
version of Java (as a string) to interpret source files as. Overrides
the value in \"source_level\" in the \"java\" section of
[`.buckconfig`](%7BROOT%7Dconcept/buckconfig.html). {/param} {/call}
{call buck.arg} {param name: \'target\' /} {param default: \'\' /}
{param desc} Specifies the version of Java (as a string) for which to
generate code. Overrides the value in \"target_level\" in the \"java\"
section of [`.buckconfig`](%7BROOT%7Dconcept/buckconfig.html). {/param}
{/call} {call buck.arg} {param name: \'java_version\' /} {param default:
\'\' /} {param desc} Equivalent to setting both `source` and `target   `
to the given value. Setting this and `source`{sp} or `target` (or both!)
is an error. {/param} {/call} {call buck.arg} {param name: \'javac\' /}
{param default: \'\' /} {param desc} Specifies the Java compiler program
to use for this rule. The value is a source path (e.g., //foo/bar:bar).
Only one of \"javac\" and \"javac_jar\" may be set for a given rule.
Overrides the value in \"javac\" in the \"tools\" section of
[`.buckconfig`](%7BROOT%7Dconcept/buckconfig.html). {/param} {/call}
{call buck.arg} {param name: \'javac_jar\' /} {param default: \'\' /}
{param desc} Specifies the Java compiler program to use for this rule.
The value is a source path (e.g., //foo/bar:bar). Only one of
\"javac_jar\" and \"javac\" may be set for a given rule. Overrides the
value in \"javac_jar\" in the \"tools\" section of
[`.buckconfig`](%7BROOT%7Dconcept/buckconfig.html). {/param} {/call}
{call jvm_common.compiler_class_name_arg /} {call buck.arg} {param name:
\'extra_arguments\' /} {param default: \'\[\]\' /} {param desc} List of
additional arguments to pass into the Java compiler. These arguments
follow the ones specified in
[`.buckconfig`](%7BROOT%7Dconcept/buckconfig.html). {/param} {/call}
{call jvm_common.remove_classes_arg /} {call jvm_common.exported_deps}
{param library: \'java_library\' /} {/call} {call
jvm_common.provided_deps} {param binary: \'java_library\' /} {/call}
{call jvm_common.exported_provided_deps /} {call
jvm_common.abi_generation_mode /} {call jvm_common.source_only_abi_deps
/} {call jvm_common.required_for_source_only_abi /} {call
jvm_common.on_unused_dependencies /} {call buck.tests_arg /} {/param} //
close args {param examples} {literal}

``` {.prettyprint .lang-py}
# A rule that compiles a single .java file.
java_library(
  name = 'JsonUtil',
  srcs = ['JsonUtil.java'],
  deps = [
    '//third_party/guava:guava',
    '//third_party/jackson:jackson',
  ],
)

# A rule that compiles all of the .java files under the directory in
# which the rule is defined using glob(). It also excludes an
# individual file that may have additional dependencies, so it is
# compiled by a separate rule.
java_library(
  name = 'messenger',
  srcs = glob(['**/*.java'], excludes = ['MessengerModule.java']),
  deps = [
    '//src/com/facebook/base:base',
    '//third_party/guava:guava',
  ],
)

java_library(
  name = 'MessengerModule',
  srcs = ['MessengerModule.java'],
  deps = [
    '//src/com/facebook/base:base',
    '//src/com/google/inject:inject',
    '//third_party/guava:guava',
    '//third_party/jsr-330:jsr-330',
  ],
)

# A rule that builds a library with both relative and
# fully-qualified deps.
java_library(
  name = 'testutil',
  srcs = glob(['tests/**/*.java'], excludes = 'tests/**/*Test.java'),
  deps = [
    ':lib-fb4a',
    '//java/com/facebook/base:base',
  ],
)
```

{/literal} {/param} {/call} // close buck.rule {/param} {/call}
{/template}
