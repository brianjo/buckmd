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

-   [Overview](../../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../index-all.html)
-   [Help](../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.core.rules.analysis.impl](package-summary.html)
:::

## Class LegacyProviderRuleAnalysisResult {#class-legacyproviderruleanalysisresult .title title="Class LegacyProviderRuleAnalysisResult"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.rules.analysis.impl.LegacyProviderRuleAnalysisResult

::: description
-   

    All Implemented Interfaces:
    :   `ComputeResult`, `ActionAnalysisDataLookUp`,
        `RuleAnalysisResult`

    ------------------------------------------------------------------------

        public abstract class LegacyProviderRuleAnalysisResult
        extends Object
        implements RuleAnalysisResult

    ::: block
    An implementation of the
    [`RuleAnalysisResult`](../RuleAnalysisResult.html "interface in com.facebook.buck.core.rules.analysis")
    for legacy provider results from
    [`LegacyProviderCompatibleDescription.createProviders(ProviderCreationContext,  BuildTarget, BuildRuleArg)`](../../LegacyProviderCompatibleDescription.html#createProviders(com.facebook.buck.core.rules.ProviderCreationContext,com.facebook.buck.core.model.BuildTarget,T)).
    This implementation throws on any operation relating to
    [`ActionAnalysisData`](../action/ActionAnalysisData.html "interface in com.facebook.buck.core.rules.analysis.action")
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                            Description
          -------------------------------------- -------------
          `LegacyProviderRuleAnalysisResult()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                                    Method                                           Description
          ------------------------------------------------------------------------------------ ------------------------------------------------ -------------
          `boolean`                                                                            `actionExists​(ActionAnalysisData.ID key)`         
          `Optional<ActionAnalysisData>`                                                       `getActionOptional​(ActionAnalysisData.ID key)`    
          `abstract BuildTarget`                                                               `getBuildTarget()`                                
          `abstract ProviderInfoCollection`                                                    `getProviderInfos()`                              
          `com.google.common.collect.ImmutableMap<ActionAnalysisData.ID,​ActionAnalysisData>`   `getRegisteredActions()`                          

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Abstract
          Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
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

        []{#<init>()}

        -   #### LegacyProviderRuleAnalysisResult

                public LegacyProviderRuleAnalysisResult()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getBuildTarget()}

        -   #### getBuildTarget

            ``` methodSignature
            public abstract BuildTarget getBuildTarget()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getBuildTarget` in interface `RuleAnalysisResult`

            [Returns:]{.returnLabel}
            :   [`BuildTarget`](../../../model/BuildTarget.html "class in com.facebook.buck.core.model")
                of the rule

        []{#getProviderInfos()}

        -   #### getProviderInfos

            ``` methodSignature
            public abstract ProviderInfoCollection getProviderInfos()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getProviderInfos` in interface `RuleAnalysisResult`

            [Returns:]{.returnLabel}
            :   a
                [`ProviderInfoCollection`](../../providers/collect/ProviderInfoCollection.html "interface in com.facebook.buck.core.rules.providers.collect")
                exported by the rule

        []{#actionExists(com.facebook.buck.core.rules.analysis.action.ActionAnalysisData.ID)}

        -   #### actionExists

            ``` methodSignature
            public final boolean actionExists​(ActionAnalysisData.ID key)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `actionExists` in interface `ActionAnalysisDataLookUp`

            [Returns:]{.returnLabel}
            :   if the given key exists in the look up

        []{#getActionOptional(com.facebook.buck.core.rules.analysis.action.ActionAnalysisData.ID)}

        -   #### getActionOptional

            ``` methodSignature
            public final Optional<ActionAnalysisData> getActionOptional​(ActionAnalysisData.ID key)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getActionOptional` in
                interface `ActionAnalysisDataLookUp`

            [Returns:]{.returnLabel}
            :   the
                [`ActionAnalysisData`](../action/ActionAnalysisData.html "interface in com.facebook.buck.core.rules.analysis.action")
                if exists, else `Optional.empty`

        []{#getRegisteredActions()}

        -   #### getRegisteredActions

            ``` methodSignature
            public final com.google.common.collect.ImmutableMap<ActionAnalysisData.ID,​ActionAnalysisData> getRegisteredActions()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getRegisteredActions` in
                interface `ActionAnalysisDataLookUp`

            [Returns:]{.returnLabel}
            :   all the registered
                [`ActionAnalysisData`](../action/ActionAnalysisData.html "interface in com.facebook.buck.core.rules.analysis.action")
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

-   [Overview](../../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../index-all.html)
-   [Help](../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../allclasses.html)

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
