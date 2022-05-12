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
[Package]{.packageLabelInType} [com.facebook.buck.util.trace](package-summary.html)
:::

## Class ChromeTraceParser {#class-chrometraceparser .title title="Class ChromeTraceParser"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.util.trace.ChromeTraceParser

::: description
-   

    ------------------------------------------------------------------------

        public class ChromeTraceParser
        extends Object

    ::: block
    Event-driven parser for [Chrome
    traces](https://docs.google.com/document/d/1CvAClvFfyA5R-PhYUmn5OOQtYMH4h6I0nSsKchNAySU/preview).
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static interface `   | `Chr                  | ::: block             |
        |                       | omeTraceParser.Chrome | Extracts data of      |
        |                       | TraceEventMatcher<T>` | interest if it finds  |
        |                       |                       | a Chrome trace event  |
        |                       |                       | of the type it is     |
        |                       |                       | looking for.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Field                 | Description           |
        +=======================+=======================+=======================+
        | `static ChromeTr      | `COMMAND`             | ::: block             |
        | aceParser.ChromeTrace |                       | Tries to extract the  |
        | EventMatcher<String>` |                       | command that was used |
        |                       |                       | to trigger the        |
        |                       |                       | invocation of Buck    |
        |                       |                       | that generated the    |
        |                       |                       | trace.                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                Description
          ---------------------------------------------------------- -------------
          `ChromeTraceParser​(ProjectFilesystem projectFilesystem)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `st                   | `getResultFor         | ::: block             |
        | atic <T> Optional<T>` | Matcher​(ChromeTracePa | Designed for use with |
        |                       | rser.ChromeTraceEvent | the result of         |
        |                       | Matcher<T> matcher,   | [`parse(Path, Set)`]( |
        |                       |                   Map | #parse(java.nio.file. |
        |                       | <ChromeTraceParser.Ch | Path,java.util.Set)). |
        |                       | romeTraceEventMatcher | :::                   |
        |                       | <?>,​Object> results)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Map<ChromeTrace      | `                     | ::: block             |
        | Parser.ChromeTraceEve | parse​(Path pathToTrac | Parses a Chrome trace |
        | ntMatcher<?>,​Object>` | e,      Set<ChromeTra | and stops parsing     |
        |                       | ceParser.ChromeTraceE | once all of the       |
        |                       | ventMatcher<?>> chrom | specified matchers    |
        |                       | eTraceEventMatchers)` | have been satisfied.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
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
    -   []{#field.detail}

        ### Field Detail

        []{#COMMAND}

        -   #### COMMAND

                public static final ChromeTraceParser.ChromeTraceEventMatcher<String> COMMAND

            ::: block
            Tries to extract the command that was used to trigger the
            invocation of Buck that generated the trace. If found, it
            returns the command as an opaque string.
            :::
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.io.filesystem.ProjectFilesystem)}

        -   #### ChromeTraceParser

                public ChromeTraceParser​(ProjectFilesystem projectFilesystem)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#parse(java.nio.file.Path,java.util.Set)}

        -   #### parse

            ``` methodSignature
            public Map<ChromeTraceParser.ChromeTraceEventMatcher<?>,​Object> parse​(Path pathToTrace,
                                                                                        Set<ChromeTraceParser.ChromeTraceEventMatcher<?>> chromeTraceEventMatchers)
                                                                                 throws IOException
            ```

            ::: block
            Parses a Chrome trace and stops parsing once all of the
            specified matchers have been satisfied. This method parses
            only one Chrome trace event at a time, which avoids loading
            the entire trace into memory.
            :::

            [Parameters:]{.paramLabel}
            :   `pathToTrace` - is a relative path \[to the
                ProjectFilesystem\] to a Chrome trace in the \"JSON
                Array Format.\"
            :   `chromeTraceEventMatchers` - set of matchers this
                invocation of `parse()` is trying to satisfy. Once a
                matcher finds a match, it will not consider any other
                events in the trace.

            [Returns:]{.returnLabel}
            :   a `Map` where every matcher that found a match will have
                an entry whose key is the matcher and whose value is the
                one returned by
                [`ChromeTraceParser.ChromeTraceEventMatcher.test(Map,      String)`](ChromeTraceParser.ChromeTraceEventMatcher.html#test(java.util.Map,java.lang.String))
                without the
                [`Optional`](http://docs.oracle.com/javase/7/docs/api/java/util/Optional.html?is-external=true "class or interface in java.util"){.externalLink}
                wrapper.

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#getResultForMatcher(com.facebook.buck.util.trace.ChromeTraceParser.ChromeTraceEventMatcher,java.util.Map)}

        -   #### getResultForMatcher

            ``` methodSignature
            public static <T> Optional<T> getResultForMatcher​(ChromeTraceParser.ChromeTraceEventMatcher<T> matcher,
                                                              Map<ChromeTraceParser.ChromeTraceEventMatcher<?>,​Object> results)
            ```

            ::: block
            Designed for use with the result of
            [`parse(Path, Set)`](#parse(java.nio.file.Path,java.util.Set)).
            Helper function to avoid some distasteful casting logic.
            :::
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
