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
-   Field \| 
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   [Constr](#constructor.detail) \| 
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

## Class DefaultOnDiskBuildInfo {#class-defaultondiskbuildinfo .title title="Class DefaultOnDiskBuildInfo"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.build.engine.buildinfo.DefaultOnDiskBuildInfo

::: description
-   

    All Implemented Interfaces:
    :   `OnDiskBuildInfo`

    ------------------------------------------------------------------------

        public class DefaultOnDiskBuildInfo
        extends Object
        implements OnDiskBuildInfo

    ::: block
    Utility for reading the metadata associated with a build rule\'s
    output. This is metadata that would have been written by a
    [`BuildInfoRecorder`](BuildInfoRecorder.html "class in com.facebook.buck.core.build.engine.buildinfo")
    when the rule was built initially.
    Such metadata is stored as key/value pairs.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                    Description
          -------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `DefaultOnDiskBuildInfo​(BuildTarget target,                       ProjectFilesystem projectFilesystem,                       BuildInfoStore buildInfoStore)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `void`                | `calculateOutput      |                       |
        |                       | SizeAndWriteMetadata​( |                       |
        |                       | FileHashLoader fileHa |                       |
        |                       | shLoader,             |                       |
        |                       |                       |                       |
        |                       |    com.google.common. |                       |
        |                       | collect.ImmutableSort |                       |
        |                       | edSet<Path> recordedP |                       |
        |                       | aths,                 |                       |
        |                       |                     c |                       |
        |                       | om.google.common.base |                       |
        |                       | .Predicate<Long> shou |                       |
        |                       | ldWriteOutputHashes)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `dele                 | ::: block             |
        |                       | teExistingMetadata()` | Deletes both          |
        |                       |                       | \"artifact\" and      |
        |                       |                       | \"build\" metadata.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `getBu                |                       |
        |                       | ildValue​(String key)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `O                    | `getMap​(String key)`  |                       |
        | ptional<com.google.co |                       |                       |
        | mmon.collect.Immutabl |                       |                       |
        | eMap<String,​String>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.common.   | `getM                 | ::: block             |
        | collect.ImmutableSort | etadataForArtifact()` | Returns the \"build\" |
        | edMap<String,​String>` |                       | metadata that is      |
        |                       |                       | stored with a cache   |
        |                       |                       | artifact              |
        |                       |                       | (\"artifact\"         |
        |                       |                       | metadata is stored    |
        |                       |                       | within the artifact   |
        |                       |                       | itself).              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.googl            | `getOutputPaths()`    |                       |
        | e.common.collect.Immu |                       |                       |
        | tableSortedSet<Path>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.googl            | `g                    | ::: block             |
        | e.common.collect.Immu | etPathsForArtifact()` | Returns the recorded  |
        | tableSortedSet<Path>` |                       | output paths of the   |
        |                       |                       | rule for creating a   |
        |                       |                       | cache artifact.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<RuleKey>`   | `ge                   | ::: block             |
        |                       | tRuleKey​(String key)` | Returns the           |
        |                       |                       | [`RuleKey`](../../../ |
        |                       |                       | rulekey/RuleKey.html  |
        |                       |                       | "class in com.faceboo |
        |                       |                       | k.buck.core.rulekey") |
        |                       |                       | for the rule whose    |
        |                       |                       | output is currently   |
        |                       |                       | stored on disk.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Eith                 | `                     |                       |
        | er<String,​Exception>` | getValue​(String key)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<com.goo     | `g                    |                       |
        | gle.common.collect.Im | etValues​(String key)` |                       |
        | mutableList<String>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.go               | `getValue             | ::: block             |
        | ogle.common.collect.I | sOrThrow​(String key)` | Tries to read the     |
        | mmutableList<String>` |                       | \"artifact\" values   |
        |                       |                       | and if it fails it    |
        |                       |                       | logs the attributes   |
        |                       |                       | of the file it tried  |
        |                       |                       | to read.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `v                    |                       |
        |                       | alidateArtifact​(Set<P |                       |
        |                       | ath> extractedFiles)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.build.engine.buildinfo.BuildInfoStore)}

        -   #### DefaultOnDiskBuildInfo

                public DefaultOnDiskBuildInfo​(BuildTarget target,
                                              ProjectFilesystem projectFilesystem,
                                              BuildInfoStore buildInfoStore)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getValue(java.lang.String)}

        -   #### getValue

            ``` methodSignature
            public Either<String,​Exception> getValue​(String key)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getValue` in interface `OnDiskBuildInfo`

            [Returns:]{.returnLabel}
            :   the rule \"artifact\" metadata value associated with the
                specified key, if it exists.

        []{#getBuildValue(java.lang.String)}

        -   #### getBuildValue

            ``` methodSignature
            public Optional<String> getBuildValue​(String key)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getBuildValue` in interface `OnDiskBuildInfo`

            [Returns:]{.returnLabel}
            :   the build engine metadata value associated with the
                specified key, if it exists.

        []{#getValues(java.lang.String)}

        -   #### getValues

            ``` methodSignature
            public Optional<com.google.common.collect.ImmutableList<String>> getValues​(String key)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getValues` in interface `OnDiskBuildInfo`

            [Returns:]{.returnLabel}
            :   the sequence of \"artifact\" values associated with the
                specified key, if it exists.

        []{#getValuesOrThrow(java.lang.String)}

        -   #### getValuesOrThrow

            ``` methodSignature
            public com.google.common.collect.ImmutableList<String> getValuesOrThrow​(String key)
                                                                             throws IOException
            ```

            ::: block
            [Description copied from
            interface: `OnDiskBuildInfo`]{.descfrmTypeLabel}
            :::

            ::: block
            Tries to read the \"artifact\" values and if it fails it
            logs the attributes of the file it tried to read.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getValuesOrThrow` in interface `OnDiskBuildInfo`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#getMap(java.lang.String)}

        -   #### getMap

            ``` methodSignature
            public Optional<com.google.common.collect.ImmutableMap<String,​String>> getMap​(String key)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getMap` in interface `OnDiskBuildInfo`

            [Returns:]{.returnLabel}
            :   the map of strings associated with the specified key in
                the \"build\" metadata, if it exists.

        []{#getOutputPaths()}

        -   #### getOutputPaths

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedSet<Path> getOutputPaths()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getOutputPaths` in interface `OnDiskBuildInfo`

        []{#getPathsForArtifact()}

        -   #### getPathsForArtifact

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedSet<Path> getPathsForArtifact()
                                                                                   throws IOException
            ```

            ::: block
            [Description copied from
            interface: `OnDiskBuildInfo`]{.descfrmTypeLabel}
            :::

            ::: block
            Returns the recorded output paths of the rule for creating a
            cache artifact.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getPathsForArtifact` in interface `OnDiskBuildInfo`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#getMetadataForArtifact()}

        -   #### getMetadataForArtifact

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedMap<String,​String> getMetadataForArtifact()
                                                                                                     throws IOException
            ```

            ::: block
            [Description copied from
            interface: `OnDiskBuildInfo`]{.descfrmTypeLabel}
            :::

            ::: block
            Returns the \"build\" metadata that is stored with a cache
            artifact (\"artifact\" metadata is stored within the
            artifact itself).
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getMetadataForArtifact` in interface `OnDiskBuildInfo`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#getRuleKey(java.lang.String)}

        -   #### getRuleKey

            ``` methodSignature
            public Optional<RuleKey> getRuleKey​(String key)
            ```

            ::: block
            [Description copied from
            interface: `OnDiskBuildInfo`]{.descfrmTypeLabel}
            :::

            ::: block
            Returns the
            [`RuleKey`](../../../rulekey/RuleKey.html "class in com.facebook.buck.core.rulekey")
            for the rule whose output is currently stored on disk.
            This value would have been written the last time the rule
            was built successfully.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getRuleKey` in interface `OnDiskBuildInfo`

        []{#deleteExistingMetadata()}

        -   #### deleteExistingMetadata

            ``` methodSignature
            public void deleteExistingMetadata()
                                        throws IOException
            ```

            ::: block
            [Description copied from
            interface: `OnDiskBuildInfo`]{.descfrmTypeLabel}
            :::

            ::: block
            Deletes both \"artifact\" and \"build\" metadata.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `deleteExistingMetadata` in interface `OnDiskBuildInfo`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#calculateOutputSizeAndWriteMetadata(com.facebook.buck.util.hashing.FileHashLoader,com.google.common.collect.ImmutableSortedSet,com.google.common.base.Predicate)}

        -   #### calculateOutputSizeAndWriteMetadata

            ``` methodSignature
            public void calculateOutputSizeAndWriteMetadata​(FileHashLoader fileHashLoader,
                                                            com.google.common.collect.ImmutableSortedSet<Path> recordedPaths,
                                                            com.google.common.base.Predicate<Long> shouldWriteOutputHashes)
                                                     throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `calculateOutputSizeAndWriteMetadata` in
                interface `OnDiskBuildInfo`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#validateArtifact(java.util.Set)}

        -   #### validateArtifact

            ``` methodSignature
            public void validateArtifact​(Set<Path> extractedFiles)
                                  throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `validateArtifact` in interface `OnDiskBuildInfo`

            [Throws:]{.throwsLabel}
            :   `IOException`
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
-   Field \| 
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   [Constr](#constructor.detail) \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
