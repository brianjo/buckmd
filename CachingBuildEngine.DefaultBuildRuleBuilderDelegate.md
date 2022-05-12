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

## Class CachingBuildEngine.DefaultBuildRuleBuilderDelegate {#class-cachingbuildengine.defaultbuildrulebuilderdelegate .title title="Class CachingBuildEngine.DefaultBuildRuleBuilderDelegate"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.build.engine.impl.CachingBuildEngine.DefaultBuildRuleBuilderDelegate

::: description
-   

    All Implemented Interfaces:
    :   `com.facebook.buck.core.build.engine.impl.CachingBuildRuleBuilder.BuildRuleBuilderDelegate`

    ```{=html}
    <!-- -->
    ```

    Enclosing class:
    :   [CachingBuildEngine](CachingBuildEngine.html "class in com.facebook.buck.core.build.engine.impl")

    ------------------------------------------------------------------------

        public static class CachingBuildEngine.DefaultBuildRuleBuilderDelegate
        extends Object
        implements com.facebook.buck.core.build.engine.impl.CachingBuildRuleBuilder.BuildRuleBuilderDelegate
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                     Description
          ----------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `DefaultBuildRuleBuilderDelegate​(CachingBuildEngine cachingBuildEngine,                                BuildEngineBuildContext buildContext)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                         Method                                                                                  Description
          ------------------------------------------------------------------------- --------------------------------------------------------------------------------------- -------------
          `void`                                                                    `addAsyncCallback​(com.google.common.util.concurrent.ListenableFuture<Unit> callback)`    
          `com.google.common.util.concurrent.ListenableFuture<List<BuildResult>>`   `getDepResults​(BuildRule rule,              ExecutionContext executionContext)`          
          `void`                                                                    `markRuleAsUsed​(BuildRule rule,               BuckEventBus eventBus)`                    
          `void`                                                                    `onRuleAboutToBeBuilt​(BuildRule rule)`                                                   
          `void`                                                                    `setFirstFailure​(BuildRuleFailedException throwable)`                                    

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

        []{#<init>(com.facebook.buck.core.build.engine.impl.CachingBuildEngine,com.facebook.buck.core.build.engine.BuildEngineBuildContext)}

        -   #### DefaultBuildRuleBuilderDelegate

                public DefaultBuildRuleBuilderDelegate​(CachingBuildEngine cachingBuildEngine,
                                                       BuildEngineBuildContext buildContext)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#markRuleAsUsed(com.facebook.buck.core.rules.BuildRule,com.facebook.buck.event.BuckEventBus)}

        -   #### markRuleAsUsed

            ``` methodSignature
            public void markRuleAsUsed​(BuildRule rule,
                                       BuckEventBus eventBus)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `markRuleAsUsed` in
                interface `com.facebook.buck.core.build.engine.impl.CachingBuildRuleBuilder.BuildRuleBuilderDelegate`

        []{#setFirstFailure(com.facebook.buck.core.build.engine.impl.BuildRuleFailedException)}

        -   #### setFirstFailure

            ``` methodSignature
            public void setFirstFailure​(BuildRuleFailedException throwable)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `setFirstFailure` in
                interface `com.facebook.buck.core.build.engine.impl.CachingBuildRuleBuilder.BuildRuleBuilderDelegate`

        []{#getDepResults(com.facebook.buck.core.rules.BuildRule,com.facebook.buck.core.build.execution.context.ExecutionContext)}

        -   #### getDepResults

            ``` methodSignature
            public com.google.common.util.concurrent.ListenableFuture<List<BuildResult>> getDepResults​(BuildRule rule,
                                                                                                       ExecutionContext executionContext)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getDepResults` in
                interface `com.facebook.buck.core.build.engine.impl.CachingBuildRuleBuilder.BuildRuleBuilderDelegate`

        []{#addAsyncCallback(com.google.common.util.concurrent.ListenableFuture)}

        -   #### addAsyncCallback

            ``` methodSignature
            public void addAsyncCallback​(com.google.common.util.concurrent.ListenableFuture<Unit> callback)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `addAsyncCallback` in
                interface `com.facebook.buck.core.build.engine.impl.CachingBuildRuleBuilder.BuildRuleBuilderDelegate`

        []{#onRuleAboutToBeBuilt(com.facebook.buck.core.rules.BuildRule)}

        -   #### onRuleAboutToBeBuilt

            ``` methodSignature
            public void onRuleAboutToBeBuilt​(BuildRule rule)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `onRuleAboutToBeBuilt` in
                interface `com.facebook.buck.core.build.engine.impl.CachingBuildRuleBuilder.BuildRuleBuilderDelegate`
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
