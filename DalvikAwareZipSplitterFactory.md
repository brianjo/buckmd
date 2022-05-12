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
[Package]{.packageLabelInType} [com.facebook.buck.android.dalvik](package-summary.html)
:::

## Class DalvikAwareZipSplitterFactory {#class-dalvikawarezipsplitterfactory .title title="Class DalvikAwareZipSplitterFactory"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.android.dalvik.DalvikAwareZipSplitterFactory

::: description
-   

    All Implemented Interfaces:
    :   `ZipSplitterFactory`

    ------------------------------------------------------------------------

        public class DalvikAwareZipSplitterFactory
        extends Object
        implements ZipSplitterFactory
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                           Description
          --------------------------------------------------------------------------------------------------------------------- -------------
          `DalvikAwareZipSplitterFactory​(long linearAllocLimit,                              Set<String> wantedInPrimaryZip)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `ZipSplitter`         | `newInstance​(         | ::: block             |
        |                       | ProjectFilesystem fil | Both combines and     |
        |                       | esystem,            S | splits a set of input |
        |                       | et<Path> inFiles,     | files into zip files  |
        |                       |         Path outPrima | such that no one      |
        |                       | ry,            Path o | output zip file has   |
        |                       | utSecondaryDir,       | entries that in total |
        |                       |       String secondar | exceed                |
        |                       | yPattern,             | `zipSizeHardLimit`.   |
        |                       | Path outDexStoresDir, | :::                   |
        |                       |             java.util |                       |
        |                       | .function.Predicate<S |                       |
        |                       | tring> requiredInPrim |                       |
        |                       | aryZip,            co |                       |
        |                       | m.google.common.colle |                       |
        |                       | ct.ImmutableSet<Strin |                       |
        |                       | g> secondaryHeadSet,  |                       |
        |                       |            com.google |                       |
        |                       | .common.collect.Immut |                       |
        |                       | ableSet<String> secon |                       |
        |                       | daryTailSet,          |                       |
        |                       |    com.google.common. |                       |
        |                       | collect.ImmutableMult |                       |
        |                       | imap<APKModule,​String |                       |
        |                       | > additionalDexStoreS |                       |
        |                       | ets,            APKMo |                       |
        |                       | dule rootAPKModule,   |                       |
        |                       |           ZipSplitter |                       |
        |                       | .DexSplitStrategy dex |                       |
        |                       | SplitStrategy,        |                       |
        |                       |      Path reportDir)` |                       |
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

        []{#<init>(long,java.util.Set)}

        -   #### DalvikAwareZipSplitterFactory

                public DalvikAwareZipSplitterFactory​(long linearAllocLimit,
                                                     Set<String> wantedInPrimaryZip)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#newInstance(com.facebook.buck.io.filesystem.ProjectFilesystem,java.util.Set,java.nio.file.Path,java.nio.file.Path,java.lang.String,java.nio.file.Path,java.util.function.Predicate,com.google.common.collect.ImmutableSet,com.google.common.collect.ImmutableSet,com.google.common.collect.ImmutableMultimap,com.facebook.buck.android.apkmodule.APKModule,com.facebook.buck.android.dalvik.ZipSplitter.DexSplitStrategy,java.nio.file.Path)}

        -   #### newInstance

            ``` methodSignature
            public ZipSplitter newInstance​(ProjectFilesystem filesystem,
                                           Set<Path> inFiles,
                                           Path outPrimary,
                                           Path outSecondaryDir,
                                           String secondaryPattern,
                                           Path outDexStoresDir,
                                           java.util.function.Predicate<String> requiredInPrimaryZip,
                                           com.google.common.collect.ImmutableSet<String> secondaryHeadSet,
                                           com.google.common.collect.ImmutableSet<String> secondaryTailSet,
                                           com.google.common.collect.ImmutableMultimap<APKModule,​String> additionalDexStoreSets,
                                           APKModule rootAPKModule,
                                           ZipSplitter.DexSplitStrategy dexSplitStrategy,
                                           Path reportDir)
            ```

            ::: block
            [Description copied from
            interface: `ZipSplitterFactory`]{.descfrmTypeLabel}
            :::

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

            [Specified by:]{.overrideSpecifyLabel}
            :   `newInstance` in interface `ZipSplitterFactory`
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
            :   `additionalDexStoreSets` - mapping of APKModules to
                module names for creating additional dex stores beyond
                the primary and secondary dex
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
