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
-   [Nested](#nested.class.summary) \| 
-   [Field](#field.summary) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.util.network](package-summary.html)
:::

## Class ScribeBatchingLogger {#class-scribebatchinglogger .title title="Class ScribeBatchingLogger"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.util.network.AbstractBatchingLogger](AbstractBatchingLogger.html "class in com.facebook.buck.util.network")

    -   -   com.facebook.buck.util.network.ScribeBatchingLogger

::: description
-   

    All Implemented Interfaces:
    :   `BatchingLogger`

    ------------------------------------------------------------------------

        public class ScribeBatchingLogger
        extends AbstractBatchingLogger

    ::: block
    Uploads log entries to the given scribe category.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        -   []{#nested.classes.inherited.from.class.com.facebook.buck.util.network.AbstractBatchingLogger}

            ### Nested classes/interfaces inherited from class com.facebook.buck.util.network.[AbstractBatchingLogger](AbstractBatchingLogger.html "class in com.facebook.buck.util.network")

            `AbstractBatchingLogger.BatchEntry`
    :::

    ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        -   []{#fields.inherited.from.class.com.facebook.buck.util.network.AbstractBatchingLogger}

            ### Fields inherited from class com.facebook.buck.util.network.[AbstractBatchingLogger](AbstractBatchingLogger.html "class in com.facebook.buck.util.network")

            `DEFAULT_MIN_BATCH_SIZE`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                              Description
          ---------------------------------------------------------------------------------------- -------------
          `ScribeBatchingLogger​(String category,                     ScribeLogger scribeLogger)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                      Method                                                                                                 Description
          ---------------------------------------------------------------------- ------------------------------------------------------------------------------------------------------ -------------
          `protected com.google.common.util.concurrent.ListenableFuture<Unit>`   `logMultiple​(com.google.common.collect.ImmutableCollection<AbstractBatchingLogger.BatchEntry> data)`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.util.network.AbstractBatchingLogger}

            ### Methods inherited from class com.facebook.buck.util.network.[AbstractBatchingLogger](AbstractBatchingLogger.html "class in com.facebook.buck.util.network")

            `forceFlush, log`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(java.lang.String,com.facebook.buck.util.network.ScribeLogger)}

        -   #### ScribeBatchingLogger

                public ScribeBatchingLogger​(String category,
                                            ScribeLogger scribeLogger)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#logMultiple(com.google.common.collect.ImmutableCollection)}

        -   #### logMultiple

            ``` methodSignature
            protected com.google.common.util.concurrent.ListenableFuture<Unit> logMultiple​(com.google.common.collect.ImmutableCollection<AbstractBatchingLogger.BatchEntry> data)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `logMultiple` in class `AbstractBatchingLogger`
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
-   [Nested](#nested.class.summary) \| 
-   [Field](#field.summary) \| 
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
