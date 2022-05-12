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

## Interface RuleKeyFactoryWithDiagnostics\<RULE_KEY\> {#interface-rulekeyfactorywithdiagnosticsrule_key .title title="Interface RuleKeyFactoryWithDiagnostics"}
:::

::: contentContainer
::: description
-   

    All Superinterfaces:
    :   `RuleKeyFactory<RULE_KEY>`

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `DefaultRuleKeyFactory`

    ------------------------------------------------------------------------

        public interface RuleKeyFactoryWithDiagnostics<RULE_KEY>
        extends RuleKeyFactory<RULE_KEY>

    ::: block
    A rule key factory that provides diagnostic facilities.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `<DIAG_KEY> Rul       | `buildForDiagn        | ::: block             |
        | eKeyDiagnostics.Resul | ostics​(BuildEngineAct | Builds a diagnostic   |
        | t<RULE_KEY,​DIAG_KEY>` | ion action,           | result for the given  |
        |                       |           RuleKeyHash | rule or appendable.   |
        |                       | er<DIAG_KEY> hasher)` | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `<DIAG_KEY> Rul       | `buildForDiagn        |                       |
        | eKeyDiagnostics.Resul | ostics​(AddsToRuleKey  |                       |
        | t<RULE_KEY,​DIAG_KEY>` | appendable,           |                       |
        |                       |           RuleKeyHash |                       |
        |                       | er<DIAG_KEY> hasher)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.rules.keys.RuleKeyFactory}

            ### Methods inherited from interface com.facebook.buck.rules.keys.[RuleKeyFactory](RuleKeyFactory.html "interface in com.facebook.buck.rules.keys")

            `build, getFromCache, getInputSizeLimit`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#buildForDiagnostics(com.facebook.buck.core.build.action.BuildEngineAction,com.facebook.buck.rules.keys.hasher.RuleKeyHasher)}

        -   #### buildForDiagnostics

            ``` methodSignature
            <DIAG_KEY> RuleKeyDiagnostics.Result<RULE_KEY,​DIAG_KEY> buildForDiagnostics​(BuildEngineAction action,
                                                                                              RuleKeyHasher<DIAG_KEY> hasher)
            ```

            ::: block
            Builds a diagnostic result for the given rule or appendable.
            This method is intended to be used exclusively for
            diagnostic purposes and not for computing rule keys used for
            build process in any other way.

            The provided custom hasher is used for all the elements
            hashed under this rule or appendable.

            Note however that if the factory chooses to hash nested
            build rules and appendables separately, and only include
            their final hash for the computation of this hash, this
            choice applies both to real rule keys and the diagnostic
            keys. The client may need to perform a separate call for
            each build rule or appendable of interest. Moreover, the
            hash for the nested build rules and appendables is obtained
            by using the default hasher and not the provided custom
            hasher. This is the natural choice as it allows the custom
            hasher to see precisely those elements that the default
            hasher sees. It is also more efficient because factories
            usually cache rule keys computed with the default hasher,
            whereas using the custom hasher prevents that and would
            require hashing all of its transitive dependencies.
            :::

        []{#buildForDiagnostics(com.facebook.buck.core.rulekey.AddsToRuleKey,com.facebook.buck.rules.keys.hasher.RuleKeyHasher)}

        -   #### buildForDiagnostics

            ``` methodSignature
            <DIAG_KEY> RuleKeyDiagnostics.Result<RULE_KEY,​DIAG_KEY> buildForDiagnostics​(AddsToRuleKey appendable,
                                                                                              RuleKeyHasher<DIAG_KEY> hasher)
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
