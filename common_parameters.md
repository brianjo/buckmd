/\* \* Copyright (c) Facebook, Inc. and its affiliates. \* \* Licensed
under the Apache License, Version 2.0 (the \"License\"); \* you may not
use this file except in compliance with the License. \* You may obtain a
copy of the License at \* \* http://www.apache.org/licenses/LICENSE-2.0
\* \* Unless required by applicable law or agreed to in writing,
software \* distributed under the License is distributed on an \"AS IS\"
BASIS, \* WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
or implied. \* See the License for the specific language governing
permissions and \* limitations under the License. \*/ {namespace
buck.commonparameters} /\*\* \* \@param value The numeric value for the
verbosity level. \* \@param bool The Java boolean function for the
verbosity level. \* \@param description A description of what the
verbosity level means. \*/ {template .verbose_levels}

`{$value}`{.not-inline}

`{$bool}`{.not-inline}

{\$description\|noAutoescape}

{/template} /\*\*\*/ {template .soyweb} {call buck.page} {param title:
\'Common Parameters\' /} {param navid: \'command_common_parameters\' /}
{param description} Command-line parameters that affect all commands.
{/param} {param content} {call buck.command} {param overview}

This topic describes command-line parameters that affect the operation
of Buck itself and that are available irrespective of which subcommand
(`build`, `run`, `test`, etc) you invoke.

{/param} {param params} {call buck.param} {param name: \'verbose\' /}
{param desc}

Set the verbosity level of the console output. The verbosity level is a
single numeric value between `1` and `8`{sp} inclusive. For example:

    {literal}
    buck targets --verbose 8
    {/literal}

Higher verbosity levels include all the output of lower levels.

The output that Buck produces is affected by factors in addition to the
verbosity level. Such factors include the subcommand (`build`,
`install`, `test`, etc), the types of rules being built, and the degree
to which artifacts from previous builds have been cached.

Buck has not yet implemented differences between all levels. For
example, there are currently no differences in verbosity between levels
`5` and `7` inclusive.

Numeric level

Boolean function

Description

{call .verbose_levels} {param value: \'1\' /} {param bool:
\'shouldPrintStandardInformation()\' /} {param description} Print
warnings from build steps and summary information for tests. {/param}
{/call} {call .verbose_levels} {param value: \'2\' /} {param bool:
\'shouldPrintBinaryRunInformation()\' /} {param description} Print
additional output for generated binaries or tests. {/param} {/call}
{call .verbose_levels} {param value: \'3\' /} {param bool:
\'shouldPrintCommand()\' /} {param description} Print commands that Buck
runs during the build process. {/param} {/call} {call .verbose_levels}
{param value: \'4\' /} {param bool: \'shouldPrintSelectCommandOutput()\'
/} {param description} Print output for selected commands that Buck
runs. {/param} {/call} {call .verbose_levels} {param value: \'5 - 7\' /}
{param bool: \'shouldPrintOutput()\' /} {param description} Print output
for all commands that Buck runs. {/param} {/call} {call .verbose_levels}
{param value: \'8\' /} {param bool:
\'shouldUseVerbosityFlagIfAvailable()\' /} {param description} Print all
available diagnostic/logging information. {/param} {/call} {/param}
{/call}

For more precise information about how a particular verbosity level
affects output, you can search the Buck source code for the
corresponding boolean function. For example:

    {literal}
    grep --recursive "getVerbosity().shouldPrintOutput()" ~/local/buck/src
    {/literal}

{call buck.param} {param name: \'no-cache\' /} {param desc}

Disable the build artifact caches. If this parameter is specified, Buck
ignores any artifacts in any of the caches specified in the {call
buckconfig.cache /} section of `.buckconfig`. These include the
filesystem cache (`dir`), remote cache (`http`), and SQLite cache
(`sqlite`).

The contents of the caches are unaffected, but Buck does not use them
for the specified command.

Note that if there is an output file in the `buck-out` directory for a
previously-built and unchanged rule, Buck still uses that output file in
your build---even if `--no-cache` is specified. If you don\'t want Buck
to use these (valid) build artifacts, run the {call buck.cmd_link}{param
name: \'clean\' /}{/call} command before your build to delete them from
`buck-out`.

{/param} {/call} {call buck.param} {param name: \'config\' /} {param
desc}

Specify configuration settings or override existing settings in {call
buck.buckconfig_link /}. For example:

    {literal}
    buck build --config cache.mode=dir //java/com/example/app:amazing
    {/literal}

The `--config` parameter can be abbreviated as `-c`.

You can specify the `--config` parameter multiple times on the same
command line. Note, however, that if the same configuration option is
specified more than once, Buck uses the last value specified (\"last
write wins\"). For example, the following invocation of `buck build`
builds the `//:prod` target, rather than the `//:dev` target, which was
specified earlier on the command line. (The example uses the
abbreviated, `-c`, version of the parameter.)

    {literal}
    #
    # Build for development? 
    #
    # No, build for production.
    #
    buck build -c 'alias.main=//:dev' -c 'alias.main=//:prod' main
    {/literal}

The preferred method of overriding values in `.buckconfig` is by using a
`.buckconfig.local` file. Overriding values of `.buckconfig` from the
command line can make it difficult to reproduce builds.

{/param} {/call} {call buck.param} {param name: \'config-file\' /}
{param desc}

Specify build-configuration settings in a file that uses the same syntax
as {call buck.buckconfig_link /}. For example:

    {literal}
    buck build --config-file debug.buckconfig
    {/literal}

The `--config-file` parameter provides functionality similar to
`--flagfile` (see below), but with `.buckconfig` syntax rather than
command-line parameter syntax.

Any values specified using `--config-file` override values specified in
`.buckconfig` and `.buckconfig.local`.

You can specify the path to the configuration file in one of three ways.

##### Use a path that is relative to the directory that contains the current cell\'s `.buckconfig`.

    {literal}
    --config-file relative/path/to/file.buckconfig
    {/literal}

##### Use a path that is relative to the directory that contains a *specified* cell\'s `.buckconfig`.

    {literal}
    --config-file <cell name>//path/to/file.buckconfig
    {/literal}

##### Use an absolute path from the root of your file system.

    {literal}
    --config-file /absolute/path/to/file.buckconfig
    {/literal}

You can also specify a particular cell to which to apply the
configuration. By default, the settings in the configuration file apply
to *all* cells in the current build.

##### Apply the configuration only to the *current* cell.

    {literal}
    --config-file //=<path-to-config-file>
    {/literal}

##### Apply the configuration only to a *specified* cell.

    {literal}
    --config-file <target-cell>=<path-to-config-file>
    {/literal}

If you specify `*` as the target cell, the configuration is applied to
*all* the cells in the build. This is the default, but this syntax
enables you to be explicit.

To learn more about Buck\'s concept of cells, see the {sp}{call
buck.key_concepts_link}{param rendered_text: \'Key Concepts\'
/}{/call}{sp} topic.

{/param} {/call} {call buck.param} {param name: \'num-threads\' /}
{param desc}

Specify the number of threads that buck uses when executing jobs. The
default value is 1.25 times the number of *logical*{sp} cores in the
system; on systems with hyperthreading, this means that each physical
core is counted as two logical cores. You can also set the number of
threads to use for building by adding a `threads` key to the{sp}
`[build]` section of the `.buckconfig` file.

The order of precedence for setting the number of build threads (from
highest to lowest) is:

1.  The `--num-threads` command-line parameter.
2.  The `.buckconfig` setting.
3.  The default value (see above).

The number of *active* threads might not always be equal to this
argument.

{/param} {/call} {call buck.param} {param name: \'\--flagfile
/path/to/commandline-args or @/path/to/commandline-args\' /} {param
nodash: true /} {param desc}

Specify additional command-line arguments in external files (*flag
files*), one argument per line. The arguments in these files can
themselves be `--flagfile` or `@` arguments, which would then include
the additional specified file\'s contents as arguments.

``` {.prettyprint .lang-ini}
{literal}
# File config/common
--verbose
{/literal}
```

``` {.prettyprint .lang-ini}
{literal}
# File config/gcc
@config/common
--config
cxx.cxx=/usr/bin/g++
...
{/literal}
```

``` {.prettyprint .lang-ini}
{literal}
# File config/clang
@config/common
--config
cxx.cxx=/usr/bin/clang++
...
{/literal}
```

``` {.prettyprint .lang-ini}
{literal}
buck build @config/gcc foo/bar:
buck build @config/clang foo/bar:
{/literal}
```

Lines in flag files must not have any leading or trailing white space.

The equals sign (`=`) separates the specified property and value. There
should be no white space between the property and the equals sign, nor
between the equals sign and the value.

We recommend that you use `--flagfile` rather than the{sp} `@` symbol as
`--flagfile` is more self-describing.

This `--config-file` parameter (described earlier) provides
functionality similar to `--flagfile`, but with `.buckconfig` syntax
rather than command-line parameter syntax.

If Buck is regularly invoked with different sets of arguments, we
recommend that you use flag files or config files, as they can be stored
in source control, which makes builds more reproducible.

{/param} {/call} {/param} {/call} {/param} // content {/call} //
buck.page {/template}
