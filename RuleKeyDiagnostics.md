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
-   [Nested](#nested.class.summary) \| 
-   Field \| 
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   [Constr](#constructor.detail) \| 
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

## Class RuleKeyDiagnostics\<RULE_KEY,​DIAG_KEY\> {#class-rulekeydiagnosticsrule_keydiag_key .title title="Class RuleKeyDiagnostics"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.rules.keys.RuleKeyDiagnostics\<RULE_KEY,​DIAG_KEY\>

::: description
-   

    ------------------------------------------------------------------------

        @ThreadSafe
        public class RuleKeyDiagnostics<RULE_KEY,​DIAG_KEY>
        extends Object

    ::: block
    Contains functionality related to rulekey diagnostics.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type   Class                                            Description
          ------------------- ------------------------------------------------ -------------
          `static class `     `RuleKeyDiagnostics.Result<RULE_KEY,​DIAG_KEY>`    

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                        Description
          ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ -------------
          `RuleKeyDiagnostics​(java.util.function.Function<BuildRule,​RuleKeyDiagnostics.Result<RULE_KEY,​DIAG_KEY>> ruleResultSupplier,                   java.util.function.Function<AddsToRuleKey,​RuleKeyDiagnostics.Result<RULE_KEY,​DIAG_KEY>> appendableResultSupplier)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `s                    | `nop()`               |                       |
        | tatic <RULE_KEY,​DIAG_ |                       |                       |
        | KEY>RuleKeyDiagnostic |                       |                       |
        | s<RULE_KEY,​DIAG_KEY>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `pro                  | ::: block             |
        |                       | cessRule​(BuildRule ru | Computes the          |
        |                       | le,            java.u | diagnostic rulekey    |
        |                       | til.function.Consumer | data for the given    |
        |                       | <RuleKeyDiagnostics.R | rule and all of its   |
        |                       | esult<RULE_KEY,​DIAG_K | appendables           |
        |                       | EY>> resultConsumer)` | recursively.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(java.util.function.Function,java.util.function.Function)}

        -   #### RuleKeyDiagnostics

                public RuleKeyDiagnostics​(java.util.function.Function<BuildRule,​RuleKeyDiagnostics.Result<RULE_KEY,​DIAG_KEY>> ruleResultSupplier,
                                          java.util.function.Function<AddsToRuleKey,​RuleKeyDiagnostics.Result<RULE_KEY,​DIAG_KEY>> appendableResultSupplier)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#nop()}

        -   #### nop

            ``` methodSignature
            public static <RULE_KEY,​DIAG_KEY> RuleKeyDiagnostics<RULE_KEY,​DIAG_KEY> nop()
            ```

        []{#processRule(com.facebook.buck.core.rules.BuildRule,java.util.function.Consumer)}

        -   #### processRule

            ``` methodSignature
            public void processRule​(BuildRule rule,
                                    java.util.function.Consumer<RuleKeyDiagnostics.Result<RULE_KEY,​DIAG_KEY>> resultConsumer)
            ```

            ::: block
            Computes the diagnostic rulekey data for the given rule and
            all of its appendables recursively. Previously processed
            rules and appendables are skipped and not fed to the
            consumer. Results for the newly processed rule and
            appendables are fed to the consumer, but not stored
            otherwise. Only information of whether something has been
            processed or not gets stored.
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
-   [Nested](#nested.class.summary) \| 
-   Field \| 
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   [Constr](#constructor.detail) \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
