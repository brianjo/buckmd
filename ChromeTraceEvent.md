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
[Package]{.packageLabelInType} [com.facebook.buck.event.chrome_trace](package-summary.html)
:::

## Class ChromeTraceEvent {#class-chrometraceevent .title title="Class ChromeTraceEvent"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.event.chrome_trace.ChromeTraceEvent

::: description
-   

    ------------------------------------------------------------------------

        public class ChromeTraceEvent
        extends Object

    ::: block
    Json format for Chrome Trace events that can be viewed in
    chrome://tracing. See https://github.com/google/trace-viewer for
    more information.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type   Class                      Description
          ------------------- -------------------------- -------------
          `static class `     `ChromeTraceEvent.Phase`    

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                                                                                     Description
          ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `ChromeTraceEvent​(String category,                 String name,                 ChromeTraceEvent.Phase phase,                 long processId,                 long threadId,                 long microTime,                 long microThreadUserTime,                 com.google.common.collect.ImmutableMap<String,​? extends Object> args)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                   Method                       Description
          ------------------------------------------------------------------- ---------------------------- -------------
          `com.google.common.collect.ImmutableMap<String,​? extends Object>`   `getArgs()`                   
          `String`                                                            `getCategory()`               
          `long`                                                              `getMicroThreadUserTime()`    
          `long`                                                              `getMicroTime()`              
          `String`                                                            `getName()`                   
          `ChromeTraceEvent.Phase`                                            `getPhase()`                  
          `long`                                                              `getProcessId()`              
          `long`                                                              `getThreadId()`               

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

        []{#<init>(java.lang.String,java.lang.String,com.facebook.buck.event.chrome_trace.ChromeTraceEvent.Phase,long,long,long,long,com.google.common.collect.ImmutableMap)}

        -   #### ChromeTraceEvent

                public ChromeTraceEvent​(String category,
                                        String name,
                                        ChromeTraceEvent.Phase phase,
                                        long processId,
                                        long threadId,
                                        long microTime,
                                        long microThreadUserTime,
                                        com.google.common.collect.ImmutableMap<String,​? extends Object> args)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getName()}

        -   #### getName

            ``` methodSignature
            public String getName()
            ```

        []{#getPhase()}

        -   #### getPhase

            ``` methodSignature
            public ChromeTraceEvent.Phase getPhase()
            ```

        []{#getProcessId()}

        -   #### getProcessId

            ``` methodSignature
            public long getProcessId()
            ```

        []{#getThreadId()}

        -   #### getThreadId

            ``` methodSignature
            public long getThreadId()
            ```

        []{#getMicroTime()}

        -   #### getMicroTime

            ``` methodSignature
            public long getMicroTime()
            ```

        []{#getMicroThreadUserTime()}

        -   #### getMicroThreadUserTime

            ``` methodSignature
            public long getMicroThreadUserTime()
            ```

        []{#getArgs()}

        -   #### getArgs

            ``` methodSignature
            public com.google.common.collect.ImmutableMap<String,​? extends Object> getArgs()
            ```

        []{#getCategory()}

        -   #### getCategory

            ``` methodSignature
            public String getCategory()
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
