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
[Package]{.packageLabelInType} [com.facebook.buck.cxx.toolchain](package-summary.html)
:::

## Class BuildRuleResolverCacheByTargetConfiguration\<T\> {#class-buildruleresolvercachebytargetconfigurationt .title title="Class BuildRuleResolverCacheByTargetConfiguration"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.cxx.toolchain.BuildRuleResolverCacheByTargetConfiguration\<T\>

::: description
-   

    ------------------------------------------------------------------------

        public class BuildRuleResolverCacheByTargetConfiguration<T>
        extends Object

    ::: block
    Custom cache to use with
    [`CxxToolProvider`](CxxToolProvider.html "class in com.facebook.buck.cxx.toolchain")
    and similar classes that need to cache build rules for a given build
    rule resolver and target configuration.
    This is basically two level cache to allow to use build rule
    resolver as a key in a cache with weak keys and target configuration
    as the key at second level (without weak keys).
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                Description
          ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `BuildRuleResolverCacheByTargetConfiguration​(BuildRuleResolver buildRuleResolver,                                            ToolProvider toolProvider,                                            java.util.function.Function<Tool,​T> delegateBuilder)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                                           Description
          ------------------- ------------------------------------------------ -------------
          `T`                 `get​(TargetConfiguration targetConfiguration)`    

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

        []{#<init>(com.facebook.buck.core.rules.BuildRuleResolver,com.facebook.buck.core.toolchain.toolprovider.ToolProvider,java.util.function.Function)}

        -   #### BuildRuleResolverCacheByTargetConfiguration

                public BuildRuleResolverCacheByTargetConfiguration​(BuildRuleResolver buildRuleResolver,
                                                                   ToolProvider toolProvider,
                                                                   java.util.function.Function<Tool,​T> delegateBuilder)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#get(com.facebook.buck.core.model.TargetConfiguration)}

        -   #### get

            ``` methodSignature
            public T get​(TargetConfiguration targetConfiguration)
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
