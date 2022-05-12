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

-   [Overview](../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../deprecated-list.html)
-   [Index](../../../../../index-all.html)
-   [Help](../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.android.dalvik](package-summary.html)
:::

## Interface ZipSplitterFactory {#interface-zipsplitterfactory .title title="Interface ZipSplitterFactory"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `DalvikAwareZipSplitterFactory`

    ------------------------------------------------------------------------

        public interface ZipSplitterFactory
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `ZipSplitter`         | `newInstan            | ::: block             |
        |                       | ce​(ProjectFilesystem  | Both combines and     |
        |                       | filesystem,           | splits a set of input |
        |                       |   Set<Path> inFiles,  | files into zip files  |
        |                       |            Path outPr | such that no one      |
        |                       | imary,            Pat | output zip file has   |
        |                       | h outSecondaryDir,    | entries that in total |
        |                       |          String secon | exceed                |
        |                       | daryPattern,          | `zipSizeHardLimit`.   |
        |                       |    Path outDexStoresD | :::                   |
        |                       | ir,            java.u |                       |
        |                       | til.function.Predicat |                       |
        |                       | e<String> requiredInP |                       |
        |                       | rimaryZip,            |                       |
        |                       |  com.google.common.co |                       |
        |                       | llect.ImmutableSet<St |                       |
        |                       | ring> secondaryHeadSe |                       |
        |                       | t,            com.goo |                       |
        |                       | gle.common.collect.Im |                       |
        |                       | mutableSet<String> se |                       |
        |                       | condaryTailSet,       |                       |
        |                       |       com.google.comm |                       |
        |                       | on.collect.ImmutableM |                       |
        |                       | ultimap<APKModule,​Str |                       |
        |                       | ing> additionalDexSto |                       |
        |                       | res,            APKMo |                       |
        |                       | dule rootAPKModule,   |                       |
        |                       |           ZipSplitter |                       |
        |                       | .DexSplitStrategy dex |                       |
        |                       | SplitStrategy,        |                       |
        |                       |      Path reportDir)` |                       |
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

        []{#newInstance(com.facebook.buck.io.filesystem.ProjectFilesystem,java.util.Set,java.nio.file.Path,java.nio.file.Path,java.lang.String,java.nio.file.Path,java.util.function.Predicate,com.google.common.collect.ImmutableSet,com.google.common.collect.ImmutableSet,com.google.common.collect.ImmutableMultimap,com.facebook.buck.android.apkmodule.APKModule,com.facebook.buck.android.dalvik.ZipSplitter.DexSplitStrategy,java.nio.file.Path)}

        -   #### newInstance

            ``` methodSignature
            ZipSplitter newInstance​(ProjectFilesystem filesystem,
                                    Set<Path> inFiles,
                                    Path outPrimary,
                                    Path outSecondaryDir,
                                    String secondaryPattern,
                                    Path outDexStoresDir,
                                    java.util.function.Predicate<String> requiredInPrimaryZip,
                                    com.google.common.collect.ImmutableSet<String> secondaryHeadSet,
                                    com.google.common.collect.ImmutableSet<String> secondaryTailSet,
                                    com.google.common.collect.ImmutableMultimap<APKModule,​String> additionalDexStores,
                                    APKModule rootAPKModule,
                                    ZipSplitter.DexSplitStrategy dexSplitStrategy,
                                    Path reportDir)
            ```

            ::: block
            Both combines and splits a set of input files into zip files
            such that no one output zip file has entries that in total
            exceed `zipSizeHardLimit`. Input files can be themselves zip
            files, individual class/resource files, or a directory of
            such of files. The inputs are \"opened\", and the files
            contained within them are individually processed.
            For example, given a set of inFiles of A.zip and B.zip where
            A.zip contains { A, B, C }, and B.zip contains { X, Y, Z },
            a possible outcome of this method could yield outPrimary.zip
            containing { A, B }, outSecondary1.zip containing { C, X },
            and outSecondary2.zip containing { Y, Z }.

            This method exists as a critical utility to divide source
            code so large that dx/dexopt fail due to design constraints.
            :::

            [Parameters:]{.paramLabel}
            :   `inFiles` - Set of input files (directories or zip
                files) whose contents should be placed in the output zip
                files.
            :   `outPrimary` - Primary output zip file.
            :   `outSecondaryDir` - Directory to place secondary output
                zip files (if any are generated).
            :   `secondaryPattern` - Pattern containing a single integer
                (%d) that forms the filename of output zip files placed
                in `outSecondaryDir`.
            :   `requiredInPrimaryZip` - Determine which input *entries*
                are necessary in the primary output zip file. Note that
                this is referring to the entries contained within
                `      inFiles`, not the input files themselves.
            :   `secondaryHeadSet` - list of classes to include in the
                primary dex until it is full
            :   `secondaryTailSet` - list of classes to include last in
                the secondary dex
            :   `additionalDexStores` - mapping of APKModules to module
                names for creating additional dex stores beyond the
                primary and secondary dex
            :   `rootAPKModule` -
            :   `reportDir` - Directory where to publish a report of
                which classes were written to which zip files with a
                corresponding size estimate.
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

-   [Overview](../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../deprecated-list.html)
-   [Index](../../../../../index-all.html)
-   [Help](../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../allclasses.html)

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
