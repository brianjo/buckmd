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
[Package]{.packageLabelInType} [com.facebook.buck.rules.keys](package-summary.html)
:::

## Interface RuleKeyAppendable.RuleKeyAppendableSink {#interface-rulekeyappendable.rulekeyappendablesink .title title="Interface RuleKeyAppendable.RuleKeyAppendableSink"}
:::

::: contentContainer
::: description
-   

    Enclosing interface:
    :   [RuleKeyAppendable](RuleKeyAppendable.html "interface in com.facebook.buck.rules.keys")

    ------------------------------------------------------------------------

        @Deprecated
        public static interface RuleKeyAppendable.RuleKeyAppendableSink

    ::: deprecationBlock
    [Deprecated.]{.deprecatedLabel}
    :::

    ::: block
    Deprecated. Implementations of
    [`RuleKeyAppendable`](RuleKeyAppendable.html "interface in com.facebook.buck.rules.keys")
    use this to add things to rulekey builders.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `void`                | `ad                   | ::: block             |
        |                       | dValue​(Path key,      | [Deprecate            |
        |                       |     SourcePath path)` | d.]{.deprecatedLabel} |
        |                       |                       | :::                   |
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

        []{#addValue(java.nio.file.Path,com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### addValue

            ``` methodSignature
            @Deprecated
            void addValue​(Path key,
                          SourcePath path)
            ```

            ::: deprecationBlock
            [Deprecated.]{.deprecatedLabel}
            :::

            ::: block
            Add stringified paths as keys. The paths in represent
            include directives rather than actual on-disk locations. One
            possibly non-obvious thing here is that the key will only be
            added to the rulekey if the path is. If the rulekeybuilder
            ignores the path, the key won\'t be added.
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
