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
-   [Field](#field.detail) \| 
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

## Class AbstractBatchingLogger {#class-abstractbatchinglogger .title title="Class AbstractBatchingLogger"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.util.network.AbstractBatchingLogger

::: description
-   

    All Implemented Interfaces:
    :   `BatchingLogger`

    ```{=html}
    <!-- -->
    ```

    Direct Known Subclasses:
    :   `ScribeBatchingLogger`

    ------------------------------------------------------------------------

        public abstract class AbstractBatchingLogger
        extends Object
        implements BatchingLogger

    ::: block
    Common functionality for uploading log entries in batches.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type           Class                                 Description
          --------------------------- ------------------------------------- -------------
          `protected static class `   `AbstractBatchingLogger.BatchEntry`    

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type   Field                      Description
          ------------------- -------------------------- -------------
          `static int`        `DEFAULT_MIN_BATCH_SIZE`    

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                  Description
          -------------------------------------------- -------------
          `AbstractBatchingLogger()`                    
          `AbstractBatchingLogger​(int minBatchSize)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `com.google.comm      | `forceFlush()`        | ::: block             |
        | on.util.concurrent.Li |                       | Signals to upload     |
        | stenableFuture<Unit>` |                       | whatever remaining    |
        |                       |                       | information is        |
        |                       |                       | buffered.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Opti                 | `log​(String logLine)` |                       |
        | onal<com.google.commo |                       |                       |
        | n.util.concurrent.Lis |                       |                       |
        | tenableFuture<Unit>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected abs        | `logMultiple​(com      |                       |
        | tract com.google.comm | .google.common.collec |                       |
        | on.util.concurrent.Li | t.ImmutableCollection |                       |
        | stenableFuture<Unit>` | <AbstractBatchingLogg |                       |
        |                       | er.BatchEntry> data)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
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
    -   []{#field.detail}

        ### Field Detail

        []{#DEFAULT_MIN_BATCH_SIZE}

        -   #### DEFAULT_MIN_BATCH_SIZE

                public static final int DEFAULT_MIN_BATCH_SIZE

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.util.network.AbstractBatchingLogger.DEFAULT_MIN_BATCH_SIZE)
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(int)}

        -   #### AbstractBatchingLogger

                public AbstractBatchingLogger​(int minBatchSize)

        []{#<init>()}

        -   #### AbstractBatchingLogger

                public AbstractBatchingLogger()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#log(java.lang.String)}

        -   #### log

            ``` methodSignature
            public Optional<com.google.common.util.concurrent.ListenableFuture<Unit>> log​(String logLine)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `log` in interface `BatchingLogger`

            [Parameters:]{.paramLabel}
            :   `logLine` - data to upload.

            [Returns:]{.returnLabel}
            :   [`Optional.empty()`](http://docs.oracle.com/javase/7/docs/api/java/util/Optional.html?is-external=true#empty() "class or interface in java.util"){.externalLink}
                if the data has merely been buffered, a
                `ListenableFuture` representing the upload otherwise.

        []{#forceFlush()}

        -   #### forceFlush

            ``` methodSignature
            public com.google.common.util.concurrent.ListenableFuture<Unit> forceFlush()
            ```

            ::: block
            [Description copied from
            interface: `BatchingLogger`]{.descfrmTypeLabel}
            :::

            ::: block
            Signals to upload whatever remaining information is
            buffered.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `forceFlush` in interface `BatchingLogger`

            [Returns:]{.returnLabel}
            :   future representing the forced upload.

        []{#logMultiple(com.google.common.collect.ImmutableCollection)}

        -   #### logMultiple

            ``` methodSignature
            protected abstract com.google.common.util.concurrent.ListenableFuture<Unit> logMultiple​(com.google.common.collect.ImmutableCollection<AbstractBatchingLogger.BatchEntry> data)
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
-   [Nested](#nested.class.summary) \| 
-   [Field](#field.summary) \| 
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
-   [Constr](#constructor.detail) \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
