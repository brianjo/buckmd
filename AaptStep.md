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
[Package]{.packageLabelInType} [com.facebook.buck.android](package-summary.html)
:::

## Class AaptStep {#class-aaptstep .title title="Class AaptStep"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.shell.ShellStep](../shell/ShellStep.html "class in com.facebook.buck.shell")

    -   -   com.facebook.buck.android.AaptStep

::: description
-   

    All Implemented Interfaces:
    :   `Step`

    ------------------------------------------------------------------------

        public class AaptStep
        extends ShellStep

    ::: block
    Runs the Android Asset Packaging Tool (`aapt`), which creates an
    `.apk` file. Frequently, the `pathsToRawFilesDirs` excludes
    `classes.dex`, as `classes.dex` will be added separately to the
    final APK via `ApkBuilder`.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type   Field                     Description
          ------------------- ------------------------- -------------
          `static String`     `IGNORE_ASSETS_PATTERN`    

          : Fields[ ]{.tabEnd}

        -   []{#fields.inherited.from.class.com.facebook.buck.shell.ShellStep}

            ### Fields inherited from class com.facebook.buck.shell.[ShellStep](../shell/ShellStep.html "class in com.facebook.buck.shell")

            `workingDirectory`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     Description
          ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `AaptStep​(SourcePathResolverAdapter pathResolver,         AndroidPlatformTarget androidPlatformTarget,         AbsPath workingDirectory,         Path androidManifest,         com.google.common.collect.ImmutableList<Path> resDirectories,         com.google.common.collect.ImmutableSortedSet<Path> assetsDirectories,         Path pathToOutputApkFile,         Path pathToRDotTxtDir,         Path pathToGeneratedProguardConfig,         com.google.common.collect.ImmutableList<Path> pathToDependecyResourceApks,         boolean isCrunchPngFiles,         boolean includesVectorDrawables,         ManifestEntries manifestEntries,         com.google.common.collect.ImmutableList<String> additionalAaptParams)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `protected com.go     | `getShell             | ::: block             |
        | ogle.common.collect.I | CommandInternal​(Execu | Implementations of    |
        | mmutableList<String>` | tionContext context)` | this method should    |
        |                       |                       | not have any          |
        |                       |                       | observable            |
        |                       |                       | side-effects.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getShortName()`      |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static boolean`      | `isSilent             | ::: block             |
        |                       | lyIgnored​(Path path)` | Determines whether    |
        |                       |                       | the default AAPT      |
        |                       |                       | ignore pattern in     |
        |                       |                       | [`                    |
        |                       |                       | DEFAULT_IGNORE_ASSETS |
        |                       |                       | _PATTERN`](#DEFAULT_I |
        |                       |                       | GNORE_ASSETS_PATTERN) |
        |                       |                       | would silently ignore |
        |                       |                       | a file.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.shell.ShellStep}

            ### Methods inherited from class com.facebook.buck.shell.[ShellStep](../shell/ShellStep.html "class in com.facebook.buck.shell")

            `addOptions, execute, getDescription, getDuration, getEnvironmentVariables, getExitCodeFromResult, getShellCommand, getShellCommandArgsForDescription, getStderr, getStdin, getStdout, getTimeout, getTimeoutHandler, shouldPrintStderr, shouldPrintStdout`

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
    -   []{#field.detail}

        ### Field Detail

        []{#IGNORE_ASSETS_PATTERN}

        -   #### IGNORE_ASSETS_PATTERN

                public static final String IGNORE_ASSETS_PATTERN

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../constant-values.html#com.facebook.buck.android.AaptStep.IGNORE_ASSETS_PATTERN)
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter,com.facebook.buck.android.toolchain.AndroidPlatformTarget,com.facebook.buck.core.filesystems.AbsPath,java.nio.file.Path,com.google.common.collect.ImmutableList,com.google.common.collect.ImmutableSortedSet,java.nio.file.Path,java.nio.file.Path,java.nio.file.Path,com.google.common.collect.ImmutableList,boolean,boolean,com.facebook.buck.rules.coercer.ManifestEntries,com.google.common.collect.ImmutableList)}

        -   #### AaptStep

                public AaptStep​(SourcePathResolverAdapter pathResolver,
                                AndroidPlatformTarget androidPlatformTarget,
                                AbsPath workingDirectory,
                                Path androidManifest,
                                com.google.common.collect.ImmutableList<Path> resDirectories,
                                com.google.common.collect.ImmutableSortedSet<Path> assetsDirectories,
                                Path pathToOutputApkFile,
                                Path pathToRDotTxtDir,
                                Path pathToGeneratedProguardConfig,
                                com.google.common.collect.ImmutableList<Path> pathToDependecyResourceApks,
                                boolean isCrunchPngFiles,
                                boolean includesVectorDrawables,
                                ManifestEntries manifestEntries,
                                com.google.common.collect.ImmutableList<String> additionalAaptParams)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#isSilentlyIgnored(java.nio.file.Path)}

        -   #### isSilentlyIgnored

            ``` methodSignature
            public static boolean isSilentlyIgnored​(Path path)
            ```

            ::: block
            Determines whether the default AAPT ignore pattern in
            [`DEFAULT_IGNORE_ASSETS_PATTERN`](#DEFAULT_IGNORE_ASSETS_PATTERN)
            would silently ignore a file.
            :::

            [Parameters:]{.paramLabel}
            :   `path` - The path of the file we are interested in.

            [Returns:]{.returnLabel}
            :   Whether the file would be silently ignored.

        []{#getShellCommandInternal(com.facebook.buck.core.build.execution.context.ExecutionContext)}

        -   #### getShellCommandInternal

            ``` methodSignature
            protected com.google.common.collect.ImmutableList<String> getShellCommandInternal​(ExecutionContext context)
            ```

            ::: block
            [Description copied from
            class: `ShellStep`]{.descfrmTypeLabel}
            :::

            ::: block
            Implementations of this method should not have any
            observable side-effects.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getShellCommandInternal` in class `ShellStep`

        []{#getShortName()}

        -   #### getShortName

            ``` methodSignature
            public String getShortName()
            ```

            [Returns:]{.returnLabel}
            :   a short name/description for the command, such as
                \"javac\". Should fit on one line.
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