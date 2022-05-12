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
[Package]{.packageLabelInType} [com.facebook.buck.core.build.engine.delegate](package-summary.html)
:::

## Class LocalCachingBuildEngineDelegate {#class-localcachingbuildenginedelegate .title title="Class LocalCachingBuildEngineDelegate"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.build.engine.delegate.LocalCachingBuildEngineDelegate

::: description
-   

    All Implemented Interfaces:
    :   `CachingBuildEngineDelegate`

    ------------------------------------------------------------------------

        public class LocalCachingBuildEngineDelegate
        extends Object
        implements CachingBuildEngineDelegate
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                             Description
          ----------------------------------------------------------------------- -------------
          `LocalCachingBuildEngineDelegate​(FileHashCache defaultFileHashCache)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `FileHashCache`       | `getFileHashCache()`  |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `                     | ::: block             |
        |                       | onRuleAboutToBeBuilt​( | Called right before   |
        |                       | BuildRule buildRule)` | the rule is going to  |
        |                       |                       | be built.             |
        |                       |                       | :::                   |
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

        []{#<init>(com.facebook.buck.util.cache.FileHashCache)}

        -   #### LocalCachingBuildEngineDelegate

                public LocalCachingBuildEngineDelegate​(FileHashCache defaultFileHashCache)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getFileHashCache()}

        -   #### getFileHashCache

            ``` methodSignature
            public FileHashCache getFileHashCache()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getFileHashCache` in
                interface `CachingBuildEngineDelegate`

        []{#onRuleAboutToBeBuilt(com.facebook.buck.core.rules.BuildRule)}

        -   #### onRuleAboutToBeBuilt

            ``` methodSignature
            public void onRuleAboutToBeBuilt​(BuildRule buildRule)
            ```

            ::: block
            [Description copied from
            interface: `CachingBuildEngineDelegate`]{.descfrmTypeLabel}
            :::

            ::: block
            Called right before the rule is going to be built. This is
            when direct inputs to the rule would get materialized on
            disk.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `onRuleAboutToBeBuilt` in
                interface `CachingBuildEngineDelegate`

            [Parameters:]{.paramLabel}
            :   `buildRule` - rule that is about to be built.
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
