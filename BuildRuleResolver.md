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
[Package]{.packageLabelInType} [com.facebook.buck.core.rules](package-summary.html)
:::

## Interface BuildRuleResolver {#interface-buildruleresolver .title title="Interface BuildRuleResolver"}
:::

::: contentContainer
::: description
-   

    All Superinterfaces:
    :   `SourcePathRuleFinder`

    ```{=html}
    <!-- -->
    ```

    All Known Subinterfaces:
    :   `ActionGraphBuilder`

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `AbstractActionGraphBuilder`, `AbstractBuildRuleResolver`,
        `MultiThreadedActionGraphBuilder`,
        `RuleAnalysisCompatibleDelegatingActionGraphBuilder`

    ------------------------------------------------------------------------

        public interface BuildRuleResolver
        extends SourcePathRuleFinder

    ::: block
    Provides functions for resolving a BuildTarget to its BuildRule.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `com.google.com       | `g                    |                       |
        | mon.collect.Immutable | etAllRules​(Iterable<B |                       |
        | SortedSet<BuildRule>` | uildTarget> targets)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `BuildRule`           | `getRule​(Buil         | ::: block             |
        |                       | dTarget buildTarget)` | Returns the           |
        |                       |                       | `BuildRule`           |
        |                       |                       | associated with the   |
        |                       |                       | `buildTarget`.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<BuildRule>` | `getRuleOptional​(Buil | ::: block             |
        |                       | dTarget buildTarget)` | Returns the           |
        |                       |                       | `BuildRule`           |
        |                       |                       | associated with the   |
        |                       |                       | given `BuildTarget`   |
        |                       |                       | if it is already      |
        |                       |                       | present.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `<T> Optional<T>`     | `ge                   | ::: block             |
        |                       | tRuleOptionalWithType | Returns the           |
        |                       | ​(BuildTarget buildTar | `BuildRule`           |
        |                       | get,                  | associated with the   |
        |                       |        Class<T> cls)` | given `BuildTarget`   |
        |                       |                       | if it is already      |
        |                       |                       | present, casting it   |
        |                       |                       | to an expected type.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `<T> T`               | `getRule              | ::: block             |
        |                       | WithType​(BuildTarget  | Returns the           |
        |                       | buildTarget,          | `BuildRule`           |
        |                       |        Class<T> cls)` | associated with the   |
        |                       |                       | `buildTarget`,        |
        |                       |                       | casting it to an      |
        |                       |                       | expected type.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.SourcePathRuleFinder}

            ### Methods inherited from interface com.facebook.buck.core.rules.[SourcePathRuleFinder](SourcePathRuleFinder.html "interface in com.facebook.buck.core.rules")

            `filterBuildRuleInputs, filterBuildRuleInputs, filterBuildRuleInputs, filterBuildRuleInputs, getRule, getRule, getSourcePathResolver`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getRuleOptional(com.facebook.buck.core.model.BuildTarget)}

        -   #### getRuleOptional

            ``` methodSignature
            Optional<BuildRule> getRuleOptional​(BuildTarget buildTarget)
            ```

            ::: block
            Returns the `BuildRule` associated with the given
            `BuildTarget` if it is already present.
            :::

        []{#getRuleOptionalWithType(com.facebook.buck.core.model.BuildTarget,java.lang.Class)}

        -   #### getRuleOptionalWithType

            ``` methodSignature
            <T> Optional<T> getRuleOptionalWithType​(BuildTarget buildTarget,
                                                    Class<T> cls)
            ```

            ::: block
            Returns the `BuildRule` associated with the given
            `BuildTarget` if it is already present, casting it to an
            expected type.
            :::

            [Throws:]{.throwsLabel}
            :   `HumanReadableException` - if the `BuildRule` is not an
                instance of the given class.

        []{#getRule(com.facebook.buck.core.model.BuildTarget)}

        -   #### getRule

            ``` methodSignature
            BuildRule getRule​(BuildTarget buildTarget)
            ```

            ::: block
            Returns the `BuildRule` associated with the `buildTarget`.
            :::

            [Throws:]{.throwsLabel}
            :   `HumanReadableException` - if no BuildRule is associated
                with the `BuildTarget`.

        []{#getRuleWithType(com.facebook.buck.core.model.BuildTarget,java.lang.Class)}

        -   #### getRuleWithType

            ``` methodSignature
            <T> T getRuleWithType​(BuildTarget buildTarget,
                                  Class<T> cls)
            ```

            ::: block
            Returns the `BuildRule` associated with the `buildTarget`,
            casting it to an expected type.
            :::

            [Throws:]{.throwsLabel}
            :   `HumanReadableException` - if no rule is associated with
                the `BuildTarget`, or if the rule is not an instance of
                the given class.

        []{#getAllRules(java.lang.Iterable)}

        -   #### getAllRules

            ``` methodSignature
            com.google.common.collect.ImmutableSortedSet<BuildRule> getAllRules​(Iterable<BuildTarget> targets)
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
