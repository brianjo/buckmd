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
[Package]{.packageLabelInType} [com.facebook.buck.swift.toolchain](package-summary.html)
:::

## Interface UnresolvedSwiftPlatform {#interface-unresolvedswiftplatform .title title="Interface UnresolvedSwiftPlatform"}
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
    :   `StaticUnresolvedSwiftPlatform`

    ------------------------------------------------------------------------

        public interface UnresolvedSwiftPlatform
        extends FlavorConvertible

    ::: block
    Used by descriptions to properly handle
    [`SwiftPlatform`](SwiftPlatform.html "interface in com.facebook.buck.swift.toolchain").
    During parsing/configuration only information about parse-time deps
    is available. During action graph creation, this can be resolved to
    the final
    [`SwiftPlatform`](SwiftPlatform.html "interface in com.facebook.buck.swift.toolchain").
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `I                    | `getParseTimeDeps     | ::: block             |
        | terable<BuildTarget>` | ​(TargetConfiguration  | Returns the parse     |
        |                       | targetConfiguration)` | time deps of this     |
        |                       |                       | platform.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Opt                  | `resolve​(BuildRuleRe  | ::: block             |
        | ional<SwiftPlatform>` | solver ruleResolver)` | Returns the resolved  |
        |                       |                       | \@{link               |
        |                       |                       | NdkCxxPlatform}.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.core.model.FlavorConvertible}

            ### Methods inherited from interface com.facebook.buck.core.model.[FlavorConvertible](../../core/model/FlavorConvertible.html "interface in com.facebook.buck.core.model")

            `getFlavor`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getParseTimeDeps(com.facebook.buck.core.model.TargetConfiguration)}

        -   #### getParseTimeDeps

            ``` methodSignature
            Iterable<BuildTarget> getParseTimeDeps​(TargetConfiguration targetConfiguration)
            ```

            ::: block
            Returns the parse time deps of this platform.
            :::

        []{#resolve(com.facebook.buck.core.rules.BuildRuleResolver)}

        -   #### resolve

            ``` methodSignature
            Optional<SwiftPlatform> resolve​(BuildRuleResolver ruleResolver)
            ```

            ::: block
            Returns the resolved \@{link NdkCxxPlatform}.
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
