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
[Package]{.packageLabelInType} [com.facebook.buck.cli.bootstrapper](package-summary.html)
:::

## Class ConsoleHandler {#class-consolehandler .title title="Class ConsoleHandler"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [java.util.logging.Handler](http://docs.oracle.com/javase/7/docs/api/java/util/logging/Handler.html?is-external=true "class or interface in java.util.logging"){.externalLink}

    -   -   com.facebook.buck.cli.bootstrapper.ConsoleHandler

::: description
-   

    All Implemented Interfaces:
    :   `Callable<Handler>`

    ------------------------------------------------------------------------

        public final class ConsoleHandler
        extends Handler
        implements Callable<Handler>
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor          Description
          -------------------- -------------
          `ConsoleHandler()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                        Description
          ------------------- ----------------------------- -------------
          `Handler`           `call()`                       
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

        []{#<init>()}

        -   #### ConsoleHandler

                public ConsoleHandler()
                               throws IllegalAccessException,
                                      InstantiationException

            [Throws:]{.throwsLabel}
            :   `IllegalAccessException`
            :   `InstantiationException`
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

        []{#call()}

        -   #### call

            ``` methodSignature
            public Handler call()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `call` in interface `Callable<Handler>`
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
