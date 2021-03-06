/\* \* Copyright (c) Facebook, Inc. and its affiliates. \* \* Licensed
under the Apache License, Version 2.0 (the \"License\"); \* you may not
use this file except in compliance with the License. \* You may obtain a
copy of the License at \* \* http://www.apache.org/licenses/LICENSE-2.0
\* \* Unless required by applicable law or agreed to in writing,
software \* distributed under the License is distributed on an \"AS IS\"
BASIS, \* WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
or implied. \* See the License for the specific language governing
permissions and \* limitations under the License. \*/ {namespace
buck.subdir_glob} /\*\*\*/ {template .soyweb} {call buck.page} {param
title: \'subdir_glob()\' /} {param navid: \'function_subdir_glob\' /}
{param prettify: true /} {param description} The subdir_glob() function
is useful for defining header maps for C/C++ libraries which should be
relative the given sub-directory. {/param} {param content} {call
buck.function} {param status: \'UNFROZEN\' /} {param overview}

The `subdir_glob()` function is useful for defining header maps for
C/C++ libraries which should be relative the given sub-directory. Given
a list of tuples, the form of (relative-sub-directory, glob-pattern),
return a dict of sub-directory relative paths to full paths.

Please refer to `{call buck.fn_glob /}` for explanations and examples of
the pattern.

{/param} {param args} {call buck.functionArg} {param name :
\'glob_specs\' /} {param desc} The array of tuples in form of
(relative-sub-directory, glob-pattern inside relative-sub-directory).
{/param} {/call} {call buck.functionArg} {param name : \'excludes\' /}
{param default : \'\[\]\' /} {param desc} A list of patterns to identify
files that should be removed from the set specified by the first
argument. {/param} {/call} {call buck.functionArg} {param name :
\'prefix\' /} {param default : \'None\' /} {param desc} If is not
`None`, prepends it to each key in the dictionary. {/param} {/call}
{/param} {param examples} Given this `exported_headers` description:
{literal}

``` {.prettyprint .lang-py}
exported_headers = subdir_glob([
    ("lib/source", "video/**/*.h"),
    ("lib/source", "audio/**/*.h"),
  ],
  excludes = [
    "lib/source/video/codecs/*.h",
  ],
  prefix = "MediaLib/")
```

{/literal} It will map the following on disk directory structure below
to the following includes: {literal}

``` {.prettyprint .lang-cpp}
lib/
  source/
    video/
      converter/
        converter.h   ->   #include "MediaLib/video/converter/converter.h"
      player/
        player.h      ->   #include "MediaLib/video/player/player.h"
      codecs/
        codec1.h      ->   not includable - defined in `excludes`
        codec2.h      ->   not includable - defined in `excludes`
    audio/
      codecs/
        codec1.h      ->   #include "MediaLib/audio/codecs/codec1.h"
        codec2.h      ->   #include "MediaLib/audio/codecs/codec2.h"
      player/
        player.h      ->   #include "MediaLib/audio/player/player.h"
    internal/
      otherheader.h   ->   not includable
```

{/literal} {/param} {/call} // buck.function {/param} // content {/call}
{/template}
