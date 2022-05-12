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

## Class TimedLogger {#class-timedlogger .title title="Class TimedLogger"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.log.TimedLogger

::: description
-   

    ------------------------------------------------------------------------

        public class TimedLogger
        extends Object

    ::: block
    Records the time that logging calls takes, and alerts if they go
    over configured threshold.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                               Description
          ------------------------------------------------------------------------- -------------
          `TimedLogger​(Logger delegate)`                                             
          `TimedLogger​(Logger delegate,            int maxLogCallDurationMillis)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                                          Description
          ------------------- ----------------------------------------------- -------------
          `void`              `debug​(String rawMessage)`                       
          `void`              `error​(String rawMessage)`                       
          `void`              `error​(Throwable ex)`                            
          `void`              `error​(Throwable ex,      String rawMessage)`    
          `void`              `info​(String rawMessage)`                        
          `boolean`           `isVerboseEnabled()`                             
          `void`              `verbose​(String rawMessage)`                     
          `void`              `warn​(String rawMessage)`                        

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

        []{#<init>(com.facebook.buck.core.util.log.Logger)}

        -   #### TimedLogger

                public TimedLogger​(Logger delegate)

        []{#<init>(com.facebook.buck.core.util.log.Logger,int)}

        -   #### TimedLogger

                public TimedLogger​(Logger delegate,
                                   int maxLogCallDurationMillis)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#verbose(java.lang.String)}

        -   #### verbose

            ``` methodSignature
            public void verbose​(String rawMessage)
            ```

        []{#info(java.lang.String)}

        -   #### info

            ``` methodSignature
            public void info​(String rawMessage)
            ```

        []{#warn(java.lang.String)}

        -   #### warn

            ``` methodSignature
            public void warn​(String rawMessage)
            ```

        []{#debug(java.lang.String)}

        -   #### debug

            ``` methodSignature
            public void debug​(String rawMessage)
            ```

        []{#error(java.lang.String)}

        -   #### error

            ``` methodSignature
            public void error​(String rawMessage)
            ```

        []{#error(java.lang.Throwable)}

        -   #### error

            ``` methodSignature
            public void error​(Throwable ex)
            ```

        []{#error(java.lang.Throwable,java.lang.String)}

        -   #### error

            ``` methodSignature
            public void error​(Throwable ex,
                              String rawMessage)
            ```

        []{#isVerboseEnabled()}

        -   #### isVerboseEnabled

            ``` methodSignature
            public boolean isVerboseEnabled()
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
