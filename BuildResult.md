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
[Package]{.packageLabelInType} [com.facebook.buck.core.build.engine](package-summary.html)
:::

## Class BuildResult {#class-buildresult .title title="Class BuildResult"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.build.engine.BuildResult

::: description
-   

    ------------------------------------------------------------------------

        public abstract class BuildResult
        extends Object

    ::: block
    This is a union type that represents either a success or a failure.
    This exists so that
    `  com.facebook.buck.core.build.engine.impl.CachingBuildEngine#buildOnceDepsAreBuilt()`
    can return a strongly typed value.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type   Class                   Description
          ------------------- ----------------------- -------------
          `static class `     `BuildResult.Builder`    

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor       Description
          ----------------- -------------
          `BuildResult()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                           Method                                                                                           Description
          ------------------------------------------- ------------------------------------------------------------------------------------------------ -------------
          `static BuildResult.Builder`                `builder()`                                                                                       
          `static BuildResult`                        `canceled​(BuildRule rule,         Throwable failure)`                                             
          `static BuildResult`                        `failure​(BuildRule rule,        Throwable failure)`                                               
          `abstract Optional<CacheResult>`            `getCacheResult()`                                                                                
          `abstract Optional<Set<String>>`            `getDepsWithCacheMisses()`                                                                        
          `Throwable`                                 `getFailure()`                                                                                    
          `abstract Optional<Throwable>`              `getFailureOptional()`                                                                            
          `abstract BuildRule`                        `getRule()`                                                                                       
          `abstract BuildRuleStatus`                  `getStatus()`                                                                                     
          `abstract Optional<String>`                 `getStrategyResult()`                                                                             
          `BuildRuleSuccessType`                      `getSuccess()`                                                                                    
          `abstract Optional<BuildRuleSuccessType>`   `getSuccessOptional()`                                                                            
          `boolean`                                   `isSuccess()`                                                                                     
          `static BuildResult`                        `success​(BuildRule rule,        BuildRuleSuccessType success,        CacheResult cacheResult)`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
          Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
          .tableTab}[[Instance
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

        -   #### BuildResult

                public BuildResult()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getRule()}

        -   #### getRule

            ``` methodSignature
            public abstract BuildRule getRule()
            ```

        []{#getStatus()}

        -   #### getStatus

            ``` methodSignature
            public abstract BuildRuleStatus getStatus()
            ```

        []{#getCacheResult()}

        -   #### getCacheResult

            ``` methodSignature
            public abstract Optional<CacheResult> getCacheResult()
            ```

        []{#getSuccessOptional()}

        -   #### getSuccessOptional

            ``` methodSignature
            public abstract Optional<BuildRuleSuccessType> getSuccessOptional()
            ```

        []{#getStrategyResult()}

        -   #### getStrategyResult

            ``` methodSignature
            public abstract Optional<String> getStrategyResult()
            ```

        []{#getFailureOptional()}

        -   #### getFailureOptional

            ``` methodSignature
            public abstract Optional<Throwable> getFailureOptional()
            ```

        []{#getDepsWithCacheMisses()}

        -   #### getDepsWithCacheMisses

            ``` methodSignature
            public abstract Optional<Set<String>> getDepsWithCacheMisses()
            ```

        []{#success(com.facebook.buck.core.rules.BuildRule,com.facebook.buck.core.build.engine.BuildRuleSuccessType,com.facebook.buck.artifact_cache.CacheResult)}

        -   #### success

            ``` methodSignature
            public static BuildResult success​(BuildRule rule,
                                              BuildRuleSuccessType success,
                                              CacheResult cacheResult)
            ```

        []{#failure(com.facebook.buck.core.rules.BuildRule,java.lang.Throwable)}

        -   #### failure

            ``` methodSignature
            public static BuildResult failure​(BuildRule rule,
                                              Throwable failure)
            ```

        []{#canceled(com.facebook.buck.core.rules.BuildRule,java.lang.Throwable)}

        -   #### canceled

            ``` methodSignature
            public static BuildResult canceled​(BuildRule rule,
                                               Throwable failure)
            ```

        []{#getSuccess()}

        -   #### getSuccess

            ``` methodSignature
            public BuildRuleSuccessType getSuccess()
            ```

        []{#getFailure()}

        -   #### getFailure

            ``` methodSignature
            public Throwable getFailure()
            ```

        []{#isSuccess()}

        -   #### isSuccess

            ``` methodSignature
            public boolean isSuccess()
            ```

        []{#builder()}

        -   #### builder

            ``` methodSignature
            public static BuildResult.Builder builder()
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
