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
[Package]{.packageLabelInType} [com.facebook.buck.cxx.toolchain](package-summary.html)
:::

## Interface UnresolvedCxxPlatform {#interface-unresolvedcxxplatform .title title="Interface UnresolvedCxxPlatform"}
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
    :   `ProviderBasedUnresolvedCxxPlatform`,
        `StaticUnresolvedCxxPlatform`

    ------------------------------------------------------------------------

        public interface UnresolvedCxxPlatform
        extends FlavorConvertible

    ::: block
    Used by descriptions to properly handle
    [`CxxPlatform`](CxxPlatform.html "interface in com.facebook.buck.cxx.toolchain").
    During parsing/configuration only information about parse-time deps
    is available. During action graph creation, this can be resolved to
    the final
    [`CxxPlatform`](CxxPlatform.html "interface in com.facebook.buck.cxx.toolchain").
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `Flavor`              | `getFlavor()`         |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Iterable<?           | `g                    | ::: block             |
        | extends BuildTarget>` | etLinkerParseTimeDeps | This probably         |
        |                       | ​(TargetConfiguration  | shouldn\'t exist.     |
        |                       | targetConfiguration)` | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `I                    | `getParseTimeDeps     | ::: block             |
        | terable<BuildTarget>` | ​(TargetConfiguration  | Returns the           |
        |                       | targetConfiguration)` | parse-time deps       |
        |                       |                       | required for this     |
        |                       |                       | platform.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxPlatform`         | `                     | ::: block             |
        |                       | resolve​(BuildRuleReso | Resolves the          |
        |                       | lver resolver,        | platform.             |
        |                       |  TargetConfiguration  | :::                   |
        |                       | targetConfiguration)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `U                    | `withFlavo            | ::: block             |
        | nresolvedCxxPlatform` | r​(Flavor hostFlavor)` | Returns this provider |
        |                       |                       | as a different        |
        |                       |                       | flavor.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

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

        []{#resolve(com.facebook.buck.core.rules.BuildRuleResolver,com.facebook.buck.core.model.TargetConfiguration)}

        -   #### resolve

            ``` methodSignature
            CxxPlatform resolve​(BuildRuleResolver resolver,
                                TargetConfiguration targetConfiguration)
            ```

            ::: block
            Resolves the platform.
            :::

        []{#getFlavor()}

        -   #### getFlavor

            ``` methodSignature
            Flavor getFlavor()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getFlavor` in interface `FlavorConvertible`

        []{#withFlavor(com.facebook.buck.core.model.Flavor)}

        -   #### withFlavor

            ``` methodSignature
            UnresolvedCxxPlatform withFlavor​(Flavor hostFlavor)
            ```

            ::: block
            Returns this provider as a different flavor. This might only
            make sense for .buckconfig-configured cxx platforms and be
            removed in the future.
            :::

        []{#getParseTimeDeps(com.facebook.buck.core.model.TargetConfiguration)}

        -   #### getParseTimeDeps

            ``` methodSignature
            Iterable<BuildTarget> getParseTimeDeps​(TargetConfiguration targetConfiguration)
            ```

            ::: block
            Returns the parse-time deps required for this platform.
            :::

        []{#getLinkerParseTimeDeps(com.facebook.buck.core.model.TargetConfiguration)}

        -   #### getLinkerParseTimeDeps

            ``` methodSignature
            Iterable<? extends BuildTarget> getLinkerParseTimeDeps​(TargetConfiguration targetConfiguration)
            ```

            ::: block
            This probably shouldn\'t exist. Users probably shouldn\'t be
            able to specify specific individual pieces of the platform
            that they want to use. If you\'re tempted to use this, use
            getParseTimeDeps() instead or update this comment with your
            valid use case.
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
