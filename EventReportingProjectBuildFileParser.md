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
-   [Field](#field.summary) \| 
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   Constr \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.parser.decorators](package-summary.html)
:::

## Class EventReportingProjectBuildFileParser {#class-eventreportingprojectbuildfileparser .title title="Class EventReportingProjectBuildFileParser"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.parser.api.ForwardingProjectBuildFileParserDecorator](../api/ForwardingProjectBuildFileParserDecorator.html "class in com.facebook.buck.parser.api")

    -   -   com.facebook.buck.parser.decorators.EventReportingProjectBuildFileParser

::: description
-   

    All Implemented Interfaces:
    :   `FileParser<BuildFileManifest>`, `ProjectBuildFileParser`,
        `AutoCloseable`

    ------------------------------------------------------------------------

        public class EventReportingProjectBuildFileParser
        extends ForwardingProjectBuildFileParserDecorator

    ::: block
    Decorator for
    [`ProjectBuildFileParser`](../api/ProjectBuildFileParser.html "interface in com.facebook.buck.parser.api")
    that is responsible for reporting parse lifecycle events like start
    and finish.
    This decouples status reporting functionality so that it can be used
    with different underlying
    [`ProjectBuildFileParser`](../api/ProjectBuildFileParser.html "interface in com.facebook.buck.parser.api")s.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        -   []{#fields.inherited.from.class.com.facebook.buck.parser.api.ForwardingProjectBuildFileParserDecorator}

            ### Fields inherited from class com.facebook.buck.parser.api.[ForwardingProjectBuildFileParserDecorator](../api/ForwardingProjectBuildFileParserDecorator.html "class in com.facebook.buck.parser.api")

            `delegate`
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `void`                | `close()`             |                       |
        +-----------------------+-----------------------+-----------------------+
        | `BuildFileManifest`   | `getMani              | ::: block             |
        |                       | fest​(Path buildFile)` | Collect all           |
        |                       |                       | information from a    |
        |                       |                       | particular, along     |
        |                       |                       | with metadata about   |
        |                       |                       | the information, for  |
        |                       |                       | example which other   |
        |                       |                       | files were also       |
        |                       |                       | parsed.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `st                   | `of​(ProjectBuildFile  | ::: block             |
        | atic EventReportingPr | Parser delegate,   Bu | Static factory method |
        | ojectBuildFileParser` | ckEventBus eventBus)` | for producing         |
        |                       |                       | instances of          |
        |                       |                       | [`Eve                 |
        |                       |                       | ntReportingProjectBui |
        |                       |                       | ldFileParser`](EventR |
        |                       |                       | eportingProjectBuildF |
        |                       |                       | ileParser.html "class |
        |                       |                       |  in com.facebook.buck |
        |                       |                       | .parser.decorators"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.parser.api.ForwardingProjectBuildFileParserDecorator}

            ### Methods inherited from class com.facebook.buck.parser.api.[ForwardingProjectBuildFileParserDecorator](../api/ForwardingProjectBuildFileParserDecorator.html "class in com.facebook.buck.parser.api")

            `getIncludedFiles, globResultsMatchCurrentState, reportProfile`

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
    -   []{#method.detail}

        ### Method Detail

        []{#getManifest(java.nio.file.Path)}

        -   #### getManifest

            ``` methodSignature
            public BuildFileManifest getManifest​(Path buildFile)
                                          throws BuildFileParseException,
                                                 InterruptedException,
                                                 IOException
            ```

            ::: block
            [Description copied from
            interface: `FileParser`]{.descfrmTypeLabel}
            :::

            ::: block
            Collect all information from a particular, along with
            metadata about the information, for example which other
            files were also parsed.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getManifest` in
                interface `FileParser<BuildFileManifest>`

            [Overrides:]{.overrideSpecifyLabel}
            :   `getManifest` in
                class `ForwardingProjectBuildFileParserDecorator`

            [Parameters:]{.paramLabel}
            :   `buildFile` - should be an absolute path to a file. Must
                have rootPath as its prefix.

            [Throws:]{.throwsLabel}
            :   `BuildFileParseException`
            :   `InterruptedException`
            :   `IOException`

        []{#close()}

        -   #### close

            ``` methodSignature
            public void close()
                       throws BuildFileParseException,
                              InterruptedException,
                              IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `close` in interface `AutoCloseable`

            [Specified by:]{.overrideSpecifyLabel}
            :   `close` in interface `FileParser<BuildFileManifest>`

            [Overrides:]{.overrideSpecifyLabel}
            :   `close` in
                class `ForwardingProjectBuildFileParserDecorator`

            [Throws:]{.throwsLabel}
            :   `BuildFileParseException`
            :   `InterruptedException`
            :   `IOException`

        []{#of(com.facebook.buck.parser.api.ProjectBuildFileParser,com.facebook.buck.event.BuckEventBus)}

        -   #### of

            ``` methodSignature
            public static EventReportingProjectBuildFileParser of​(ProjectBuildFileParser delegate,
                                                                  BuckEventBus eventBus)
            ```

            ::: block
            Static factory method for producing instances of
            [`EventReportingProjectBuildFileParser`](EventReportingProjectBuildFileParser.html "class in com.facebook.buck.parser.decorators").
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
-   Nested \| 
-   [Field](#field.summary) \| 
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   Constr \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
