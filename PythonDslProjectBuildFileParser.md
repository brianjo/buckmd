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

## Class PythonDslProjectBuildFileParser {#class-pythondslprojectbuildfileparser .title title="Class PythonDslProjectBuildFileParser"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.parser.PythonDslProjectBuildFileParser

::: description
-   

    All Implemented Interfaces:
    :   `FileParser<BuildFileManifest>`, `ProjectBuildFileParser`,
        `AutoCloseable`

    ------------------------------------------------------------------------

        public class PythonDslProjectBuildFileParser
        extends Object
        implements ProjectBuildFileParser

    ::: block
    Delegates to buck.py for parsing of buck build files. Constructed on
    demand for the parsing phase and must be closed afterward to free up
    resources.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             Description
          --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `PythonDslProjectBuildFileParser​(ProjectBuildFileParserOptions options,                                TypeCoercerFactory typeCoercerFactory,                                com.google.common.collect.ImmutableMap<String,​String> environment,                                BuckEventBus buckEventBus,                                ProcessExecutor processExecutor,                                Optional<AtomicLong> processedBytes,                                Optional<UserDefinedRuleLoader> userDefinedRulesParser)`    

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
        | `protect              | `getAllRulesInte      |                       |
        | ed BuildFileManifest` | rnal​(Path buildFile)` |                       |
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
        |                       | fest​(Path buildFile)` | Collect all rules     |
        |                       |                       | from a particular     |
        |                       |                       | build file, along     |
        |                       |                       | with meta rules about |
        |                       |                       | the rules, for        |
        |                       |                       | example which build   |
        |                       |                       | files the rules       |
        |                       |                       | depend on.            |
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
        | `void`                | `initIfNeeded()`      | ::: block             |
        |                       |                       | Initialization on     |
        |                       |                       | demand moves around   |
        |                       |                       | the performance       |
        |                       |                       | impact of creating    |
        |                       |                       | the Python            |
        |                       |                       | interpreter to when   |
        |                       |                       | parsing actually      |
        |                       |                       | begins.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isClosed()`          |                       |
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

        []{#<init>(com.facebook.buck.parser.options.ProjectBuildFileParserOptions,com.facebook.buck.rules.coercer.TypeCoercerFactory,com.google.common.collect.ImmutableMap,com.facebook.buck.event.BuckEventBus,com.facebook.buck.util.ProcessExecutor,java.util.Optional,java.util.Optional)}

        -   #### PythonDslProjectBuildFileParser

                public PythonDslProjectBuildFileParser​(ProjectBuildFileParserOptions options,
                                                       TypeCoercerFactory typeCoercerFactory,
                                                       com.google.common.collect.ImmutableMap<String,​String> environment,
                                                       BuckEventBus buckEventBus,
                                                       ProcessExecutor processExecutor,
                                                       Optional<AtomicLong> processedBytes,
                                                       Optional<UserDefinedRuleLoader> userDefinedRulesParser)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#isClosed()}

        -   #### isClosed

            ``` methodSignature
            public boolean isClosed()
            ```

        []{#initIfNeeded()}

        -   #### initIfNeeded

            ``` methodSignature
            public void initIfNeeded()
                              throws IOException
            ```

            ::: block
            Initialization on demand moves around the performance impact
            of creating the Python interpreter to when parsing actually
            begins. This makes it easier to attribute this time to the
            actual parse phase.
            :::

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#getManifest(java.nio.file.Path)}

        -   #### getManifest

            ``` methodSignature
            public BuildFileManifest getManifest​(Path buildFile)
                                          throws BuildFileParseException,
                                                 InterruptedException
            ```

            ::: block
            Collect all rules from a particular build file, along with
            meta rules about the rules, for example which build files
            the rules depend on.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getManifest` in
                interface `FileParser<BuildFileManifest>`

            [Parameters:]{.paramLabel}
            :   `buildFile` - should be an absolute path to a build
                file. Must have rootPath as its prefix.

            [Throws:]{.throwsLabel}
            :   `BuildFileParseException`
            :   `InterruptedException`

        []{#getAllRulesInternal(java.nio.file.Path)}

        -   #### getAllRulesInternal

            ``` methodSignature
            protected BuildFileManifest getAllRulesInternal​(Path buildFile)
                                                     throws IOException,
                                                            BuildFileParseException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`
            :   `BuildFileParseException`

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
                                                                                         InterruptedException
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

        []{#globResultsMatchCurrentState(java.nio.file.Path,com.google.common.collect.ImmutableList)}

        -   #### globResultsMatchCurrentState

            ``` methodSignature
            public boolean globResultsMatchCurrentState​(Path buildFile,
                                                        com.google.common.collect.ImmutableList<GlobSpecWithResult> existingGlobsWithResults)
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
