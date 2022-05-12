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

## Interface DexWithClasses {#interface-dexwithclasses .title title="Interface DexWithClasses"}
:::

::: contentContainer
::: description
-   

    ------------------------------------------------------------------------

        public interface DexWithClasses

    ::: block
    Object that represents a `.dex.jar` file that knows what `.class`
    files went into it, as well as its estimated dex weight.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type                                                                 Field                           Description
          --------------------------------------------------------------------------------- ------------------------------- -------------
          `static Comparator<DexWithClasses>`                                               `DEX_WITH_CLASSES_COMPARATOR`    
          `static java.util.function.Function<DexProducedFromJavaLibrary,​DexWithClasses>`   `TO_DEX_WITH_CLASSES`            

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                  Method                       Description
          -------------------------------------------------- ---------------------------- -------------
          `Sha1HashCode`                                     `getClassesHash()`            
          `com.google.common.collect.ImmutableSet<String>`   `getClassNames()`             
          `BuildTarget`                                      `getSourceBuildTarget()`      
          `SourcePath`                                       `getSourcePathToDexFile()`    
          `int`                                              `getWeightEstimate()`         

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Abstract
          Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#field.detail}

        ### Field Detail

        []{#TO_DEX_WITH_CLASSES}

        -   #### TO_DEX_WITH_CLASSES

                static final java.util.function.Function<DexProducedFromJavaLibrary,​DexWithClasses> TO_DEX_WITH_CLASSES

        []{#DEX_WITH_CLASSES_COMPARATOR}

        -   #### DEX_WITH_CLASSES_COMPARATOR

                static final Comparator<DexWithClasses> DEX_WITH_CLASSES_COMPARATOR
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getSourceBuildTarget()}

        -   #### getSourceBuildTarget

            ``` methodSignature
            @Nullable
            BuildTarget getSourceBuildTarget()
            ```

        []{#getSourcePathToDexFile()}

        -   #### getSourcePathToDexFile

            ``` methodSignature
            SourcePath getSourcePathToDexFile()
            ```

            [Returns:]{.returnLabel}
            :   path from the project root where the `.dex.jar` file can
                be found.

        []{#getClassNames()}

        -   #### getClassNames

            ``` methodSignature
            com.google.common.collect.ImmutableSet<String> getClassNames()
            ```

            [Returns:]{.returnLabel}
            :   the names of the `.class` files that went into the DEX
                file.

        []{#getClassesHash()}

        -   #### getClassesHash

            ``` methodSignature
            Sha1HashCode getClassesHash()
            ```

            [Returns:]{.returnLabel}
            :   a hash of the `.class` files that went into the DEX
                file.

        []{#getWeightEstimate()}

        -   #### getWeightEstimate

            ``` methodSignature
            int getWeightEstimate()
            ```

            [Returns:]{.returnLabel}
            :   A value that estimates how much space the Dalvik code
                represented by this object will take up in a DEX file.
                The units for this estimate are not important, so long
                as they are consistent with those used by
                [`PreDexedFilesSorter`](PreDexedFilesSorter.html "class in com.facebook.buck.android")
                to determine how secondary DEX files should be packed.
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
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
