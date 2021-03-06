/\* \* Copyright (c) Facebook, Inc. and its affiliates. \* \* Licensed
under the Apache License, Version 2.0 (the \"License\"); \* you may not
use this file except in compliance with the License. \* You may obtain a
copy of the License at \* \* http://www.apache.org/licenses/LICENSE-2.0
\* \* Unless required by applicable law or agreed to in writing,
software \* distributed under the License is distributed on an \"AS IS\"
BASIS, \* WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
or implied. \* See the License for the specific language governing
permissions and \* limitations under the License. \*/ {namespace
http_archive} /\*\*\*/ {template .soyweb} {call buck.page} {param title:
\'http_archive()\' /} {param navid: \'rule_http_archive\' /} {param
prettify: true /} {param description} A rule that is used to download
and extract archives from the Internet to be used as dependencies of
other rules. {/param} {param content} {call buck.rule} {param status:
\'UNFROZEN\' /} {param overview} An `http_archive()` rule is used to
download and extract archives from the Internet to be used as
dependencies for other rules. These rules are downloaded by running
{call buck.cmd_fetch /}, or can be downloaded as part of {call
buck.cmd_build /} by setting {call buckconfig.download_in_build /}
{/param} {param args} {call remote_common.name_arg }{param rule:
\'http_archive\' /}{/call} {call remote_common.urls_arg /} {call
remote_common.sha256_arg /} {call buck.arg} {param name: \'out\' /}
{param example : \'foo\' /} {param default: \'None\' /} {param desc} An
optional name to call the directory that the downloaded artifact is
extracted into. Buck will generate a default name if one is not provided
that uses the `name` of the rule. {/param} {/call} {call buck.arg}
{param name: \'strip_prefix\' /} {param example: \'foobar-0.1.2\' /}
{param default: \'None\' /} {param desc} If set, files under this path
will be extracted to the root of the output directory. Siblings or
cousins to this prefix will not be extracted at all.\
\
For example, if a tarball has the layout:

-   foo/bar/bar-0.1.2/data.dat
-   foo/baz/baz-0.2.3
-   foo_prime/bar-0.1.2

Only `data.dat` will be extracted, and it will be extracted into the
output directory specified in??{call buck.ruleLink}{param name:
\'http_archive\' /}{param section: \'out\' /}{/call}. {/param} {/call}
{call buck.arg} {param name: \'type\' /} {param example: \'tar.gz\' /}
{param default: \'None\' /} {param desc} Normally, archive type is
determined by the file\'s extension. If `type` is set, then
autodetection is overriden, and the specified type is used instead.\
\
Supported values are: `zip`, `tar`, `tar.gz`, `tar.bz2`, `tar.xz`, and
`tar.zst`. {/param} {/call} {/param} // close args {param examples}

Using `http_archive()`, third party packages can be downloaded from an
`https` URL and used in other library types.

{literal}

``` {.prettyprint .lang-py}
http_archive(
  name = 'thrift-archive',
  urls = [
    'https://internal-mirror.example.com/bin/thrift-compiler-0.1.tar.gz.badextension',
  ],
  sha256 = '7baa80df284117e5b945b19b98d367a85ea7b7801bd358ff657946c3bd1b6596',
  type='tar.gz',
  strip_prefix='thrift-compiler-0.1'
)

genrule(
  name = 'thrift-compiler-bin',
  out = 'thrift',
  cmd = 'cp $(location :thrift-archive)/bin/thrift $OUT',
)

genrule(
  name="my-thrift-lib-cpp2",
  cmd="$(exe :thrift-compiler-bin) --gen cpp2 -o $OUT $(location //:thrift-file)",
  out="gen-cpp2",
)
```

{/literal} {/param} // close examples {/call} // close buck.rule
{/param} {/call} {/template}
