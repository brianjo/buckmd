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
[Package]{.packageLabelInType} [com.facebook.buck.event.chrome_trace](package-summary.html)
:::

## Class ChromeTraceWriter {#class-chrometracewriter .title title="Class ChromeTraceWriter"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.event.chrome_trace.ChromeTraceWriter

::: description
-   

    All Implemented Interfaces:
    :   `AutoCloseable`

    ------------------------------------------------------------------------

        public class ChromeTraceWriter
        extends Object
        implements AutoCloseable

    ::: block
    Type-safe utility to write Chrome trace events to files.
    :::

    [See Also:]{.seeLabel}
    :   [`ChromeTraceEvent`](ChromeTraceEvent.html "class in com.facebook.buck.event.chrome_trace")
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

        +-----------------------------------+-----------------------------------+
        | Constructor                       | Description                       |
        +===================================+===================================+
        | `ChromeTr                         | ::: block                         |
        | aceWriter​(com.fasterxml.jackson.c | Create a writer backed by         |
        | ore.JsonGenerator jsonGenerator)` | specified json generator.         |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+
        | `ChromeTrace                      | ::: block                         |
        | Writer​(OutputStream traceStream)` | Create a writer backed by         |
        |                                   | specified output stream.          |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+

        : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `void`                | `close()`             | ::: block             |
        |                       |                       | Close the underlying  |
        |                       |                       | json generator.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `writeEnd()`          | ::: block             |
        |                       |                       | Must be called after  |
        |                       |                       | all events to         |
        |                       |                       | properly terminate    |
        |                       |                       | event stream.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `writ                 | ::: block             |
        |                       | eEvent​(ChromeTraceEve | Write single event.   |
        |                       | nt chromeTraceEvent)` | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `writeStart()`        | ::: block             |
        |                       |                       | Must be called prior  |
        |                       |                       | to emitting first     |
        |                       |                       | event to properly     |
        |                       |                       | initialize stream.    |
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

        []{#<init>(java.io.OutputStream)}

        -   #### ChromeTraceWriter

                public ChromeTraceWriter​(OutputStream traceStream)
                                  throws IOException

            ::: block
            Create a writer backed by specified output stream.
            :::

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#<init>(com.fasterxml.jackson.core.JsonGenerator)}

        -   #### ChromeTraceWriter

                public ChromeTraceWriter​(com.fasterxml.jackson.core.JsonGenerator jsonGenerator)

            ::: block
            Create a writer backed by specified json generator.
            :::
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#writeEvent(com.facebook.buck.event.chrome_trace.ChromeTraceEvent)}

        -   #### writeEvent

            ``` methodSignature
            public void writeEvent​(ChromeTraceEvent chromeTraceEvent)
                            throws IOException
            ```

            ::: block
            Write single event.
            :::

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#writeStart()}

        -   #### writeStart

            ``` methodSignature
            public void writeStart()
                            throws IOException
            ```

            ::: block
            Must be called prior to emitting first event to properly
            initialize stream.
            :::

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#writeEnd()}

        -   #### writeEnd

            ``` methodSignature
            public void writeEnd()
                          throws IOException
            ```

            ::: block
            Must be called after all events to properly terminate event
            stream.
            :::

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#close()}

        -   #### close

            ``` methodSignature
            public void close()
                       throws IOException
            ```

            ::: block
            Close the underlying json generator.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `close` in interface `AutoCloseable`

            [Throws:]{.throwsLabel}
            :   `IOException`
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
