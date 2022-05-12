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
-   [Nested](#nested.class.summary) \| 
-   [Field](#field.summary) \| 
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
-   Constr \| 
-   [Method](#method.detail)

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

## Class BuildInfo {#class-buildinfo .title title="Class BuildInfo"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.build.engine.buildinfo.BuildInfo

::: description
-   

    ------------------------------------------------------------------------

        public class BuildInfo
        extends Object

    ::: block
    Shared utilities for
    [`BuildInfoRecorder`](BuildInfoRecorder.html "class in com.facebook.buck.core.build.engine.buildinfo")
    and
    [`OnDiskBuildInfo`](OnDiskBuildInfo.html "interface in com.facebook.buck.core.build.engine.buildinfo").
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type   Class                     Description
          ------------------- ------------------------- -------------
          `static class `     `BuildInfo.MetadataKey`    

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Field                 | Description           |
        +=======================+=======================+=======================+
        | `static String`       | `MANIFEST`            | ::: block             |
        |                       |                       | Key for               |
        |                       |                       | [`OnDiskBuildInfo`    |
        |                       |                       | ](OnDiskBuildInfo.htm |
        |                       |                       | l "interface in com.f |
        |                       |                       | acebook.buck.core.bui |
        |                       |                       | ld.engine.buildinfo") |
        |                       |                       | to store the manifest |
        |                       |                       | for build rules       |
        |                       |                       | supporting            |
        |                       |                       | manifest-based        |
        |                       |                       | caching.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static com.g         | `METADATA_KEYS`       |                       |
        | oogle.common.collect. |                       |                       |
        | ImmutableSet<String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static com.g         | `RULE_KEY_NAMES`      | ::: block             |
        | oogle.common.collect. |                       | All keys              |
        | ImmutableSet<String>` |                       | corresponding to rule |
        |                       |                       | keys.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static Path`         | `getPathToArtif       |                       |
        |                       | actMetadataDirectory​( |                       |
        |                       | BuildTarget target,   |                       |
        |                       |                       |                       |
        |                       |             ProjectFi |                       |
        |                       | lesystem filesystem)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static Path`         | `getP                 |                       |
        |                       | athToArtifactMetadata |                       |
        |                       | File​(BuildTarget targ |                       |
        |                       | et,                   |                       |
        |                       |             ProjectFi |                       |
        |                       | lesystem filesystem)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static Path`         | `getPathToMetadataDi  | ::: block             |
        |                       | rectory​(BuildTarget t | Returns the path to a |
        |                       | arget,                | directory where       |
        |                       |             ProjectFi | metadata files for a  |
        |                       | lesystem filesystem)` | build rule with the   |
        |                       |                       | specified target      |
        |                       |                       | should be stored.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static Path`         | `getPathT             |                       |
        |                       | oOtherMetadataDirecto |                       |
        |                       | ry​(BuildTarget target |                       |
        |                       | ,                     |                       |
        |                       |             ProjectFi |                       |
        |                       | lesystem filesystem)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static boolean`      | `isArtifact           | ::: block             |
        |                       | Metadata​(String key)` | Whether this is a key |
        |                       |                       | that represents data  |
        |                       |                       | to be stored as       |
        |                       |                       | [`Buil                |
        |                       |                       | dInfo.MetadataKey.ART |
        |                       |                       | IFACT_METADATA`](Buil |
        |                       |                       | dInfo.MetadataKey.htm |
        |                       |                       | l#ARTIFACT_METADATA). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#field.detail}

        ### Field Detail

        []{#METADATA_KEYS}

        -   #### METADATA_KEYS

                public static final com.google.common.collect.ImmutableSet<String> METADATA_KEYS

        []{#RULE_KEY_NAMES}

        -   #### RULE_KEY_NAMES

                public static final com.google.common.collect.ImmutableSet<String> RULE_KEY_NAMES

            ::: block
            All keys corresponding to rule keys.
            :::

        []{#MANIFEST}

        -   #### MANIFEST

                public static final String MANIFEST

            ::: block
            Key for
            [`OnDiskBuildInfo`](OnDiskBuildInfo.html "interface in com.facebook.buck.core.build.engine.buildinfo")
            to store the manifest for build rules supporting
            manifest-based caching.
            :::

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../../constant-values.html#com.facebook.buck.core.build.engine.buildinfo.BuildInfo.MANIFEST)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getPathToMetadataDirectory(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem)}

        -   #### getPathToMetadataDirectory

            ``` methodSignature
            public static Path getPathToMetadataDirectory​(BuildTarget target,
                                                          ProjectFilesystem filesystem)
            ```

            ::: block
            Returns the path to a directory where metadata files for a
            build rule with the specified target should be stored.
            :::

            [Returns:]{.returnLabel}
            :   A path relative to the project root that includes a
                trailing slash.

        []{#getPathToArtifactMetadataDirectory(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem)}

        -   #### getPathToArtifactMetadataDirectory

            ``` methodSignature
            public static Path getPathToArtifactMetadataDirectory​(BuildTarget target,
                                                                  ProjectFilesystem filesystem)
            ```

        []{#getPathToArtifactMetadataFile(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem)}

        -   #### getPathToArtifactMetadataFile

            ``` methodSignature
            public static Path getPathToArtifactMetadataFile​(BuildTarget target,
                                                             ProjectFilesystem filesystem)
            ```

        []{#getPathToOtherMetadataDirectory(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem)}

        -   #### getPathToOtherMetadataDirectory

            ``` methodSignature
            public static Path getPathToOtherMetadataDirectory​(BuildTarget target,
                                                               ProjectFilesystem filesystem)
            ```

        []{#isArtifactMetadata(java.lang.String)}

        -   #### isArtifactMetadata

            ``` methodSignature
            public static boolean isArtifactMetadata​(String key)
            ```

            ::: block
            Whether this is a key that represents data to be stored as
            [`BuildInfo.MetadataKey.ARTIFACT_METADATA`](BuildInfo.MetadataKey.html#ARTIFACT_METADATA).
            :::
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
-   [Nested](#nested.class.summary) \| 
-   [Field](#field.summary) \| 
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
-   Constr \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
