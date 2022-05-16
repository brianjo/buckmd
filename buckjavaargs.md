/\* \* Copyright (c) Facebook, Inc. and its affiliates. \* \* Licensed
under the Apache License, Version 2.0 (the \"License\"); \* you may not
use this file except in compliance with the License. \* You may obtain a
copy of the License at \* \* http://www.apache.org/licenses/LICENSE-2.0
\* \* Unless required by applicable law or agreed to in writing,
software \* distributed under the License is distributed on an \"AS IS\"
BASIS, \* WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
or implied. \* See the License for the specific language governing
permissions and \* limitations under the License. \*/ {namespace
buck.buckjavaargs} /\*\*\*/ {template .soyweb} {call buck.header} {param
title: \'.buckjavaargs\' /} {param navid: \'buckjavaargs\' /} {param
description} An optional file that specifies additional java command
line arguments to pass to Buck. {/param} {/call}

::: {.{css .overview}}
The root of your project may contain a configuration file named
`.buckjavaargs`. If present, Buck will read this file and append any
flags specified in it when launching its java process. Note the flags
are only used when launching the main Buck java process, and not any
other java tools Buck will invoke. The content of this file is split
into individual arguments according to the rules of Python\'s
`shlex.split`. On POSIX systems, Bourne shell quoting rules apply.

Here are some examples of why you would want to use `.buckjavaargs`.

To specify a larger heap size:

{literal}

    -Xmx2g

{/literal}

To ensure you can talk to the Maven Central Repo on a machine that uses
IPv6:

{literal}

    -Djava.net.preferIPv6Addresses=true

{/literal}
:::

// close overview {call buck.footer} {param navid: \'buckjavaargs\' /}
{/call} {/template}
