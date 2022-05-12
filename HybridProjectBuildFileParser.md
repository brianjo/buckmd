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
[Package]{.packageLabelInType} [com.facebook.buck.parser](package-summary.html)
:::

## Class HybridProjectBuildFileParser {#class-hybridprojectbuildfileparser .title title="Class HybridProjectBuildFileParser"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.parser.HybridProjectBuildFileParser

::: description
-   

    All Implemented Interfaces:
    :   `FileParser<BuildFileManifest>`, `ProjectBuildFileParser`,
        `AutoCloseable`

    ------------------------------------------------------------------------

        public class HybridProjectBuildFileParser
        extends Object
        implements ProjectBuildFileParser

    ::: block
    Hybrid project build file parser that uses Python DSL, Skylark or
    any other
    [`Syntax`](api/Syntax.html "enum in com.facebook.buck.parser.api")
    depending on which one is requested for the individual build file.
    The default syntax determines the syntax used in cases when marker
    is not used, but clients can explicitly request desired syntax by
    adding parser directive to the beginning of the build file followed
    by one of the supported
    [`Syntax`](api/Syntax.html "enum in com.facebook.buck.parser.api")
    values.

    Note that default syntax is not used in cases when invalid syntax
    value is provided - instead in such cases an exception is thrown.
    :::
:::

::: summary
-   ::: {.section role="region"}
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
        | `static HybridPr      | `using​(c              |                       |
        | ojectBuildFileParser` | om.google.common.coll |                       |
        |                       | ect.ImmutableMap<Synt |                       |
        |                       | ax,​ProjectBuildFilePa |                       |
        |                       | rser> parsers,      S |                       |
        |                       | yntax defaultSyntax)` |                       |
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

        []{#using(com.google.common.collect.ImmutableMap,com.facebook.buck.parser.api.Syntax)}

        -   #### using

            ``` methodSignature
            public static HybridProjectBuildFileParser using​(com.google.common.collect.ImmutableMap<Syntax,​ProjectBuildFileParser> parsers,
                                                             Syntax defaultSyntax)
            ```

            [Returns:]{.returnLabel}
            :   The hybrid parser that supports Python DSL and Skylark
                syntax.
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