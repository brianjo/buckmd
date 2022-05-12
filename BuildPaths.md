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
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.core.model.impl](package-summary.html)
:::

## Class BuildPaths {#class-buildpaths .title title="Class BuildPaths"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.model.impl.BuildPaths

::: description
-   

    ------------------------------------------------------------------------

        public class BuildPaths
        extends Object

    ::: block
    Utility class that generates the build output paths for
    [`BuildTarget`](../BuildTarget.html "class in com.facebook.buck.core.model")s
    in a systematic manner.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static Path`         | `getAnnotationDir​(Pro | ::: block             |
        |                       | jectFilesystem filesy | Return a path to a    |
        |                       | stem,                 | file in the           |
        |                       |  BuildTarget target)` | buck-out/annotation/  |
        |                       |                       | directory, formatted  |
        |                       |                       | with the target short |
        |                       |                       | name.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static               | `getBaseD             | ::: block             |
        |  ForwardRelativePath` | ir​(ProjectFilesystem  | Return a relative     |
        |                       | filesystem,           | path to a file taking |
        |                       |  BuildTarget target)` | into account the      |
        |                       |                       | `target`\'s package   |
        |                       |                       | path and formatting   |
        |                       |                       | with the short name.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static Path`         | `getGen               | ::: block             |
        |                       | Dir​(ProjectFilesystem | Return a relative     |
        |                       |  filesystem,          | path to a file in the |
        |                       |  BuildTarget target)` | buck-out/gen/         |
        |                       |                       | directory, formatted  |
        |                       |                       | with the target short |
        |                       |                       | name.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static Path`         | `getScratchDir​(       | ::: block             |
        |                       | ProjectFilesystem fil | Return a path to a    |
        |                       | esystem,              | file in the           |
        |                       |  BuildTarget target)` | buck-out/bin/         |
        |                       |                       | directory, formatted  |
        |                       |                       | with the target short |
        |                       |                       | name.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `s                    | `removeHashFrom​(Pat   | ::: block             |
        | tatic Optional<Path>` | h path,               | Removes the hash from |
        |                       |  BuildTarget target)` | the buck-out path.    |
        |                       |                       | :::                   |
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
    -   []{#method.detail}

        ### Method Detail

        []{#getScratchDir(com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.model.BuildTarget)}

        -   #### getScratchDir

            ``` methodSignature
            public static Path getScratchDir​(ProjectFilesystem filesystem,
                                             BuildTarget target)
            ```

            ::: block
            Return a path to a file in the buck-out/bin/ directory,
            formatted with the target short name.
            :::

            [Parameters:]{.paramLabel}
            :   `target` - The
                [`BuildTarget`](../BuildTarget.html "class in com.facebook.buck.core.model")
                to scope this path to.

            [Returns:]{.returnLabel}
            :   A
                [`Path`](http://docs.oracle.com/javase/7/docs/api/java/nio/file/Path.html?is-external=true "class or interface in java.nio.file"){.externalLink}
                under buck-out/bin, scoped to the base path of
                `      target`.

        []{#getAnnotationDir(com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.model.BuildTarget)}

        -   #### getAnnotationDir

            ``` methodSignature
            public static Path getAnnotationDir​(ProjectFilesystem filesystem,
                                                BuildTarget target)
            ```

            ::: block
            Return a path to a file in the buck-out/annotation/
            directory, formatted with the target short name.
            :::

            [Parameters:]{.paramLabel}
            :   `target` - The
                [`BuildTarget`](../BuildTarget.html "class in com.facebook.buck.core.model")
                to scope this path to.

            [Returns:]{.returnLabel}
            :   A
                [`Path`](http://docs.oracle.com/javase/7/docs/api/java/nio/file/Path.html?is-external=true "class or interface in java.nio.file"){.externalLink}
                under buck-out/annotation, scoped to the base path of
                `target`.

        []{#getGenDir(com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.model.BuildTarget)}

        -   #### getGenDir

            ``` methodSignature
            public static Path getGenDir​(ProjectFilesystem filesystem,
                                         BuildTarget target)
            ```

            ::: block
            Return a relative path to a file in the buck-out/gen/
            directory, formatted with the target short name.
            :::

            [Parameters:]{.paramLabel}
            :   `target` - The
                [`BuildTarget`](../BuildTarget.html "class in com.facebook.buck.core.model")
                to scope this path to.

            [Returns:]{.returnLabel}
            :   A
                [`Path`](http://docs.oracle.com/javase/7/docs/api/java/nio/file/Path.html?is-external=true "class or interface in java.nio.file"){.externalLink}
                under buck-out/gen, scoped to the base path of
                `      target`.

        []{#getBaseDir(com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.model.BuildTarget)}

        -   #### getBaseDir

            ``` methodSignature
            public static ForwardRelativePath getBaseDir​(ProjectFilesystem filesystem,
                                                         BuildTarget target)
            ```

            ::: block
            Return a relative path to a file taking into account the
            `target`\'s package path and formatting with the short name.
            This is a portion of the path returned by, e.g.,
            [`getGenDir(ProjectFilesystem,  BuildTarget)`](#getGenDir(com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.model.BuildTarget))
            :::

            [Parameters:]{.paramLabel}
            :   `target` - The
                [`BuildTarget`](../BuildTarget.html "class in com.facebook.buck.core.model")
                to scope this path to.

            [Returns:]{.returnLabel}
            :   A
                [`Path`](http://docs.oracle.com/javase/7/docs/api/java/nio/file/Path.html?is-external=true "class or interface in java.nio.file"){.externalLink}
                scoped to the base path to `target`.

        []{#removeHashFrom(java.nio.file.Path,com.facebook.buck.core.model.BuildTarget)}

        -   #### removeHashFrom

            ``` methodSignature
            public static Optional<Path> removeHashFrom​(Path path,
                                                        BuildTarget target)
            ```

            ::: block
            Removes the hash from the buck-out path. Used temporarily to
            create links.
            :::

            [Parameters:]{.paramLabel}
            :   `path` - Hashed buck-out path
            :   `target` - Build target that generated `path`

            [Returns:]{.returnLabel}
            :   A path without the hash directory or `Optional.empty()`
                if the hash was not found.
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
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   Constr \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
