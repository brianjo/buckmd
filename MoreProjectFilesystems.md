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
[Package]{.packageLabelInType} [com.facebook.buck.io](package-summary.html)
:::

## Class MoreProjectFilesystems {#class-moreprojectfilesystems .title title="Class MoreProjectFilesystems"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.io.MoreProjectFilesystems

::: description
-   

    ------------------------------------------------------------------------

        public class MoreProjectFilesystems
        extends Object

    ::: block
    Common functions that are done with a
    [`ProjectFilesystem`](filesystem/ProjectFilesystem.html "interface in com.facebook.buck.io.filesystem").
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static Path`         | `createRelative       | ::: block             |
        |                       | Symlink​(Path pathToDe | Creates a symlink at  |
        |                       | siredLinkUnderProject | `  projectFiles       |
        |                       | Root,                 | ystem.getRootPath().r |
        |                       |       Path pathToExis | esolve(pathToDesiredL |
        |                       | tingFileUnderProjectR | inkUnderProjectRoot)` |
        |                       | oot,                  | that points to        |
        |                       |      ProjectFilesyste | `projectFilesy        |
        |                       | m projectFilesystem)` | stem.getRootPath().re |
        |                       |                       | solve(pathToExistingF |
        |                       |                       | ileUnderProjectRoot)` |
        |                       |                       | using a relative      |
        |                       |                       | symlink.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static boolean`      | `fileContentsDiffer​(I |                       |
        |                       | nputStream contents,  |                       |
        |                       |                   Pat |                       |
        |                       | h path,               |                       |
        |                       |      ProjectFilesyste |                       |
        |                       | m projectFilesystem)` |                       |
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

        []{#createRelativeSymlink(java.nio.file.Path,java.nio.file.Path,com.facebook.buck.io.filesystem.ProjectFilesystem)}

        -   #### createRelativeSymlink

            ``` methodSignature
            public static Path createRelativeSymlink​(Path pathToDesiredLinkUnderProjectRoot,
                                                     Path pathToExistingFileUnderProjectRoot,
                                                     ProjectFilesystem projectFilesystem)
                                              throws IOException
            ```

            ::: block
            Creates a symlink at
            `  projectFilesystem.getRootPath().resolve(pathToDesiredLinkUnderProjectRoot)`
            that points to
            `projectFilesystem.getRootPath().resolve(pathToExistingFileUnderProjectRoot)`
            using a relative symlink.
            :::

            [Parameters:]{.paramLabel}
            :   `pathToDesiredLinkUnderProjectRoot` - must reference a
                file, not a directory.
            :   `pathToExistingFileUnderProjectRoot` - must reference a
                file, not a directory.
            :   `projectFilesystem` - the projectFileSystem.

            [Returns:]{.returnLabel}
            :   Path to the newly created symlink (relative path on Unix
                absolute path on Windows).

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#fileContentsDiffer(java.io.InputStream,java.nio.file.Path,com.facebook.buck.io.filesystem.ProjectFilesystem)}

        -   #### fileContentsDiffer

            ``` methodSignature
            public static boolean fileContentsDiffer​(InputStream contents,
                                                     Path path,
                                                     ProjectFilesystem projectFilesystem)
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
