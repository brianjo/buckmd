/\* \* Copyright (c) Facebook, Inc. and its affiliates. \* \* Licensed
under the Apache License, Version 2.0 (the \"License\"); \* you may not
use this file except in compliance with the License. \* You may obtain a
copy of the License at \* \* http://www.apache.org/licenses/LICENSE-2.0
\* \* Unless required by applicable law or agreed to in writing,
software \* distributed under the License is distributed on an \"AS IS\"
BASIS, \* WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
or implied. \* See the License for the specific language governing
permissions and \* limitations under the License. \*/ {namespace
buck.faq} /\*\* \* \@param id attribute for this blob of HTML so users
can link to an individual FAQ. We should make \* an effort to keep these
identifiers stable to avoid breaking links. Therefore, when choosing \*
an id, try to make it generic enough so that it is forward-compatible.
\* \@param question Question. \* \@param shortAnswer Try to keep this to
a one-liner. \* \@param? longAnswer This portion of the answer can
include more detail. \*/ {template .faq}

::: {#{$id|id} .{css .faq}}
::: {.{css .faq_q}}
Q: {\$question}
:::

::: {.{css .faq_a}}
A: {\$shortAnswer\|noAutoescape} {if \$longAnswer}

{\$longAnswer\|noAutoescape} {/if}
:::
:::

{/template} /\*\*\*/ {template .soyweb} {call buck.page} {param title:
\'FAQ\' /} {param navid: \'concept_faq\' /} {param description} Frequent
questions and answers about Buck. {/param} {param content} {call .faq}
{param id: \'why-is-it-called-buck\' /} {param question} Why is it
called Buck? {/param} {param shortAnswer} The word \"buck\" is similar
to the word \"build\" and is quick to type. It also has awesome mascot
potential. {/param} {/call} {call .faq} {param id:
\'why-is-buck-built-with-ant\' /} {param question} Why is Buck built
with Ant instead of Buck? {/param} {param shortAnswer} Self-hosting
systems can be more difficult to maintain and debug. {/param} {param
longAnswer} If Buck built itself using Buck, then every time a change
was made to Buck\'s source, the commit would have to include a new Buck
binary that included that change. It would be easy to forget to include
the binary, difficult to verify that it was the correct binary, and
wasteful to bloat the Git history of the repository with binaries that
could be rebuilt from source. Building Buck using Ant ensures we are
always building from source, which is simpler to verify.

Also, because Ant is a more mature build system than Buck, it has
support for features that we have not had time to include in Buck yet,
such as generating Javadoc, static analysis via
[PMD](http://pmd.sourceforge.net/), Python unit tests, etc.

That said, as a sanity check, Buck is capable of building itself. Once
you build Buck using Ant, you can re-build Buck using Buck by running
`./bin/buck build buck`. {/param} {/call} {/param} {/call} {/template}
