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

## Class BuildTargetPaths {#class-buildtargetpaths .title title="Class BuildTargetPaths"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.model.impl.BuildTargetPaths

::: description
-   

    ------------------------------------------------------------------------

        @Deprecated
        public class BuildTargetPaths
        extends Object

    ::: deprecationBlock
    [Deprecated.]{.deprecatedLabel}

    ::: deprecationComment
    use
    [`BuildPaths`](BuildPaths.html "class in com.facebook.buck.core.model.impl")
    instead, which handles flavoured and unflavoured
    [`BuildTarget`](../BuildTarget.html "class in com.facebook.buck.core.model")s
    in the paths the same way as
    RE/[`ModernBuildRule`](../../../rules/modern/ModernBuildRule.html "class in com.facebook.buck.rules.modern")s
    do.
    :::
    :::

    ::: block
    Static helpers for working with build targets.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static Path`         | `getAnnotatio         | ::: block             |
        |                       | nPath​(ProjectFilesyst | [Deprecate            |
        |                       | em filesystem,        | d.]{.deprecatedLabel} |
        |                       |            BuildTarge | :::                   |
        |                       | t target,             |                       |
        |                       |       String format)` | ::: block             |
        |                       |                       | Return a path to a    |
        |                       |                       | file in the           |
        |                       |                       | buck-out/annotation/  |
        |                       |                       | directory.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static               | `getBasePath​(Pro      | ::: block             |
        |  ForwardRelativePath` | jectFilesystem filesy | [Deprecate            |
        |                       | stem,            Buil | d.]{.deprecatedLabel} |
        |                       | dTarget target,       | :::                   |
        |                       |       String format)` |                       |
        |                       |                       | ::: block             |
        |                       |                       | Return a relative     |
        |                       |                       | path to a file.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static               | `getBasePath          | ::: block             |
        |  ForwardRelativePath` | ForBaseName​(ProjectFi | [Deprecate            |
        |                       | lesystem filesystem,  | d.]{.deprecatedLabel} |
        |                       |                       | :::                   |
        |                       |  BuildTarget target)` |                       |
        |                       |                       | ::: block             |
        |                       |                       | Return a relative     |
        |                       |                       | path for all targets  |
        |                       |                       | in a package of a     |
        |                       |                       | [`BuildTarget`        |
        |                       |                       | ](../BuildTarget.html |
        |                       |                       |  "class in com.facebo |
        |                       |                       | ok.buck.core.model"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static Path`         | `getGenPath​(P         | ::: block             |
        |                       | rojectFilesystem file | [Deprecate            |
        |                       | system,           Bui | d.]{.deprecatedLabel} |
        |                       | ldTarget target,      | :::                   |
        |                       |       String format)` |                       |
        |                       |                       | ::: block             |
        |                       |                       | Return a relative     |
        |                       |                       | path to a file in the |
        |                       |                       | buck-out/gen/         |
        |                       |                       | directory.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static Path`         | `getGenPat            | ::: block             |
        |                       | hForBaseName​(ProjectF | [Deprecate            |
        |                       | ilesystem filesystem, | d.]{.deprecatedLabel} |
        |                       |                       | :::                   |
        |                       |  BuildTarget target)` |                       |
        |                       |                       | ::: block             |
        |                       |                       | A folder where all    |
        |                       |                       | targets in the file   |
        |                       |                       | of target are         |
        |                       |                       | created.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static Path`         | `get                  | ::: block             |
        |                       | ScratchPath​(ProjectFi | [Deprecate            |
        |                       | lesystem filesystem,  | d.]{.deprecatedLabel} |
        |                       |               BuildTa | :::                   |
        |                       | rget target,          |                       |
        |                       |       String format)` | ::: block             |
        |                       |                       | Return a path to a    |
        |                       |                       | file in the           |
        |                       |                       | buck-out/bin/         |
        |                       |                       | directory.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4
        .tableTab}[[Deprecated
        Methods](javascript:show(32);)[ ]{.tabEnd}]{#t6 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getScratchPath(com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.model.BuildTarget,java.lang.String)}

        -   #### getScratchPath

            ``` methodSignature
            public static Path getScratchPath​(ProjectFilesystem filesystem,
                                              BuildTarget target,
                                              String format)
            ```

            ::: deprecationBlock
            [Deprecated.]{.deprecatedLabel}
            :::

            ::: block
            Return a path to a file in the buck-out/bin/ directory.
            `format` will be prepended with the
            [`BuckPaths.getScratchDir()`](../../../io/filesystem/BuckPaths.html#getScratchDir())
            and the target base path, then formatted with the target
            short name.
            :::

            [Parameters:]{.paramLabel}
            :   `target` - The
                [`BuildTarget`](../BuildTarget.html "class in com.facebook.buck.core.model")
                to scope this path to.
            :   `format` -
                [`String.format(java.lang.String, java.lang.Object...)`](http://docs.oracle.com/javase/7/docs/api/java/lang/String.html?is-external=true#format(java.lang.String,java.lang.Object...) "class or interface in java.lang"){.externalLink}
                string for the path name. It should contain one \"%s\",
                which will be filled in with the rule\'s short name. It
                should not start with a slash.

            [Returns:]{.returnLabel}
            :   A
                [`Path`](http://docs.oracle.com/javase/7/docs/api/java/nio/file/Path.html?is-external=true "class or interface in java.nio.file"){.externalLink}
                under buck-out/bin, scoped to the base path of
                `      target`.

        []{#getAnnotationPath(com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.model.BuildTarget,java.lang.String)}

        -   #### getAnnotationPath

            ``` methodSignature
            public static Path getAnnotationPath​(ProjectFilesystem filesystem,
                                                 BuildTarget target,
                                                 String format)
            ```

            ::: deprecationBlock
            [Deprecated.]{.deprecatedLabel}
            :::

            ::: block
            Return a path to a file in the buck-out/annotation/
            directory. `format` will be prepended with the
            [`BuckPaths.getAnnotationDir()`](../../../io/filesystem/BuckPaths.html#getAnnotationDir())
            and the target base path, then formatted with the target
            short name.
            :::

            [Parameters:]{.paramLabel}
            :   `target` - The
                [`BuildTarget`](../BuildTarget.html "class in com.facebook.buck.core.model")
                to scope this path to.
            :   `format` -
                [`String.format(java.lang.String, java.lang.Object...)`](http://docs.oracle.com/javase/7/docs/api/java/lang/String.html?is-external=true#format(java.lang.String,java.lang.Object...) "class or interface in java.lang"){.externalLink}
                string for the path name. It should contain one \"%s\",
                which will be filled in with the rule\'s short name. It
                should not start with a slash.

            [Returns:]{.returnLabel}
            :   A
                [`Path`](http://docs.oracle.com/javase/7/docs/api/java/nio/file/Path.html?is-external=true "class or interface in java.nio.file"){.externalLink}
                under buck-out/annotation, scoped to the base path of
                `target`.

        []{#getGenPath(com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.model.BuildTarget,java.lang.String)}

        -   #### getGenPath

            ``` methodSignature
            public static Path getGenPath​(ProjectFilesystem filesystem,
                                          BuildTarget target,
                                          String format)
            ```

            ::: deprecationBlock
            [Deprecated.]{.deprecatedLabel}
            :::

            ::: block
            Return a relative path to a file in the buck-out/gen/
            directory. `format` will be prepended with the
            [`BuckPaths.getGenDir()`](../../../io/filesystem/BuckPaths.html#getGenDir())
            and the target base path, then formatted with the target
            short name.
            :::

            [Parameters:]{.paramLabel}
            :   `target` - The
                [`BuildTarget`](../BuildTarget.html "class in com.facebook.buck.core.model")
                to scope this path to.
            :   `format` -
                [`String.format(java.lang.String, java.lang.Object...)`](http://docs.oracle.com/javase/7/docs/api/java/lang/String.html?is-external=true#format(java.lang.String,java.lang.Object...) "class or interface in java.lang"){.externalLink}
                string for the path name. It should contain one \"%s\",
                which will be filled in with the rule\'s short name. It
                should not start with a slash.

            [Returns:]{.returnLabel}
            :   A
                [`Path`](http://docs.oracle.com/javase/7/docs/api/java/nio/file/Path.html?is-external=true "class or interface in java.nio.file"){.externalLink}
                under buck-out/gen, scoped to the base path of
                `      target`.

        []{#getGenPathForBaseName(com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.model.BuildTarget)}

        -   #### getGenPathForBaseName

            ``` methodSignature
            public static Path getGenPathForBaseName​(ProjectFilesystem filesystem,
                                                     BuildTarget target)
            ```

            ::: deprecationBlock
            [Deprecated.]{.deprecatedLabel}
            :::

            ::: block
            A folder where all targets in the file of target are
            created.
            :::

        []{#getBasePath(com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.model.BuildTarget,java.lang.String)}

        -   #### getBasePath

            ``` methodSignature
            public static ForwardRelativePath getBasePath​(ProjectFilesystem filesystem,
                                                          BuildTarget target,
                                                          String format)
            ```

            ::: deprecationBlock
            [Deprecated.]{.deprecatedLabel}
            :::

            ::: block
            Return a relative path to a file. `format` will be prepended
            with the target base path, then formatted with the target
            short name.
            This is portion of the path returned by, e.g.,
            [`getGenPath(ProjectFilesystem,  BuildTarget, String)`](#getGenPath(com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.model.BuildTarget,java.lang.String))
            :::

            [Parameters:]{.paramLabel}
            :   `target` - The
                [`BuildTarget`](../BuildTarget.html "class in com.facebook.buck.core.model")
                to scope this path to.
            :   `format` -
                [`String.format(java.lang.String, java.lang.Object...)`](http://docs.oracle.com/javase/7/docs/api/java/lang/String.html?is-external=true#format(java.lang.String,java.lang.Object...) "class or interface in java.lang"){.externalLink}
                string for the path name. It should contain one \"%s\",
                which will be filled in with the rule\'s short name. It
                should not start with a slash.

            [Returns:]{.returnLabel}
            :   A
                [`Path`](http://docs.oracle.com/javase/7/docs/api/java/nio/file/Path.html?is-external=true "class or interface in java.nio.file"){.externalLink}
                scoped to the base path of `target`.

        []{#getBasePathForBaseName(com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.model.BuildTarget)}

        -   #### getBasePathForBaseName

            ``` methodSignature
            public static ForwardRelativePath getBasePathForBaseName​(ProjectFilesystem filesystem,
                                                                     BuildTarget target)
            ```

            ::: deprecationBlock
            [Deprecated.]{.deprecatedLabel}
            :::

            ::: block
            Return a relative path for all targets in a package of a
            [`BuildTarget`](../BuildTarget.html "class in com.facebook.buck.core.model").
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
