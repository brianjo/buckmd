/\* \* Copyright (c) Facebook, Inc. and its affiliates. \* \* Licensed
under the Apache License, Version 2.0 (the \"License\"); \* you may not
use this file except in compliance with the License. \* You may obtain a
copy of the License at \* \* http://www.apache.org/licenses/LICENSE-2.0
\* \* Unless required by applicable law or agreed to in writing,
software \* distributed under the License is distributed on an \"AS IS\"
BASIS, \* WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
or implied. \* See the License for the specific language governing
permissions and \* limitations under the License. \*/ {namespace
kotlin_library} /\*\*\*/ {template .soyweb} {call buck.page} {param
title: \'kotlin_library()\' /} {param navid: \'rule_kotlin_library\' /}
{param prettify: true /} {param description} A rule that is used to
define a set of Kotlin files that can be compiled together. {/param}
{param content} {call buck.rule} {param status: \'UNFROZEN\' /} {param
overview} A `kotlin_library()` rule is used to define a set of Kotlin
files that can be compiled together. The main output of a
{sp}`kotlin_library()` rule is a single JAR file containing all of the
compiled class files, as well as the static files specified in the
`resources` argument. {/param} {param args} {call buck.name_arg /} {call
buck.arg} {param name: \'srcs\' /} {param default: \'\[\]\' /} {param
desc} The set of `.kt`, `.java` or `.kts` files to compile for this
rule. If any of the files in this list end in `.src.zip`, then the
entries in the ZIP file that end in `.java` or `.kt` will be included as
ordinary inputs to compilation. {/param} {/call} {call
jvm_common.resources_arg /} {call buck.arg} {param name: \'deps\' /}
{param default: \'\[\]\' /} {param desc} Rules (usually other
`kotlin_library` rules) that are used to generate the classpath required
to compile this `kotlin_library`. {/param} {/call} {call buck.arg}
{param name: \'kotlinc_plugins\' /} {param default: \'\[\]\' /} {param
desc} Use this to specify [Kotlin compiler
plugins](https://kotlinlang.org/docs/reference/compiler-plugins.html) to
use when compiling this library. This takes a list of source paths, each
of which will be prefixed with `-Xplugin=` and passed as extra arguments
to the compiler. Unlike `free_compiler_args`, these can be *source
paths*, not just strings (though `free_compiler_args` should be used to
specify plugin compiler options with `-P`).

For example, if you want to use{sp}
[kotlinx.serialization](https://github.com/Kotlin/kotlinx.serialization)
{sp}with `kotlin_library()`, you need to specify{sp}
`kotlinx-serialization-compiler-plugin.jar` under{sp} `kotlinc_plugins`
and `kotlinx-serialization-runtime.jar`{sp} (which you may have to fetch
from Maven) in your `deps`: {literal}

``` {.prettyprint .lang-py}
kotlin_library(
    name = "example",
    srcs = glob(["*.kt"]),
    deps = [
        ":kotlinx-serialization-runtime",
    ],
    kotlinc_plugins = [
        # Likely copied from your $KOTLIN_HOME directory.
        "kotlinx-serialization-compiler-plugin.jar",
    ],
)

prebuilt_jar(
    name = "kotlinx-serialization-runtime",
    binary_jar = ":kotlinx-serialization-runtime-0.10.0",
)

# Note you probably want to set
# maven_repo=http://jcenter.bintray.com/ in your .buckconfig until
# https://github.com/Kotlin/kotlinx.serialization/issues/64
# is closed.
remote_file(
    name = "kotlinx-serialization-runtime-0.10.0",
    out = "kotlinx-serialization-runtime-0.10.0.jar",
    url = "mvn:org.jetbrains.kotlinx:kotlinx-serialization-runtime:jar:0.10.0",
    sha1 = "23d777a5282c1957c7ce35946374fff0adab114c"
)
```

{/literal} {/param} {/call} {call buck.arg} {param name:
\'free_compiler_args\' /} {param default: \'\[\]\' /} {param desc} A
list of additional compiler arguments. {/param} {/call} {call buck.arg}
{param name: \'all_warnings_as_errors\' /} {param default: \'false\' /}
{param desc} Report an error if there are any warnings. {/param} {/call}
{call buck.arg} {param name: \'suppress_warnings\' /} {param default:
\'false\' /} {param desc} Generate no warnings. {/param} {/call} {call
buck.arg} {param name: \'verbose\' /} {param default: \'false\' /}
{param desc} Enable verbose logging output. {/param} {/call} {call
buck.arg} {param name: \'include_runtime\' /} {param default: \'false\'
/} {param desc} Include Kotlin runtime in to resulting .jar {/param}
{/call} {call buck.arg} {param name: \'jvm_target\' /} {param default:
\'1.6\' /} {param desc} Target version of the generated JVM bytecode
(1.6 or 1.8), default is 1.6 Possible values: \"1.6\", \"1.8\" {/param}
{/call} {call buck.arg} {param name: \'jdk_home\' /} {param default:
\'None\' /} {param desc} Path to JDK home directory to include into
classpath, if differs from default JAVA_HOME {/param} {/call} {call
buck.arg} {param name: \'no_jdk\' /} {param default: \'false\' /} {param
desc} Don\'t include Java runtime into classpath. {/param} {/call} {call
buck.arg} {param name: \'no_stdlib\' /} {param default: \'true\' /}
{param desc} Don\'t include kotlin-stdlib.jar or kotlin-reflect.jar into
classpath. {/param} {/call} {call buck.arg} {param name: \'no_reflect\'
/} {param default: \'true\' /} {param desc} Don\'t include
kotlin-reflect.jar into classpath. {/param} {/call} {call buck.arg}
{param name: \'java_parameters\' /} {param default: \'false\' /} {param
desc} Generate metadata for Java 1.8 reflection on method parameters.
{/param} {/call} {call buck.arg} {param name: \'api_version\' /} {param
default: \'None\' /} {param desc} Allow to use declarations only from
the specified version of bundled libraries. Possible values: \"1.0\",
\"1.1\", \"1.2\", \"1.3\", \"1.4 (EXPERIMENTAL)\". {/param} {/call}
{call buck.arg} {param name: \'language_version\' /} {param default:
\'None\' /} {param desc} Provide source compatibility with specified
language version. Possible values: \"1.0\", \"1.1\", \"1.2\", \"1.3\",
\"1.4 (EXPERIMENTAL)\". {/param} {/call} {call buck.arg} {param name:
\'friend_paths\' /} {param default: \'\[\]\' /} {param desc} List of
source paths to pass into the Kotlin compiler as friend-paths, that is,
modules you can have access to internal methods. {/param} {/call} {call
buck.arg} {param name: \'annotation_processing_tool\' /} {param default
: \'kapt\' /} {param desc} Specifies the tool to use for annotation
processing. Possible values: \"kapt\" or \"javac\". \"kapt\" allows
running Java annotation processors against Kotlin sources while
backporting it for Java sources too. \"javac\" works only against Java
sources, Kotlin sources won\'t have access to generated classes at
compile time. {/param} {/call} {call buck.arg} {param name:
\'kapt_ap_options\' /} {param desc}{literal} Map of annotation processor
options to pass into kapt via the apoptions plugin option. Each entry
should be a key value pair of the processor option and its value.
Default is an empty map. E.g. kapt_ap_options = {
\'someAnnotationOption\': \'someValue\' } More information here:
https://kotlinlang.org/docs/reference/kapt.html{/literal} {/param}
{/call} {call jvm_common.remove_classes_arg /} {call
jvm_common.exported_deps} {param library: \'kotlin_library\' /} {/call}
{call jvm_common.provided_deps} {param binary: \'kotlin_library\' /}
{/call} {call jvm_common.exported_provided_deps /} {call buck.labels_arg
/} {call buck.tests_arg /} {/param} // close args {param examples}
{literal}

``` {.prettyprint .lang-py}
# A rule that compiles a single .kt file.
kotlin_library(
  name = 'JsonUtil',
  srcs = ['JsonUtil.kt'],
  deps = [
    '//third_party/guava:guava',
    '//third_party/jackson:jackson',
  ],
)

# A rule that compiles all of the .kt files under the directory in
# which the rule is defined using glob(). It also excludes an
# individual file that may have additional dependencies, so it is
# compiled by a separate rule.
kotlin_library(
  name = 'messenger',
  srcs = glob(['**/*.kt'], excludes = ['MessengerModule.kt']),
  deps = [
    '//src/com/facebook/base:base',
    '//third_party/guava:guava',
  ],
)

kotlin_library(
  name = 'MessengerModule',
  srcs = ['MessengerModule.kt'],
  deps = [
    '//src/com/facebook/base:base',
    '//src/com/google/inject:inject',
    '//third_party/guava:guava',
    '//third_party/jsr-330:jsr-330',
  ],
)

# A rule that builds a library with both relative and
# fully-qualified deps.
kotlin_library(
  name = 'testutil',
  srcs = glob(['tests/**/*.kt'], excludes = 'tests/**/*Test.kt'),
  deps = [
    ':lib-fb4a',
    '//java/com/facebook/base:base',
  ],
)
```

{/literal} {/param} {/call} // close buck.rule {/param} {/call}
{/template}
