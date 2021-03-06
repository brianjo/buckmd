/\* \* Copyright (c) Facebook, Inc. and its affiliates. \* \* Licensed
under the Apache License, Version 2.0 (the \"License\"); \* you may not
use this file except in compliance with the License. \* You may obtain a
copy of the License at \* \* http://www.apache.org/licenses/LICENSE-2.0
\* \* Unless required by applicable law or agreed to in writing,
software \* distributed under the License is distributed on an \"AS IS\"
BASIS, \* WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
or implied. \* See the License for the specific language governing
permissions and \* limitations under the License. \*/ {namespace
buck.index} /\*\*\*/ {template .soyweb} {call buck.page} {param navid:
\'home\' /} {param title: \'A fast build tool\' /} {param description}
Buck is a build system developed and used by Facebook. It encourages the
creation of small, reusable modules consisting of code and resources,
and supports a variety of languages. {/param} {param content}

Buck is a build system developed and used by Facebook. It encourages the
creation of small, reusable modules consisting of code and resources,
and supports a variety of languages on many platforms.

## Why Buck?

Buck can help you and your team in many ways:

-   **Speed up your builds.** Buck builds independent artifacts in
    parallel to take advantage of multiple cores on your machine.
    Further, it reduces incremental build times by keeping track of
    unchanged modules so that the minimal set of modules is rebuilt.
-   **Add reproducibility to your builds.** Buck only uses the declared
    inputs, which means everybody gets the same results.
-   **Get correct incremental builds.** Buck looks at the contents of
    your inputs, not their timestamps to figure out what needs to be
    built. As a result, incremental builds should always be correct, so
    there\'s no need to perform a clean build.
-   **Understand your dependencies.** With {sp}{call
    buck.cmd_link}{param name: \'query\' /}{/call}, you can better
    understand your dependencies and what is required to build your
    product.
-   **Integrate with your IDE.** With {sp}{call buck.cmd_link}{param
    name: \'project\' /}{/call}, your project can be better understood
    by your IDE, making you and your team more productive.

{/param} {/call} {/template}
