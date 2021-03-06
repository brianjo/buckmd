/\* \* Copyright (c) Facebook, Inc. and its affiliates. \* \* Licensed
under the Apache License, Version 2.0 (the \"License\"); \* you may not
use this file except in compliance with the License. \* You may obtain a
copy of the License at \* \* http://www.apache.org/licenses/LICENSE-2.0
\* \* Unless required by applicable law or agreed to in writing,
software \* distributed under the License is distributed on an \"AS IS\"
BASIS, \* WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
or implied. \* See the License for the specific language governing
permissions and \* limitations under the License. \*/ {namespace
buck.skylark.package_name} /\*\*\*/ {template .soyweb} {call buck.page}
{param title: \'package_name()\' /} {param navid:
\'skylark/generated_package_name\' /} {param prettify: true /} {param
description} The name of the package being evaluated. For example, in
the build file `some/package/BUCK`, its value will be `some/package`. If
the BUCK file calls a function defined in a .bzl file, `package_name()`
will match the caller BUCK file package. This function is equivalent to
the deprecated variable `PACKAGE_NAME`. {/param} {param content} {call
buck.function} {param status: \'UNFROZEN\' /} {param overview} The name
of the package being evaluated. For example, in the build file
`some/package/BUCK`, its value will be `some/package`. If the BUCK file
calls a function defined in a .bzl file, `package_name()` will match the
caller BUCK file package. This function is equivalent to the deprecated
variable `PACKAGE_NAME`. {/param} {/call} {/param} // content {/call}
{/template}
