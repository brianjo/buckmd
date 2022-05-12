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

-   [Overview](../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../deprecated-list.html)
-   [Index](../../../../index-all.html)
-   [Help](../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.android](package-summary.html)
:::

## Class PreDexedFilesSorter {#class-predexedfilessorter .title title="Class PreDexedFilesSorter"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.android.PreDexedFilesSorter

::: description
-   

    ------------------------------------------------------------------------

        public class PreDexedFilesSorter
        extends Object

    ::: block
    Responsible for bucketing pre-dexed objects into primary and
    secondary dex files.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type   Class                                    Description
          ------------------- ---------------------------------------- -------------
          `class `            `PreDexedFilesSorter.DexStoreContents`    
          `static class `     `PreDexedFilesSorter.Result`              

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         Description
          --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `PreDexedFilesSorter​(Collection<DexWithClasses> dexFilesToMerge,                    com.google.common.collect.ImmutableSet<String> primaryDexPatterns,                    APKModuleGraph apkModuleGraph,                    APKModule module,                    Path canaryDirectory,                    long dexWeightLimit,                    com.facebook.buck.android.DexStore dexStore,                    Path secondaryDexJarFilesDir,                    Optional<Integer> groupIndex)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `PreDex               | `sortIntoP            | ::: block             |
        | edFilesSorter.Result` | rimaryAndSecondaryDex | Sorts dex files into  |
        |                       | es​(ProjectFilesystem  | primary and secondary |
        |                       | filesystem,           | dexes, generate       |
        |                       |                       | canary classes, and   |
        |                       |   com.google.common.c | metadata for use by   |
        |                       | ollect.ImmutableList. | SmartDexingStep       |
        |                       | Builder<Step> steps)` | :::                   |
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

        []{#<init>(java.util.Collection,com.google.common.collect.ImmutableSet,com.facebook.buck.android.apkmodule.APKModuleGraph,com.facebook.buck.android.apkmodule.APKModule,java.nio.file.Path,long,com.facebook.buck.android.DexStore,java.nio.file.Path,java.util.Optional)}

        -   #### PreDexedFilesSorter

                public PreDexedFilesSorter​(Collection<DexWithClasses> dexFilesToMerge,
                                           com.google.common.collect.ImmutableSet<String> primaryDexPatterns,
                                           APKModuleGraph apkModuleGraph,
                                           APKModule module,
                                           Path canaryDirectory,
                                           long dexWeightLimit,
                                           com.facebook.buck.android.DexStore dexStore,
                                           Path secondaryDexJarFilesDir,
                                           Optional<Integer> groupIndex)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#sortIntoPrimaryAndSecondaryDexes(com.facebook.buck.io.filesystem.ProjectFilesystem,com.google.common.collect.ImmutableList.Builder)}

        -   #### sortIntoPrimaryAndSecondaryDexes

            ``` methodSignature
            public PreDexedFilesSorter.Result sortIntoPrimaryAndSecondaryDexes​(ProjectFilesystem filesystem,
                                                                               com.google.common.collect.ImmutableList.Builder<Step> steps)
            ```

            ::: block
            Sorts dex files into primary and secondary dexes, generate
            canary classes, and metadata for use by SmartDexingStep
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

-   [Overview](../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../deprecated-list.html)
-   [Index](../../../../index-all.html)
-   [Help](../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../allclasses.html)

<div>

<div>

JavaScript is disabled on your browser.

</div>

</div>

<div>

-   Summary: 
-   [Nested](#nested.class.summary) \| 
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
