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
[Package]{.packageLabelInType} [com.facebook.buck.parser.config](package-summary.html)
:::

## Class ParserConfig {#class-parserconfig .title title="Class ParserConfig"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.parser.config.ParserConfig

::: description
-   

    All Implemented Interfaces:
    :   `ConfigView<BuckConfig>`

    ------------------------------------------------------------------------

        public abstract class ParserConfig
        extends Object
        implements ConfigView<BuckConfig>
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static class `       | `Parser               |                       |
        |                       | Config.AllowSymlinks` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static class `       | `ParserConfig.App     | ::: block             |
        |                       | lyDefaultFlavorsMode` | Controls whether      |
        |                       |                       | default flavors       |
        |                       |                       | should be applied to  |
        |                       |                       | unflavored targets.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static class `       | `ParserConfig.B       |                       |
        |                       | uildFileSearchMethod` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static class `       | `Pars                 |                       |
        |                       | erConfig.GlobHandler` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static class `       | `ParserConfig.Packag  | ::: block             |
        |                       | eBoundaryEnforcement` | How package boundary  |
        |                       |                       | violation should be   |
        |                       |                       | enforced              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static class `       | `ParserConfi          | ::: block             |
        |                       | g.SkylarkGlobHandler` | Glob handler          |
        |                       |                       | supported by Skylark  |
        |                       |                       | parser.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static class `       | `ParserConfig.Wat     |                       |
        |                       | chmanGlobSanityCheck` |                       |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type   Field                              Description
          ------------------- ---------------------------------- -------------
          `static String`     `BUILDFILE_SECTION_NAME`            
          `static boolean`    `DEFAULT_ALLOW_EMPTY_GLOBS`         
          `static String`     `DEFAULT_BUILD_FILE_NAME`           
          `static String`     `INCLUDES_PROPERTY_NAME`            
          `static String`     `PACKAGE_INCLUDES_PROPERTY_NAME`    

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor        Description
          ------------------ -------------
          `ParserConfig()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `AbsPath`             | `getAbsoluteP         |                       |
        |                       | athToBuildFile​(Cell c |                       |
        |                       | ell,                  |                       |
        |                       |           Unconfigure |                       |
        |                       | dBuildTarget target)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `AbsPath`             | `get                  | ::: block             |
        |                       | AbsolutePathToBuildFi | For use in            |
        |                       | leUnsafe​(Cell cell,   | performance-sensitive |
        |                       |                       | code or if you don\'t |
        |                       |           Unconfigure | care if the build     |
        |                       | dBuildTarget target)` | file actually exists, |
        |                       |                       | otherwise prefer      |
        |                       |                       | [`ge                  |
        |                       |                       | tAbsolutePathToBuildF |
        |                       |                       | ile(com.facebook.buck |
        |                       |                       | .core.cell.Cell, com. |
        |                       |                       | facebook.buck.core.mo |
        |                       |                       | del.UnconfiguredBuild |
        |                       |                       | Target)`](#getAbsolut |
        |                       |                       | ePathToBuildFile(com. |
        |                       |                       | facebook.buck.core.ce |
        |                       |                       | ll.Cell,com.facebook. |
        |                       |                       | buck.core.model.Uncon |
        |                       |                       | figuredBuildTarget)). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `                     |                       |
        |                       | getAllowEmptyGlobs()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Parser               | `getAllowSymlinks()`  |                       |
        | Config.AllowSymlinks` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.                 | `getBuckPackage       | ::: block             |
        | google.common.collect | BoundaryExceptions()` | A list of absolute    |
        | .ImmutableList<Path>` |                       | paths under which     |
        |                       |                       | buck package boundary |
        |                       |                       | checks should not be  |
        |                       |                       | performed.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.go               | `getBuildF            |                       |
        | ogle.common.collect.I | ileImportWhitelist()` |                       |
        | mmutableList<String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getBuildFileName()`  |                       |
        +-----------------------+-----------------------+-----------------------+
        | `ParserConfig.B       | `getBui               |                       |
        | uildFileSearchMethod` | ldFileSearchMethod()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Syntax`              | `getDefa              |                       |
        |                       | ultBuildFileSyntax()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `ParserConfig.App     | `get                  |                       |
        | lyDefaultFlavorsMode` | DefaultFlavorsMode()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Iterable<String>`    | `                     | ::: block             |
        |                       | getDefaultIncludes()` | A (possibly empty)    |
        |                       |                       | sequence of paths to  |
        |                       |                       | files that should be  |
        |                       |                       | included by default   |
        |                       |                       | when evaluating a     |
        |                       |                       | build file.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `abstract BuckConfig` | `getDelegate()`       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `get                  |                       |
        |                       | EnablePackageFiles()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `getEna               |                       |
        |                       | bleParallelParsing()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `getEnableTargetC     |                       |
        |                       | ompatibilityChecks()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `getEnforceB          |                       |
        |                       | uckPackageBoundary()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Pars                 | `getGlobHandler()`    |                       |
        | erConfig.GlobHandler` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `getHostPlatform()`   |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Impl                 | `getImplic            |                       |
        | icitNativeRulesState` | itNativeRulesState()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `g                    |                       |
        |                       | etLogPackageBoundaryE |                       |
        |                       | xceptionViolations()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `getMissingTargetL    |                       |
        |                       | evenshteinDistance()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `ge                   |                       |
        |                       | tNumParsingThreads()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `ParserConfig.Packag  | `getPa                | ::: block             |
        | eBoundaryEnforcement` | ckageBoundaryEnforcem | Whether the cell is   |
        |                       | entPolicy​(Path path)` | enforcing buck        |
        |                       |                       | package boundaries    |
        |                       |                       | for the package at    |
        |                       |                       | the passed path.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getPacka             |                       |
        | com.google.common.col | geImplicitIncludes()` |                       |
        | lect.ImmutableMap<Str |                       |                       |
        | ing,​ImplicitInclude>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `getParserPyt         |                       |
        |                       | honInterpreterPath()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `getPar               |                       |
        |                       | serTargetThreshold()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `getPyth              | ::: block             |
        |                       | onModuleSearchPath()` | Returns the module    |
        |                       |                       | search path           |
        |                       |                       | PYTHONPATH to set for |
        |                       |                       | the parser, as        |
        |                       |                       | specified by the      |
        |                       |                       | \'python_path\' key   |
        |                       |                       | of the \'parser\'     |
        |                       |                       | section.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<com.g       | `getReadOnlyPaths()`  |                       |
        | oogle.common.collect. |                       |                       |
        | ImmutableList<Path>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `getReq               | ::: block             |
        |                       | uireTargetPlatform()` | When set, requested   |
        |                       |                       | target node will fail |
        |                       |                       | to configure if       |
        |                       |                       | platform is not       |
        |                       |                       | specified either      |
        |                       |                       | per-target with       |
        |                       |                       | `def                  |
        |                       |                       | ault_target_platform` |
        |                       |                       | or globally with      |
        |                       |                       | `--target-platforms=` |
        |                       |                       | command line flag.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ParserConfi          | `get                  |                       |
        | g.SkylarkGlobHandler` | SkylarkGlobHandler()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getTargetPl          |                       |
        |                       | atformDetectorSpec()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `                     |                       |
        |                       | getTargetPlatforms()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `U                    | `getUse               |                       |
        | serDefinedRulesState` | rDefinedRulesState()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `getWatchCells()`     |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Watchm               | `getWatchmanCursor()` |                       |
        | anWatcher.CursorType` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `ParserConfig.Wat     | `getWatch             |                       |
        | chmanGlobSanityCheck` | manGlobSanityCheck()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Long>`      | `getWatc              |                       |
        |                       | hmanQueryTimeoutMs()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isPoly               |                       |
        |                       | glotParsingEnabled()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isWarnAbo            |                       |
        |                       | utDeprecatedSyntax()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static ParserConfig` | `of​(                  |                       |
        |                       | BuckConfig delegate)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
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

        []{#DEFAULT_ALLOW_EMPTY_GLOBS}

        -   #### DEFAULT_ALLOW_EMPTY_GLOBS

                public static final boolean DEFAULT_ALLOW_EMPTY_GLOBS

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.parser.config.ParserConfig.DEFAULT_ALLOW_EMPTY_GLOBS)

        []{#DEFAULT_BUILD_FILE_NAME}

        -   #### DEFAULT_BUILD_FILE_NAME

                public static final String DEFAULT_BUILD_FILE_NAME

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.parser.config.ParserConfig.DEFAULT_BUILD_FILE_NAME)

        []{#BUILDFILE_SECTION_NAME}

        -   #### BUILDFILE_SECTION_NAME

                public static final String BUILDFILE_SECTION_NAME

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.parser.config.ParserConfig.BUILDFILE_SECTION_NAME)

        []{#INCLUDES_PROPERTY_NAME}

        -   #### INCLUDES_PROPERTY_NAME

                public static final String INCLUDES_PROPERTY_NAME

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.parser.config.ParserConfig.INCLUDES_PROPERTY_NAME)

        []{#PACKAGE_INCLUDES_PROPERTY_NAME}

        -   #### PACKAGE_INCLUDES_PROPERTY_NAME

                public static final String PACKAGE_INCLUDES_PROPERTY_NAME

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.parser.config.ParserConfig.PACKAGE_INCLUDES_PROPERTY_NAME)
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### ParserConfig

                public ParserConfig()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getDelegate()}

        -   #### getDelegate

            ``` methodSignature
            public abstract BuckConfig getDelegate()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getDelegate` in interface `ConfigView<BuckConfig>`

        []{#of(com.facebook.buck.core.config.BuckConfig)}

        -   #### of

            ``` methodSignature
            public static ParserConfig of​(BuckConfig delegate)
            ```

        []{#getAllowEmptyGlobs()}

        -   #### getAllowEmptyGlobs

            ``` methodSignature
            @Lazy
            public boolean getAllowEmptyGlobs()
            ```

        []{#getBuildFileName()}

        -   #### getBuildFileName

            ``` methodSignature
            @Lazy
            public String getBuildFileName()
            ```

        []{#getDefaultIncludes()}

        -   #### getDefaultIncludes

            ``` methodSignature
            @Lazy
            public Iterable<String> getDefaultIncludes()
            ```

            ::: block
            A (possibly empty) sequence of paths to files that should be
            included by default when evaluating a build file.
            :::

        []{#getPackageImplicitIncludes()}

        -   #### getPackageImplicitIncludes

            ``` methodSignature
            @Lazy
            public com.google.common.collect.ImmutableMap<String,​ImplicitInclude> getPackageImplicitIncludes()
            ```

        []{#getEnforceBuckPackageBoundary()}

        -   #### getEnforceBuckPackageBoundary

            ``` methodSignature
            @Lazy
            public boolean getEnforceBuckPackageBoundary()
            ```

        []{#getBuckPackageBoundaryExceptions()}

        -   #### getBuckPackageBoundaryExceptions

            ``` methodSignature
            @Lazy
            public com.google.common.collect.ImmutableList<Path> getBuckPackageBoundaryExceptions()
            ```

            ::: block
            A list of absolute paths under which buck package boundary
            checks should not be performed.
            :::

        []{#getReadOnlyPaths()}

        -   #### getReadOnlyPaths

            ``` methodSignature
            @Lazy
            public Optional<com.google.common.collect.ImmutableList<Path>> getReadOnlyPaths()
            ```

        []{#getAllowSymlinks()}

        -   #### getAllowSymlinks

            ``` methodSignature
            @Lazy
            public ParserConfig.AllowSymlinks getAllowSymlinks()
            ```

        []{#getBuildFileSearchMethod()}

        -   #### getBuildFileSearchMethod

            ``` methodSignature
            @Lazy
            public ParserConfig.BuildFileSearchMethod getBuildFileSearchMethod()
            ```

        []{#getGlobHandler()}

        -   #### getGlobHandler

            ``` methodSignature
            @Lazy
            public ParserConfig.GlobHandler getGlobHandler()
            ```

        []{#getWatchmanGlobSanityCheck()}

        -   #### getWatchmanGlobSanityCheck

            ``` methodSignature
            @Lazy
            public ParserConfig.WatchmanGlobSanityCheck getWatchmanGlobSanityCheck()
            ```

        []{#getWatchmanQueryTimeoutMs()}

        -   #### getWatchmanQueryTimeoutMs

            ``` methodSignature
            @Lazy
            public Optional<Long> getWatchmanQueryTimeoutMs()
            ```

        []{#getWatchCells()}

        -   #### getWatchCells

            ``` methodSignature
            @Lazy
            public boolean getWatchCells()
            ```

        []{#getWatchmanCursor()}

        -   #### getWatchmanCursor

            ``` methodSignature
            @Lazy
            public WatchmanWatcher.CursorType getWatchmanCursor()
            ```

        []{#getEnableParallelParsing()}

        -   #### getEnableParallelParsing

            ``` methodSignature
            @Lazy
            public boolean getEnableParallelParsing()
            ```

        []{#getNumParsingThreads()}

        -   #### getNumParsingThreads

            ``` methodSignature
            @Lazy
            public int getNumParsingThreads()
            ```

        []{#getDefaultFlavorsMode()}

        -   #### getDefaultFlavorsMode

            ``` methodSignature
            @Lazy
            public ParserConfig.ApplyDefaultFlavorsMode getDefaultFlavorsMode()
            ```

        []{#getBuildFileImportWhitelist()}

        -   #### getBuildFileImportWhitelist

            ``` methodSignature
            @Lazy
            public com.google.common.collect.ImmutableList<String> getBuildFileImportWhitelist()
            ```

        []{#getParserPythonInterpreterPath()}

        -   #### getParserPythonInterpreterPath

            ``` methodSignature
            @Lazy
            public Optional<String> getParserPythonInterpreterPath()
            ```

        []{#getPythonModuleSearchPath()}

        -   #### getPythonModuleSearchPath

            ``` methodSignature
            @Lazy
            public Optional<String> getPythonModuleSearchPath()
            ```

            ::: block
            Returns the module search path PYTHONPATH to set for the
            parser, as specified by the \'python_path\' key of the
            \'parser\' section.
            :::

            [Returns:]{.returnLabel}
            :   The PYTHONPATH value or an empty string if not set.

        []{#isPolyglotParsingEnabled()}

        -   #### isPolyglotParsingEnabled

            ``` methodSignature
            @Lazy
            public boolean isPolyglotParsingEnabled()
            ```

            [Returns:]{.returnLabel}

            :   boolean flag indicating whether support for parsing
                build files using non default syntax (currently Python
                DSL).

                For a list of supported syntax see
                [`Syntax`](../api/Syntax.html "enum in com.facebook.buck.parser.api").

        []{#getDefaultBuildFileSyntax()}

        -   #### getDefaultBuildFileSyntax

            ``` methodSignature
            @Lazy
            public Syntax getDefaultBuildFileSyntax()
            ```

            [Returns:]{.returnLabel}

            :   a syntax to assume for build files without explicit
                build file syntax marker. \*

                For a list of supported syntax see
                [`Syntax`](../api/Syntax.html "enum in com.facebook.buck.parser.api").

        []{#getImplicitNativeRulesState()}

        -   #### getImplicitNativeRulesState

            ``` methodSignature
            @Lazy
            public ImplicitNativeRulesState getImplicitNativeRulesState()
            ```

            [Returns:]{.returnLabel}
            :   whether native build rules are available for users in
                build files. If not, they are only accessible in
                extension files under the \'native\' object

        []{#isWarnAboutDeprecatedSyntax()}

        -   #### isWarnAboutDeprecatedSyntax

            ``` methodSignature
            @Lazy
            public boolean isWarnAboutDeprecatedSyntax()
            ```

            [Returns:]{.returnLabel}
            :   whether Buck should warn about deprecated syntax.

        []{#getSkylarkGlobHandler()}

        -   #### getSkylarkGlobHandler

            ``` methodSignature
            @Lazy
            public ParserConfig.SkylarkGlobHandler getSkylarkGlobHandler()
            ```

            [Returns:]{.returnLabel}
            :   the type of the glob handler used by the Skylark parser.

        []{#getParserTargetThreshold()}

        -   #### getParserTargetThreshold

            ``` methodSignature
            @Lazy
            public int getParserTargetThreshold()
            ```

            [Returns:]{.returnLabel}
            :   the parser target threshold. When the current targets
                produced exceed this value, a warning is emitted.

        []{#getEnableTargetCompatibilityChecks()}

        -   #### getEnableTargetCompatibilityChecks

            ``` methodSignature
            @Lazy
            public boolean getEnableTargetCompatibilityChecks()
            ```

        []{#getRequireTargetPlatform()}

        -   #### getRequireTargetPlatform

            ``` methodSignature
            @Lazy
            public boolean getRequireTargetPlatform()
            ```

            ::: block
            When set, requested target node will fail to configure if
            platform is not specified either per-target with
            `default_target_platform` or globally with
            `--target-platforms=` command line flag.
            :::

        []{#getTargetPlatformDetectorSpec()}

        -   #### getTargetPlatformDetectorSpec

            ``` methodSignature
            @Lazy
            public String getTargetPlatformDetectorSpec()
            ```

        []{#getTargetPlatforms()}

        -   #### getTargetPlatforms

            ``` methodSignature
            @Lazy
            public Optional<String> getTargetPlatforms()
            ```

            [Returns:]{.returnLabel}
            :   a target that points to a `platform` rule that describes
                the target platforms. This is used when command-line
                argument is unspecified. Please do not use this option.

        []{#getHostPlatform()}

        -   #### getHostPlatform

            ``` methodSignature
            @Lazy
            public Optional<String> getHostPlatform()
            ```

            [Returns:]{.returnLabel}
            :   a target that points to a `platform` rule that describes
                the host platforms. This is used when command-line
                argument is unspecified. Please do not use this option.

        []{#getAbsolutePathToBuildFileUnsafe(com.facebook.buck.core.cell.Cell,com.facebook.buck.core.model.UnconfiguredBuildTarget)}

        -   #### getAbsolutePathToBuildFileUnsafe

            ``` methodSignature
            public AbsPath getAbsolutePathToBuildFileUnsafe​(Cell cell,
                                                            UnconfiguredBuildTarget target)
            ```

            ::: block
            For use in performance-sensitive code or if you don\'t care
            if the build file actually exists, otherwise prefer
            [`getAbsolutePathToBuildFile(com.facebook.buck.core.cell.Cell, com.facebook.buck.core.model.UnconfiguredBuildTarget)`](#getAbsolutePathToBuildFile(com.facebook.buck.core.cell.Cell,com.facebook.buck.core.model.UnconfiguredBuildTarget)).
            :::

            [Parameters:]{.paramLabel}
            :   `cell` - the cell where the given target is defined
            :   `target` - target to look up

            [Returns:]{.returnLabel}
            :   path which may or may not exist.

        []{#getAbsolutePathToBuildFile(com.facebook.buck.core.cell.Cell,com.facebook.buck.core.model.UnconfiguredBuildTarget)}

        -   #### getAbsolutePathToBuildFile

            ``` methodSignature
            public AbsPath getAbsolutePathToBuildFile​(Cell cell,
                                                      UnconfiguredBuildTarget target)
                                               throws MissingBuildFileException
            ```

            [Parameters:]{.paramLabel}
            :   `cell` - the cell where the given target is defined
            :   `target` - target to look up

            [Returns:]{.returnLabel}
            :   an absolute path to a build file that contains the
                definition of the given target.

            [Throws:]{.throwsLabel}
            :   `MissingBuildFileException`

        []{#getLogPackageBoundaryExceptionViolations()}

        -   #### getLogPackageBoundaryExceptionViolations

            ``` methodSignature
            @Lazy
            public boolean getLogPackageBoundaryExceptionViolations()
            ```

        []{#getPackageBoundaryEnforcementPolicy(java.nio.file.Path)}

        -   #### getPackageBoundaryEnforcementPolicy

            ``` methodSignature
            public ParserConfig.PackageBoundaryEnforcement getPackageBoundaryEnforcementPolicy​(Path path)
            ```

            ::: block
            Whether the cell is enforcing buck package boundaries for
            the package at the passed path.
            :::

            [Parameters:]{.paramLabel}
            :   `path` - Path of package (or file in a package) relative
                to the cell root.

            [Returns:]{.returnLabel}
            :   How to enforce buck package boundaries for `path`

        []{#getUserDefinedRulesState()}

        -   #### getUserDefinedRulesState

            ``` methodSignature
            @Lazy
            public UserDefinedRulesState getUserDefinedRulesState()
            ```

            [Returns:]{.returnLabel}
            :   whether to enable user-defined rule in .bzl files and
                export various symbols (such as rule()) into the
                evaluation context. This is disabled if
                [`RuleAnalysisComputation`](../../core/rules/analysis/impl/RuleAnalysisComputation.html "class in com.facebook.buck.core.rules.analysis.impl")
                is also disabled. This is in progress work, and
                experimental at this time.

        []{#getEnablePackageFiles()}

        -   #### getEnablePackageFiles

            ``` methodSignature
            @Lazy
            public boolean getEnablePackageFiles()
            ```

            [Returns:]{.returnLabel}
            :   Whether to enable parsing of PACKAGE files and apply
                their attributes to nodes.

        []{#getMissingTargetLevenshteinDistance()}

        -   #### getMissingTargetLevenshteinDistance

            ``` methodSignature
            @Lazy
            public int getMissingTargetLevenshteinDistance()
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
