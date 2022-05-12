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
[Package]{.packageLabelInType} [com.facebook.buck.android.exopackage](package-summary.html)
:::

## Class ExopackageInstaller {#class-exopackageinstaller .title title="Class ExopackageInstaller"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.android.exopackage.ExopackageInstaller

::: description
-   

    ------------------------------------------------------------------------

        public class ExopackageInstaller
        extends Object

    ::: block
    ExopackageInstaller manages the installation of apps with the
    \"exopackage\" flag set to true.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type   Field                       Description
          ------------------- --------------------------- -------------
          `static Path`       `EXOPACKAGE_INSTALL_ROOT`    
          `static String`     `NATIVE_LIBRARY_TYPE`        
          `static String`     `RESOURCES_TYPE`             
          `static String`     `SECONDARY_DEX_TYPE`         

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                          Description
          ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `ExopackageInstaller​(SourcePathResolverAdapter pathResolver,                    ExecutionContext context,                    ProjectFilesystem projectFilesystem,                    String packageName,                    AndroidDevice device)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `boolean`             | `doInstall​(H          |                       |
        |                       | asInstallableApk.ApkI |                       |
        |                       | nfo apkInfo,          |                       |
        |                       |  String processName)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static boolean`      | `exopackageE          |                       |
        |                       | nabled​(HasInstallable |                       |
        |                       | Apk.ApkInfo apkInfo)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `finishExoFileI       |                       |
        |                       | nstallation​(com.googl |                       |
        |                       | e.common.collect.Immu |                       |
        |                       | tableSortedSet<Path>  |                       |
        |                       | presentFiles,         |                       |
        |                       |                   Exo |                       |
        |                       | packageInfo exoInfo)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `installApkIfNec      |                       |
        |                       | essary​(HasInstallable |                       |
        |                       | Apk.ApkInfo apkInfo)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `i                    |                       |
        |                       | nstallMissingExopacka |                       |
        |                       | geFiles​(com.google.co |                       |
        |                       | mmon.collect.Immutabl |                       |
        |                       | eSortedSet<Path> pres |                       |
        |                       | entFiles,             |                       |
        |                       |                   Exo |                       |
        |                       | packageInfo exoInfo)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `ins                  |                       |
        |                       | tallMissingFiles​(com. |                       |
        |                       | google.common.collect |                       |
        |                       | .ImmutableSortedSet<P |                       |
        |                       | ath> presentFiles,    |                       |
        |                       |                  com. |                       |
        |                       | google.common.collect |                       |
        |                       | .ImmutableMap<Path,​Pa |                       |
        |                       | th> wantedFilesToInst |                       |
        |                       | all,                  |                       |
        |                       |    String filesType)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `killApp              |                       |
        |                       | ​(HasInstallableApk.Ap |                       |
        |                       | kInfo apkInfo,        |                       |
        |                       |  String processName)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `s                    | `parseExo             | ::: block             |
        | tatic com.google.comm | packageInfoMetadata​(P | Parses a text file    |
        | on.collect.ImmutableM | ath metadataTxt,      | which is supposed to  |
        | ultimap<String,​Path>` |                       | be in the following   |
        |                       |   Path resolvePathAga | format:               |
        |                       | inst,                 | \"fil                 |
        |                       |             ProjectFi | e_path_without_spaces |
        |                       | lesystem filesystem)` | file_hash \....\"     |
        |                       |                       | i.e.                  |
        |                       |                       | :::                   |
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
    -   []{#field.detail}

        ### Field Detail

        []{#EXOPACKAGE_INSTALL_ROOT}

        -   #### EXOPACKAGE_INSTALL_ROOT

                public static final Path EXOPACKAGE_INSTALL_ROOT

        []{#SECONDARY_DEX_TYPE}

        -   #### SECONDARY_DEX_TYPE

                public static final String SECONDARY_DEX_TYPE

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.android.exopackage.ExopackageInstaller.SECONDARY_DEX_TYPE)

        []{#NATIVE_LIBRARY_TYPE}

        -   #### NATIVE_LIBRARY_TYPE

                public static final String NATIVE_LIBRARY_TYPE

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.android.exopackage.ExopackageInstaller.NATIVE_LIBRARY_TYPE)

        []{#RESOURCES_TYPE}

        -   #### RESOURCES_TYPE

                public static final String RESOURCES_TYPE

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.android.exopackage.ExopackageInstaller.RESOURCES_TYPE)
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter,com.facebook.buck.core.build.execution.context.ExecutionContext,com.facebook.buck.io.filesystem.ProjectFilesystem,java.lang.String,com.facebook.buck.android.exopackage.AndroidDevice)}

        -   #### ExopackageInstaller

                public ExopackageInstaller​(SourcePathResolverAdapter pathResolver,
                                           ExecutionContext context,
                                           ProjectFilesystem projectFilesystem,
                                           String packageName,
                                           AndroidDevice device)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#doInstall(com.facebook.buck.android.HasInstallableApk.ApkInfo,java.lang.String)}

        -   #### doInstall

            ``` methodSignature
            public boolean doInstall​(HasInstallableApk.ApkInfo apkInfo,
                                     @Nullable
                                     String processName)
                              throws Exception
            ```

            [Returns:]{.returnLabel}
            :   Returns true.

            [Throws:]{.throwsLabel}
            :   `Exception`

        []{#killApp(com.facebook.buck.android.HasInstallableApk.ApkInfo,java.lang.String)}

        -   #### killApp

            ``` methodSignature
            public void killApp​(HasInstallableApk.ApkInfo apkInfo,
                                @Nullable
                                String processName)
                         throws Exception
            ```

            [Throws:]{.throwsLabel}
            :   `Exception`

        []{#installApkIfNecessary(com.facebook.buck.android.HasInstallableApk.ApkInfo)}

        -   #### installApkIfNecessary

            ``` methodSignature
            public void installApkIfNecessary​(HasInstallableApk.ApkInfo apkInfo)
                                       throws Exception
            ```

            [Throws:]{.throwsLabel}
            :   `Exception`

        []{#finishExoFileInstallation(com.google.common.collect.ImmutableSortedSet,com.facebook.buck.android.exopackage.ExopackageInfo)}

        -   #### finishExoFileInstallation

            ``` methodSignature
            public void finishExoFileInstallation​(com.google.common.collect.ImmutableSortedSet<Path> presentFiles,
                                                  ExopackageInfo exoInfo)
                                           throws Exception
            ```

            [Throws:]{.throwsLabel}
            :   `Exception`

        []{#installMissingExopackageFiles(com.google.common.collect.ImmutableSortedSet,com.facebook.buck.android.exopackage.ExopackageInfo)}

        -   #### installMissingExopackageFiles

            ``` methodSignature
            public void installMissingExopackageFiles​(com.google.common.collect.ImmutableSortedSet<Path> presentFiles,
                                                      ExopackageInfo exoInfo)
                                               throws Exception
            ```

            [Throws:]{.throwsLabel}
            :   `Exception`

        []{#exopackageEnabled(com.facebook.buck.android.HasInstallableApk.ApkInfo)}

        -   #### exopackageEnabled

            ``` methodSignature
            public static boolean exopackageEnabled​(HasInstallableApk.ApkInfo apkInfo)
            ```

            [Parameters:]{.paramLabel}
            :   `apkInfo` - the apk info to examine for exopackage items

            [Returns:]{.returnLabel}
            :   true if the given apk info contains any items which need
                to be installed via exopackage

        []{#installMissingFiles(com.google.common.collect.ImmutableSortedSet,com.google.common.collect.ImmutableMap,java.lang.String)}

        -   #### installMissingFiles

            ``` methodSignature
            public void installMissingFiles​(com.google.common.collect.ImmutableSortedSet<Path> presentFiles,
                                            com.google.common.collect.ImmutableMap<Path,​Path> wantedFilesToInstall,
                                            String filesType)
                                     throws Exception
            ```

            [Throws:]{.throwsLabel}
            :   `Exception`

        []{#parseExopackageInfoMetadata(java.nio.file.Path,java.nio.file.Path,com.facebook.buck.io.filesystem.ProjectFilesystem)}

        -   #### parseExopackageInfoMetadata

            ``` methodSignature
            public static com.google.common.collect.ImmutableMultimap<String,​Path> parseExopackageInfoMetadata​(Path metadataTxt,
                                                                                                                     Path resolvePathAgainst,
                                                                                                                     ProjectFilesystem filesystem)
                                                                                                              throws IOException
            ```

            ::: block
            Parses a text file which is supposed to be in the following
            format: \"file_path_without_spaces file_hash \....\" i.e. it
            parses the first two columns of each line and ignores the
            rest of it.
            :::

            [Returns:]{.returnLabel}
            :   A multi map from the file hash to its path, which equals
                the raw path resolved against `resolvePathAgainst`.

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
