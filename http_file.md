/\* \* Copyright (c) Facebook, Inc. and its affiliates. \* \* Licensed
under the Apache License, Version 2.0 (the \"License\"); \* you may not
use this file except in compliance with the License. \* You may obtain a
copy of the License at \* \* http://www.apache.org/licenses/LICENSE-2.0
\* \* Unless required by applicable law or agreed to in writing,
software \* distributed under the License is distributed on an \"AS IS\"
BASIS, \* WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
or implied. \* See the License for the specific language governing
permissions and \* limitations under the License. \*/ {namespace
http_file} /\*\*\*/ {template .soyweb} {call buck.page} {param title:
\'http_file()\' /} {param navid: \'rule_http_file\' /} {param prettify:
true /} {param description} A rule that is used to download files from
the Internet to be used as dependencies of other rules. {/param} {param
content} {call buck.rule} {param status: \'UNFROZEN\' /} {param
overview} An `http_file()` rule is used to download files from the
Internet to be used as dependencies for other rules. This rule only
downloads single files, and can optionally make them executable (see
{call buck.ruleLink}{param name: \'http_file\' /} {param section:
\'executable\' /}{/call}) These rules are downloaded by running {call
buck.cmd_fetch /}, or can be downloaded as part of {call buck.cmd_build
/} by setting {call buckconfig.download_in_build /} {/param} {param
args} {call remote_common.name_arg }{param rule: \'http_file\' /}{/call}
{call remote_common.urls_arg /} {call remote_common.sha256_arg /} {call
buck.arg} {param name: \'out\' /} {param example : \'foo.exe\' /} {param
default: \'None\' /} {param desc} An optional name to call the
downloaded artifact. Buck will generate a default name if one is not
provided that uses the `name` of the rule. {/param} {/call} {call
buck.arg} {param name: \'executable\' /} {param example: \'true\' /}
{param desc} Whether or not the file should be made executable after
downloading. If true, this can also be used via {call buck.cmd_run /}
and the?? `$(exe )`??{call buck.string_parameter_macros /} {/param}
{/call} {/param} // close args {param examples}

Using `http_file()`, third party packages can be downloaded from an
`https` URL and used in java libraries.

{literal}

``` {.prettyprint .lang-py}
http_file(
  name = 'guava-23-bin',
  urls = [
    'http://search.maven.org/remotecontent?filepath=com/google/guava/guava/23.0/guava-23.0.jar',
  ],
  sha256 = '7baa80df284117e5b945b19b98d367a85ea7b7801bd358ff657946c3bd1b6596',
)
http_file(
  name = 'guava-23-sources',
  urls = [
    'http://search.maven.org/remotecontent?filepath=com/google/guava/guava/23.0/guava-23.0-sources.jar',
  ],
  sha256 = '37fe8ba804fb3898c3c8f0cbac319cc9daa58400e5f0226a380ac94fb2c3ca14',
)

prebuilt_java_library(
  name = 'guava-23',
  binary_jar = ':guava-23-bin',
  source_jar = ':guava-23-source',
)
```

{/literal}

Tooling can also be fetched with `http_file()` and used by a {call
buck.genrule /}.

{literal}

``` {.prettyprint .lang-py}
genrule(
  name="my-thrift-lib-cpp2",
  cmd="$(exe :thrift-compiler-bin) --gen cpp2 -o $OUT $(location //:thrift-file)",
  out="gen-cpp2",
)

http_file(
  name = 'thrift-compiler-bin',
  url = 'https://internal-mirror.example.com/bin/thrift-compiler',
  sha256 = 'c24932ccabb66fffb2d7122298f7f1f91e0b1f14e05168e3036333f84bdf58dc',
)
```

{/literal}

Here\'s an example of a `http_file()` using a mvn URI which uses a Maven
classifier.

{literal}

``` {.prettyprint .lang-py}
http_file(
  name = 'guava-23-bin',
  urls = [
    'mvn:com.google.guava:guava:jar:23.0',
  ],
  sha256 = '7baa80df284117e5b945b19b98d367a85ea7b7801bd358ff657946c3bd1b6596',
)
```

{/literal} {/param} {/call} // close buck.rule {/param} {/call}
{/template}
