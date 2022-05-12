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
[Package]{.packageLabelInType} [com.facebook.buck.core.toolchain](package-summary.html)
:::

## Interface ToolchainSupplier {#interface-toolchainsupplier .title title="Interface ToolchainSupplier"}
:::

::: contentContainer
::: description
-   

    All Superinterfaces:
    :   `org.pf4j.ExtensionPoint`

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `AndroidNdkToolchainsSupplier`, `AndroidSdkToolchainsSupplier`,
        `AppleToolchainsSupplier`, `CxxToolchainsSupplier`,
        `DotnetToolchainSupplier`, `DownloaderSupplier`,
        `GoToolchainSupplier`, `HaskellToolchainSupplier`,
        `InferToolchainSupplier`, `JavaToolchainsSupplier`,
        `LuaToolchainsSupplier`, `OcamlToolchainsSupplier`,
        `PythonToolchainsSupplier`, `RustToolchainSupplier`,
        `SwiftToolchainsSupplier`

    ------------------------------------------------------------------------

        public interface ToolchainSupplier
        extends org.pf4j.ExtensionPoint

    ::: block
    An `ExtensionPoint` which provides a way to register an arbitrary
    set of
    [`ToolchainDescriptor`](ToolchainDescriptor.html "interface in com.facebook.buck.core.toolchain")s.
    Clients that want to provide descriptions need to implement this
    interface and annotation that class with `Extension` annotation.

    For example:

           @Extension
           public class LanguageToolchainsSupplier implements ToolchainSupplier {
             @Override
             public Collection<ToolchainDescriptor<?>> getToolchainDescriptor() {
               return Arrays.asList(
                 new LanguageToolchainDescriptor()
               );
             }
           }
         

    Then the target with the client provider should be added to the
    dependencies of `  //src/com/facebook/buck/cli:main` target.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                      Method                       Description
          -------------------------------------- ---------------------------- -------------
          `Collection<ToolchainDescriptor<?>>`   `getToolchainDescriptor()`    

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

        []{#getToolchainDescriptor()}

        -   #### getToolchainDescriptor

            ``` methodSignature
            Collection<ToolchainDescriptor<?>> getToolchainDescriptor()
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
