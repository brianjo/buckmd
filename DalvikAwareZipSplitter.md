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
-   [Nested](#nested.class.summary) \| 
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

## Class DalvikAwareZipSplitter {#class-dalvikawarezipsplitter .title title="Class DalvikAwareZipSplitter"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.android.dalvik.DalvikAwareZipSplitter

::: description
-   

    All Implemented Interfaces:
    :   `ZipSplitter`

    ------------------------------------------------------------------------

        public class DalvikAwareZipSplitter
        extends Object
        implements ZipSplitter

    ::: block
    Implementation of
    [`ZipSplitter`](ZipSplitter.html "interface in com.facebook.buck.android.dalvik")
    that uses estimates from
    [`DalvikStatsTool`](DalvikStatsTool.html "class in com.facebook.buck.android.dalvik")
    to determine how many classes to pack into a dex.
    It does three passes through the .class files:

    -   During the first pass, it uses the `requiredInPrimaryZip`
        predicate to filter the set of classes that *must* be included
        in the primary dex. These classes are added to the primary zip.
    -   During the second pass, it uses the `wantedInPrimaryZip` list to
        find classes that were not included in the first pass but that
        should still be in the primary zip for performance reasons, and
        adds them to the primary zip.
    -   During the third pass, classes that were not matched during the
        earlier passes are added to zips as space allows. This is a
        simple, greedy algorithm.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        -   []{#nested.classes.inherited.from.class.com.facebook.buck.android.dalvik.ZipSplitter}

            ### Nested classes/interfaces inherited from interface com.facebook.buck.android.dalvik.[ZipSplitter](ZipSplitter.html "interface in com.facebook.buck.android.dalvik")

            `ZipSplitter.DexSplitStrategy`
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `com.google.common.   | `execute()`           | ::: block             |
        | collect.ImmutableMult |                       | Writes the primary    |
        | imap<APKModule,​Path>` |                       | zip file and if       |
        |                       |                       | necessary, the        |
        |                       |                       | secondary zip files.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static Da            | `sp                   |                       |
        | lvikAwareZipSplitter` | litZip​(ProjectFilesys |                       |
        |                       | tem filesystem,       |                       |
        |                       |    Set<Path> inFiles, |                       |
        |                       |          Path outPrim |                       |
        |                       | ary,         Path out |                       |
        |                       | SecondaryDir,         |                       |
        |                       |  String secondaryPatt |                       |
        |                       | ern,         Path out |                       |
        |                       | DexStoresDir,         |                       |
        |                       |  long linearAllocLimi |                       |
        |                       | t,         java.util. |                       |
        |                       | function.Predicate<St |                       |
        |                       | ring> requiredInPrima |                       |
        |                       | ryZip,         Set<St |                       |
        |                       | ring> wantedInPrimary |                       |
        |                       | Zip,         com.goog |                       |
        |                       | le.common.collect.Imm |                       |
        |                       | utableSet<String> sec |                       |
        |                       | ondaryHeadSet,        |                       |
        |                       |   com.google.common.c |                       |
        |                       | ollect.ImmutableSet<S |                       |
        |                       | tring> secondaryTailS |                       |
        |                       | et,         com.googl |                       |
        |                       | e.common.collect.Immu |                       |
        |                       | tableMultimap<APKModu |                       |
        |                       | le,​String> additional |                       |
        |                       | DexStoreSets,         |                       |
        |                       |  APKModule rootAPKMod |                       |
        |                       | ule,         ZipSplit |                       |
        |                       | ter.DexSplitStrategy  |                       |
        |                       | dexSplitStrategy,     |                       |
        |                       |      Path reportDir)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
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
    -   []{#method.detail}

        ### Method Detail

        []{#splitZip(com.facebook.buck.io.filesystem.ProjectFilesystem,java.util.Set,java.nio.file.Path,java.nio.file.Path,java.lang.String,java.nio.file.Path,long,java.util.function.Predicate,java.util.Set,com.google.common.collect.ImmutableSet,com.google.common.collect.ImmutableSet,com.google.common.collect.ImmutableMultimap,com.facebook.buck.android.apkmodule.APKModule,com.facebook.buck.android.dalvik.ZipSplitter.DexSplitStrategy,java.nio.file.Path)}

        -   #### splitZip

            ``` methodSignature
            public static DalvikAwareZipSplitter splitZip​(ProjectFilesystem filesystem,
                                                          Set<Path> inFiles,
                                                          Path outPrimary,
                                                          Path outSecondaryDir,
                                                          String secondaryPattern,
                                                          Path outDexStoresDir,
                                                          long linearAllocLimit,
                                                          java.util.function.Predicate<String> requiredInPrimaryZip,
                                                          Set<String> wantedInPrimaryZip,
                                                          com.google.common.collect.ImmutableSet<String> secondaryHeadSet,
                                                          com.google.common.collect.ImmutableSet<String> secondaryTailSet,
                                                          com.google.common.collect.ImmutableMultimap<APKModule,​String> additionalDexStoreSets,
                                                          APKModule rootAPKModule,
                                                          ZipSplitter.DexSplitStrategy dexSplitStrategy,
                                                          Path reportDir)
            ```

        []{#execute()}

        -   #### execute

            ``` methodSignature
            public com.google.common.collect.ImmutableMultimap<APKModule,​Path> execute()
                                                                                      throws IOException
            ```

            ::: block
            [Description copied from
            interface: `ZipSplitter`]{.descfrmTypeLabel}
            :::

            ::: block
            Writes the primary zip file and if necessary, the secondary
            zip files.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `execute` in interface `ZipSplitter`

            [Returns:]{.returnLabel}
            :   output map of dex store to zip files.

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
-   [Nested](#nested.class.summary) \| 
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
