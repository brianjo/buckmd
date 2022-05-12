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
-   [Nested](#nested.class.summary) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.features.apple.projectV2](package-summary.html)
:::

## Class ProjectFileWriter {#class-projectfilewriter .title title="Class ProjectFileWriter"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.features.apple.projectV2.ProjectFileWriter

::: description
-   

    ------------------------------------------------------------------------

        public class ProjectFileWriter
        extends Object

    ::: block
    A class for writing files in SourcePath or Path objects to a
    PBXProject.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static class `       | `Proj                 | ::: block             |
        |                       | ectFileWriter.Result` | Helper class for      |
        |                       |                       | returning metadata    |
        |                       |                       | about a created       |
        |                       |                       | PBXFileReference      |
        |                       |                       | Includes a reference  |
        |                       |                       | to the                |
        |                       |                       | PBXFileReference and  |
        |                       |                       | the Source Tree Path  |
        |                       |                       | We probably won\'t    |
        |                       |                       | need this long term   |
        |                       |                       | as we kill off Xcode  |
        |                       |                       | build phases but for  |
        |                       |                       | now, let\'s just use  |
        |                       |                       | this since it\'s      |
        |                       |                       | named and structured  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                              Description
          ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ -------------
          `ProjectFileWriter​(PBXProject project,                  com.facebook.buck.features.apple.projectV2.PathRelativizer pathRelativizer,                  java.util.function.Function<SourcePath,​Path> sourcePathResolver)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `Proj                 | `writeFilePath​(Path   | ::: block             |
        | ectFileWriter.Result` | path,              Op | Writes a file at a    |
        |                       | tional<String> type)` | path to a             |
        |                       |                       | PBXFileReference in   |
        |                       |                       | the input project.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Proj                 | `writeSourcePath​(Sou  | ::: block             |
        | ectFileWriter.Result` | rcePath sourcePath,   | Writes a source path  |
        |                       |               Optiona | to a PBXFileReference |
        |                       | l<Path> packagePath)` | in the input project. |
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

        []{#<init>(com.facebook.buck.apple.xcode.xcodeproj.PBXProject,com.facebook.buck.features.apple.projectV2.PathRelativizer,java.util.function.Function)}

        -   #### ProjectFileWriter

                public ProjectFileWriter​(PBXProject project,
                                         com.facebook.buck.features.apple.projectV2.PathRelativizer pathRelativizer,
                                         java.util.function.Function<SourcePath,​Path> sourcePathResolver)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#writeSourcePath(com.facebook.buck.core.sourcepath.SourcePath,java.util.Optional)}

        -   #### writeSourcePath

            ``` methodSignature
            public ProjectFileWriter.Result writeSourcePath​(SourcePath sourcePath,
                                                            Optional<Path> packagePath)
            ```

            ::: block
            Writes a source path to a PBXFileReference in the input
            project. This will create the relative directory structure
            based on the path relativizer (cell root).
            Thus, if a file is absolutely located at:
            /Users/me/dev/MyProject/Header.h And the cell is:
            /Users/me/dev/ Then this will create a path in the
            PBXProject mainGroup as: /MyProject/Header.h
            :::

        []{#writeFilePath(java.nio.file.Path,java.util.Optional)}

        -   #### writeFilePath

            ``` methodSignature
            public ProjectFileWriter.Result writeFilePath​(Path path,
                                                          Optional<String> type)
            ```

            ::: block
            Writes a file at a path to a PBXFileReference in the input
            project.
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
-   [Nested](#nested.class.summary) \| 
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
