/\* \* Copyright (c) Facebook, Inc. and its affiliates. \* \* Licensed
under the Apache License, Version 2.0 (the \"License\"); \* you may not
use this file except in compliance with the License. \* You may obtain a
copy of the License at \* \* http://www.apache.org/licenses/LICENSE-2.0
\* \* Unless required by applicable law or agreed to in writing,
software \* distributed under the License is distributed on an \"AS IS\"
BASIS, \* WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
or implied. \* See the License for the specific language governing
permissions and \* limitations under the License. \*/ {namespace
zip_file} /\*\*\*/ {template .soyweb} {call buck.page} {param title:
\'zip_file()\' /} {param navid: \'rule_zip_file\' /} {param prettify:
true /} {param description} A rule that is used to create a zip file as
its output. {/param} {param content} {call buck.rule} {param status:
\'UNFROZEN\' /} {param overview} A `zip_file()` allows builds to create
basic zip files in a platform-agnostic way. {/param} {param args} {call
buck.name_arg /} {call buck.arg} {param name: \'out\' /} {param default:
\'name.zip\' /} {param desc} The name of the zip file that should be
generated. This allows builds to use a meaningful target name coupled
with a meaningful zip file name. The default value takes the rule\'s
`name` and appends `.zip`. {/param} {/call} {call buck.arg} {param name:
\'srcs\' /} {param desc} The set of files to include in the zip.

Each `src` will be added to the zip as follows:

-   If the `src` is the output of another rule, the output will be
    included using just the output\'s file name.
-   If the `src` is a file relative to the rule\'s declaration, it will
    be included in the zip with its relative file name.

{/param} {/call} {call buck.arg} {param name: \'zip_srcs\' /} {param
default : \'\[\]\' /} {param desc} The set of zip files whose content to
include in the output zip file.

Note that the order of files in `zip_srcs` matters because the same zip
entry can be included from multiple files. See the `on_duplicate_entry`
argument to learn how to control the behavior when there are multiple
entries with the same name. The entries from `zip_srcs` are added before
files from `srcs`. {/param} {/call} {call buck.arg} {param name:
\'entries_to_exclude\' /} {param default : \'\[\]\' /} {param desc} List
of regex expressions that describe entries that should not be included
in the output zip file.

The regexes must be defined using `java.util.regex.Pattern` syntax.
{/param} {/call} {call buck.arg} {param name: \'on_duplicate_entry\' /}
{param default : \'overwrite\' /} {param desc} Action performed when
Buck detects that zip_file input contains multiple entries with the same
name.

The valid values are:

-   `overwrite` (default): the last entry overwrites all previous
    entries with the same name.
-   `append`: all entries are added to the output file.
-   `fail`: fail the build when duplicate entries are present.

{/param} {/call} {/param} // close args {param examples}

This example will create a simple zip file.

{literal}

``` {.prettyprint .lang-py}
zip_file(
  # The output will be "example.zip"
  name = 'example',
  srcs = 
    # These files will be found in the zip under "dir/"
    glob(['dir/**/*']) +
    [
      # Imagine this generates the output 
      # "buck-out/gen/foo/hello.txt". This output will 
      # be found in the zip at "hello.txt"
      '//some/other:target',
  
    ],
  zip_srcs = [
     # The contents of this zip will be added to the generated zip.
    'amazing-library-1.0-sources.zip',
  ],
  entries_to_exclude = [
    "com/example/amazinglibrary/Source1.java",
  ],
)
```

{/literal} If you were to examine the generated zip, the contents would
look something like (assuming the output of \"`//some/other:target`\"
was a file who\'s path ended with {sp}`hello.txt`, the \"`dir`\" glob
found two files, and \"`amazing-library-1.0-sources.zip`\" contained two
Java source files): {literal}

    dir/file1.txt
    dir/subdir/file2.txt
    hello.txt
    com/example/amazinglibrary/Source2.java

{/literal} {/param} {/call} // close buck.rule {/param} {/call}
{/template}
