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
-   [Field](#field.detail) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.skylark.parser](package-summary.html)
:::

## Class SkylarkPackageFileParser {#class-skylarkpackagefileparser .title title="Class SkylarkPackageFileParser"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.skylark.parser.SkylarkPackageFileParser

::: description
-   

    All Implemented Interfaces:
    :   `FileParser<PackageFileManifest>`, `PackageFileParser`,
        `AutoCloseable`

    ------------------------------------------------------------------------

        public class SkylarkPackageFileParser
        extends Object
        implements PackageFileParser

    ::: block
    Parser for package files written using Skylark syntax.
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
        | `PackageFileManifest` | `getManife            | ::: block             |
        |                       | st​(Path packageFile)` | Collect all           |
        |                       |                       | information from a    |
        |                       |                       | particular, along     |
        |                       |                       | with metadata about   |
        |                       |                       | the information, for  |
        |                       |                       | example which other   |
        |                       |                       | files were also       |
        |                       |                       | parsed.               |
        |                       |                       | :::                   |
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
        | `static Skyl          | `using​(P              | ::: block             |
        | arkPackageFileParser` | rojectBuildFileParser | Create an instance of |
        |                       | Options options,      | Skylark package file  |
        |                       |  BuckEventBus buckEve | parser using provided |
        |                       | ntBus,      com.googl | options.              |
        |                       | e.devtools.build.lib. | :::                   |
        |                       | vfs.FileSystem fileSy |                       |
        |                       | stem,      BuckGlobal |                       |
        |                       | s buckGlobals,      c |                       |
        |                       | om.google.devtools.bu |                       |
        |                       | ild.lib.events.EventH |                       |
        |                       | andler eventHandler)` |                       |
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
    -   []{#method.detail}

        ### Method Detail

        []{#using(com.facebook.buck.parser.options.ProjectBuildFileParserOptions,com.facebook.buck.event.BuckEventBus,com.google.devtools.build.lib.vfs.FileSystem,com.facebook.buck.skylark.parser.BuckGlobals,com.google.devtools.build.lib.events.EventHandler)}

        -   #### using

            ``` methodSignature
            public static SkylarkPackageFileParser using​(ProjectBuildFileParserOptions options,
                                                         BuckEventBus buckEventBus,
                                                         com.google.devtools.build.lib.vfs.FileSystem fileSystem,
                                                         BuckGlobals buckGlobals,
                                                         com.google.devtools.build.lib.events.EventHandler eventHandler)
            ```

            ::: block
            Create an instance of Skylark package file parser using
            provided options.
            :::

        []{#getManifest(java.nio.file.Path)}

        -   #### getManifest

            ``` methodSignature
            public PackageFileManifest getManifest​(Path packageFile)
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
                interface `FileParser<PackageFileManifest>`

            [Parameters:]{.paramLabel}
            :   `packageFile` - should be an absolute path to a file.
                Must have rootPath as its prefix.

            [Throws:]{.throwsLabel}
            :   `BuildFileParseException`
            :   `InterruptedException`
            :   `IOException`

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
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
-   Constr \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
