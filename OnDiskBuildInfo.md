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
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
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

## Interface OnDiskBuildInfo {#interface-ondiskbuildinfo .title title="Interface OnDiskBuildInfo"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `DefaultOnDiskBuildInfo`

    ------------------------------------------------------------------------

        public interface OnDiskBuildInfo

    ::: block
    Provides access to the on-disk rule metadata (both \"artifact\" and
    \"build\").
    :::
:::

::: summary
-   ::: {.section role="region"}
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
        | `com.google.c         | `getM                 | ::: block             |
        | ommon.collect.Immutab | etadataForArtifact()` | Returns the \"build\" |
        | leMap<String,​String>` |                       | metadata that is      |
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
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getValue(java.lang.String)}

        -   #### getValue

            ``` methodSignature
            Either<String,​Exception> getValue​(String key)
            ```

            [Returns:]{.returnLabel}
            :   the rule \"artifact\" metadata value associated with the
                specified key, if it exists.

        []{#getBuildValue(java.lang.String)}

        -   #### getBuildValue

            ``` methodSignature
            Optional<String> getBuildValue​(String key)
            ```

            [Returns:]{.returnLabel}
            :   the build engine metadata value associated with the
                specified key, if it exists.

        []{#getValues(java.lang.String)}

        -   #### getValues

            ``` methodSignature
            Optional<com.google.common.collect.ImmutableList<String>> getValues​(String key)
            ```

            [Returns:]{.returnLabel}
            :   the sequence of \"artifact\" values associated with the
                specified key, if it exists.

        []{#getValuesOrThrow(java.lang.String)}

        -   #### getValuesOrThrow

            ``` methodSignature
            com.google.common.collect.ImmutableList<String> getValuesOrThrow​(String key)
                                                                      throws IOException
            ```

            ::: block
            Tries to read the \"artifact\" values and if it fails it
            logs the attributes of the file it tried to read.
            :::

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#getMap(java.lang.String)}

        -   #### getMap

            ``` methodSignature
            Optional<com.google.common.collect.ImmutableMap<String,​String>> getMap​(String key)
            ```

            [Returns:]{.returnLabel}
            :   the map of strings associated with the specified key in
                the \"build\" metadata, if it exists.

        []{#getRuleKey(java.lang.String)}

        -   #### getRuleKey

            ``` methodSignature
            Optional<RuleKey> getRuleKey​(String key)
            ```

            ::: block
            Returns the
            [`RuleKey`](../../../rulekey/RuleKey.html "class in com.facebook.buck.core.rulekey")
            for the rule whose output is currently stored on disk.
            This value would have been written the last time the rule
            was built successfully.
            :::

        []{#getPathsForArtifact()}

        -   #### getPathsForArtifact

            ``` methodSignature
            com.google.common.collect.ImmutableSortedSet<Path> getPathsForArtifact()
                                                                            throws IOException
            ```

            ::: block
            Returns the recorded output paths of the rule for creating a
            cache artifact.
            :::

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#getMetadataForArtifact()}

        -   #### getMetadataForArtifact

            ``` methodSignature
            com.google.common.collect.ImmutableMap<String,​String> getMetadataForArtifact()
                                                                                        throws IOException
            ```

            ::: block
            Returns the \"build\" metadata that is stored with a cache
            artifact (\"artifact\" metadata is stored within the
            artifact itself).
            :::

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#deleteExistingMetadata()}

        -   #### deleteExistingMetadata

            ``` methodSignature
            void deleteExistingMetadata()
                                 throws IOException
            ```

            ::: block
            Deletes both \"artifact\" and \"build\" metadata.
            :::

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#calculateOutputSizeAndWriteMetadata(com.facebook.buck.util.hashing.FileHashLoader,com.google.common.collect.ImmutableSortedSet,com.google.common.base.Predicate)}

        -   #### calculateOutputSizeAndWriteMetadata

            ``` methodSignature
            void calculateOutputSizeAndWriteMetadata​(FileHashLoader fileHashLoader,
                                                     com.google.common.collect.ImmutableSortedSet<Path> recordedPaths,
                                                     com.google.common.base.Predicate<Long> shouldWriteOutputHashes)
                                              throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#validateArtifact(java.util.Set)}

        -   #### validateArtifact

            ``` methodSignature
            void validateArtifact​(Set<Path> extractedFiles)
                           throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#getOutputPaths()}

        -   #### getOutputPaths

            ``` methodSignature
            com.google.common.collect.ImmutableSortedSet<Path> getOutputPaths()
            ```
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
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   Constr \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
