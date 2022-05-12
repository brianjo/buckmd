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
[Package]{.packageLabelInType} [com.facebook.buck.cxx](package-summary.html)
:::

## Interface CxxLibraryDescriptionDelegate {#interface-cxxlibrarydescriptiondelegate .title title="Interface CxxLibraryDescriptionDelegate"}
:::

::: contentContainer
::: description
-   

    ------------------------------------------------------------------------

        public interface CxxLibraryDescriptionDelegate

    ::: block
    Defines a plugin interface for
    [`CxxLibraryDescription`](CxxLibraryDescription.html "class in com.facebook.buck.cxx")
    so that its behavior can be extended. This is usually useful for
    description that use
    [`CxxLibraryDescription`](CxxLibraryDescription.html "class in com.facebook.buck.cxx")
    as a delegate (e.g.,
    [`AppleLibraryDescription`](../apple/AppleLibraryDescription.html "class in com.facebook.buck.apple").
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Interface             | Description           |
        +=======================+=======================+=======================+
        | `static interface `   | `CxxLibr              | ::: block             |
        |                       | aryDescriptionDelegat | The delegate for a    |
        |                       | e.ConfiguredDelegate` | specific target and   |
        |                       |                       | platform.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                              Method                                                                                                                       Description
          -------------------------------------------------------------- ---------------------------------------------------------------------------------------------------------------------------- -------------
          `static CxxLibraryDescriptionDelegate`                         `noop()`                                                                                                                      
          `Optional<CxxLibraryDescriptionDelegate.ConfiguredDelegate>`   `requireDelegate​(BuildTarget target,                CxxPlatform platform,                ActionGraphBuilder graphBuilder)`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
          Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
          .tableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Abstract
          Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#requireDelegate(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.cxx.toolchain.CxxPlatform,com.facebook.buck.core.rules.ActionGraphBuilder)}

        -   #### requireDelegate

            ``` methodSignature
            Optional<CxxLibraryDescriptionDelegate.ConfiguredDelegate> requireDelegate​(BuildTarget target,
                                                                                       CxxPlatform platform,
                                                                                       ActionGraphBuilder graphBuilder)
            ```

        []{#noop()}

        -   #### noop

            ``` methodSignature
            static CxxLibraryDescriptionDelegate noop()
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
