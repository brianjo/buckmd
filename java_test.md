/\* \* Copyright (c) Facebook, Inc. and its affiliates. \* \* Licensed
under the Apache License, Version 2.0 (the \"License\"); \* you may not
use this file except in compliance with the License. \* You may obtain a
copy of the License at \* \* http://www.apache.org/licenses/LICENSE-2.0
\* \* Unless required by applicable law or agreed to in writing,
software \* distributed under the License is distributed on an \"AS IS\"
BASIS, \* WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
or implied. \* See the License for the specific language governing
permissions and \* limitations under the License. \*/ {namespace
java_test} /\*\*\*/ {template .soyweb} {call buck.page} {param title:
\'java_test()\' /} {param navid: \'rule_java_test\' /} {param prettify:
true /} {param description} A rule that is used to define a set of Java
files that contain tests. {/param} {param content} {call buck.rule}
{param status: \'FROZEN\' /} {param overview} A `java_test()` rule is
used to define a set of {sp}`.java` files that contain tests to run via
JUnit. {/param} {param args} {call buck.name_arg /} {call buck.arg}
{param name: \'srcs\' /} {param default : \'\[\]\' /} {param desc} Like
[`java_library()`](java_library.html), all of the `.java` files
specified by the {sp}`srcs` argument will be compiled when this rule is
built. In addition, all of the corresponding `.class`{sp} files that are
built by this rule will be passed as arguments to JUnit when this rule
is run as a test. `.class` files that are passed to JUnit that do not
have any methods annotated with {sp}`@Test` are considered failed tests,
so make sure that only test case classes are specified as `srcs`. This
is frequently done by specifying `srcs` as
{sp}{literal}`glob(['**/*Test.java'])`{/literal}. {/param} {/call} {call
buck.arg} {param name: \'resources\' /} {param default : \'\[\]\' /}
{param desc} Same as [`java_library()`](java_library.html). {/param}
{/call} {call buck.test_label_arg /} {call buck.arg} {param name:
\'source\' /} {param default : \'\\\'6\\\'\' /} {param desc} Java
language level for compiling. Corresponds to the {sp}`-source` argument
for `javac`. {/param} {/call} {call buck.arg} {param name: \'target\' /}
{param default : \'\\\'6\\\'\' /} {param desc} Bytecode target level for
compiling. Corresponds to the {sp}`-target` argument for `javac`.
{/param} {/call} {call buck.arg} {param name: \'deps\' /} {param default
: \'\[\]\' /} {param desc} Same as
[`java_library()`](java_library.html). // org.junit.rules.Timeout was
not introduced until 4.7. Must include JUnit (version 4.7 or later) as a
dependency for JUnit tests. Must include TestNG (version 6.2 or later)
and hamcrest as a dependencies for TestNG tests. {/param} {/call} {call
buck.arg} {param name: \'test_type\' /} {param default : \'junit\' /}
{param desc} Specifies which test framework to use. The currently
supported options are \'junit\' and \'testng\'. {/param} {/call} {call
buck.run_test_separately_arg /} {call buck.fork_mode /} {call
buck.test_rule_timeout_ms /} {call buck.arg} {param name:
\'std_out_log_level\' /} {param default : \'FINE\' /} {param desc} Log
level for messages from the source under test that buck will output to
std out.

Value must be a valid `java.util.logging.Level` value.

{/param} {/call} {call buck.arg} {param name: \'std_err_log_level\' /}
{param default : \'WARNING\' /} {param desc} Same as
`std_out_log_level`, but for std err. {/param} {/call} {call buck.arg}
{param name: \'use_cxx_libraries\' /} {param default: \'False\' /}
{param desc} Whether or not to build and link against {call
buck.cxx_library /} dependencies when testing. {/param} {/call} {call
buck.arg} {param name: \'cxx_library_whitelist\' /} {param default:
\'\[\]\' /} {param status: \'FROZEN\' /} {param desc} EXPERIMENTAL. List
of cxx_libraries to build, if use_cxx_libraries is true. This can be
useful if some dependencies are Android-only and won\'t build on the
default platform. {/param} {/call} {call test_common.contacts_arg /}
{call buck.arg} {param name: \'vm_args\' /} {param default : \'\[\]\' /}
{param desc} Runtime arguments to the JVM running the tests. {/param}
{/call} {call jvm_common.test_env /} {/param} // close args {/call} //
close buck.rule {/param} {/call} {/template}
