/\* \* Copyright (c) Facebook, Inc. and its affiliates. \* \* Licensed
under the Apache License, Version 2.0 (the \"License\"); \* you may not
use this file except in compliance with the License. \* You may obtain a
copy of the License at \* \* http://www.apache.org/licenses/LICENSE-2.0
\* \* Unless required by applicable law or agreed to in writing,
software \* distributed under the License is distributed on an \"AS IS\"
BASIS, \* WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
or implied. \* See the License for the specific language governing
permissions and \* limitations under the License. \*/ {namespace
buck.skylark.dummy} /\*\*\*/ {template .soyweb} {call buck.page} {param
title: \'dummy()\' /} {param navid: \'skylark/generated_dummy\' /}
{param prettify: true /} {param description} Returns a dummy list of
strings. {/param} {param content} {call buck.function} {param status:
\'UNFROZEN\' /} {param overview} Returns a dummy list of strings.
{/param} {param args} {call buck.functionArg} {param name : \'kwargs\'
/} {param desc } the dummy attributes. {/param} {param default :
\'None\' /} {/call} {/param} {/call} {/param} // content {/call}
{/template}
