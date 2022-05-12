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
[Package]{.packageLabelInType} [com.facebook.buck.core.rules.attr](package-summary.html)
:::

## Interface HasCustomDepsLogic {#interface-hascustomdepslogic .title title="Interface HasCustomDepsLogic"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `CxxHeaders`, `CxxHeadersDir`, `CxxRawHeaders`,
        `CxxSymlinkTreeHeaders`

    ------------------------------------------------------------------------

        @Deprecated
        public interface HasCustomDepsLogic

    ::: deprecationBlock
    [Deprecated.]{.deprecatedLabel}
    :::

    ::: block
    Deriving deps directly from the \@AddToRuleKey annotated fields of
    some objects doesn\'t work correctly or is too slow. When deriving
    deps from an object that implements HasCustomDepsLogic, the
    framework (BuildableSupport/ModernBuildRule) will call getDeps()
    instead of deriving from \@AddToRuleKey fields.
    This is primarily meant to ease the transition to a state where all
    deps are derived automatically.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `java.util.stre       | `getDeps​(SourcePathRu | ::: block             |
        | am.Stream<BuildRule>` | leFinder ruleFinder)` | [Deprecate            |
        |                       |                       | d.]{.deprecatedLabel} |
        |                       |                       | :::                   |
        |                       |                       |                       |
        |                       |                       |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
        .tableTab}[[Deprecated
        Methods](javascript:show(32);)[ ]{.tabEnd}]{#t6 .tableTab}
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getDeps(com.facebook.buck.core.rules.SourcePathRuleFinder)}

        -   #### getDeps

            ``` methodSignature
            java.util.stream.Stream<BuildRule> getDeps​(SourcePathRuleFinder ruleFinder)
            ```

            ::: deprecationBlock
            [Deprecated.]{.deprecatedLabel}
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
