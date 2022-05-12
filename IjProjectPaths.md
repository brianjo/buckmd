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

-   [Overview](../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../deprecated-list.html)
-   [Index](../../../../../../index-all.html)
-   [Help](../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.features.project.intellij](package-summary.html)
:::

## Class IjProjectPaths {#class-ijprojectpaths .title title="Class IjProjectPaths"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.features.project.intellij.IjProjectPaths

::: description
-   

    ------------------------------------------------------------------------

        public class IjProjectPaths
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                               Description
          ----------------------------------------------------------------------------------------- -------------
          `IjProjectPaths​(String projectRoot,               boolean keepModuleFilesInModuleDirs)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static String`       | `getAndroidFacetRel   | ::: block             |
        |                       | ativePath​(Path path)` | Paths in Android      |
        |                       |                       | facet config marked   |
        |                       |                       | RELATIVE_PATH expect  |
        |                       |                       | / prefix              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Path`                | `getIdeaConfigDir()`  |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Path`                | `getLibrariesDir()`   |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Path`                | `getLibraryXmlFilePat |                       |
        |                       | h​(IjLibrary library)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Path`                | `getModule            |                       |
        |                       | Dir​(IjModule module)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Path`                | `getModuleImlFileP    |                       |
        |                       | ath​(IjModule module)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getModuleQ           |                       |
        |                       | ualifiedPath​(Path pat |                       |
        |                       | h,                    |                       |
        |                       |     IjModule module)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Path`                | `getModul             |                       |
        |                       | eRelativePath​(Path pa |                       |
        |                       | th,                   |                       |
        |                       |     IjModule module)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getProjectQual       |                       |
        |                       | ifiedPath​(Path path)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Path`                | `getProjectRel        |                       |
        |                       | ativePath​(Path path)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static String`       | `getUrl​(S             |                       |
        |                       | tring qualifiedPath)` |                       |
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
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(java.lang.String,boolean)}

        -   #### IjProjectPaths

                public IjProjectPaths​(String projectRoot,
                                      boolean keepModuleFilesInModuleDirs)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getIdeaConfigDir()}

        -   #### getIdeaConfigDir

            ``` methodSignature
            public Path getIdeaConfigDir()
            ```

        []{#getLibrariesDir()}

        -   #### getLibrariesDir

            ``` methodSignature
            public Path getLibrariesDir()
            ```

        []{#getModuleImlFilePath(com.facebook.buck.features.project.intellij.model.IjModule)}

        -   #### getModuleImlFilePath

            ``` methodSignature
            public Path getModuleImlFilePath​(IjModule module)
            ```

            [Returns:]{.returnLabel}
            :   path where the XML describing the module to IntelliJ
                will be written to.

        []{#getModuleDir(com.facebook.buck.features.project.intellij.model.IjModule)}

        -   #### getModuleDir

            ``` methodSignature
            public Path getModuleDir​(IjModule module)
            ```

            [Returns:]{.returnLabel}
            :   the directory containing the modules .iml file,
                \$MODULE_DIR\$ points to this.

        []{#getModuleQualifiedPath(java.nio.file.Path,com.facebook.buck.features.project.intellij.model.IjModule)}

        -   #### getModuleQualifiedPath

            ``` methodSignature
            public String getModuleQualifiedPath​(Path path,
                                                 IjModule module)
            ```

            [Returns:]{.returnLabel}
            :   path relative to module path, prefixed with
                \$MODULE_DIR\$

        []{#getModuleRelativePath(java.nio.file.Path,com.facebook.buck.features.project.intellij.model.IjModule)}

        -   #### getModuleRelativePath

            ``` methodSignature
            public Path getModuleRelativePath​(Path path,
                                              IjModule module)
            ```

            [Returns:]{.returnLabel}
            :   path relative to module dir, for a path relative to the
                project root

        []{#getLibraryXmlFilePath(com.facebook.buck.features.project.intellij.model.IjLibrary)}

        -   #### getLibraryXmlFilePath

            ``` methodSignature
            public Path getLibraryXmlFilePath​(IjLibrary library)
            ```

            [Returns:]{.returnLabel}
            :   path where the XML describing the IntelliJ library will
                be written to.

        []{#getProjectQualifiedPath(java.nio.file.Path)}

        -   #### getProjectQualifiedPath

            ``` methodSignature
            public String getProjectQualifiedPath​(Path path)
            ```

            [Returns:]{.returnLabel}
            :   path relative to project root, prefixed with
                \$PROJECT_DIR\$

        []{#getProjectRelativePath(java.nio.file.Path)}

        -   #### getProjectRelativePath

            ``` methodSignature
            public Path getProjectRelativePath​(Path path)
            ```

            [Returns:]{.returnLabel}
            :   path relative to project root

        []{#getUrl(java.lang.String)}

        -   #### getUrl

            ``` methodSignature
            public static String getUrl​(String qualifiedPath)
            ```

            [Returns:]{.returnLabel}
            :   url string for qualified path

        []{#getAndroidFacetRelativePath(java.nio.file.Path)}

        -   #### getAndroidFacetRelativePath

            ``` methodSignature
            public static String getAndroidFacetRelativePath​(Path path)
            ```

            ::: block
            Paths in Android facet config marked RELATIVE_PATH expect /
            prefix
            :::
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

-   [Overview](../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../deprecated-list.html)
-   [Index](../../../../../../index-all.html)
-   [Help](../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../allclasses.html)

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
