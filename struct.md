/\* \* Copyright (c) Facebook, Inc. and its affiliates. \* \* Licensed
under the Apache License, Version 2.0 (the \"License\"); \* you may not
use this file except in compliance with the License. \* You may obtain a
copy of the License at \* \* http://www.apache.org/licenses/LICENSE-2.0
\* \* Unless required by applicable law or agreed to in writing,
software \* distributed under the License is distributed on an \"AS IS\"
BASIS, \* WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
or implied. \* See the License for the specific language governing
permissions and \* limitations under the License. \*/ {namespace
buck.skylark.struct} /\*\*\*/ {template .soyweb} {call buck.page} {param
title: \'struct()\' /} {param navid: \'skylark/generated_struct\' /}
{param prettify: true /} {param description} Creates an immutable struct
using the keyword arguments as attributes. It is used to group multiple
values and/or functions together. Example:\

``` language-python
s = struct(x = 2, y = 3)
      return s.x + getattr(s, "y")  # returns 5
```

{/param} {param content} {call buck.function} {param status:
\'UNFROZEN\' /} {param overview} Creates an immutable struct using the
keyword arguments as attributes. It is used to group multiple values
and/or functions together. Example:\

``` language-python
s = struct(x = 2, y = 3)
          return s.x + getattr(s, "y")  # returns 5
```

{/param} {param args} {call buck.functionArg} {param name : \'kwargs\'
/} {param desc } the struct attributes. {/param} {param default :
\'None\' /} {/call} {/param} {/call} {/param} // content {/call}
{/template}
