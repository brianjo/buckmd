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
[Package]{.packageLabelInType} [com.facebook.buck.support.build.report](package-summary.html)
:::

## Class BuildReportConfig {#class-buildreportconfig .title title="Class BuildReportConfig"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.support.build.report.BuildReportConfig

::: description
-   

    All Implemented Interfaces:
    :   `ConfigView<BuckConfig>`

    ------------------------------------------------------------------------

        public abstract class BuildReportConfig
        extends Object
        implements ConfigView<BuckConfig>

    ::: block
    [`ConfigView`](../../../core/config/ConfigView.html "interface in com.facebook.buck.core.config")
    for BuildReport Configuration
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor             Description
          ----------------------- -------------
          `BuildReportConfig()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type            Method                      Description
          ---------------------------- --------------------------- -------------
          `abstract BuckConfig`        `getDelegate()`              
          `boolean`                    `getEnabled()`               
          `long`                       `getEndpointTimeoutMs()`     
          `Optional<URL>`              `getEndpointUrl()`           
          `boolean`                    `getRemoveOutput()`          
          `static BuildReportConfig`   `of​(BuckConfig delegate)`    

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

        -   #### BuildReportConfig

                public BuildReportConfig()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getDelegate()}

        -   #### getDelegate

            ``` methodSignature
            public abstract BuckConfig getDelegate()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getDelegate` in interface `ConfigView<BuckConfig>`

        []{#of(com.facebook.buck.core.config.BuckConfig)}

        -   #### of

            ``` methodSignature
            public static BuildReportConfig of​(BuckConfig delegate)
            ```

        []{#getEnabled()}

        -   #### getEnabled

            ``` methodSignature
            @Lazy
            public boolean getEnabled()
            ```

        []{#getEndpointUrl()}

        -   #### getEndpointUrl

            ``` methodSignature
            @Lazy
            public Optional<URL> getEndpointUrl()
                                         throws HumanReadableException
            ```

            [Throws:]{.throwsLabel}
            :   `HumanReadableException`

        []{#getEndpointTimeoutMs()}

        -   #### getEndpointTimeoutMs

            ``` methodSignature
            @Lazy
            public long getEndpointTimeoutMs()
            ```

        []{#getRemoveOutput()}

        -   #### getRemoveOutput

            ``` methodSignature
            @Lazy
            public boolean getRemoveOutput()
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