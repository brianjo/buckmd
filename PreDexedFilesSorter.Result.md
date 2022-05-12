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
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
-   [Constr](#constructor.detail) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.android](package-summary.html)
:::

## Class PreDexedFilesSorter.Result {#class-predexedfilessorter.result .title title="Class PreDexedFilesSorter.Result"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.android.PreDexedFilesSorter.Result

::: description
-   

    Enclosing class:
    :   [PreDexedFilesSorter](PreDexedFilesSorter.html "class in com.facebook.buck.android")

    ------------------------------------------------------------------------

        public static class PreDexedFilesSorter.Result
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type                                                   Field                       Description
          ------------------------------------------------------------------- --------------------------- -------------
          `Map<Path,​DexWithClasses>`                                          `metadataTxtDexEntries`      
          `com.facebook.buck.android.ImmutablePrimaryDexInputMetadata`        `primaryDexInputMetadata`    
          `Map<String,​SourcePath>`                                            `primaryDexInputs`           
          `com.google.common.collect.ImmutableMap<SourcePath,​Sha1HashCode>`   `secondaryDexInputHashes`    
          `com.google.common.collect.Multimap<Path,​SourcePath>`               `secondaryOutputToInputs`    

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                                                                                                                           Description
          ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `Result​(Map<String,​SourcePath> primaryDexInputs,       com.google.common.collect.Multimap<Path,​SourcePath> secondaryOutputToInputs,       Map<Path,​DexWithClasses> metadataTxtDexEntries,       com.facebook.buck.android.ImmutablePrimaryDexInputMetadata primaryDexInputMetadata,       com.google.common.collect.ImmutableMap<SourcePath,​Sha1HashCode> secondaryDexInputHashes)`    

          : Constructors[ ]{.tabEnd}
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

        []{#primaryDexInputs}

        -   #### primaryDexInputs

                public final Map<String,​SourcePath> primaryDexInputs

        []{#secondaryOutputToInputs}

        -   #### secondaryOutputToInputs

                public final com.google.common.collect.Multimap<Path,​SourcePath> secondaryOutputToInputs

        []{#metadataTxtDexEntries}

        -   #### metadataTxtDexEntries

                public final Map<Path,​DexWithClasses> metadataTxtDexEntries

        []{#primaryDexInputMetadata}

        -   #### primaryDexInputMetadata

                public final com.facebook.buck.android.ImmutablePrimaryDexInputMetadata primaryDexInputMetadata

        []{#secondaryDexInputHashes}

        -   #### secondaryDexInputHashes

                public final com.google.common.collect.ImmutableMap<SourcePath,​Sha1HashCode> secondaryDexInputHashes
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(java.util.Map,com.google.common.collect.Multimap,java.util.Map,com.facebook.buck.android.ImmutablePrimaryDexInputMetadata,com.google.common.collect.ImmutableMap)}

        -   #### Result

                public Result​(Map<String,​SourcePath> primaryDexInputs,
                              com.google.common.collect.Multimap<Path,​SourcePath> secondaryOutputToInputs,
                              Map<Path,​DexWithClasses> metadataTxtDexEntries,
                              com.facebook.buck.android.ImmutablePrimaryDexInputMetadata primaryDexInputMetadata,
                              com.google.common.collect.ImmutableMap<SourcePath,​Sha1HashCode> secondaryDexInputHashes)
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
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
-   [Constr](#constructor.detail) \| 
-   Method

</div>

[]{#skip.navbar.bottom}
:::
