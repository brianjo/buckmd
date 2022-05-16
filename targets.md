/\* \* Copyright (c) Facebook, Inc. and its affiliates. \* \* Licensed
under the Apache License, Version 2.0 (the \"License\"); \* you may not
use this file except in compliance with the License. \* You may obtain a
copy of the License at \* \* http://www.apache.org/licenses/LICENSE-2.0
\* \* Unless required by applicable law or agreed to in writing,
software \* distributed under the License is distributed on an \"AS IS\"
BASIS, \* WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
or implied. \* See the License for the specific language governing
permissions and \* limitations under the License. \*/ {namespace
buck.targets} /\*\*\*/ {template .soyweb} {call buck.page} {param title:
\'buck targets\' /} {param navid: \'command_targets\' /} {param
description} A command that lists all the available build targets in the
current project. {/param} {param content} {call buck.command} {param
overview}

List information about the build targets in the current project.

    buck targets <{call buck.build_target /}> | <{call buck.build_target_pattern /}> ...

The `buck targets` command must take at least one parameter: a {call
buck.build_target /} or {call buck.build_target_pattern /} or a
combination of these.

The following prints all build targets in the project (sorted
alphabetically) to standard out:

    {literal}
    buck targets //...
    {/literal}

You can pass a list of targets to `buck targets`, and Buck prints
information only for those targets. For example, the following command
line prints the target `main` from the `BUCK` file in the root of the
Buck project and all the targets from the `BUCK` file in the
subdirectory `myclass`.

    {literal}
    buck targets //:main //myclass:
    {/literal}

The `buck targets` command is commonly used with the `--show-output`
option to obtain the output paths for the build artifacts for Buck
targets.

    {literal}
    buck targets --show-output //java/com/myproject:binary
    > //java/com/myproject:binary buck-out/gen/java/com/myproject/binary.apk
    {/literal}

{/param} {param params} {call buck.param} {param name: \'type\' /}
{param desc}

The types of target by which to filter. For example:

    {literal}
    buck targets //java/com/myproject/... --type java_test java_binary
    {/literal}

Note that the `--type` parameter comes *after* the specified targets.

This parameter can be handy in programmatic tasks, such as running all
of the Java tests under `//java/com/myproject`:

    {literal}
    buck targets //java/com/myproject/... --type java_test | xargs buck test
    {/literal}

{/param} {/call} {call buck.param} {param name: \'referenced-file\' /}
{param desc}

Filters targets by the list of rules that include the specified file in
their transitive closure.

For example, to run all tests that could be affected by a particular
file, you could use:

    {literal}
    buck targets //java/com/myproject/... --type java_test \
      --referenced-file java/com/example/Foo.java |
      xargs buck test
    {/literal}

{/param} {/call} {call buck.param} {param name: \'json\' /} {param desc}

Print a JSON representation of each target.

In addition, the JSON includes a list of `direct_dependencies` for each
target, which may include additional dependencies for targets whose
descriptions implement `ImplicitDepsInferringDescription`. The fully
qualified names of targets are given.

For example, when resolving a genrule, the direct dependencies includes
both the build targets in `deps` as well as any build targets in a
script associated with the genrule.

{/param} {/call} {call buck.param} {param name: \'output-attributes\' /}
{param desc}

Specify the attributes used in the JSON representation.

If you omit this option, Buck shows all attributes.

{/param} {/call} {call buck.param} {param name: \'print0\' /} {param
desc}

Delimit targets using the ASCII NUL character if `--json` is not
specified. This facilitates use with `xargs`:

    {literal}
    buck targets --print0 | xargs -0 buck build
    {/literal}

{/param} {/call} {call buck.param} {param name: \'resolve-alias\' /}
{param desc}

Print the fully-qualified build target for the specified alias\[es\].
This command also accepts build targets. For more information, see {call
buckconfig.alias /} in the `.buckconfig` documentation.

{/param} {/call} {call command_common.show_output_param /} {call
buck.param} {param name: \'show-rulekey\' /} {param desc}

Print the {call buck.concept_link}{param page: \'rule_keys\' /}{param
name: \'rule keys\' /}{/call}, for the specified targets.

For example, if you have a rule named `main` defined in the build file
in your current directory, the following command prints its rule key.

    {literal}
    buck targets --show-rulekey ':main'
    {/literal}

Note that the rule key for a target is different from the *target hash*
for that target. (See `show-target-hash` below.) Further, the inputs for
the computation of the rule key are *not* a superset of the inputs for
the target hash. For example, the value of the {call
buck.concept_link}{param page: \'Visibility\' /}{param name:
\'visibility\' /}{/call} argument *is not* an input for the rule key but
*is* an input for the target hash.

{/param} {/call} {call buck.param} {param name:
\'show-transitive-rulekeys\' /} {param desc}

When specified in conjunction with `--show-rulekey`, prints the {call
buck.concept_link}{param page: \'rule_keys\' /}{param name: \'rule
keys\' /}{/call} for the specified targets *and their transitive
closure*.

For example, if you have a rule named `main` defined in the build file
in your current directory, the following command prints the rule key for
that rule and the rule keys for all of the rules that are in its
transitive closure.

    {literal}
    buck targets --show-rulekey --show-transitive-rulekeys ':main'
    {/literal}

{/param} {/call} {call buck.param} {param name: \'show-target-hash\' /}
{param desc}

Print each rule\'s target hash after the rule\'s name. Target hashes can
be used to detect which targets are affected when source files in BUCK
files change: if a target is affected, its target hash will be different
after the change from what it was before.

A target hash is created by finding all the transitive dependencies of
the given target and hashing all their attributes and the files they
reference. For more details about how the referenced files are hashed
see the {sp} `--target-hash-file-mode` flag. *The format of the data
that is hashed is undocumented and can change between Buck versions.*

{/param} {/call} {call buck.param} {param name:
\'target-hash-file-mode\' /} {param desc}

Modify how target hashes are computed.

Can be set to either `PATHS_AND_CONTENTS` or {sp}`PATHS_ONLY`.

If set to `PATHS_AND_CONTENTS` (the default), the contents of all files
referenced from the targets will be used to compute the target hash.

If set to {sp} `PATHS_ONLY`, only files\' paths contribute to the hash.
`PATHS_ONLY` will generally be faster because it does not need to read
all of the referenced files, but it will not detect file changes
automatically. See `--target-hash-modified-paths` for another way to
handle changes to referenced files without losing the performance
benefits.

{/param} {/call} {call buck.param} {param name:
\'target-hash-modified-paths\' /} {param desc}

Modify how target hashes are computed.

If a target or its dependencies reference a file from the specified set
of paths, the target\'s hash will be different than if this option had
been omitted. Otherwise, the target\'s hash will be the same as if this
option was omitted.

This option can be used to detect changes in referenced files if the
list of modified files is available from an external source, such as a
source control system.

This option is effective only when {sp} `--target-hash-file-mode` is set
to `PATHS_ONLY`. Otherwise, the actual contents of the files are used to
detect modifications and this option is ignored.

{/param} {/call} {/param} {/call} {/param} // content {/call} //
buck.page {/template}
