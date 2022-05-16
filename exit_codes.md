/\* \* Copyright (c) Facebook, Inc. and its affiliates. \* \* Licensed
under the Apache License, Version 2.0 (the \"License\"); \* you may not
use this file except in compliance with the License. \* You may obtain a
copy of the License at \* \* http://www.apache.org/licenses/LICENSE-2.0
\* \* Unless required by applicable law or agreed to in writing,
software \* distributed under the License is distributed on an \"AS IS\"
BASIS, \* WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
or implied. \* See the License for the specific language governing
permissions and \* limitations under the License. \*/ {namespace
buck.exitcodes} /\* \* These exit codes are defined in the following
source file. \* \* src/com/facebook/buck/util/ExitCode.java \*/ /\*\* \*
\@param value The numeric value of the error code. \* \@param enum The
Java enum for the error code. \* \@param description A description of
what the error-code means. \*/ {template .exit_codes}

`{$value}`{.not-inline}

`{$enum}`{.not-inline}

{\$description\|noAutoescape}

{/template} /\*\*\*/ {template .soyweb} {call buck.page} {param title:
\'Exit Codes\' /} {param navid: \'command_exit_codes\' /} {param
description} Exit codes that are returned from a Buck command to the
shell. {/param} {param content}

These exit codes are returned from a Buck command to the shell when the
command exits.

These exit codes are Buck\'s *binary protocol* for interacting with
other software such as shell scripts.

Note that in the case of some fatal errors---such as `FATAL_OOM`,
`FATAL_IO`, or `FATAL_DISK_FULL`---Buck itself might not be able to
*reliably* detect the source of the failure. If this occurs, Buck falls
back to reporting `FATAL_GENERIC`.

/\* \* Non-fatal generic errors 1-9 \*/ {call .exit_codes} {param value:
\'0\' /} {param enum: \'SUCCESS\' /} {param description} The command
returned successfully. No errors. No warnings. {/param} {/call} {call
.exit_codes} {param value: \'1\' /} {param enum: \'BUILD_ERROR\' /}
{param description} Build resulted in a non-specific user error.
{/param} {/call} {call .exit_codes} {param value: \'2\' /} {param enum:
\'BUSY\' /} {param description} Buck daemon is busy processing another
command. For more information, see {call buck.cmd_link}{param name:
\'buckd\' /}{param rendered_text: \'**Buck Daemon (buckd)**\' /}{/call}.
{/param} {/call} {call .exit_codes} {param value: \'3\' /} {param enum:
\'COMMANDLINE_ERROR\' /} {param description} Incorrect user-supplied
command-line options. For more information, see {call
buck.cmd_link}{param name: \'common_parameters\' /}{param rendered_text:
\'**Common Parameters**\' /}{/call} or the topic page for the specific
command that you executed. {/param} {/call} {call .exit_codes} {param
value: \'4\' /} {param enum: \'NOTHING_TO_DO\' /} {param description}
Nothing to build or evaluate for the specified command. {/param} {/call}
{call .exit_codes} {param value: \'5\' /} {param enum: \'PARSE_ERROR\'
/} {param description} Error in parsing the build file or in
constructing the target or action graph. {/param} {/call} {call
.exit_codes} {param value: \'6\' /} {param enum: \'RUN_ERROR\' /} {param
description} Failure while running a binary or installing a binary on a
device. For more information, see {call buck.cmd_link}{param name:
\'run\' /}{/call}. {/param} {/call} /\* \* Fatal errors 10-19 \*/ {call
.exit_codes} {param value: \'10\' /} {param enum: \'FATAL_GENERIC\' /}
{param description} Generic non-recoverable internal error. {/param}
{/call} {call .exit_codes} {param value: \'11\' /} {param enum:
\'FATAL_BOOTSTRAP\' /} {param description} Non-recoverable error in Buck
bootstrapper. {/param} {/call} {call .exit_codes} {param value: \'12\'
/} {param enum: \'FATAL_OOM\' /} {param description} Non-recoverable
out-of-memory (OOM) error. {/param} {/call} {call .exit_codes} {param
value: \'13\' /} {param enum: \'FATAL_IO\' /} {param description}
Generic non-recoverable I/0 error. {/param} {/call} {call .exit_codes}
{param value: \'14\' /} {param enum: \'FATAL_DISK_FULL\' /} {param
description} No space on storage device. {/param} {/call} /\* \* Other
non-fatal errors 20 - 127 \*/ {call .exit_codes} {param value: \'32\' /}
{param enum: \'TEST_ERROR\' /} {param description} Test run had
user-specific test errors. For more information, see {call
buck.cmd_link}{param name: \'test\' /}{/call}. {/param} {/call} {call
.exit_codes} {param value: \'64\' /} {param enum: \'TEST_NOTHING\' /}
{param description} There were no tests to run. For more information,
see {call buck.cmd_link}{param name: \'test\' /}{/call}. {/param}
{/call} /\* \* Signal processors 128+ \*/ {call .exit_codes} {param
value: \'130\' /} {param enum: \'SIGNAL_INTERRUPT\' /} {param
description} Command was interrupted (Ctrl + C) {/param} {/call}

{/param} // content {/call} // buck.page {/template}
