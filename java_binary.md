/\* \* Copyright (c) Facebook, Inc. and its affiliates. \* \* Licensed
under the Apache License, Version 2.0 (the \"License\"); \* you may not
use this file except in compliance with the License. \* You may obtain a
copy of the License at \* \* http://www.apache.org/licenses/LICENSE-2.0
\* \* Unless required by applicable law or agreed to in writing,
software \* distributed under the License is distributed on an \"AS IS\"
BASIS, \* WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
or implied. \* See the License for the specific language governing
permissions and \* limitations under the License. \*/ {namespace
java_binary} /\*\*\*/ {template .soyweb} {call buck.page} {param title:
\'java_binary()\' /} {param navid: \'rule_java_binary\' /} {param
prettify: true /} {param description} A rule that is used to create a
JAR file of the compiled .class files and resources of the
java_library() rules on which it depends. {/param} {param content} {call
buck.rule} {param status: \'FROZEN\' /} {param overview} A
`java_binary()` rule is used to create a JAR file of the compiled .class
files and resources of the `java_library()` {sp}rules on which it
depends. {/param} {param args} {call buck.arg} {param name: \'name\' /}
{param desc} The *short name* for this {call buck.build_target /}. Also,
the name of the generated JAR file. {/param} {/call} {call buck.arg}
{param name: \'deps\' /} {param default : \'\[\]\' /} {param desc} Rules
(normally of type `java_library`) that should be compiled and whose
`.class` files and resources should be included in the generated JAR
file. {/param} {/call} {call buck.arg} {param name: \'main_class\' /}
{param default: \'None\' /} {param desc} If provided, this will be the
value specified as the {sp}`Main-Class` attribute of the
`META-INF/MANIFEST.MF` {sp}file in the generated JAR file. Also, when
this rule is used as an executable in a [`genrule()`](genrule.html),
{sp}`main_class` will indicate the class whose `main()`{sp} method will
be invoked to process the command-line arguments. This is consistent
with the expected usage of `java -jar   <name.jar> <args>`. {/param}
{/call} {call buck.arg} {param name: \'manifest_file\' /} {param
default: \'None\' /} {param desc} If provided, this manifest will be
used when generating the JAR file. If combined with `main_class`, the
specified manifest file will be used but the `main_class` will override
the main class in the manifest. {/param} {/call} {call buck.arg} {param
name: \'meta_inf_directory\' /} {param default: \'None\' /} {param desc}
Note: This has beta support currently. If provided, the contents in this
directory will end up in the {sp}`META-INF` directory inside the
generated JAR file. {/param} {/call} {call buck.arg} {param name:
\'blacklist\' /} {param default: \'\[\]\' /} {param desc} A list of
patterns that identify files to exclude from the final generated JAR
file. Example:

{literal}

``` {.prettyprint .lang-py}
java_binary(
  name = 'example',
  blacklist = [
    # Excludes com.example.A and com.example.Alligator,
    # as well as their inner classes and any non-class files that happen to match
    # the pattern
    'com.example.A',

    # Excludes all files from org/slf4j/**/*.
    'org.slf4j',
  ],
  deps = [
    ':example1',
    ':third-party-stuff',
  ],
)
```

{/literal} {/param} {/call} {call buck.tests_arg /} {/param} // close
args {/call} // close buck.rule {/param} {/call} {/template}
