/\* \* Copyright (c) Facebook, Inc. and its affiliates. \* \* Licensed
under the Apache License, Version 2.0 (the \"License\"); \* you may not
use this file except in compliance with the License. \* You may obtain a
copy of the License at \* \* http://www.apache.org/licenses/LICENSE-2.0
\* \* Unless required by applicable law or agreed to in writing,
software \* distributed under the License is distributed on an \"AS IS\"
BASIS, \* WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
or implied. \* See the License for the specific language governing
permissions and \* limitations under the License. \*/ {namespace
remote_file} /\*\*\*/ {template .soyweb} {call buck.page} {param title:
\'remote_file()\' /} {param navid: \'rule_remote_file\' /} {param
prettify: true /} {param description} A rule that is used to download
files from the Internet to be used as dependencies of other rules.
{/param} {param content} {call buck.rule} {param status: \'UNFROZEN\' /}
{param overview} A `remote_file()` rule is used to download files from
the Internet to be used as dependencies for other rules. These rules are
downloaded by running {call buck.cmd_fetch /}, or can be downloaded as
part of {call buck.cmd_build /}. See the note there about the
{sp}`.buckconfig` setting to configure that. {/param} {param args} {call
buck.name_arg /} {call buck.arg} {param name: \'url\' /} {param desc}
You can specify an `http`, `https`, or a `mvn` URL. If you specify a
`mvn` URL, it will be decoded as described in the {sp}[javadocs for
MavenUrlDecoder](%7BROOT%7Djavadoc/com/facebook/buck/file/MavenUrlDecoder.html).
See the example section below. {/param} {/call} {call buck.arg} {param
name: \'sha1\' /} {param desc} The [`SHA-1`](//wikipedia.org/wiki/SHA-1)
hash of the downloaded artifact. Buck verifies this is correct and fails
the fetch command if it doesn\'t match in order to guarantee repeatable
builds. {/param} {/call} {call buck.arg} {param name: \'out\' /} {param
default: \'None\' /} {param desc} An optional name to call the
downloaded artifact. Buck will generate a default name if one is not
provided that uses the `name` of the rule. {/param} {/call} {call
buck.arg} {param name: \'type\' /} {param default: \'data\' /} {param
desc} An optional type of the downloaded file.

`data`
:   Regular data file.

`executable`
:   Executable file. Buck will ensure that output has appropriate
    permissions if applicable.

`exploded_zip`
:   Zip archive which will be automatically unzipped into an output
    directory.

{/param} {/call} {/param} // close args {param examples}

Here\'s an example of a `remote_file()` using an `https` URL.

{literal}

``` {.prettyprint .lang-py}
remote_file(
  name = 'android-ndk-r10e-darwin-x86_64',
  url = 'https://dl.google.com/android/ndk/android-ndk-r10e-darwin-x86_64.bin',
  sha1 = 'b57c2b9213251180dcab794352bfc9a241bf2557',
)
```

{/literal}

Here\'s an example of a `remote_file()` using a `mvn` URL being
referenced by a {call buck.prebuilt_jar /}.

{literal}

``` {.prettyprint .lang-py}
prebuilt_jar(
  name = 'jetty-all',
  binary_jar = 'jetty-all-9.2.10.v20150310.jar',
  source_jar = ':jetty-source',
)

remote_file(
  name = 'jetty-source',
  out = 'jetty-all-9.2.10.v20150310-sources.jar',
  url = 'mvn:org.eclipse.jetty.aggregate:jetty-all:src:9.2.10.v20150310',
  sha1 = '311da310416d2feb3de227081d7c3f48742d7075',
)
```

{/literal}

Here\'s an example of a `remote_file()` using a `mvn` URI which uses a
non-default maven repository host.

{literal}

``` {.prettyprint .lang-py}
remote_file(
  name = 'jetty-source',
  out = 'jetty-all-9.2.10.v20150310-sources.jar',
  url = 'mvn:https://maven-repo.com:org.eclipse.jetty.aggregate:jetty-all:src:9.2.10.v20150310',
  sha1 = '311da310416d2feb3de227081d7c3f48742d7075',
)
```

{/literal}

Here\'s an example of a `remote_file()` using a `mvn` URI which uses a
Maven classifier.

{literal}

``` {.prettyprint .lang-py}
remote_file(
  name = 'groovy-groovysh-indy',
  out = 'jetty-all-9.2.10.v20150310-sources.jar',
  url = 'mvn:org.codehaus.groovy:groovy-groovysh:jar:indy:2.4.1',
  sha1 = '1600fde728c885cc9506cb102deb1b494bd7c130',
)
```

{/literal} {/param} {/call} // close buck.rule {/param} {/call}
{/template}
