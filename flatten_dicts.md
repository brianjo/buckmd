/\* \* Copyright (c) Facebook, Inc. and its affiliates. \* \* Licensed
under the Apache License, Version 2.0 (the \"License\"); \* you may not
use this file except in compliance with the License. \* You may obtain a
copy of the License at \* \* http://www.apache.org/licenses/LICENSE-2.0
\* \* Unless required by applicable law or agreed to in writing,
software \* distributed under the License is distributed on an \"AS IS\"
BASIS, \* WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
or implied. \* See the License for the specific language governing
permissions and \* limitations under the License. \*/ {namespace
buck.flatten_dicts} /\*\*\*/ {template .soyweb} {call buck.page} {param
title: \'flatten_dicts()\' /} {param navid: \'function_flatten_dicts\'
/} {param prettify: true /} {param description} The flatten_dicts()
function is used to merge a list of maps together. {/param} {param
content} {call buck.function} {param status: \'FROZEN\' /} {param
overview} The `flatten_dicts()` function is used to merge a list of
dicts together. It is useful for sharing a set of defaults across
different build rules while allowing for customization. You will
probably want to use it in conjunction with `include_defs()` in order to
easily share configurations between your BUCK files. {/param} {param
args} {call buck.functionArg} {param desc} The function takes a varargs
of dictionaries, with the lowest-priority dictionary first. {/param}
{/call} {/param} {param examples} {literal}

``` {.prettyprint .lang-py}
default_config = {
  'a': 'bar',
  'b': false,
}

flatten_dicts(
  default_config,
  dict(a='foo', c=[])
)
# Outputs
# {
#   'a': 'foo',
#   'b': false,
#   'c': [],
# }
```

{/literal} Values in dictionaries which appear later in the list have
priority over values which appear earlier. {/param} {/call} //
buck.function {/param} // content {/call} {/template}
