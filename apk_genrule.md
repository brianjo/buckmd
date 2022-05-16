/\* \* Copyright (c) Facebook, Inc. and its affiliates. \* \* Licensed
under the Apache License, Version 2.0 (the \"License\"); \* you may not
use this file except in compliance with the License. \* You may obtain a
copy of the License at \* \* http://www.apache.org/licenses/LICENSE-2.0
\* \* Unless required by applicable law or agreed to in writing,
software \* distributed under the License is distributed on an \"AS IS\"
BASIS, \* WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
or implied. \* See the License for the specific language governing
permissions and \* limitations under the License. \*/ {namespace
apk_genrule} /\*\*\*/ {template .soyweb} {call buck.page} {param title:
\'apk_genrule()\' /} {param navid: \'rule_apk_genrule\' /} {param
prettify: true /} {param description} A rule that is used to
post-process an APK. {/param} {param content} {call buck.rule} {param
status: \'FROZEN\' /} {param overview} An `apk_genrule()` rule is used
to post-process an APK. What separates an apk_genrule from a genrule is
apk_genrules are known by BUCK to produce APKs, so commands like
`buck install` or {sp}`buck uninstall` still work. Additionally,
{sp}`apk_genrule()` rules can be inputs to other {sp}`apk_genrule()`
rules. {/param} {param args} {call buck.name_arg /} {call buck.arg}
{param name: \'apk\' /} {param desc} The input `android_binary()` rule.
The path to the APK can be accessed with the `$APK` shell variable.
{/param} {/call} {call genrule_common.srcs_arg /} {call
genrule_common.cmd_arg /} {call genrule_common.bash_arg /} {call
genrule_common.cmd_exe_arg /} {call genrule_common.type_arg /} {call
buck.arg} {param name: \'out\' /} {param default: \'None\' /} {param
desc} This argument only exists for historical reasons and it does not
have any effect. It will be deprecated and removed in the future.
{/param} {/call} {call genrule_common.environment_expansion_separator /}
{call buck.tests_arg /} {/param} // close args {param examples} Here is
an example of a couple `apk_genrule()` open up an APK, do some super
signing, and then zipalign that APK again. {literal}

``` {.prettyprint .lang-py}

# Building this rule will produce a file named messenger.apk.
android_binary(
  name = 'messenger',
  manifest = 'AndroidManifest.xml',
  target = 'Google Inc.:Google APIs:16',
  keystore = '//keystores:prod',
  package_type = 'release',
  proguard_config = 'proguard.cfg',
  deps = [
    ':res',
    ':src',
  ],
)

apk_genrule(
  name = 'messenger_super_sign_unalign',
  apk = ':messenger',
  bash = '$(exe //java/com/facebook/sign:super_sign) --input $APK --output $OUT',
  cmd_exe = '$(exe //java/com/facebook/sign:super_sign) --input %APK% --output %OUT%',
  out = 'messenger_super_sign_unalign.apk',
)

apk_genrule(
  name = 'messenger_super_sign',
  apk = ':messenger_super_sign_unalign',
  bash = '$ANDROID_HOME/tools/zipalign -f 4 $APK $OUT',
  cmd_exe = '%ANDROID_HOME%\\tools\\zipalign -f 4 %APK% %OUT%',
  out = 'messenger_super_sign.apk',
)
```

{/literal} {/param} {/call} // close buck.rule {/param} {/call}
{/template}
