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
[Package]{.packageLabelInType} [com.facebook.buck.android](package-summary.html)
:::

## Interface AndroidLibraryCompilerFactory {#interface-androidlibrarycompilerfactory .title title="Interface AndroidLibraryCompilerFactory"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `DefaultAndroidLibraryCompilerFactory`

    ------------------------------------------------------------------------

        public interface AndroidLibraryCompilerFactory

    ::: block
    Factory providing implementations of
    [`ConfiguredCompilerFactory`](../jvm/java/ConfiguredCompilerFactory.html "class in com.facebook.buck.jvm.java")
    for the specified `  language`.
    [`AndroidLibraryDescription`](AndroidLibraryDescription.html "class in com.facebook.buck.android")
    uses this factory to handle multiple JVM languages. Implementations
    should provide a compiler implementation for every
    [`AndroidLibraryDescription.JvmLanguage`](AndroidLibraryDescription.JvmLanguage.html "enum in com.facebook.buck.android").
    See `DefaultAndroidLibraryCompiler`
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type             Method                                                                                                                                                             Description
          ----------------------------- ------------------------------------------------------------------------------------------------------------------------------------------------------------------ -------------
          `ConfiguredCompilerFactory`   `getCompiler​(AndroidLibraryDescription.JvmLanguage language,            JavacFactory javacFactory,            TargetConfiguration toolchainTargetConfiguration)`    

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

        []{#getCompiler(com.facebook.buck.android.AndroidLibraryDescription.JvmLanguage,com.facebook.buck.jvm.java.JavacFactory,com.facebook.buck.core.model.TargetConfiguration)}

        -   #### getCompiler

            ``` methodSignature
            ConfiguredCompilerFactory getCompiler​(AndroidLibraryDescription.JvmLanguage language,
                                                  JavacFactory javacFactory,
                                                  TargetConfiguration toolchainTargetConfiguration)
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
