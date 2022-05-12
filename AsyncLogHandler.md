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
[Package]{.packageLabelInType} [com.facebook.buck.log](package-summary.html)
:::

## Class AsyncLogHandler {#class-asyncloghandler .title title="Class AsyncLogHandler"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [java.util.logging.Handler](http://docs.oracle.com/javase/7/docs/api/java/util/logging/Handler.html?is-external=true "class or interface in java.util.logging"){.externalLink}

    -   -   com.facebook.buck.log.AsyncLogHandler

::: description
-   

    ------------------------------------------------------------------------

        public class AsyncLogHandler
        extends Handler

    ::: block
    Wraps a log Handler, e.g.
    [`LogFileHandler`](LogFileHandler.html "class in com.facebook.buck.log"),
    but ensures that all requests are dispatched on a separate thread
    and do not block the caller.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Modifier       Constructor                                                                                                        Description
          -------------- ------------------------------------------------------------------------------------------------------------------ -------------
          ` `            `AsyncLogHandler​(LogFileHandler delegate)`                                                                          
          `protected `   `AsyncLogHandler​(java.util.function.Supplier<Executor> performLoggingExecutor,                Handler delegate)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                        Description
          ------------------- ----------------------------- -------------
          `void`              `close()`                      
          `void`              `flush()`                      
          `void`              `publish​(LogRecord record)`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.util.logging.Handler}

            ### Methods inherited from class java.util.logging.[Handler](http://docs.oracle.com/javase/7/docs/api/java/util/logging/Handler.html?is-external=true "class or interface in java.util.logging"){.externalLink}

            `getEncoding, getErrorManager, getFilter, getFormatter, getLevel, isLoggable, reportError, setEncoding, setErrorManager, setFilter, setFormatter, setLevel`

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

        []{#<init>(com.facebook.buck.log.LogFileHandler)}

        -   #### AsyncLogHandler

                public AsyncLogHandler​(LogFileHandler delegate)

        []{#<init>(java.util.function.Supplier,java.util.logging.Handler)}

        -   #### AsyncLogHandler

                protected AsyncLogHandler​(java.util.function.Supplier<Executor> performLoggingExecutor,
                                          Handler delegate)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#publish(java.util.logging.LogRecord)}

        -   #### publish

            ``` methodSignature
            public void publish​(LogRecord record)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `publish` in class `Handler`

        []{#flush()}

        -   #### flush

            ``` methodSignature
            public void flush()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `flush` in class `Handler`

        []{#close()}

        -   #### close

            ``` methodSignature
            public void close()
                       throws SecurityException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `close` in class `Handler`

            [Throws:]{.throwsLabel}
            :   `SecurityException`
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
