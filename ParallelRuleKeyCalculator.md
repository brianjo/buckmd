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
[Package]{.packageLabelInType} [com.facebook.buck.core.rulekey.calculator](package-summary.html)
:::

## Class ParallelRuleKeyCalculator\<T\> {#class-parallelrulekeycalculatort .title title="Class ParallelRuleKeyCalculator"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.rulekey.calculator.ParallelRuleKeyCalculator\<T\>

::: description
-   

    ------------------------------------------------------------------------

        public class ParallelRuleKeyCalculator<T>
        extends Object

    ::: block
    Calculates
    [`RuleKey`](../RuleKey.html "class in com.facebook.buck.core.rulekey"),
    bottom-up, using tree parallelism.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                                                                      Description
          -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `ParallelRuleKeyCalculator​(com.google.common.util.concurrent.ListeningExecutorService service,                          RuleKeyFactory<T> ruleKeyFactory,                          RuleDepsCache ruleDepsCache,                          java.util.function.BiFunction<BuckEventBus,​BuildRule,​Scope> ruleKeyCalculationScope)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                         Method                                                            Description
          --------------------------------------------------------- ----------------------------------------------------------------- -------------
          `com.google.common.util.concurrent.ListenableFuture<T>`   `calculate​(BuckEventBus buckEventBus,          BuildRule rule)`    
          `Set<BuildTarget>`                                        `getAllKnownTargets()`                                             
          `RuleDepsCache`                                           `getRuleDepsCache()`                                               

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
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

        []{#<init>(com.google.common.util.concurrent.ListeningExecutorService,com.facebook.buck.rules.keys.RuleKeyFactory,com.facebook.buck.core.build.engine.RuleDepsCache,java.util.function.BiFunction)}

        -   #### ParallelRuleKeyCalculator

                public ParallelRuleKeyCalculator​(com.google.common.util.concurrent.ListeningExecutorService service,
                                                 RuleKeyFactory<T> ruleKeyFactory,
                                                 RuleDepsCache ruleDepsCache,
                                                 java.util.function.BiFunction<BuckEventBus,​BuildRule,​Scope> ruleKeyCalculationScope)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#calculate(com.facebook.buck.event.BuckEventBus,com.facebook.buck.core.rules.BuildRule)}

        -   #### calculate

            ``` methodSignature
            public com.google.common.util.concurrent.ListenableFuture<T> calculate​(BuckEventBus buckEventBus,
                                                                                   BuildRule rule)
            ```

            [Returns:]{.returnLabel}
            :   a `ListenableFuture` wrapping the result of calculating
                the
                [`RuleKey`](../RuleKey.html "class in com.facebook.buck.core.rulekey")
                of the given
                [`BuildRule`](../../rules/BuildRule.html "interface in com.facebook.buck.core.rules").

        []{#getAllKnownTargets()}

        -   #### getAllKnownTargets

            ``` methodSignature
            public Set<BuildTarget> getAllKnownTargets()
            ```

        []{#getRuleDepsCache()}

        -   #### getRuleDepsCache

            ``` methodSignature
            public RuleDepsCache getRuleDepsCache()
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
