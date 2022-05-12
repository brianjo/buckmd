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

## Class RuleKeyFactories {#class-rulekeyfactories .title title="Class RuleKeyFactories"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.rules.keys.RuleKeyFactories

::: description
-   

    ------------------------------------------------------------------------

        public abstract class RuleKeyFactories
        extends Object

    ::: block
    The various rule key factories used by the build engine.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor            Description
          ---------------------- -------------
          `RuleKeyFactories()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                           Method                                                                                                                                                                                                                                                       Description
          ----------------------------------------------------------- ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ -------------
          `Optional<DependencyFileRuleKeyFactory.RuleKeyAndInputs>`   `calculateManifestKey​(SupportsDependencyFileRuleKey rule,                     BuckEventBus eventBus)`                                                                                                                                                         
          `abstract RuleKeyFactoryWithDiagnostics<RuleKey>`           `getDefaultRuleKeyFactory()`                                                                                                                                                                                                                                  
          `abstract DependencyFileRuleKeyFactory`                     `getDepFileRuleKeyFactory()`                                                                                                                                                                                                                                  
          `abstract RuleKeyFactory<RuleKey>`                          `getInputBasedRuleKeyFactory()`                                                                                                                                                                                                                               
          `static RuleKeyFactories`                                   `of​(RuleKeyConfiguration ruleKeyConfiguration,   FileHashLoader fileHashLoader,   BuildRuleResolver resolver,   long inputRuleKeyFileSizeLimit,   TrackedRuleKeyCache<RuleKey> defaultRuleKeyFactoryCache)`                                                   
          `static RuleKeyFactories`                                   `of​(RuleKeyConfiguration ruleKeyConfiguration,   FileHashLoader fileHashLoader,   BuildRuleResolver resolver,   long inputRuleKeyFileSizeLimit,   TrackedRuleKeyCache<RuleKey> defaultRuleKeyFactoryCache,   Optional<ThriftRuleKeyLogger> ruleKeyLogger)`    
          `static RuleKeyFactories`                                   `of​(RuleKeyFactoryWithDiagnostics<RuleKey> defaultRuleKeyFactory,   RuleKeyFactory<RuleKey> inputBasedRuleKeyFactory,   DependencyFileRuleKeyFactory depFileRuleKeyFactory)`                                                                                  

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

        -   #### RuleKeyFactories

                public RuleKeyFactories()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getDefaultRuleKeyFactory()}

        -   #### getDefaultRuleKeyFactory

            ``` methodSignature
            public abstract RuleKeyFactoryWithDiagnostics<RuleKey> getDefaultRuleKeyFactory()
            ```

            [Returns:]{.returnLabel}
            :   a
                [`RuleKeyFactory`](RuleKeyFactory.html "interface in com.facebook.buck.rules.keys")
                that produces
                [`RuleKey`](../../core/rulekey/RuleKey.html "class in com.facebook.buck.core.rulekey")s.

        []{#getInputBasedRuleKeyFactory()}

        -   #### getInputBasedRuleKeyFactory

            ``` methodSignature
            public abstract RuleKeyFactory<RuleKey> getInputBasedRuleKeyFactory()
            ```

            [Returns:]{.returnLabel}
            :   a
                [`RuleKeyFactory`](RuleKeyFactory.html "interface in com.facebook.buck.rules.keys")
                that produces input-based
                [`RuleKey`](../../core/rulekey/RuleKey.html "class in com.facebook.buck.core.rulekey")s.

        []{#getDepFileRuleKeyFactory()}

        -   #### getDepFileRuleKeyFactory

            ``` methodSignature
            public abstract DependencyFileRuleKeyFactory getDepFileRuleKeyFactory()
            ```

            [Returns:]{.returnLabel}
            :   a
                [`DependencyFileRuleKeyFactory`](DependencyFileRuleKeyFactory.html "interface in com.facebook.buck.rules.keys")
                that produces dep-file-based
                [`RuleKey`](../../core/rulekey/RuleKey.html "class in com.facebook.buck.core.rulekey")s.

        []{#of(com.facebook.buck.rules.keys.config.RuleKeyConfiguration,com.facebook.buck.util.hashing.FileHashLoader,com.facebook.buck.core.rules.BuildRuleResolver,long,com.facebook.buck.rules.keys.TrackedRuleKeyCache)}

        -   #### of

            ``` methodSignature
            public static RuleKeyFactories of​(RuleKeyConfiguration ruleKeyConfiguration,
                                              FileHashLoader fileHashLoader,
                                              BuildRuleResolver resolver,
                                              long inputRuleKeyFileSizeLimit,
                                              TrackedRuleKeyCache<RuleKey> defaultRuleKeyFactoryCache)
            ```

        []{#of(com.facebook.buck.rules.keys.config.RuleKeyConfiguration,com.facebook.buck.util.hashing.FileHashLoader,com.facebook.buck.core.rules.BuildRuleResolver,long,com.facebook.buck.rules.keys.TrackedRuleKeyCache,java.util.Optional)}

        -   #### of

            ``` methodSignature
            public static RuleKeyFactories of​(RuleKeyConfiguration ruleKeyConfiguration,
                                              FileHashLoader fileHashLoader,
                                              BuildRuleResolver resolver,
                                              long inputRuleKeyFileSizeLimit,
                                              TrackedRuleKeyCache<RuleKey> defaultRuleKeyFactoryCache,
                                              Optional<ThriftRuleKeyLogger> ruleKeyLogger)
            ```

        []{#of(com.facebook.buck.rules.keys.RuleKeyFactoryWithDiagnostics,com.facebook.buck.rules.keys.RuleKeyFactory,com.facebook.buck.rules.keys.DependencyFileRuleKeyFactory)}

        -   #### of

            ``` methodSignature
            public static RuleKeyFactories of​(RuleKeyFactoryWithDiagnostics<RuleKey> defaultRuleKeyFactory,
                                              RuleKeyFactory<RuleKey> inputBasedRuleKeyFactory,
                                              DependencyFileRuleKeyFactory depFileRuleKeyFactory)
            ```

        []{#calculateManifestKey(com.facebook.buck.core.rules.attr.SupportsDependencyFileRuleKey,com.facebook.buck.event.BuckEventBus)}

        -   #### calculateManifestKey

            ``` methodSignature
            public Optional<DependencyFileRuleKeyFactory.RuleKeyAndInputs> calculateManifestKey​(SupportsDependencyFileRuleKey rule,
                                                                                                BuckEventBus eventBus)
                                                                                         throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`
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
