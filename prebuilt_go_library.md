/\* \* Copyright (c) Facebook, Inc. and its affiliates. \* \* Licensed
under the Apache License, Version 2.0 (the \"License\"); \* you may not
use this file except in compliance with the License. \* You may obtain a
copy of the License at \* \* http://www.apache.org/licenses/LICENSE-2.0
\* \* Unless required by applicable law or agreed to in writing,
software \* distributed under the License is distributed on an \"AS IS\"
BASIS, \* WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
or implied. \* See the License for the specific language governing
permissions and \* limitations under the License. \*/ {namespace
prebuilt_go_library} /\*\*\*/ {template .soyweb} {call buck.page} {param
title: \'prebuilt_go_library()\' /} {param navid:
\'rule_prebuilt_go_library\' /} {param prettify: true /} {param
description} A prebuilt_go_library() rule provides a Go linkable
archive. {/param} {param content} {call buck.rule} {param status:
\'UNFROZEN\' /} {param overview}

A prebuilt_go_library() rule provides a native library from the
specified file.

{call go_common.supported_language_version /}

{/param} {param args} {call buck.name_arg /} {call buck.arg} {param
name: \'library\' /} {param desc} Path to the precompiled Go library -
typically of the form \'foo.a\'. {/param} {/call} {call
go_common.package_name_arg /} {call go_common.deps_arg /} {/param} //
close args {param examples} {call go_common.more_examples /} {literal}

``` {.prettyprint .lang-py}
prebuilt_go_library(
  name='greeting',
  package_name='greeting',
  library='greeting.a',
  deps=[
    ':join',
  ],
)
```

{/literal} {/param} {/call} // close buck.rule {/param} {/call}
{/template}
