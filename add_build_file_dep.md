/\* \* Copyright (c) Facebook, Inc. and its affiliates. \* \* Licensed
under the Apache License, Version 2.0 (the \"License\"); \* you may not
use this file except in compliance with the License. \* You may obtain a
copy of the License at \* \* http://www.apache.org/licenses/LICENSE-2.0
\* \* Unless required by applicable law or agreed to in writing,
software \* distributed under the License is distributed on an \"AS IS\"
BASIS, \* WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
or implied. \* See the License for the specific language governing
permissions and \* limitations under the License. \*/ {namespace
buck.add_build_file_dep} /\*\*\*/ {template .soyweb} {call buck.page}
{param title: \'add_build_file_dep()\' /} {param navid:
\'function_add_build_file_dep\' /} {param prettify: true /} {param
description} The add_build_file_dep() function is used mark a parse-time
dependency from a build file onto another file. {/param} {param content}
{call buck.function} {param status: \'FROZEN\' /} {param overview} The
`add_build_file_dep()` function is used to mark a parse-time dependency
onto another file, to make sure the Buck\'s internal caches invalidate
build files correctly if that file is modified. {/param} {param args}
{call buck.functionArg} {param desc} The first and only argument is a
path. As with {call buck.fn_load /} and {call buck.fn_include_defs /},
it looks similar to a build target because it starts with {sp}`//`
(indicating the root of the project), but is not a proper build target
because it identifies a file relative to the root of the project rather
than a build rule. {/param} {/call} {/param} {/call} // buck.function
{/param} // content {/call} {/template}
