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

-   [Overview](../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../deprecated-list.html)
-   [Index](../../../../index-all.html)
-   [Help](../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.artifact_cache](package-summary.html)
:::

## Class RuleKeyCacheResult {#class-rulekeycacheresult .title title="Class RuleKeyCacheResult"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.artifact_cache.RuleKeyCacheResult

::: description
-   

    ------------------------------------------------------------------------

        public abstract class RuleKeyCacheResult
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor              Description
          ------------------------ -------------
          `RuleKeyCacheResult()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type             Method                                                                                                                                                                           Description
          ----------------------------- -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `abstract String`             `buildTarget()`                                                                                                                                                                   
          `abstract CacheResultType`    `cacheResult()`                                                                                                                                                                   
          `static RuleKeyCacheResult`   `of​(String buildTarget,   String ruleKey,   long requestTimestampMillis,   RuleKeyType ruleKeyType,   CacheResultType cacheResult,   Optional<String> twoLevelContentHashKey)`    
          `abstract long`               `requestTimestampMillis()`                                                                                                                                                        
          `abstract String`             `ruleKey()`                                                                                                                                                                       
          `abstract RuleKeyType`        `ruleKeyType()`                                                                                                                                                                   
          `abstract Optional<String>`   `twoLevelContentHashKey()`                                                                                                                                                        

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

        -   #### RuleKeyCacheResult

                public RuleKeyCacheResult()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#buildTarget()}

        -   #### buildTarget

            ``` methodSignature
            public abstract String buildTarget()
            ```

        []{#ruleKey()}

        -   #### ruleKey

            ``` methodSignature
            public abstract String ruleKey()
            ```

        []{#requestTimestampMillis()}

        -   #### requestTimestampMillis

            ``` methodSignature
            public abstract long requestTimestampMillis()
            ```

        []{#ruleKeyType()}

        -   #### ruleKeyType

            ``` methodSignature
            public abstract RuleKeyType ruleKeyType()
            ```

        []{#cacheResult()}

        -   #### cacheResult

            ``` methodSignature
            public abstract CacheResultType cacheResult()
            ```

        []{#twoLevelContentHashKey()}

        -   #### twoLevelContentHashKey

            ``` methodSignature
            public abstract Optional<String> twoLevelContentHashKey()
            ```

        []{#of(java.lang.String,java.lang.String,long,com.facebook.buck.rules.keys.RuleKeyType,com.facebook.buck.artifact_cache.CacheResultType,java.util.Optional)}

        -   #### of

            ``` methodSignature
            public static RuleKeyCacheResult of​(String buildTarget,
                                                String ruleKey,
                                                long requestTimestampMillis,
                                                RuleKeyType ruleKeyType,
                                                CacheResultType cacheResult,
                                                Optional<String> twoLevelContentHashKey)
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

-   [Overview](../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../deprecated-list.html)
-   [Index](../../../../index-all.html)
-   [Help](../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../allclasses.html)

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
