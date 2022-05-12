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
[Package]{.packageLabelInType} [com.facebook.buck.core.build.engine](package-summary.html)
:::

## Class DelegatingBuildStrategyContext {#class-delegatingbuildstrategycontext .title title="Class DelegatingBuildStrategyContext"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.build.engine.DelegatingBuildStrategyContext

::: description
-   

    All Implemented Interfaces:
    :   `BuildStrategyContext`

    ------------------------------------------------------------------------

        public class DelegatingBuildStrategyContext
        extends Object
        implements BuildStrategyContext

    ::: block
    A simple delegate
    [`BuildStrategyContext`](BuildStrategyContext.html "interface in com.facebook.buck.core.build.engine")
    to make it easier to change parts of the behavior.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                              Description
          ------------------------------------------------------------------------ -------------
          `DelegatingBuildStrategyContext​(BuildStrategyContext delegateContext)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                             Method                                                                                                    Description
          ----------------------------------------------------------------------------- --------------------------------------------------------------------------------------------------------- -------------
          `Scope`                                                                       `buildRuleScope()`                                                                                         
          `BuildResult`                                                                 `createBuildResult​(BuildRuleSuccessType successType,                  Optional<String> strategyResult)`    
          `BuildResult`                                                                 `createCancelledResult​(Throwable throwable)`                                                               
          `BuildableContext`                                                            `getBuildableContext()`                                                                                    
          `BuildContext`                                                                `getBuildRuleBuildContext()`                                                                               
          `ExecutionContext`                                                            `getExecutionContext()`                                                                                    
          `com.google.common.util.concurrent.ListeningExecutorService`                  `getExecutorService()`                                                                                     
          `com.google.common.util.concurrent.ListenableFuture<Optional<BuildResult>>`   `runWithDefaultBehavior()`                                                                                 

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

        []{#<init>(com.facebook.buck.core.build.engine.BuildStrategyContext)}

        -   #### DelegatingBuildStrategyContext

                public DelegatingBuildStrategyContext​(BuildStrategyContext delegateContext)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#runWithDefaultBehavior()}

        -   #### runWithDefaultBehavior

            ``` methodSignature
            public com.google.common.util.concurrent.ListenableFuture<Optional<BuildResult>> runWithDefaultBehavior()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `runWithDefaultBehavior` in
                interface `BuildStrategyContext`

        []{#getExecutorService()}

        -   #### getExecutorService

            ``` methodSignature
            public com.google.common.util.concurrent.ListeningExecutorService getExecutorService()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getExecutorService` in interface `BuildStrategyContext`

        []{#createBuildResult(com.facebook.buck.core.build.engine.BuildRuleSuccessType,java.util.Optional)}

        -   #### createBuildResult

            ``` methodSignature
            public BuildResult createBuildResult​(BuildRuleSuccessType successType,
                                                 Optional<String> strategyResult)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `createBuildResult` in interface `BuildStrategyContext`

        []{#createCancelledResult(java.lang.Throwable)}

        -   #### createCancelledResult

            ``` methodSignature
            public BuildResult createCancelledResult​(Throwable throwable)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `createCancelledResult` in
                interface `BuildStrategyContext`

        []{#getExecutionContext()}

        -   #### getExecutionContext

            ``` methodSignature
            public ExecutionContext getExecutionContext()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getExecutionContext` in
                interface `BuildStrategyContext`

        []{#buildRuleScope()}

        -   #### buildRuleScope

            ``` methodSignature
            public Scope buildRuleScope()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `buildRuleScope` in interface `BuildStrategyContext`

        []{#getBuildRuleBuildContext()}

        -   #### getBuildRuleBuildContext

            ``` methodSignature
            public BuildContext getBuildRuleBuildContext()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getBuildRuleBuildContext` in
                interface `BuildStrategyContext`

        []{#getBuildableContext()}

        -   #### getBuildableContext

            ``` methodSignature
            public BuildableContext getBuildableContext()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getBuildableContext` in
                interface `BuildStrategyContext`
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
