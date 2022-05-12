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
[Package]{.packageLabelInType} [com.facebook.buck.android.toolchain.ndk](package-summary.html)
:::

## Interface UnresolvedNdkCxxPlatform {#interface-unresolvedndkcxxplatform .title title="Interface UnresolvedNdkCxxPlatform"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `ProviderBackedUnresolvedNdkCxxPlatform`,
        `StaticUnresolvedNdkCxxPlatform`

    ------------------------------------------------------------------------

        public interface UnresolvedNdkCxxPlatform

    ::: block
    Used by descriptions to properly handle
    [`NdkCxxPlatform`](NdkCxxPlatform.html "interface in com.facebook.buck.android.toolchain.ndk").
    During parsing/configuration only information about parse-time deps
    is available. During action graph creation, this can be resolved to
    the final
    [`NdkCxxPlatform`](NdkCxxPlatform.html "interface in com.facebook.buck.android.toolchain.ndk").
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `U                    | `getCxxPlatform()`    | ::: block             |
        | nresolvedCxxPlatform` |                       | Returns the \@{link   |
        |                       |                       | U                     |
        |                       |                       | nresolvedCxxPlatform} |
        |                       |                       | corresponding to the  |
        |                       |                       | resolved              |
        |                       |                       | [`NdkCxxPlatf         |
        |                       |                       | orm`](NdkCxxPlatform. |
        |                       |                       | html "interface in co |
        |                       |                       | m.facebook.buck.andro |
        |                       |                       | id.toolchain.ndk")\'s |
        |                       |                       | [`CxxPlatform`](../.  |
        |                       |                       | ./../cxx/toolchain/Cx |
        |                       |                       | xPlatform.html "inter |
        |                       |                       | face in com.facebook. |
        |                       |                       | buck.cxx.toolchain"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `I                    | `getParseTimeDeps     | ::: block             |
        | terable<BuildTarget>` | ​(TargetConfiguration  | Returns the parse     |
        |                       | targetConfiguration)` | time deps of this     |
        |                       |                       | platform.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `NdkCxxPlatform`      | `resolve​(BuildRuleRe  | ::: block             |
        |                       | solver ruleResolver)` | Returns the resolved  |
        |                       |                       | \@{link               |
        |                       |                       | NdkCxxPlatform}.      |
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
            NdkCxxPlatform resolve​(BuildRuleResolver ruleResolver)
            ```

            ::: block
            Returns the resolved \@{link NdkCxxPlatform}.
            :::

        []{#getCxxPlatform()}

        -   #### getCxxPlatform

            ``` methodSignature
            UnresolvedCxxPlatform getCxxPlatform()
            ```

            ::: block
            Returns the \@{link UnresolvedCxxPlatform} corresponding to
            the resolved
            [`NdkCxxPlatform`](NdkCxxPlatform.html "interface in com.facebook.buck.android.toolchain.ndk")\'s
            [`CxxPlatform`](../../../cxx/toolchain/CxxPlatform.html "interface in com.facebook.buck.cxx.toolchain").
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
