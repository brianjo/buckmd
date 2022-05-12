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

## Class BuildTraces {#class-buildtraces .title title="Class BuildTraces"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.util.trace.BuildTraces

::: description
-   

    ------------------------------------------------------------------------

        public class BuildTraces
        extends Object

    ::: block
    Utility to help with reading data from build trace files.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type   Class                           Description
          ------------------- ------------------------------- -------------
          `static class `     `BuildTraces.TraceAttributes`    

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type   Field                Description
          ------------------- -------------------- -------------
          `static Pattern`    `TRACE_ID_PATTERN`    

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                          Description
          ---------------------------------------------------- -------------
          `BuildTraces​(ProjectFilesystem projectFilesystem)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `I                    | `getInputs            |                       |
        | terable<InputStream>` | ForTraces​(String id)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `BuildTr              | `getTraceAttr         |                       |
        | aces.TraceAttributes` | ibutesFor​(String id)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `BuildTr              | `getTraceAttributesF  | ::: block             |
        | aces.TraceAttributes` | or​(Path pathToTrace)` | Parses a trace file   |
        |                       |                       | and returns the       |
        |                       |                       | command that the user |
        |                       |                       | executed to create    |
        |                       |                       | the trace.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `List<Path>`          | `listTraceF           | ::: block             |
        |                       | ilesByLastModified()` | The most recent trace |
        |                       |                       | (the one with the     |
        |                       |                       | greatest              |
        |                       |                       | last-modified time)   |
        |                       |                       | will be listed first. |
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
    -   []{#field.detail}

        ### Field Detail

        []{#TRACE_ID_PATTERN}

        -   #### TRACE_ID_PATTERN

                public static final Pattern TRACE_ID_PATTERN
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.io.filesystem.ProjectFilesystem)}

        -   #### BuildTraces

                public BuildTraces​(ProjectFilesystem projectFilesystem)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getInputsForTraces(java.lang.String)}

        -   #### getInputsForTraces

            ``` methodSignature
            public Iterable<InputStream> getInputsForTraces​(String id)
                                                     throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#getTraceAttributesFor(java.lang.String)}

        -   #### getTraceAttributesFor

            ``` methodSignature
            public BuildTraces.TraceAttributes getTraceAttributesFor​(String id)
                                                              throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#getTraceAttributesFor(java.nio.file.Path)}

        -   #### getTraceAttributesFor

            ``` methodSignature
            public BuildTraces.TraceAttributes getTraceAttributesFor​(Path pathToTrace)
                                                              throws IOException
            ```

            ::: block
            Parses a trace file and returns the command that the user
            executed to create the trace.
            This method tries to be reasonably tolerant of changes to
            the .trace file schema, returning
            [`Optional.empty()`](http://docs.oracle.com/javase/7/docs/api/java/util/Optional.html?is-external=true#empty() "class or interface in java.util"){.externalLink}
            if it does not find the fields in the JSON that it expects.
            :::

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#listTraceFilesByLastModified()}

        -   #### listTraceFilesByLastModified

            ``` methodSignature
            public List<Path> listTraceFilesByLastModified()
                                                    throws IOException
            ```

            ::: block
            The most recent trace (the one with the greatest
            last-modified time) will be listed first.
            :::

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
