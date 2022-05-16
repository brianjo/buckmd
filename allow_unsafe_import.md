/\* \* Copyright (c) Facebook, Inc. and its affiliates. \* \* Licensed
under the Apache License, Version 2.0 (the \"License\"); \* you may not
use this file except in compliance with the License. \* You may obtain a
copy of the License at \* \* http://www.apache.org/licenses/LICENSE-2.0
\* \* Unless required by applicable law or agreed to in writing,
software \* distributed under the License is distributed on an \"AS IS\"
BASIS, \* WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
or implied. \* See the License for the specific language governing
permissions and \* limitations under the License. \*/ {namespace
buck.allow_unsafe_import} /\*\*\*/ {template .soyweb} {call buck.page}
{param title: \'allow_unsafe_import()\' /} {param navid:
\'function_allow_unsafe_import\' /} {param prettify: true /} {param
description} When build file sandboxing is enabled,
allow_unsafe_import() function may be used to create a context that
lifts the module importing restrictions. {/param} {param content} {call
buck.function} {param status: \'FROZEN\' /} {param overview} Buck has
restrictions on importing arbitrary Python modules in {call
buck.build_file /}s which make it harder to accidentally violate
assumptions about determinism of {call buck.build_file /}s and build
rules. The `allow_unsafe_import()` function may be used to create a
context that lifts the restrictions on module importing.

**Using this function should be avoided**, and done carefully when
necessary. Buck\'s internal caches invalidate build files based on known
inputs, and using arbitrary Python code can introduce nondeterministic
behavior or inputs that Buck won\'t know about.

### Whitelist and safe versions

Some modules can be imported in a normal way (without using
`allow_unsafe_import()`) because they were whitelisted or a safe version
was configured. After checking if they are safe to use in build files,
more modules (e.g. local ones) can be added to the whitelist using
[`build_file_import_whitelist`](%7BROOT%7Dconcept/buckconfig.html#project.build_file_import_whitelist)
config setting.

  --------------- -------------------------------------------------------------------------------------------------------------------
  **Whitelist**   copy, re, functools, itertools, json, hashlib, types, string, ast, \_\_future\_\_, collections, operator, fnmatch
  --------------- -------------------------------------------------------------------------------------------------------------------

In the safe versions of modules only selected parts can be used.

  ------------- ------------------------------------------------------------------------------------------------------------
  **Module**    **Available parts**
  **os**        environ, getenv, path, sep, pathsep, linesep
  **os.path**   basename, commonprefix, dirname, isabs, join, normcase, relpath, split, splitdrive, splitext, sep, pathsep
  **pipes**     quote
  ------------- ------------------------------------------------------------------------------------------------------------

{/param} {param examples} Buck has no way to know if the results of
uncontrolled file system or network access change, and will not
reevaluate the build file if that happens. {literal}

``` {.prettyprint .lang-py}
import copy # whitelisted
import os   # safe version will be imported
with allow_unsafe_import():
    from os.path import isfile
    import httplib

# Warning! Buck will not detect that the existence of file A affects
# the results of the parsing. The build file will not be processed
# again when A is added/removed.
if isfile(A):
    foo()
else:
    bar()
```

{/literal} {/param} {/call} // buck.function {/param} // content {/call}
{/template}
