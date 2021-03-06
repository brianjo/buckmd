/\* \* Copyright (c) Facebook, Inc. and its affiliates. \* \* Licensed
under the Apache License, Version 2.0 (the \"License\"); \* you may not
use this file except in compliance with the License. \* You may obtain a
copy of the License at \* \* http://www.apache.org/licenses/LICENSE-2.0
\* \* Unless required by applicable law or agreed to in writing,
software \* distributed under the License is distributed on an \"AS IS\"
BASIS, \* WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
or implied. \* See the License for the specific language governing
permissions and \* limitations under the License. \*/ {namespace
buck.skylark.provider} /\*\*\*/ {template .soyweb} {call buck.page}
{param title: \'provider()\' /} {param navid:
\'skylark/generated_provider\' /} {param prettify: true /} {param
description} Creates a declared provider \'constructor\'. The return
value of this function can be used to create \"struct-like\" values.
Example:\

``` language-python
data = provider()
      d = data(x = 2, y = 3)
      print(d.x + d.y) # prints 5
```

{/param} {param content} {call buck.function} {param status:
\'UNFROZEN\' /} {param overview} Creates a declared provider
\'constructor\'. The return value of this function can be used to create
\"struct-like\" values. Example:\

``` language-python
data = provider()
          d = data(x = 2, y = 3)
          print(d.x + d.y) # prints 5
```

{/param} {param args} {call buck.functionArg} {param name : \'doc\' /}
{param desc } A description of the provider that can be extracted by
documentation generating tools. {/param} {param default : \'\\\'\\\'\'
/} {/call} {call buck.functionArg} {param name : \'fields\' /} {param
desc } If specified, restricts the set of allowed fields.\
Possible values are:

-   list of fields:\

    ``` language-python
    provider(fields = ['a', 'b'])
    ```

-   dictionary field name -\> documentation:\

    ``` language-python
    provider(
                                         fields = {lb} 'a' : 'Documentation for a', 'b' : 'Documentation for b' {rb})
    ```

All fields are optional. {/param} {param default : \'None\' /} {/call}
{/param} {/call} {/param} // content {/call} {/template}
