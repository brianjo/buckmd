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
[Package]{.packageLabelInType} [com.facebook.buck.features.python.toolchain](package-summary.html)
:::

## Interface PythonPlatform {#interface-pythonplatform .title title="Interface PythonPlatform"}
:::

::: contentContainer
::: description
-   

    All Superinterfaces:
    :   `FlavorConvertible`

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `LazyPythonPlatform`

    ------------------------------------------------------------------------

        public interface PythonPlatform
        extends FlavorConvertible

    ::: block
    A toolchain that provides access to Python environment (an
    interpreter and its version) and cxx library.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                   Method                                 Description
          --------------------------------------------------- -------------------------------------- -------------
          `Optional<BuildTarget>`                             `getCxxLibrary()`                       
          `PythonEnvironment`                                 `getEnvironment()`                      
          `Flavor`                                            `getFlavor()`                           
          `com.google.common.collect.ImmutableList<String>`   `getInplaceBinaryInterpreterFlags()`    

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

        []{#getFlavor()}

        -   #### getFlavor

            ``` methodSignature
            Flavor getFlavor()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getFlavor` in interface `FlavorConvertible`

            [Returns:]{.returnLabel}
            :   the
                [`Flavor`](../../../core/model/Flavor.html "interface in com.facebook.buck.core.model")
                associated with this python platform.

        []{#getEnvironment()}

        -   #### getEnvironment

            ``` methodSignature
            PythonEnvironment getEnvironment()
            ```

            [Returns:]{.returnLabel}
            :   the
                [`PythonEnvironment`](PythonEnvironment.html "class in com.facebook.buck.features.python.toolchain")
                for this python platform.

        []{#getCxxLibrary()}

        -   #### getCxxLibrary

            ``` methodSignature
            Optional<BuildTarget> getCxxLibrary()
            ```

            [Returns:]{.returnLabel}
            :   the
                [`BuildTarget`](../../../core/model/BuildTarget.html "class in com.facebook.buck.core.model")
                wrapping the C/C++ library used by C/C++ extensions.

        []{#getInplaceBinaryInterpreterFlags()}

        -   #### getInplaceBinaryInterpreterFlags

            ``` methodSignature
            com.google.common.collect.ImmutableList<String> getInplaceBinaryInterpreterFlags()
            ```

            [Returns:]{.returnLabel}
            :   flags that should be added to the hashbang of inplace
                python binaries
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
