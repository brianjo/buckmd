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
[Package]{.packageLabelInType} [com.facebook.buck.io](package-summary.html)
:::

## Class BuildCellRelativePath {#class-buildcellrelativepath .title title="Class BuildCellRelativePath"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.io.BuildCellRelativePath

::: description
-   

    ------------------------------------------------------------------------

        public abstract class BuildCellRelativePath
        extends Object

    ::: block
    A path which is relative to the build cell root, i.e. the top-level
    cell in which the build was invoked.
    See
    [`BuildContext.getBuildCellRootPath()`](../core/build/context/BuildContext.html#getBuildCellRootPath()).
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                 Description
          --------------------------- -------------
          `BuildCellRelativePath()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `protected void`      | `check()`             | ::: block             |
        |                       |                       | Check the path is     |
        |                       |                       | relative.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static B             | `fromCellRelativ      |                       |
        | uildCellRelativePath` | ePath​(AbsPath buildCe |                       |
        |                       | llRootPath,           |                       |
        |                       |            ProjectFil |                       |
        |                       | esystem cellProjectFi |                       |
        |                       | lesystem,             |                       |
        |                       |          Path cellRel |                       |
        |                       | ativeOrAbsolutePath)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static B             | `fromCellRela         |                       |
        | uildCellRelativePath` | tivePath​(Path buildCe |                       |
        |                       | llRootPath,           |                       |
        |                       |            ProjectFil |                       |
        |                       | esystem cellProjectFi |                       |
        |                       | lesystem,             |                       |
        |                       |          Path cellRel |                       |
        |                       | ativeOrAbsolutePath)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract Path`       | `getPathRelat         |                       |
        |                       | iveToBuildCellRoot()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static B             | `of​(Path pathRela     |                       |
        | uildCellRelativePath` | tiveToBuildCellRoot)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `toString()`          |                       |
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

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### BuildCellRelativePath

                public BuildCellRelativePath()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getPathRelativeToBuildCellRoot()}

        -   #### getPathRelativeToBuildCellRoot

            ``` methodSignature
            public abstract Path getPathRelativeToBuildCellRoot()
            ```

        []{#check()}

        -   #### check

            ``` methodSignature
            @Check
            protected void check()
            ```

            ::: block
            Check the path is relative.
            :::

        []{#fromCellRelativePath(java.nio.file.Path,com.facebook.buck.io.filesystem.ProjectFilesystem,java.nio.file.Path)}

        -   #### fromCellRelativePath

            ``` methodSignature
            public static BuildCellRelativePath fromCellRelativePath​(Path buildCellRootPath,
                                                                     ProjectFilesystem cellProjectFilesystem,
                                                                     Path cellRelativeOrAbsolutePath)
            ```

        []{#fromCellRelativePath(com.facebook.buck.core.filesystems.AbsPath,com.facebook.buck.io.filesystem.ProjectFilesystem,java.nio.file.Path)}

        -   #### fromCellRelativePath

            ``` methodSignature
            public static BuildCellRelativePath fromCellRelativePath​(AbsPath buildCellRootPath,
                                                                     ProjectFilesystem cellProjectFilesystem,
                                                                     Path cellRelativeOrAbsolutePath)
            ```

        []{#of(java.nio.file.Path)}

        -   #### of

            ``` methodSignature
            public static BuildCellRelativePath of​(Path pathRelativeToBuildCellRoot)
            ```

        []{#toString()}

        -   #### toString

            ``` methodSignature
            public String toString()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `toString` in class `Object`
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
