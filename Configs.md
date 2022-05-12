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
[Package]{.packageLabelInType} [com.facebook.buck.util.config](package-summary.html)
:::

## Class Configs {#class-configs .title title="Class Configs"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.util.config.Configs

::: description
-   

    ------------------------------------------------------------------------

        public final class Configs
        extends Object

    ::: block
    Utility functions for working with
    [`Config`](Config.html "class in com.facebook.buck.util.config")s.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type   Field                                      Description
          ------------------- ------------------------------------------ -------------
          `static String`     `DEFAULT_BUCK_CONFIG_OVERRIDE_FILE_NAME`    

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static Config`       | `createCo             | ::: block             |
        |                       | nfigFromFiles​(Path ro | Generates a config by |
        |                       | ot,                   | merging configs from  |
        |                       |     com.google.common | specified locations   |
        |                       | .collect.ImmutableLis | on disk in order of   |
        |                       | t<Path> configFiles)` | the list supplied.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static Config`       | `createDefa           | ::: block             |
        |                       | ultConfig​(Path root)` | Convienence           |
        |                       |                       | constructor           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static Config`       | `createDefaultC       | ::: block             |
        |                       | onfig​(Path root,      | Generates a Buck      |
        |                       |                RawCon | config by merging     |
        |                       | fig configOverrides)` | configs from          |
        |                       |                       | specified locations   |
        |                       |                       | on disk.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static Config`       | `createDe             | ::: block             |
        |                       | faultConfig​(Path root | Generates a config by |
        |                       | ,                     | merging configs from  |
        |                       | com.google.common.col | specified locations   |
        |                       | lect.ImmutableList<Pa | on disk in order of   |
        |                       | th> configFiles,      | the list supplied.    |
        |                       |                RawCon | :::                   |
        |                       | fig configOverrides)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static com.          | `g                    | ::: block             |
        | google.common.collect | etDefaultConfiguratio | Abs-path version of   |
        | .ImmutableList<Path>` | nFiles​(AbsPath root)` | [`getD                |
        |                       |                       | efaultConfigurationFi |
        |                       |                       | les(Path)`](#getDefau |
        |                       |                       | ltConfigurationFiles( |
        |                       |                       | java.nio.file.Path)). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static com.          | `getDefaultConfigura  | ::: block             |
        | google.common.collect | tionFiles​(Path root)` | Gets all              |
        | .ImmutableList<Path>` |                       | configuration files   |
        |                       |                       | that should be used   |
        |                       |                       | for parsing the       |
        |                       |                       | project configuration |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static Path`         | `getMainConfigur      |                       |
        |                       | ationFile​(Path root)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static com.          | `getRepoConfigura     | ::: block             |
        | google.common.collect | tionFiles​(Path root)` | Gets the repository   |
        | .ImmutableList<Path>` |                       | defined configuration |
        |                       |                       | files (excluding      |
        |                       |                       | configuration         |
        |                       |                       | directories) that     |
        |                       |                       | should be used for    |
        |                       |                       | parsing the project   |
        |                       |                       | configuration.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `sta                  | `parseC               |                       |
        | tic com.google.common | onfigFile​(Path file)` |                       |
        | .collect.ImmutableMap |                       |                       |
        | <String,​com.google.co |                       |                       |
        | mmon.collect.Immutabl |                       |                       |
        | eMap<String,​String>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
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

        []{#DEFAULT_BUCK_CONFIG_OVERRIDE_FILE_NAME}

        -   #### DEFAULT_BUCK_CONFIG_OVERRIDE_FILE_NAME

                public static final String DEFAULT_BUCK_CONFIG_OVERRIDE_FILE_NAME

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.util.config.Configs.DEFAULT_BUCK_CONFIG_OVERRIDE_FILE_NAME)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#createDefaultConfig(java.nio.file.Path)}

        -   #### createDefaultConfig

            ``` methodSignature
            public static Config createDefaultConfig​(Path root)
                                              throws IOException
            ```

            ::: block
            Convienence constructor
            :::

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#createDefaultConfig(java.nio.file.Path,com.facebook.buck.util.config.RawConfig)}

        -   #### createDefaultConfig

            ``` methodSignature
            public static Config createDefaultConfig​(Path root,
                                                     RawConfig configOverrides)
                                              throws IOException
            ```

            ::: block
            Generates a Buck config by merging configs from specified
            locations on disk.
            In order:

            1.  Files (in lexicographical order) in `/etc/buckconfig.d`
            2.  `/etc/buckconfig`
            3.  Files (in lexicographical order) in
                `<HOME>/buckconfig.d`
            4.  Files (in lexicographical order) in
                `<PROJECT ROOT >/buckconfig.d`
            5.  `<HOME>/.buckconfig`
            6.  `<PROJECT ROOT>/.buckconfig`
            7.  `<PROJECT ROOT>/.buckconfig.local`
            8.  Any overrides (usually from the command line)
            :::

            [Parameters:]{.paramLabel}
            :   `root` - Project root.
            :   `configOverrides` - Config overrides to merge in after
                the other sources.

            [Returns:]{.returnLabel}
            :   the resulting `Config`.

            [Throws:]{.throwsLabel}
            :   `IOException` - on any exceptions during the underlying
                filesystem operations.

        []{#createDefaultConfig(java.nio.file.Path,com.google.common.collect.ImmutableList,com.facebook.buck.util.config.RawConfig)}

        -   #### createDefaultConfig

            ``` methodSignature
            public static Config createDefaultConfig​(Path root,
                                                     com.google.common.collect.ImmutableList<Path> configFiles,
                                                     RawConfig configOverrides)
                                              throws IOException
            ```

            ::: block
            Generates a config by merging configs from specified
            locations on disk in order of the list supplied. The
            elements at the end of the list have higher precedence.
            :::

            [Parameters:]{.paramLabel}
            :   `root` - Project root.
            :   `configFiles` - the files to load configs from, in order
                of precedence.
            :   `configOverrides` - Config overrides to merge in after
                the other sources.

            [Returns:]{.returnLabel}
            :   the resulting `Config`.

            [Throws:]{.throwsLabel}
            :   `IOException` - on any exceptions during the underlying
                filesystem operations.

        []{#createConfigFromFiles(java.nio.file.Path,com.google.common.collect.ImmutableList)}

        -   #### createConfigFromFiles

            ``` methodSignature
            public static Config createConfigFromFiles​(Path root,
                                                       com.google.common.collect.ImmutableList<Path> configFiles)
                                                throws IOException
            ```

            ::: block
            Generates a config by merging configs from specified
            locations on disk in order of the list supplied. The
            elements at the end of the list have higher precedence.
            :::

            [Parameters:]{.paramLabel}
            :   `root` - Project root.
            :   `configFiles` - the files to load configs from, in order
                of precedence.

            [Returns:]{.returnLabel}
            :   the resulting `RawConfig`.

            [Throws:]{.throwsLabel}
            :   `IOException` - on any exceptions during the underlying
                filesystem operations.

        []{#getMainConfigurationFile(java.nio.file.Path)}

        -   #### getMainConfigurationFile

            ``` methodSignature
            public static Path getMainConfigurationFile​(Path root)
            ```

        []{#getDefaultConfigurationFiles(java.nio.file.Path)}

        -   #### getDefaultConfigurationFiles

            ``` methodSignature
            public static com.google.common.collect.ImmutableList<Path> getDefaultConfigurationFiles​(Path root)
                                                                                              throws IOException
            ```

            ::: block
            Gets all configuration files that should be used for parsing
            the project configuration
            :::

            [Parameters:]{.paramLabel}
            :   `root` - The root of the project to search

            [Returns:]{.returnLabel}
            :   Files that exist that conform to buck\'s configuration
                file precedence. Settings from files at the end of this
                list should override ones that come before.

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#getDefaultConfigurationFiles(com.facebook.buck.core.filesystems.AbsPath)}

        -   #### getDefaultConfigurationFiles

            ``` methodSignature
            public static com.google.common.collect.ImmutableList<Path> getDefaultConfigurationFiles​(AbsPath root)
                                                                                              throws IOException
            ```

            ::: block
            Abs-path version of
            [`getDefaultConfigurationFiles(Path)`](#getDefaultConfigurationFiles(java.nio.file.Path)).
            :::

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#getRepoConfigurationFiles(java.nio.file.Path)}

        -   #### getRepoConfigurationFiles

            ``` methodSignature
            public static com.google.common.collect.ImmutableList<Path> getRepoConfigurationFiles​(Path root)
            ```

            ::: block
            Gets the repository defined configuration files (excluding
            configuration directories) that should be used for parsing
            the project configuration.
            :::

            [Parameters:]{.paramLabel}
            :   `root` - The root of the project to search

            [Returns:]{.returnLabel}
            :   Files that exist that conform to buck\'s configuration
                file precedence. Settings from files at the end of this
                list should override ones that come before.

        []{#parseConfigFile(java.nio.file.Path)}

        -   #### parseConfigFile

            ``` methodSignature
            public static com.google.common.collect.ImmutableMap<String,​com.google.common.collect.ImmutableMap<String,​String>> parseConfigFile​(Path file)
                                                                                                                                                    throws IOException
            ```

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
