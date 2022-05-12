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
[Package]{.packageLabelInType} [com.facebook.buck.parser](package-summary.html)
:::

## Class ConcurrentProjectBuildFileParser {#class-concurrentprojectbuildfileparser .title title="Class ConcurrentProjectBuildFileParser"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.parser.ConcurrentProjectBuildFileParser

::: description
-   

    All Implemented Interfaces:
    :   `FileParser<BuildFileManifest>`, `ProjectBuildFileParser`,
        `AutoCloseable`

    ------------------------------------------------------------------------

        public class ConcurrentProjectBuildFileParser
        extends Object
        implements ProjectBuildFileParser

    ::: block
    Add synchronization layer over existing
    [`ProjectBuildFileParser`](api/ProjectBuildFileParser.html "interface in com.facebook.buck.parser.api")
    by creating and maintaining a pool of
    [`ProjectBuildFileParser`](api/ProjectBuildFileParser.html "interface in com.facebook.buck.parser.api")\'s
    instances.
    This
    [`PythonDslProjectBuildFileParser`](PythonDslProjectBuildFileParser.html "class in com.facebook.buck.parser")
    wrapper creates new instances of delegated parser using a provided
    factory and adds them to worker pool. If free parser is available at
    the time a request is made, it is reused, if not then it is
    recreated. Once parsing request (aka
    [`FileParser.getManifest(Path)`](api/FileParser.html#getManifest(java.nio.file.Path))
    is complete, parser is returned to the worker pool. Worker pool of
    parsers can grow unconditionally so it is really up to the user of
    this class to manage concurrency level by calling this class\'
    methods appropriate number of times in parallel.

    Note that [`reportProfile()`](#reportProfile()) and
    [`close()`](#close()) are not synchronized with the worker pool and
    just call appropriate methods from all the parsers created to the
    moment. They should only be called when no parsing is in effect.

    The main reason for this class is to overcome limitations of current
    implementation of
    [`PythonDslProjectBuildFileParser`](PythonDslProjectBuildFileParser.html "class in com.facebook.buck.parser")
    which is stateful and not multithreaded, but Graph Engine
    transformations require parsers to be concurrent.

    Another option would be to modify existing
    [`PythonDslProjectBuildFileParser`](PythonDslProjectBuildFileParser.html "class in com.facebook.buck.parser")
    to be concurrent. However the legacy
    [`Parser`](Parser.html "interface in com.facebook.buck.parser")
    pipelines use
    [`ResourcePool`](../util/concurrent/ResourcePool.html "class in com.facebook.buck.util.concurrent")s
    to shard parser instances, though in fact it is not needed for
    [`SkylarkProjectBuildFileParser`](../skylark/parser/SkylarkProjectBuildFileParser.html "class in com.facebook.buck.skylark.parser")
    which is concurrent. So, it will require to refactor existing parser
    pipelines to get rid of
    [`ResourcePool`](../util/concurrent/ResourcePool.html "class in com.facebook.buck.util.concurrent")
    which is a bigger change, so it probably should be done once parsing
    is fully switched to Graph Engine.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

        +-----------------------------------+-----------------------------------+
        | Constructor                       | Description                       |
        +===================================+===================================+
        | `ConcurrentProject                | ::: block                         |
        | BuildFileParser​(java.util.functio | Create new instance of            |
        | n.Supplier<ProjectBuildFileParser | [`Concurrent                      |
        | > projectBuildFileParserFactory)` | ProjectBuildFileParser`](Concurre |
        |                                   | ntProjectBuildFileParser.html "cl |
        |                                   | ass in com.facebook.buck.parser") |
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
        | `void`                | `close()`             |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.          | `getIncludedF         | ::: block             |
        | common.collect.Immuta | iles​(Path buildFile)` | Collects the loaded   |
        | bleSortedSet<String>` |                       | files and extensions  |
        |                       |                       | when parsing the      |
        |                       |                       | `parseFile` build     |
        |                       |                       | spec.                 |
        |                       |                       | :::                   |
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
        | `boolean`             | `globResultsM         | ::: block             |
        |                       | atchCurrentState​(Path | Checks if existing    |
        |                       |  buildFile,           | `GlobSpec`s with      |
        |                       |                    co | results are the same  |
        |                       | m.google.common.colle | as current state in   |
        |                       | ct.ImmutableList<Glob | the file system.      |
        |                       | SpecWithResult> exist | :::                   |
        |                       | ingGlobsWithResults)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `reportProfile()`     | ::: block             |
        |                       |                       | Reports profile       |
        |                       |                       | information captured  |
        |                       |                       | while parsing build   |
        |                       |                       | files.                |
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

        []{#<init>(java.util.function.Supplier)}

        -   #### ConcurrentProjectBuildFileParser

                public ConcurrentProjectBuildFileParser​(java.util.function.Supplier<ProjectBuildFileParser> projectBuildFileParserFactory)

            ::: block
            Create new instance of
            [`ConcurrentProjectBuildFileParser`](ConcurrentProjectBuildFileParser.html "class in com.facebook.buck.parser")
            :::

            [Parameters:]{.paramLabel}
            :   `projectBuildFileParserFactory` - Factory that will be
                used for creating new instances of
                [`ProjectBuildFileParser`](api/ProjectBuildFileParser.html "interface in com.facebook.buck.parser.api")
                on demand. In order to make wrapped
                [`ProjectBuildFileParser`](api/ProjectBuildFileParser.html "interface in com.facebook.buck.parser.api")
                thread-safe this factory should create instances for
                each invocation, not memoize them, otherwise the same
                object will be used for all threads.
    :::

    ::: {.section role="region"}
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

            [Parameters:]{.paramLabel}
            :   `buildFile` - should be an absolute path to a file. Must
                have rootPath as its prefix.

            [Throws:]{.throwsLabel}
            :   `BuildFileParseException`
            :   `InterruptedException`
            :   `IOException`

        []{#reportProfile()}

        -   #### reportProfile

            ``` methodSignature
            public void reportProfile()
                               throws IOException
            ```

            ::: block
            [Description copied from
            interface: `ProjectBuildFileParser`]{.descfrmTypeLabel}
            :::

            ::: block
            Reports profile information captured while parsing build
            files.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `reportProfile` in interface `ProjectBuildFileParser`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#getIncludedFiles(java.nio.file.Path)}

        -   #### getIncludedFiles

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedSet<String> getIncludedFiles​(Path buildFile)
                                                                                  throws BuildFileParseException,
                                                                                         InterruptedException,
                                                                                         IOException
            ```

            ::: block
            [Description copied from
            interface: `FileParser`]{.descfrmTypeLabel}
            :::

            ::: block
            Collects the loaded files and extensions when parsing the
            `parseFile` build spec.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getIncludedFiles` in
                interface `FileParser<BuildFileManifest>`

            [Parameters:]{.paramLabel}
            :   `buildFile` - should be an absolute path to a file. Must
                have rootPath as its prefix.

            [Throws:]{.throwsLabel}
            :   `BuildFileParseException`
            :   `InterruptedException`
            :   `IOException`

        []{#globResultsMatchCurrentState(java.nio.file.Path,com.google.common.collect.ImmutableList)}

        -   #### globResultsMatchCurrentState

            ``` methodSignature
            public boolean globResultsMatchCurrentState​(Path buildFile,
                                                        com.google.common.collect.ImmutableList<GlobSpecWithResult> existingGlobsWithResults)
                                                 throws IOException,
                                                        InterruptedException
            ```

            ::: block
            [Description copied from
            interface: `ProjectBuildFileParser`]{.descfrmTypeLabel}
            :::

            ::: block
            Checks if existing `GlobSpec`s with results are the same as
            current state in the file system.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `globResultsMatchCurrentState` in
                interface `ProjectBuildFileParser`

            [Parameters:]{.paramLabel}
            :   `buildFile` - the buildFile location to be used by the
                Globber.
            :   `existingGlobsWithResults` - the existing (deserialized)
                `GlobSpecWithResult` to check the file system state
                against.

            [Returns:]{.returnLabel}
            :   `true` if glob expansion produces results matching
                previously recorded ones, `false` otherwise.

            [Throws:]{.throwsLabel}
            :   `IOException`
            :   `InterruptedException`

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

            [Throws:]{.throwsLabel}
            :   `BuildFileParseException`
            :   `InterruptedException`
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
