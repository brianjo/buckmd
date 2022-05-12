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

-   [Overview](../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../deprecated-list.html)
-   [Index](../../../../../../index-all.html)
-   [Help](../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.cxx.toolchain.linker](package-summary.html)
:::

## Interface HasImportLibrary {#interface-hasimportlibrary .title title="Interface HasImportLibrary"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `WindowsLinker`

    ------------------------------------------------------------------------

        public interface HasImportLibrary

    ::: block
    A windows shared library consists of two files: (1) a dll to be used
    at runtime and (2) an import library (static library) to be used to
    link against a given shared library. Wnen creating a dll, link.exe
    produces a dll file and a corresponding import library file. This
    interface represents those concepts.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                             Description
          ------------------- ---------------------------------- -------------
          `Iterable<Arg>`     `importLibrary​(Path output)`        
          `Path`              `importLibraryPath​(Path output)`    

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

        []{#importLibrary(java.nio.file.Path)}

        -   #### importLibrary

            ``` methodSignature
            Iterable<Arg> importLibrary​(Path output)
            ```

            [Parameters:]{.paramLabel}
            :   `output` - the path of the output binary

            [Returns:]{.returnLabel}
            :   the platform-specific way to generate an implib file.

        []{#importLibraryPath(java.nio.file.Path)}

        -   #### importLibraryPath

            ``` methodSignature
            Path importLibraryPath​(Path output)
            ```

            [Parameters:]{.paramLabel}
            :   `output` - the path of the output binary

            [Returns:]{.returnLabel}
            :   the path of the output binary\'s link-map file generated
                by the linker.
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

-   [Overview](../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../deprecated-list.html)
-   [Index](../../../../../../index-all.html)
-   [Help](../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../allclasses.html)

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
