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
[Package]{.packageLabelInType} [com.facebook.buck.skylark.parser](package-summary.html)
:::

## Class SkylarkProjectBuildFileParser {#class-skylarkprojectbuildfileparser .title title="Class SkylarkProjectBuildFileParser"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.skylark.parser.SkylarkProjectBuildFileParser

::: description
-   

    All Implemented Interfaces:
    :   `FileParser<BuildFileManifest>`, `ProjectBuildFileParser`,
        `UserDefinedRuleLoader`, `AutoCloseable`

    ------------------------------------------------------------------------

        public class SkylarkProjectBuildFileParser
        extends Object
        implements ProjectBuildFileParser, UserDefinedRuleLoader

    ::: block
    Parser for build files written using Skylark syntax.
    NOTE: This parser is still a work in progress and does not support
    some functions provided by Python DSL parser like `include_defs`, so
    use in production at your own risk.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type                                               Field            Description
          --------------------------------------------------------------- ---------------- -------------
          `protected BuckGlobals`                                         `buckGlobals`     
          `protected com.google.devtools.build.lib.events.EventHandler`   `eventHandler`    
          `protected com.google.devtools.build.lib.vfs.FileSystem`        `fileSystem`      
          `protected ProjectBuildFileParserOptions`                       `options`         

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Modifier       Constructor                                                            Description
          -------------- ---------------------------------------------------------------------- -------------
          `protected `   `SkylarkProjectBuildFileParser​(SkylarkProjectBuildFileParser other)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `protected com.f      | `buildExtensionData​(  | ::: block             |
        | acebook.buck.skylark. | com.facebook.buck.sky | Given fully loaded    |
        | parser.ExtensionData` | lark.parser.AbstractS | extension represented |
        |                       | kylarkFileParser.Exte | by                    |
        |                       | nsionLoadState load)` | `Abst                 |
        |                       |                       | ractSkylarkFileParser |
        |                       |                       | .ExtensionLoadState`, |
        |                       |                       | evaluates extension   |
        |                       |                       | and returns           |
        |                       |                       | `ExtensionData`       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `close()`             |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected co         | `createContainingLa   |                       |
        | m.google.devtools.bui | bel​(String basePath)` |                       |
        | ld.lib.cmdline.Label` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.          | `getIncludedF         | ::: block             |
        | common.collect.Immuta | iles​(Path parseFile)` | Collects the loaded   |
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
        | `protected com.       | `loadExten            | ::: block             |
        | google.common.collect | sions​(com.google.devt | Loads all extensions  |
        | .ImmutableList<com.fa | ools.build.lib.cmdlin | identified by         |
        | cebook.buck.skylark.p | e.Label containingLab | corresponding         |
        | arser.ExtensionData>` | el,               com | `SkylarkImport`s.     |
        |                       | .google.common.collec | :::                   |
        |                       | t.ImmutableList<com.g |                       |
        |                       | oogle.devtools.build. |                       |
        |                       | lib.syntax.SkylarkImp |                       |
        |                       | ort> skylarkImports)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `loadEx               | ::: block             |
        |                       | tensionsForUserDefine | Loads all of the      |
        |                       | dRules​(Path buildFile | extensions mentioned  |
        |                       | ,                     | in a build manifest   |
        |                       |               BuildFi | :::                   |
        |                       | leManifest manifest)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `p                    | `p                    |                       |
        | rotected ParseResult` | arse​(Path parseFile)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected com.goog   | `readSkyla            | ::: block             |
        | le.devtools.build.lib | rkAST​(com.google.devt | Reads file and        |
        | .syntax.BuildFileAST` | ools.build.lib.vfs.Pa | returns abstract      |
        |                       | th path,              | syntax tree for that  |
        |                       |   FileKind fileKind)` | file.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `reportProfile()`     | ::: block             |
        |                       |                       | Reports profile       |
        |                       |                       | information captured  |
        |                       |                       | while parsing build   |
        |                       |                       | files.                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static SkylarkPr     | `u                    | ::: block             |
        | ojectBuildFileParser` | sing​(ProjectBuildFile | Create an instance of |
        |                       | ParserOptions options | Skylark project build |
        |                       | ,      BuckEventBus b | file parser using     |
        |                       | uckEventBus,      com | provided options.     |
        |                       | .google.devtools.buil | :::                   |
        |                       | d.lib.vfs.FileSystem  |                       |
        |                       | fileSystem,      Buck |                       |
        |                       | Globals buckGlobals,  |                       |
        |                       |      com.google.devto |                       |
        |                       | ols.build.lib.events. |                       |
        |                       | EventHandler eventHan |                       |
        |                       | dler,      GlobberFac |                       |
        |                       | tory globberFactory)` |                       |
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

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.parser.api.FileParser}

            ### Methods inherited from interface com.facebook.buck.parser.api.[FileParser](../../parser/api/FileParser.html "interface in com.facebook.buck.parser.api")

            `close, getIncludedFiles`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#field.detail}

        ### Field Detail

        []{#fileSystem}

        -   #### fileSystem

                protected final com.google.devtools.build.lib.vfs.FileSystem fileSystem

        []{#options}

        -   #### options

                protected final ProjectBuildFileParserOptions options

        []{#eventHandler}

        -   #### eventHandler

                protected final com.google.devtools.build.lib.events.EventHandler eventHandler

        []{#buckGlobals}

        -   #### buckGlobals

                protected final BuckGlobals buckGlobals
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.skylark.parser.SkylarkProjectBuildFileParser)}

        -   #### SkylarkProjectBuildFileParser

                protected SkylarkProjectBuildFileParser​(SkylarkProjectBuildFileParser other)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#using(com.facebook.buck.parser.options.ProjectBuildFileParserOptions,com.facebook.buck.event.BuckEventBus,com.google.devtools.build.lib.vfs.FileSystem,com.facebook.buck.skylark.parser.BuckGlobals,com.google.devtools.build.lib.events.EventHandler,com.facebook.buck.skylark.io.GlobberFactory)}

        -   #### using

            ``` methodSignature
            public static SkylarkProjectBuildFileParser using​(ProjectBuildFileParserOptions options,
                                                              BuckEventBus buckEventBus,
                                                              com.google.devtools.build.lib.vfs.FileSystem fileSystem,
                                                              BuckGlobals buckGlobals,
                                                              com.google.devtools.build.lib.events.EventHandler eventHandler,
                                                              GlobberFactory globberFactory)
            ```

            ::: block
            Create an instance of Skylark project build file parser
            using provided options.
            :::

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

        []{#loadExtensionsForUserDefinedRules(java.nio.file.Path,com.facebook.buck.parser.api.BuildFileManifest)}

        -   #### loadExtensionsForUserDefinedRules

            ``` methodSignature
            public void loadExtensionsForUserDefinedRules​(Path buildFile,
                                                          BuildFileManifest manifest)
            ```

            ::: block
            [Description copied from
            interface: `UserDefinedRuleLoader`]{.descfrmTypeLabel}
            :::

            ::: block
            Loads all of the extensions mentioned in a build manifest
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `loadExtensionsForUserDefinedRules` in
                interface `UserDefinedRuleLoader`

            [Parameters:]{.paramLabel}
            :   `buildFile` - The full path to the build file
            :   `manifest` - The manifest from parsing a build file

        []{#parse(java.nio.file.Path)}

        -   #### parse

            ``` methodSignature
            protected ParseResult parse​(Path parseFile)
                                 throws IOException,
                                        BuildFileParseException,
                                        InterruptedException
            ```

            [Returns:]{.returnLabel}
            :   The parsed result defined in `parseFile`.

            [Throws:]{.throwsLabel}
            :   `IOException`
            :   `BuildFileParseException`
            :   `InterruptedException`

        []{#createContainingLabel(java.lang.String)}

        -   #### createContainingLabel

            ``` methodSignature
            protected com.google.devtools.build.lib.cmdline.Label createContainingLabel​(String basePath)
            ```

        []{#readSkylarkAST(com.google.devtools.build.lib.vfs.Path,com.facebook.buck.skylark.parser.FileKind)}

        -   #### readSkylarkAST

            ``` methodSignature
            protected com.google.devtools.build.lib.syntax.BuildFileAST readSkylarkAST​(com.google.devtools.build.lib.vfs.Path path,
                                                                                       FileKind fileKind)
                                                                                throws IOException
            ```

            ::: block
            Reads file and returns abstract syntax tree for that file.
            :::

            [Parameters:]{.paramLabel}
            :   `path` - file path to read the data from.

            [Returns:]{.returnLabel}
            :   abstract syntax tree; does not handle any errors.

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#loadExtensions(com.google.devtools.build.lib.cmdline.Label,com.google.common.collect.ImmutableList)}

        -   #### loadExtensions

            ``` methodSignature
            protected com.google.common.collect.ImmutableList<com.facebook.buck.skylark.parser.ExtensionData> loadExtensions​(com.google.devtools.build.lib.cmdline.Label containingLabel,
                                                                                                                             com.google.common.collect.ImmutableList<com.google.devtools.build.lib.syntax.SkylarkImport> skylarkImports)
                                                                                                                      throws BuildFileParseException,
                                                                                                                             IOException,
                                                                                                                             InterruptedException
            ```

            ::: block
            Loads all extensions identified by corresponding
            `SkylarkImport`s.
            :::

            [Throws:]{.throwsLabel}
            :   `BuildFileParseException`
            :   `IOException`
            :   `InterruptedException`

        []{#buildExtensionData(com.facebook.buck.skylark.parser.AbstractSkylarkFileParser.ExtensionLoadState)}

        -   #### buildExtensionData

            ``` methodSignature
            protected com.facebook.buck.skylark.parser.ExtensionData buildExtensionData​(com.facebook.buck.skylark.parser.AbstractSkylarkFileParser.ExtensionLoadState load)
                                                                                 throws InterruptedException
            ```

            ::: block
            Given fully loaded extension represented by
            `AbstractSkylarkFileParser.ExtensionLoadState`, evaluates
            extension and returns `ExtensionData`
            :::

            [Parameters:]{.paramLabel}
            :   `load` - `AbstractSkylarkFileParser.ExtensionLoadState`
                representing loaded extension

            [Throws:]{.throwsLabel}
            :   `InterruptedException`

        []{#getIncludedFiles(java.nio.file.Path)}

        -   #### getIncludedFiles

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedSet<String> getIncludedFiles​(Path parseFile)
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
                interface `FileParser<T extends FileManifest>`

            [Parameters:]{.paramLabel}
            :   `parseFile` - should be an absolute path to a file. Must
                have rootPath as its prefix.

            [Throws:]{.throwsLabel}
            :   `BuildFileParseException`
            :   `InterruptedException`
            :   `IOException`

        []{#close()}

        -   #### close

            ``` methodSignature
            public void close()
                       throws BuildFileParseException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `close` in interface `AutoCloseable`

            [Specified by:]{.overrideSpecifyLabel}
            :   `close` in
                interface `FileParser<T extends FileManifest>`

            [Throws:]{.throwsLabel}
            :   `BuildFileParseException`
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
