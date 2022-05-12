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
[Package]{.packageLabelInType} [com.facebook.buck.io.filesystem](package-summary.html)
:::

## Class BuckPaths {#class-buckpaths .title title="Class BuckPaths"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.io.filesystem.BuckPaths

::: description
-   

    ------------------------------------------------------------------------

        public abstract class BuckPaths
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Field                 | Description           |
        +=======================+=======================+=======================+
        | `static boolean`      | `DE                   | ::: block             |
        |                       | FAULT_BUCK_OUT_INCLUD | Default value for     |
        |                       | E_TARGET_CONFIG_HASH` | [`shou                |
        |                       |                       | ldIncludeTargetConfig |
        |                       |                       | Hash()`](#shouldInclu |
        |                       |                       | deTargetConfigHash()) |
        |                       |                       | when it is not        |
        |                       |                       | specified by user.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor     Description
          --------------- -------------
          `BuckPaths()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `protected void`      | `checkBuckOut()`      |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static BuckPaths`    | `cre                  |                       |
        |                       | ateDefaultBuckPaths​(C |                       |
        |                       | anonicalCellName cell |                       |
        |                       | Name,                 |                       |
        |                       |        Path rootPath, |                       |
        |                       |                       |                       |
        |                       |   boolean buckOutIncl |                       |
        |                       | udeTargetConfigHash)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Path`                | `getAnnotationDir()`  |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract Path`       | `getBuckOut()`        | ::: block             |
        |                       |                       | The relative path to  |
        |                       |                       | the directory where   |
        |                       |                       | Buck will generate    |
        |                       |                       | its files.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static boolean`      | `getB                 | ::: block             |
        |                       | uckOutIncludeTargetCo | Is hashed buck-out    |
        |                       | nfigHashFromRootCellC | enabled? Must be      |
        |                       | onfig​(Config config)` | queried using root    |
        |                       |                       | cell buckconfig.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Path`                | `getCacheDir()`       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstra               | `getCellName()`       |                       |
        | ct CanonicalCellName` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract Path`       | `ge                   | ::: block             |
        |                       | tConfiguredBuckOut()` | The relative path to  |
        |                       |                       | the directory where   |
        |                       |                       | Buck will generate    |
        |                       |                       | its files.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Path`                | `get                  | ::: block             |
        |                       | CurrentVersionFile()` | The version the buck  |
        |                       |                       | output directory was  |
        |                       |                       | created for           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Path`                | `getEmbeddedC         |                       |
        |                       | ellsBuckOutBaseDir()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Path`                | `getGenDir()`         |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Path`                | `getJournalDir()`     |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Path`                | `getLastOutputDir()`  |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Path`                | `getLogDir()`         |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Path`                | `getOfflineLogDir()`  |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Path`                | `getProjectRootDir()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Path`                | `g                    |                       |
        |                       | etRemoteSandboxDir()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Path`                | `getResDir()`         |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Path`                | `getScratchDir()`     |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Path`                | `getSymlink           |                       |
        |                       | PathForDir​(Path uncon |                       |
        |                       | figuredDirInBuckOut)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Path`                | `getTmpDir()`         |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Path`                | `getTraceDir()`       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Path`                | `getTrashDir()`       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Path`                | `getXcodeDir()`       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static BuckPaths`    | `of​(Canoni            |                       |
        |                       | calCellName cellName, |                       |
        |                       |    Path buckOut,   Pa |                       |
        |                       | th configuredBuckOut, |                       |
        |                       |    boolean shouldIncl |                       |
        |                       | udeTargetConfigHash)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract boolean`    | `shouldInclu          | ::: block             |
        |                       | deTargetConfigHash()` | Whether to include    |
        |                       |                       | the target            |
        |                       |                       | configuration hash on |
        |                       |                       | buck-out.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `BuckPaths`           | `withB                |                       |
        |                       | uckOut​(Path buckOut)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `BuckPaths`           | `with                 |                       |
        |                       | ConfiguredBuckOut​(Pat |                       |
        |                       | h configuredBuckOut)` |                       |
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

        []{#DEFAULT_BUCK_OUT_INCLUDE_TARGET_CONFIG_HASH}

        -   #### DEFAULT_BUCK_OUT_INCLUDE_TARGET_CONFIG_HASH

                public static final boolean DEFAULT_BUCK_OUT_INCLUDE_TARGET_CONFIG_HASH

            ::: block
            Default value for
            [`shouldIncludeTargetConfigHash()`](#shouldIncludeTargetConfigHash())
            when it is not specified by user.
            :::

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.io.filesystem.BuckPaths.DEFAULT_BUCK_OUT_INCLUDE_TARGET_CONFIG_HASH)
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### BuckPaths

                public BuckPaths()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#createDefaultBuckPaths(com.facebook.buck.core.cell.name.CanonicalCellName,java.nio.file.Path,boolean)}

        -   #### createDefaultBuckPaths

            ``` methodSignature
            public static BuckPaths createDefaultBuckPaths​(CanonicalCellName cellName,
                                                           Path rootPath,
                                                           boolean buckOutIncludeTargetConfigHash)
            ```

        []{#getBuckOutIncludeTargetConfigHashFromRootCellConfig(com.facebook.buck.util.config.Config)}

        -   #### getBuckOutIncludeTargetConfigHashFromRootCellConfig

            ``` methodSignature
            public static boolean getBuckOutIncludeTargetConfigHashFromRootCellConfig​(Config config)
            ```

            ::: block
            Is hashed buck-out enabled? Must be queried using root cell
            buckconfig.
            :::

        []{#getCellName()}

        -   #### getCellName

            ``` methodSignature
            public abstract CanonicalCellName getCellName()
            ```

        []{#getBuckOut()}

        -   #### getBuckOut

            ``` methodSignature
            public abstract Path getBuckOut()
            ```

            ::: block
            The relative path to the directory where Buck will generate
            its files.
            :::

        []{#checkBuckOut()}

        -   #### checkBuckOut

            ``` methodSignature
            @Check
            protected void checkBuckOut()
            ```

        []{#getConfiguredBuckOut()}

        -   #### getConfiguredBuckOut

            ``` methodSignature
            public abstract Path getConfiguredBuckOut()
            ```

            ::: block
            The relative path to the directory where Buck will generate
            its files. This is used when configuring the output
            directory to some used-defined value and is a stop-gap until
            we can support configuring all output paths. However, for
            now, only certain paths below will use this path.
            :::

        []{#shouldIncludeTargetConfigHash()}

        -   #### shouldIncludeTargetConfigHash

            ``` methodSignature
            public abstract boolean shouldIncludeTargetConfigHash()
            ```

            ::: block
            Whether to include the target configuration hash on
            buck-out.
            :::

        []{#getCurrentVersionFile()}

        -   #### getCurrentVersionFile

            ``` methodSignature
            @Derived
            public Path getCurrentVersionFile()
            ```

            ::: block
            The version the buck output directory was created for
            :::

        []{#getGenDir()}

        -   #### getGenDir

            ``` methodSignature
            @Derived
            public Path getGenDir()
            ```

        []{#getResDir()}

        -   #### getResDir

            ``` methodSignature
            @Derived
            public Path getResDir()
            ```

        []{#getScratchDir()}

        -   #### getScratchDir

            ``` methodSignature
            @Derived
            public Path getScratchDir()
            ```

        []{#getAnnotationDir()}

        -   #### getAnnotationDir

            ``` methodSignature
            @Derived
            public Path getAnnotationDir()
            ```

        []{#getLogDir()}

        -   #### getLogDir

            ``` methodSignature
            @Derived
            public Path getLogDir()
            ```

        []{#getJournalDir()}

        -   #### getJournalDir

            ``` methodSignature
            @Derived
            public Path getJournalDir()
            ```

        []{#getTraceDir()}

        -   #### getTraceDir

            ``` methodSignature
            @Derived
            public Path getTraceDir()
            ```

        []{#getCacheDir()}

        -   #### getCacheDir

            ``` methodSignature
            @Derived
            public Path getCacheDir()
            ```

        []{#getTmpDir()}

        -   #### getTmpDir

            ``` methodSignature
            @Derived
            public Path getTmpDir()
            ```

        []{#getXcodeDir()}

        -   #### getXcodeDir

            ``` methodSignature
            @Derived
            public Path getXcodeDir()
            ```

        []{#getTrashDir()}

        -   #### getTrashDir

            ``` methodSignature
            @Derived
            public Path getTrashDir()
            ```

        []{#getOfflineLogDir()}

        -   #### getOfflineLogDir

            ``` methodSignature
            @Derived
            public Path getOfflineLogDir()
            ```

        []{#getRemoteSandboxDir()}

        -   #### getRemoteSandboxDir

            ``` methodSignature
            @Derived
            public Path getRemoteSandboxDir()
            ```

        []{#getLastOutputDir()}

        -   #### getLastOutputDir

            ``` methodSignature
            @Derived
            public Path getLastOutputDir()
            ```

        []{#getEmbeddedCellsBuckOutBaseDir()}

        -   #### getEmbeddedCellsBuckOutBaseDir

            ``` methodSignature
            @Derived
            public Path getEmbeddedCellsBuckOutBaseDir()
            ```

        []{#getProjectRootDir()}

        -   #### getProjectRootDir

            ``` methodSignature
            @Derived
            public Path getProjectRootDir()
            ```

        []{#getSymlinkPathForDir(java.nio.file.Path)}

        -   #### getSymlinkPathForDir

            ``` methodSignature
            public Path getSymlinkPathForDir​(Path unconfiguredDirInBuckOut)
            ```

        []{#of(com.facebook.buck.core.cell.name.CanonicalCellName,java.nio.file.Path,java.nio.file.Path,boolean)}

        -   #### of

            ``` methodSignature
            public static BuckPaths of​(CanonicalCellName cellName,
                                       Path buckOut,
                                       Path configuredBuckOut,
                                       boolean shouldIncludeTargetConfigHash)
            ```

        []{#withConfiguredBuckOut(java.nio.file.Path)}

        -   #### withConfiguredBuckOut

            ``` methodSignature
            public BuckPaths withConfiguredBuckOut​(Path configuredBuckOut)
            ```

        []{#withBuckOut(java.nio.file.Path)}

        -   #### withBuckOut

            ``` methodSignature
            public BuckPaths withBuckOut​(Path buckOut)
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
