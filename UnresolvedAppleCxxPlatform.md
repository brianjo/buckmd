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
[Package]{.packageLabelInType} [com.facebook.buck.apple.toolchain](package-summary.html)
:::

## Interface UnresolvedAppleCxxPlatform {#interface-unresolvedapplecxxplatform .title title="Interface UnresolvedAppleCxxPlatform"}
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
    :   `ProviderBackedUnresolvedAppleCxxPlatform`,
        `StaticUnresolvedAppleCxxPlatform`

    ------------------------------------------------------------------------

        public interface UnresolvedAppleCxxPlatform
        extends FlavorConvertible

    ::: block
    Used by descriptions to properly handle
    [`AppleCxxPlatform`](AppleCxxPlatform.html "class in com.facebook.buck.apple.toolchain").
    During parsing/configuration only information about parse-time deps
    is available. During action graph creation, this can be resolved to
    the final
    [`AppleCxxPlatform`](AppleCxxPlatform.html "class in com.facebook.buck.apple.toolchain").
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
        | `U                    | `getUnr               | ::: block             |
        | nresolvedCxxPlatform` | esolvedCxxPlatform()` | Returns the \@{link   |
        |                       |                       | U                     |
        |                       |                       | nresolvedCxxPlatform} |
        |                       |                       | corresponding to the  |
        |                       |                       | resolved              |
        |                       |                       | [`Apple               |
        |                       |                       | CxxPlatform`](AppleCx |
        |                       |                       | xPlatform.html "class |
        |                       |                       |  in com.facebook.buck |
        |                       |                       | .apple.toolchain")\'s |
        |                       |                       | [`CxxPlatform`](.     |
        |                       |                       | ./../cxx/toolchain/Cx |
        |                       |                       | xPlatform.html "inter |
        |                       |                       | face in com.facebook. |
        |                       |                       | buck.cxx.toolchain"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Unr                  | `getUnres             | ::: block             |
        | esolvedSwiftPlatform` | olvedSwiftPlatform()` | Returns the \@{link   |
        |                       |                       | Unr                   |
        |                       |                       | esolvedSwiftPlatform} |
        |                       |                       | corresponding to the  |
        |                       |                       | resolved              |
        |                       |                       | [`Apple               |
        |                       |                       | CxxPlatform`](AppleCx |
        |                       |                       | xPlatform.html "class |
        |                       |                       |  in com.facebook.buck |
        |                       |                       | .apple.toolchain")\'s |
        |                       |                       | [`CxxPlatform`](.     |
        |                       |                       | ./../cxx/toolchain/Cx |
        |                       |                       | xPlatform.html "inter |
        |                       |                       | face in com.facebook. |
        |                       |                       | buck.cxx.toolchain"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleCxxPlatform`    | `resolve​(BuildRuleRe  | ::: block             |
        |                       | solver ruleResolver)` | Returns the resolved  |
        |                       |                       | \@{link               |
        |                       |                       | AppleCxxPlatform}.    |
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
            AppleCxxPlatform resolve​(BuildRuleResolver ruleResolver)
            ```

            ::: block
            Returns the resolved \@{link AppleCxxPlatform}.
            :::

        []{#getUnresolvedCxxPlatform()}

        -   #### getUnresolvedCxxPlatform

            ``` methodSignature
            UnresolvedCxxPlatform getUnresolvedCxxPlatform()
            ```

            ::: block
            Returns the \@{link UnresolvedCxxPlatform} corresponding to
            the resolved
            [`AppleCxxPlatform`](AppleCxxPlatform.html "class in com.facebook.buck.apple.toolchain")\'s
            [`CxxPlatform`](../../cxx/toolchain/CxxPlatform.html "interface in com.facebook.buck.cxx.toolchain").
            :::

        []{#getUnresolvedSwiftPlatform()}

        -   #### getUnresolvedSwiftPlatform

            ``` methodSignature
            UnresolvedSwiftPlatform getUnresolvedSwiftPlatform()
            ```

            ::: block
            Returns the \@{link UnresolvedSwiftPlatform} corresponding
            to the resolved
            [`AppleCxxPlatform`](AppleCxxPlatform.html "class in com.facebook.buck.apple.toolchain")\'s
            [`CxxPlatform`](../../cxx/toolchain/CxxPlatform.html "interface in com.facebook.buck.cxx.toolchain").
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
