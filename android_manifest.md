/\* \* Copyright (c) Facebook, Inc. and its affiliates. \* \* Licensed
under the Apache License, Version 2.0 (the \"License\"); \* you may not
use this file except in compliance with the License. \* You may obtain a
copy of the License at \* \* http://www.apache.org/licenses/LICENSE-2.0
\* \* Unless required by applicable law or agreed to in writing,
software \* distributed under the License is distributed on an \"AS IS\"
BASIS, \* WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
or implied. \* See the License for the specific language governing
permissions and \* limitations under the License. \*/ {namespace
android_manifest} /\*\*\*/ {template .soyweb} {call buck.page} {param
title: \'android_manifest()\' /} {param navid: \'rule_android_manifest\'
/} {param prettify: true /} {param description} A rule that is used to
generate an Android Manifest. {/param} {param content} {call buck.rule}
{param status: \'UNFROZEN\' /} {param overview} An `android_manifest()`
rule is used to generate an {sp}[Android
Manifest](http://developer.android.com/guide/topics/manifest/manifest-intro.html)
to be used by {call buck.android_binary /} and {call buck.android_aar /}
rules. This rule takes a skeleton manifest, and merges it with manifests
found in any deps. {/param} {param args} {call buck.name_arg /} {call
buck.arg} {param name: \'skeleton\' /} {param desc} Either a {call
buck.build_target /} or a path to a file representing the manifest that
will be merged with any manifests associated with this rule\'s `deps`.
{/param} {/call} {call buck.arg} {param name: \'deps\' /} {param default
: \'\[\]\' /} {param desc} A collection of dependencies that includes
android_library rules. The manifest files of the {sp}{call
buck.android_library /} rules will be filtered out to become dependent
source files for the manifest. {/param} {/call} {/param} // close args
{param examples}

Here\'s an example of an `android_manifest()` that has no deps.

{literal}

``` {.prettyprint .lang-py}
android_manifest(
  name = 'my-manifest',
  skeleton = 'AndroidManifestSkeleton.xml',
)
```

{/literal}

This is what `AndroidManfiestSkeleton.xml` looks like.

{literal}

``` {.prettyprint .lang-xml}
<?xml version="1.0" encoding="utf-8"?>
<manifest xmlns:android="http://schemas.android.com/apk/res/android"
          package="com.example"
          android:versionCode="1"
          android:versionName="1.0">

    <uses-sdk targetSdkVersion="19" minSdkVersion="17"/>
    <application
        android:label="@string/app_name"
        android:icon="@drawable/ic_launcher">
        <activity
            android:name="MyActivity"
            android:label="@string/app_name">
            <intent-filter>
                <action android:name="android.intent.action.MAIN"/>
                <category android:name="android.intent.category.LAUNCHER"/>
            </intent-filter>
        </activity>
    </application>
</manifest>
```

{/literal}

You could also use a {call buck.genrule /} to generate the manifest file
and reference the {sp}{call buck.build_target /} in the `skeleton`
argument.

{/param} {/call} // close buck.rule {/param} {/call} {/template}
