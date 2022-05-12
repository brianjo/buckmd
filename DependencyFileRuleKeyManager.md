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

-   [Overview](../../../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../../index-all.html)
-   [Help](../../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.core.build.engine.cache.manager](package-summary.html)
:::

## Class DependencyFileRuleKeyManager {#class-dependencyfilerulekeymanager .title title="Class DependencyFileRuleKeyManager"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.build.engine.cache.manager.DependencyFileRuleKeyManager

::: description
-   

    ------------------------------------------------------------------------

        public class DependencyFileRuleKeyManager
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                                                                                                  Description
          ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ -------------
          `DependencyFileRuleKeyManager​(DepFiles depFiles,                             BuildRule rule,                             Discardable<BuildInfoRecorder> buildInfoRecorder,                             OnDiskBuildInfo onDiskBuildInfo,                             RuleKeyFactories ruleKeyFactories,                             BuckEventBus eventBus)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                           Method                                                                                                                                            Description
          ----------------------------------------------------------- ------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `Optional<DependencyFileRuleKeyFactory.RuleKeyAndInputs>`   `calculateDepFileRuleKey​(Optional<com.google.common.collect.ImmutableList<String>> depFile,                        boolean allowMissingInputs)`    
          `boolean`                                                   `checkMatchingDepfile()`                                                                                                                           
          `boolean`                                                   `useDependencyFileRuleKey()`                                                                                                                       

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

        []{#<init>(com.facebook.buck.core.build.engine.type.DepFiles,com.facebook.buck.core.rules.BuildRule,com.facebook.buck.util.Discardable,com.facebook.buck.core.build.engine.buildinfo.OnDiskBuildInfo,com.facebook.buck.rules.keys.RuleKeyFactories,com.facebook.buck.event.BuckEventBus)}

        -   #### DependencyFileRuleKeyManager

                public DependencyFileRuleKeyManager​(DepFiles depFiles,
                                                    BuildRule rule,
                                                    Discardable<BuildInfoRecorder> buildInfoRecorder,
                                                    OnDiskBuildInfo onDiskBuildInfo,
                                                    RuleKeyFactories ruleKeyFactories,
                                                    BuckEventBus eventBus)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#useDependencyFileRuleKey()}

        -   #### useDependencyFileRuleKey

            ``` methodSignature
            public boolean useDependencyFileRuleKey()
            ```

        []{#checkMatchingDepfile()}

        -   #### checkMatchingDepfile

            ``` methodSignature
            public boolean checkMatchingDepfile()
                                         throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#calculateDepFileRuleKey(java.util.Optional,boolean)}

        -   #### calculateDepFileRuleKey

            ``` methodSignature
            public Optional<DependencyFileRuleKeyFactory.RuleKeyAndInputs> calculateDepFileRuleKey​(Optional<com.google.common.collect.ImmutableList<String>> depFile,
                                                                                                   boolean allowMissingInputs)
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

-   [Overview](../../../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../../index-all.html)
-   [Help](../../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../../allclasses.html)

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
