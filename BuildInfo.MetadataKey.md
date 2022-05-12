<div>

JavaScript is disabled on your browser.

</div>

::: {role="banner"}
::: fixedNav
::: topNav
[]{#navbar.top}

::: skipNav
[Skip navigation links](#skip.navbar.top "Skip navigation links")
:::

[]{#navbar.top.firstrow}

-   [Overview](../../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../index-all.html)
-   [Help](../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../allclasses.html)

```{=html}
<!-- -->
```
-   SEARCH:

<div>

<div>

JavaScript is disabled on your browser.

</div>

</div>

<div>

-   Summary: 
-   Nested \| 
-   [Field](#field.summary) \| 
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
-   Constr \| 
-   Method

</div>

[]{#skip.navbar.top}
:::
:::

::: navPadding
 
:::
:::

::: {role="main"}
::: header
::: subTitle
[Package]{.packageLabelInType} [com.facebook.buck.core.build.engine.buildinfo](package-summary.html)
:::

## Class BuildInfo.MetadataKey {#class-buildinfo.metadatakey .title title="Class BuildInfo.MetadataKey"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.build.engine.buildinfo.BuildInfo.MetadataKey

::: description
-   

    Enclosing class:
    :   [BuildInfo](BuildInfo.html "class in com.facebook.buck.core.build.engine.buildinfo")

    ------------------------------------------------------------------------

        public static class BuildInfo.MetadataKey
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Field                 | Description           |
        +=======================+=======================+=======================+
        | `static String`       | `ADDITIONAL_INFO`     | ::: block             |
        |                       |                       | Key for               |
        |                       |                       | [`OnDiskBuildInfo`    |
        |                       |                       | ](OnDiskBuildInfo.htm |
        |                       |                       | l "interface in com.f |
        |                       |                       | acebook.buck.core.bui |
        |                       |                       | ld.engine.buildinfo") |
        |                       |                       | to identify           |
        |                       |                       | additional info       |
        |                       |                       | describing a build.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static String`       | `ARTIFACT_METADATA`   | ::: block             |
        |                       |                       | Value for file that   |
        |                       |                       | contains all artifact |
        |                       |                       | metadata as a json    |
        |                       |                       | bundle.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static String`       | `BUILD_ID`            | ::: block             |
        |                       |                       | Key containing the ID |
        |                       |                       | of the current build. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static String`       | `CONFIGURATION`       | ::: block             |
        |                       |                       | Key for               |
        |                       |                       | [`OnDiskBuildInfo`    |
        |                       |                       | ](OnDiskBuildInfo.htm |
        |                       |                       | l "interface in com.f |
        |                       |                       | acebook.buck.core.bui |
        |                       |                       | ld.engine.buildinfo") |
        |                       |                       | to store the build    |
        |                       |                       | target configuration  |
        |                       |                       | of the owning build   |
        |                       |                       | rule.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static String`       | `DEP_FILE`            | ::: block             |
        |                       |                       | Key for               |
        |                       |                       | [`OnDiskBuildInfo`    |
        |                       |                       | ](OnDiskBuildInfo.htm |
        |                       |                       | l "interface in com.f |
        |                       |                       | acebook.buck.core.bui |
        |                       |                       | ld.engine.buildinfo") |
        |                       |                       | to identify the       |
        |                       |                       | dependency-file for a |
        |                       |                       | build rule.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static String`       | `DEP_FILE_RULE_KEY`   | ::: block             |
        |                       |                       | Key for               |
        |                       |                       | [`OnDiskBuildInfo`    |
        |                       |                       | ](OnDiskBuildInfo.htm |
        |                       |                       | l "interface in com.f |
        |                       |                       | acebook.buck.core.bui |
        |                       |                       | ld.engine.buildinfo") |
        |                       |                       | to identify the       |
        |                       |                       | dependency-file       |
        |                       |                       | [`RuleKey`](../../../ |
        |                       |                       | rulekey/RuleKey.html  |
        |                       |                       | "class in com.faceboo |
        |                       |                       | k.buck.core.rulekey") |
        |                       |                       | for a build rule.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static String`       | `                     | ::: block             |
        |                       | INPUT_BASED_RULE_KEY` | Key for               |
        |                       |                       | [`OnDiskBuildInfo`    |
        |                       |                       | ](OnDiskBuildInfo.htm |
        |                       |                       | l "interface in com.f |
        |                       |                       | acebook.buck.core.bui |
        |                       |                       | ld.engine.buildinfo") |
        |                       |                       | to identify the input |
        |                       |                       | RuleKey for a build   |
        |                       |                       | rule.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static String`       | `MANIFEST_KEY`        | ::: block             |
        |                       |                       | Key for               |
        |                       |                       | [`OnDiskBuildInfo`    |
        |                       |                       | ](OnDiskBuildInfo.htm |
        |                       |                       | l "interface in com.f |
        |                       |                       | acebook.buck.core.bui |
        |                       |                       | ld.engine.buildinfo") |
        |                       |                       | to store the cache    |
        |                       |                       | key of the manifest.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static String`       | `ORIGIN_BUILD_ID`     | ::: block             |
        |                       |                       | Key containing the ID |
        |                       |                       | of the build that     |
        |                       |                       | previously            |
        |                       |                       | built/cached this     |
        |                       |                       | rule\'s outputs.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static String`       | `OUTPUT_HASH`         | ::: block             |
        |                       |                       | Key for               |
        |                       |                       | [`OnDiskBuildInfo`    |
        |                       |                       | ](OnDiskBuildInfo.htm |
        |                       |                       | l "interface in com.f |
        |                       |                       | acebook.buck.core.bui |
        |                       |                       | ld.engine.buildinfo") |
        |                       |                       | to store the hash of  |
        |                       |                       | the output.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static String`       | `OUTPUT_SIZE`         | ::: block             |
        |                       |                       | Key for               |
        |                       |                       | [`OnDiskBuildInfo`    |
        |                       |                       | ](OnDiskBuildInfo.htm |
        |                       |                       | l "interface in com.f |
        |                       |                       | acebook.buck.core.bui |
        |                       |                       | ld.engine.buildinfo") |
        |                       |                       | to store the size of  |
        |                       |                       | the output.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static String`       | `                     | ::: block             |
        |                       | RECORDED_PATH_HASHES` | Key for               |
        |                       |                       | [`OnDiskBuildInfo`    |
        |                       |                       | ](OnDiskBuildInfo.htm |
        |                       |                       | l "interface in com.f |
        |                       |                       | acebook.buck.core.bui |
        |                       |                       | ld.engine.buildinfo") |
        |                       |                       | with a map of outputs |
        |                       |                       | to hashes.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static String`       | `RECORDED_PATHS`      | ::: block             |
        |                       |                       | Key for               |
        |                       |                       | [`OnDiskBuildInfo`    |
        |                       |                       | ](OnDiskBuildInfo.htm |
        |                       |                       | l "interface in com.f |
        |                       |                       | acebook.buck.core.bui |
        |                       |                       | ld.engine.buildinfo") |
        |                       |                       | which lists the       |
        |                       |                       | recorded items.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static String`       | `RULE_KEY`            | ::: block             |
        |                       |                       | Key for               |
        |                       |                       | [`OnDiskBuildInfo`    |
        |                       |                       | ](OnDiskBuildInfo.htm |
        |                       |                       | l "interface in com.f |
        |                       |                       | acebook.buck.core.bui |
        |                       |                       | ld.engine.buildinfo") |
        |                       |                       | to identify the       |
        |                       |                       | RuleKey for a build   |
        |                       |                       | rule.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static String`       | `TARGET`              | ::: block             |
        |                       |                       | Key for               |
        |                       |                       | [`OnDiskBuildInfo`    |
        |                       |                       | ](OnDiskBuildInfo.htm |
        |                       |                       | l "interface in com.f |
        |                       |                       | acebook.buck.core.bui |
        |                       |                       | ld.engine.buildinfo") |
        |                       |                       | to store the build    |
        |                       |                       | target of the owning  |
        |                       |                       | build rule.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#field.detail}

        ### Field Detail

        []{#ARTIFACT_METADATA}

        -   #### ARTIFACT_METADATA

                public static final String ARTIFACT_METADATA

            ::: block
            Value for file that contains all artifact metadata as a json
            bundle.
            :::

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../../constant-values.html#com.facebook.buck.core.build.engine.buildinfo.BuildInfo.MetadataKey.ARTIFACT_METADATA)

        []{#RECORDED_PATHS}

        -   #### RECORDED_PATHS

                public static final String RECORDED_PATHS

            ::: block
            Key for
            [`OnDiskBuildInfo`](OnDiskBuildInfo.html "interface in com.facebook.buck.core.build.engine.buildinfo")
            which lists the recorded items.
            :::

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../../constant-values.html#com.facebook.buck.core.build.engine.buildinfo.BuildInfo.MetadataKey.RECORDED_PATHS)

        []{#RECORDED_PATH_HASHES}

        -   #### RECORDED_PATH_HASHES

                public static final String RECORDED_PATH_HASHES

            ::: block
            Key for
            [`OnDiskBuildInfo`](OnDiskBuildInfo.html "interface in com.facebook.buck.core.build.engine.buildinfo")
            with a map of outputs to hashes.
            :::

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../../constant-values.html#com.facebook.buck.core.build.engine.buildinfo.BuildInfo.MetadataKey.RECORDED_PATH_HASHES)

        []{#ADDITIONAL_INFO}

        -   #### ADDITIONAL_INFO

                public static final String ADDITIONAL_INFO

            ::: block
            Key for
            [`OnDiskBuildInfo`](OnDiskBuildInfo.html "interface in com.facebook.buck.core.build.engine.buildinfo")
            to identify additional info describing a build.
            :::

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../../constant-values.html#com.facebook.buck.core.build.engine.buildinfo.BuildInfo.MetadataKey.ADDITIONAL_INFO)

        []{#RULE_KEY}

        -   #### RULE_KEY

                public static final String RULE_KEY

            ::: block
            Key for
            [`OnDiskBuildInfo`](OnDiskBuildInfo.html "interface in com.facebook.buck.core.build.engine.buildinfo")
            to identify the RuleKey for a build rule.
            :::

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../../constant-values.html#com.facebook.buck.core.build.engine.buildinfo.BuildInfo.MetadataKey.RULE_KEY)

        []{#INPUT_BASED_RULE_KEY}

        -   #### INPUT_BASED_RULE_KEY

                public static final String INPUT_BASED_RULE_KEY

            ::: block
            Key for
            [`OnDiskBuildInfo`](OnDiskBuildInfo.html "interface in com.facebook.buck.core.build.engine.buildinfo")
            to identify the input RuleKey for a build rule.
            :::

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../../constant-values.html#com.facebook.buck.core.build.engine.buildinfo.BuildInfo.MetadataKey.INPUT_BASED_RULE_KEY)

        []{#DEP_FILE_RULE_KEY}

        -   #### DEP_FILE_RULE_KEY

                public static final String DEP_FILE_RULE_KEY

            ::: block
            Key for
            [`OnDiskBuildInfo`](OnDiskBuildInfo.html "interface in com.facebook.buck.core.build.engine.buildinfo")
            to identify the dependency-file
            [`RuleKey`](../../../rulekey/RuleKey.html "class in com.facebook.buck.core.rulekey")
            for a build rule.
            :::

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../../constant-values.html#com.facebook.buck.core.build.engine.buildinfo.BuildInfo.MetadataKey.DEP_FILE_RULE_KEY)

        []{#DEP_FILE}

        -   #### DEP_FILE

                public static final String DEP_FILE

            ::: block
            Key for
            [`OnDiskBuildInfo`](OnDiskBuildInfo.html "interface in com.facebook.buck.core.build.engine.buildinfo")
            to identify the dependency-file for a build rule.
            :::

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../../constant-values.html#com.facebook.buck.core.build.engine.buildinfo.BuildInfo.MetadataKey.DEP_FILE)

        []{#TARGET}

        -   #### TARGET

                public static final String TARGET

            ::: block
            Key for
            [`OnDiskBuildInfo`](OnDiskBuildInfo.html "interface in com.facebook.buck.core.build.engine.buildinfo")
            to store the build target of the owning build rule.
            :::

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../../constant-values.html#com.facebook.buck.core.build.engine.buildinfo.BuildInfo.MetadataKey.TARGET)

        []{#CONFIGURATION}

        -   #### CONFIGURATION

                public static final String CONFIGURATION

            ::: block
            Key for
            [`OnDiskBuildInfo`](OnDiskBuildInfo.html "interface in com.facebook.buck.core.build.engine.buildinfo")
            to store the build target configuration of the owning build
            rule.
            :::

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../../constant-values.html#com.facebook.buck.core.build.engine.buildinfo.BuildInfo.MetadataKey.CONFIGURATION)

        []{#MANIFEST_KEY}

        -   #### MANIFEST_KEY

                public static final String MANIFEST_KEY

            ::: block
            Key for
            [`OnDiskBuildInfo`](OnDiskBuildInfo.html "interface in com.facebook.buck.core.build.engine.buildinfo")
            to store the cache key of the manifest.
            :::

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../../constant-values.html#com.facebook.buck.core.build.engine.buildinfo.BuildInfo.MetadataKey.MANIFEST_KEY)

        []{#BUILD_ID}

        -   #### BUILD_ID

                public static final String BUILD_ID

            ::: block
            Key containing the ID of the current build.
            :::

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../../constant-values.html#com.facebook.buck.core.build.engine.buildinfo.BuildInfo.MetadataKey.BUILD_ID)

        []{#ORIGIN_BUILD_ID}

        -   #### ORIGIN_BUILD_ID

                public static final String ORIGIN_BUILD_ID

            ::: block
            Key containing the ID of the build that previously
            built/cached this rule\'s outputs.
            :::

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../../constant-values.html#com.facebook.buck.core.build.engine.buildinfo.BuildInfo.MetadataKey.ORIGIN_BUILD_ID)

        []{#OUTPUT_SIZE}

        -   #### OUTPUT_SIZE

                public static final String OUTPUT_SIZE

            ::: block
            Key for
            [`OnDiskBuildInfo`](OnDiskBuildInfo.html "interface in com.facebook.buck.core.build.engine.buildinfo")
            to store the size of the output.
            :::

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../../constant-values.html#com.facebook.buck.core.build.engine.buildinfo.BuildInfo.MetadataKey.OUTPUT_SIZE)

        []{#OUTPUT_HASH}

        -   #### OUTPUT_HASH

                public static final String OUTPUT_HASH

            ::: block
            Key for
            [`OnDiskBuildInfo`](OnDiskBuildInfo.html "interface in com.facebook.buck.core.build.engine.buildinfo")
            to store the hash of the output.
            :::

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../../constant-values.html#com.facebook.buck.core.build.engine.buildinfo.BuildInfo.MetadataKey.OUTPUT_HASH)
    :::
:::
:::
:::

::: bottomNav
[]{#navbar.bottom}

::: skipNav
[Skip navigation links](#skip.navbar.bottom "Skip navigation links")
:::

[]{#navbar.bottom.firstrow}

-   [Overview](../../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../index-all.html)
-   [Help](../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../allclasses.html)

<div>

<div>

JavaScript is disabled on your browser.

</div>

</div>

<div>

-   Summary: 
-   Nested \| 
-   [Field](#field.summary) \| 
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
-   Constr \| 
-   Method

</div>

[]{#skip.navbar.bottom}
:::
