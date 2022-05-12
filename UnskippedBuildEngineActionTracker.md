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
[Package]{.packageLabelInType} [com.facebook.buck.core.build.engine.impl](package-summary.html)
:::

## Class UnskippedBuildEngineActionTracker {#class-unskippedbuildengineactiontracker .title title="Class UnskippedBuildEngineActionTracker"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.build.engine.impl.UnskippedBuildEngineActionTracker

::: description
-   

    ------------------------------------------------------------------------

        public class UnskippedBuildEngineActionTracker
        extends Object

    ::: block
    Keeps track of the number of
    [`BuildEngineAction`](../../action/BuildEngineAction.html "interface in com.facebook.buck.core.build.action")
    that either were already executed or might be executed in the
    future. This class assumes that a
    [`BuildEngineAction`](../../action/BuildEngineAction.html "interface in com.facebook.buck.core.build.action")
    that was not yet executed might be executed in the future if either
    there is a dependency path from a top level
    [`BuildEngineAction`](../../action/BuildEngineAction.html "interface in com.facebook.buck.core.build.action")
    to this
    [`BuildEngineAction`](../../action/BuildEngineAction.html "interface in com.facebook.buck.core.build.action")
    such that no rule on the path was yet executed or the rule is a
    runtime dependency of a rule fulfilling the previous condition. This
    model is consistent with
    [`CachingBuildEngine`](CachingBuildEngine.html "class in com.facebook.buck.core.build.engine.impl")\'s
    shallow build mode. The class uses reference counting to efficiently
    keep track of those
    [`BuildEngineAction`](../../action/BuildEngineAction.html "interface in com.facebook.buck.core.build.action").
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                         Description
          ----------------------------------------------------------------------------------------------------------------------------------- -------------
          `UnskippedBuildEngineActionTracker​(RuleDepsCache ruleDepsCache,                                  BuildRuleResolver ruleResolver)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                                                                                        Description
          ------------------- --------------------------------------------------------------------------------------------- -------------
          `void`              `markRuleAsUsed​(BuildEngineAction action,               BuckEventBus eventBus)`                
          `void`              `registerTopLevelRule​(BuildEngineAction action,                     BuckEventBus eventBus)`    

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

        []{#<init>(com.facebook.buck.core.build.engine.RuleDepsCache,com.facebook.buck.core.rules.BuildRuleResolver)}

        -   #### UnskippedBuildEngineActionTracker

                public UnskippedBuildEngineActionTracker​(RuleDepsCache ruleDepsCache,
                                                         BuildRuleResolver ruleResolver)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#registerTopLevelRule(com.facebook.buck.core.build.action.BuildEngineAction,com.facebook.buck.event.BuckEventBus)}

        -   #### registerTopLevelRule

            ``` methodSignature
            public void registerTopLevelRule​(BuildEngineAction action,
                                             BuckEventBus eventBus)
            ```

        []{#markRuleAsUsed(com.facebook.buck.core.build.action.BuildEngineAction,com.facebook.buck.event.BuckEventBus)}

        -   #### markRuleAsUsed

            ``` methodSignature
            public void markRuleAsUsed​(BuildEngineAction action,
                                       BuckEventBus eventBus)
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
