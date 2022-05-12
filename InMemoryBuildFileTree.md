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
[Package]{.packageLabelInType} [com.facebook.buck.core.model.impl](package-summary.html)
:::

## Class InMemoryBuildFileTree {#class-inmemorybuildfiletree .title title="Class InMemoryBuildFileTree"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.model.impl.InMemoryBuildFileTree

::: description
-   

    All Implemented Interfaces:
    :   `BuildFileTree`

    ------------------------------------------------------------------------

        public class InMemoryBuildFileTree
        extends Object
        implements BuildFileTree

    ::: block
    A tree of build files that reflects their tree structure in the
    filesystem. This makes it possible to see which build files are
    \"under\" other build files.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

        +-----------------------------------+-----------------------------------+
        | Constructor                       | Description                       |
        +===================================+===================================+
        | `InMem                            | ::: block                         |
        | oryBuildFileTree​(Iterable<BuildTa | Creates an InMemoryBuildFileTree  |
        | rget> targets,                    | from the base paths in the given  |
        |    ProjectFilesystem filesystem)` | BuildTargetPaths.                 |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+
        | `InMemoryBuildFileTre             |                                   |
        | e​(Collection<RelPath> basePaths)` |                                   |
        +-----------------------------------+-----------------------------------+

        : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `Optional<RelPath>`   | `getB                 | ::: block             |
        |                       | asePathOfAncestorTarg | Returns the base path |
        |                       | et​(RelPath filePath)` | for a given path.     |
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

        []{#<init>(java.lang.Iterable,com.facebook.buck.io.filesystem.ProjectFilesystem)}

        -   #### InMemoryBuildFileTree

                public InMemoryBuildFileTree​(Iterable<BuildTarget> targets,
                                             ProjectFilesystem filesystem)

            ::: block
            Creates an InMemoryBuildFileTree from the base paths in the
            given BuildTargetPaths.
            :::

            [Parameters:]{.paramLabel}
            :   `targets` - BuildTargetPaths to get base paths from.

        []{#<init>(java.util.Collection)}

        -   #### InMemoryBuildFileTree

                public InMemoryBuildFileTree​(Collection<RelPath> basePaths)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getBasePathOfAncestorTarget(com.facebook.buck.core.filesystems.RelPath)}

        -   #### getBasePathOfAncestorTarget

            ``` methodSignature
            public Optional<RelPath> getBasePathOfAncestorTarget​(RelPath filePath)
            ```

            ::: block
            [Description copied from
            interface: `BuildFileTree`]{.descfrmTypeLabel}
            :::

            ::: block
            Returns the base path for a given path. The base path is the
            nearest directory at or above filePath that contains a build
            file.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getBasePathOfAncestorTarget` in
                interface `BuildFileTree`

            [Parameters:]{.paramLabel}
            :   `filePath` - the path whose base path to find.

            [Returns:]{.returnLabel}
            :   the base path if there is one.
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
