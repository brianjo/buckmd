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
[Package]{.packageLabelInType} [com.facebook.buck.util.filesystem](package-summary.html)
:::

## Class PathFragments {#class-pathfragments .title title="Class PathFragments"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.util.filesystem.PathFragments

::: description
-   

    ------------------------------------------------------------------------

        public final class PathFragments
        extends Object

    ::: block
    Conversion utilities between Paths and PathFragments.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static Path`         | `fragmentT            | ::: block             |
        |                       | oPath​(com.google.devt | Convert a skylark     |
        |                       | ools.build.lib.vfs.Pa | PathFragment to a     |
        |                       | thFragment fragment)` | Path using the        |
        |                       |                       | default filesystem.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static Path`         | `frag                 | ::: block             |
        |                       | mentToPath​(FileSystem | Convert a skylark     |
        |                       |  fileSystem,          | PathFragment to a     |
        |                       |       com.google.devt | Path.                 |
        |                       | ools.build.lib.vfs.Pa | :::                   |
        |                       | thFragment fragment)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static com.g         | `pathT                | ::: block             |
        | oogle.devtools.build. | oFragment​(Path path)` | Convert a Skylark     |
        | lib.vfs.PathFragment` |                       | PathFragment to a     |
        |                       |                       | Java Path.            |
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

        []{#pathToFragment(java.nio.file.Path)}

        -   #### pathToFragment

            ``` methodSignature
            public static com.google.devtools.build.lib.vfs.PathFragment pathToFragment​(Path path)
            ```

            ::: block
            Convert a Skylark PathFragment to a Java Path.
            :::

        []{#fragmentToPath(com.google.devtools.build.lib.vfs.PathFragment)}

        -   #### fragmentToPath

            ``` methodSignature
            public static Path fragmentToPath​(com.google.devtools.build.lib.vfs.PathFragment fragment)
            ```

            ::: block
            Convert a skylark PathFragment to a Path using the default
            filesystem.
            :::

        []{#fragmentToPath(java.nio.file.FileSystem,com.google.devtools.build.lib.vfs.PathFragment)}

        -   #### fragmentToPath

            ``` methodSignature
            public static Path fragmentToPath​(FileSystem fileSystem,
                                              com.google.devtools.build.lib.vfs.PathFragment fragment)
            ```

            ::: block
            Convert a skylark PathFragment to a Path.
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
