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
[Package]{.packageLabelInType} [com.facebook.buck.core.rules.config](package-summary.html)
:::

## Interface ConfigurationRuleResolver {#interface-configurationruleresolver .title title="Interface ConfigurationRuleResolver"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `SameThreadConfigurationRuleResolver`

    ------------------------------------------------------------------------

        public interface ConfigurationRuleResolver

    ::: block
    Provides access to
    [`ConfigurationRule`](ConfigurationRule.html "interface in com.facebook.buck.core.rules.config").
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `<R extends           | `getRule​(BuildTar     | ::: block             |
        |  ConfigurationRule>R` | get buildTarget,      | Returns the           |
        |                       |    Class<R> ruleClass | [`Configurat          |
        |                       | ,        DependencySt | ionRule`](Configurati |
        |                       | ack dependencyStack)` | onRule.html "interfac |
        |                       |                       | e in com.facebook.buc |
        |                       |                       | k.core.rules.config") |
        |                       |                       | associated with the   |
        |                       |                       | given                 |
        |                       |                       | [`                    |
        |                       |                       | BuildTarget`](../../m |
        |                       |                       | odel/BuildTarget.html |
        |                       |                       |  "class in com.facebo |
        |                       |                       | ok.buck.core.model"). |
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

        []{#getRule(com.facebook.buck.core.model.BuildTarget,java.lang.Class,com.facebook.buck.core.exceptions.DependencyStack)}

        -   #### getRule

            ``` methodSignature
            <R extends ConfigurationRule> R getRule​(BuildTarget buildTarget,
                                                    Class<R> ruleClass,
                                                    DependencyStack dependencyStack)
            ```

            ::: block
            Returns the
            [`ConfigurationRule`](ConfigurationRule.html "interface in com.facebook.buck.core.rules.config")
            associated with the given
            [`BuildTarget`](../../model/BuildTarget.html "class in com.facebook.buck.core.model").
            :::

            [Throws:]{.throwsLabel}
            :   `HumanReadableException` - if no rule is associated with
                the target.
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
