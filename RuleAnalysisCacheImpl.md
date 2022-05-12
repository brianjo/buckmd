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

## Class RuleAnalysisCacheImpl {#class-ruleanalysiscacheimpl .title title="Class RuleAnalysisCacheImpl"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.rules.analysis.impl.RuleAnalysisCacheImpl

::: description
-   

    All Implemented Interfaces:
    :   `GraphEngineCache<RuleAnalysisKey,​RuleAnalysisResult>`,
        `RuleAnalysisCache`

    ------------------------------------------------------------------------

        public class RuleAnalysisCacheImpl
        extends Object
        implements RuleAnalysisCache

    ::: block
    Cache for performing rule analysis
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                 Description
          --------------------------- -------------
          `RuleAnalysisCacheImpl()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `Optional             | `get​(                 | ::: block             |
        | <RuleAnalysisResult>` | RuleAnalysisKey key)` | Optionally returns    |
        |                       |                       | the cached result     |
        |                       |                       | given the key         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `put​(                 | ::: block             |
        |                       | RuleAnalysisKey key,  | Offers the given key  |
        |                       |    RuleAnalysisResult | and value for caching |
        |                       |  ruleAnalysisResult)` | :::                   |
        +-----------------------+-----------------------+-----------------------+

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

        []{#<init>()}

        -   #### RuleAnalysisCacheImpl

                public RuleAnalysisCacheImpl()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#get(com.facebook.buck.core.rules.analysis.RuleAnalysisKey)}

        -   #### get

            ``` methodSignature
            public Optional<RuleAnalysisResult> get​(RuleAnalysisKey key)
            ```

            ::: block
            [Description copied from
            interface: `GraphEngineCache`]{.descfrmTypeLabel}
            :::

            ::: block
            Optionally returns the cached result given the key
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `get` in
                interface `GraphEngineCache<RuleAnalysisKey,​RuleAnalysisResult>`

            [Parameters:]{.paramLabel}
            :   `key` - The desired key

            [Returns:]{.returnLabel}
            :   the result if cached, otherwise an empty Optional

        []{#put(com.facebook.buck.core.rules.analysis.RuleAnalysisKey,com.facebook.buck.core.rules.analysis.RuleAnalysisResult)}

        -   #### put

            ``` methodSignature
            public void put​(RuleAnalysisKey key,
                            RuleAnalysisResult ruleAnalysisResult)
            ```

            ::: block
            [Description copied from
            interface: `GraphEngineCache`]{.descfrmTypeLabel}
            :::

            ::: block
            Offers the given key and value for caching
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `put` in
                interface `GraphEngineCache<RuleAnalysisKey,​RuleAnalysisResult>`

            [Parameters:]{.paramLabel}
            :   `key` - the key to cache
            :   `ruleAnalysisResult` - the value to cache
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
