/\* \* Copyright (c) Facebook, Inc. and its affiliates. \* \* Licensed
under the Apache License, Version 2.0 (the \"License\"); \* you may not
use this file except in compliance with the License. \* You may obtain a
copy of the License at \* \* http://www.apache.org/licenses/LICENSE-2.0
\* \* Unless required by applicable law or agreed to in writing,
software \* distributed under the License is distributed on an \"AS IS\"
BASIS, \* WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
or implied. \* See the License for the specific language governing
permissions and \* limitations under the License. \*/ {namespace
buck.command.test} /\*\*\*/ {template .soyweb} {call buck.page} {param
title: \'buck test\' /} {param navid: \'command_test\' /} {param
description} A command that builds and runs the tests for one or more
specified targets. {/param} {param content} {call buck.command} {param
overview} Builds and runs the tests for one or more specified targets:

    buck test //javatests/com/example:tests

You can either directly specify test targets, or any other target which
contains a `tests = ['...']` field to specify its tests.

{/param} {param params} {call buck.param} {param name: \'all\' /} {param
desc} Run all tests available in the tree. If no targets are specified,
this is the default. {/param} {/call} {call buck.param} {param name:
\'code-coverage\' /} {param desc} Collects code coverage information
while running tests. Currently, this only works with Java using
[JaCoCo](http://www.eclemma.org/jacoco/). After running:

    buck test --code-coverage

The code coverage information can be found in:

    buck-out/gen/jacoco/code-coverage/

{/param} {/call} {call buck.param} {param name: \'debug\' /} {param
desc} If specified, tests will start suspended and will not run until a
debugger is attached. Tests compatible with JDWP will be listening on
the default port (5005), lldb tests print out a process ID to attach to.
{/param} {/call} {call buck.param} {param name: \'include\' /} {param
desc} Test labels to run with this test. Labels are a way to group
together tests of a particular type and run them together. For example,
a developer could mark all tests that run in less than 100 milliseconds
with the `fast` label, and then use:

    buck test --all --include fast

to run only fast tests. See
[`{sp}   java_test()`](%7BROOT%7Drule/java_test.html) for more details.

Use multiple arguments to match any label, and `+` to match a set of
labels. For example to match all the fast tests that are either stable
or trustworthy, and aren\'t unstable:

    … --include fast+stable fast+trustworthy --exclude fast+unstable

{/param} {/call} {call buck.param} {param name: \'exclude\' /} {param
desc} The inverse of `include`. Labels specified with the exclude option
won\'t be run. For example, if we wanted to run all tests except slow
ones, we would run:

    buck test --all --exclude slow

{/param} {/call} {call buck.param} {param name: \'test-selectors\' /}
{param alias: \'filter\' /} {param desc} Select tests to run by name,
using a `class#method` syntax. All other tests will not be run and test
result caching is disabled:

    buck test --all --test-selectors 'com.example.MyTest#testX'

Matching is done using `java.util.regex` regular expressions, and the
class part (or method) part can be omitted to match all classes (or
methods). Selectors are anchored to the end of each class and/or method
name (i.e. a `$` at the end of your regular expressions is implied.)

    buck test --all --filter 'Foo.*'  # ...every class starting Foo

    buck test --all --filter '#testX' # ...run testX in every class

You can exclude tests with `!`, and if all your test selectors are
exclusive, then the default is to run everything except those tests:

    buck test --all --test-selectors '!MyTest'  # ...all except MyTest

Test selectors can also be read from a file by formatting the command
line argument as {sp}`:/path/to/file`. The file should contain one test
selector per line.

The first matching selector decides whether to include or exclude a
test. The full logic is described in the `--help`. {/param} {/call}
{call buck.param} {param name: \'num-threads\' /} {param desc} The
number of threads that buck should use when executing the build. This
defaults to 1.25 times the number of processors in the system (on
systems with hyperthreading, this means that each core is counted
twice). The number of active threads may not always be equal to this
argument. {/param} {/call} {call buck.param} {param name:
\'ignore-when-dependencies-fail\'/} {param desc} If a library is broken
its tests are probably failing. If another library depends on that
library and its tests are also failing, it is probably because the
dependency has a bug.

For example, if the library `HouseBuilder` depends on {sp}`Bricks` and
the `Bricks` library is broken, it will probably cause its own tests as
well as `HouseBuilder`\'s to fail.

Accordingly, if the libraries are tested respectively by
{sp}`HouseBuilderTest` and `BricksTest`, and both tests fail then only
the error for `BricksTest` is printed; the error for `HouseBuilderTest`
is ignored.

You\'ll still be notified that `HouseBuilderTest` is failing, and
running the tests again without this option will show the cached test
result (and error) in full. {/param} {/call} {call buck.param} {param
name: \'test-runner-env\' /} {param desc} Add or override an environment
variable passed to the test runner. Can be specified multiple times for
different environment variables. Later occurrences override earlier
occurrences. Currently this only support Apple(ios/osx) tests.

        {literal}buck test --test-runner-env FOO=BAR --test-runner-env BAZ=QUUX //some:target{/literal}
        

{/param} {/call} {call buck.param} {param name: \'verbose\' /} {param
alias: \'v\'/} {param desc} How verbose logging to the console should
be, with 1 as the minimum and 10 as the most verbose. {/param} {/call}
{call buck.param} {param name: \'xml\' /} {param desc} If specified,
Buck will write the test results as XML to the location specified. For
example:

    buck test --all --xml testOutput.xml

{/param} {/call} {/param} {/call} {/param} // content {/call} //
buck.page {/template}
