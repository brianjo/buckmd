/\* \* Copyright (c) Facebook, Inc. and its affiliates. \* \* Licensed
under the Apache License, Version 2.0 (the \"License\"); \* you may not
use this file except in compliance with the License. \* You may obtain a
copy of the License at \* \* http://www.apache.org/licenses/LICENSE-2.0
\* \* Unless required by applicable law or agreed to in writing,
software \* distributed under the License is distributed on an \"AS IS\"
BASIS, \* WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
or implied. \* See the License for the specific language governing
permissions and \* limitations under the License. \*/ {namespace
buck.skylark.rule_exists} /\*\*\*/ {template .soyweb} {call buck.page}
{param title: \'rule_exists()\' /} {param navid:
\'skylark/generated_rule_exists\' /} {param prettify: true /} {param
description} Returns True if there is a previously defined rule with
provided name, or False if the rule with such name does not exist.
{/param} {param content} {call buck.function} {param status:
\'UNFROZEN\' /} {param overview} Returns True if there is a previously
defined rule with provided name, or False if the rule with such name
does not exist. {/param} {param args} {call buck.functionArg} {param
name : \'name\' /} {param desc } The name of the rule. {/param} {param
default : \'None\' /} {/call} {/param} {/call} {/param} // content
{/call} {/template}
