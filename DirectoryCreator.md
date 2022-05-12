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
[Package]{.packageLabelInType} [com.facebook.buck.util.unarchive](package-summary.html)
:::

## Class DirectoryCreator {#class-directorycreator .title title="Class DirectoryCreator"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.util.unarchive.DirectoryCreator

::: description
-   

    ------------------------------------------------------------------------

        public class DirectoryCreator
        extends Object

    ::: block
    Simple class that creates directories, but keeps track of what it
    has created to ensure that it does not create directories more than
    once. This is useful when extracting archives that may or may not
    have duplicate entries, or to just ensure that a directory always
    exists before writing out a new file
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

        +-----------------------------------+-----------------------------------+
        | Constructor                       | Description                       |
        +===================================+===================================+
        | `DirectoryCreat                   | ::: block                         |
        | or​(ProjectFilesystem filesystem)` | Creates an instance of            |
        |                                   | [`DirectoryCreator`](             |
        |                                   | DirectoryCreator.html "class in c |
        |                                   | om.facebook.buck.util.unarchive") |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+

        : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `void`                | `forcefullyCre        | ::: block             |
        |                       | ateDirs​(Path target)` | Force a directory to  |
        |                       |                       | be created.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ProjectFilesystem`   | `getFilesystem()`     |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `mkdirs​(Path target)` | ::: block             |
        |                       |                       | Create a directory    |
        |                       |                       | and all of its        |
        |                       |                       | parents               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Set<Path>`           | `r                    | ::: block             |
        |                       | ecordedDirectories()` | Get the set of        |
        |                       |                       | directories that were |
        |                       |                       | either created by     |
        |                       |                       | this class, or        |
        |                       |                       | manually specified in |
        |                       |                       | [`recordPat           |
        |                       |                       | h(Path)`](#recordPath |
        |                       |                       | (java.nio.file.Path)) |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `rec                  | ::: block             |
        |                       | ordPath​(Path target)` | Ensure that we record |
        |                       |                       | that a path was       |
        |                       |                       | created.              |
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

        []{#<init>(com.facebook.buck.io.filesystem.ProjectFilesystem)}

        -   #### DirectoryCreator

                public DirectoryCreator​(ProjectFilesystem filesystem)

            ::: block
            Creates an instance of
            [`DirectoryCreator`](DirectoryCreator.html "class in com.facebook.buck.util.unarchive")
            :::

            [Parameters:]{.paramLabel}
            :   `filesystem` - The filesystem to operate on
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#recordedDirectories()}

        -   #### recordedDirectories

            ``` methodSignature
            public Set<Path> recordedDirectories()
            ```

            ::: block
            Get the set of directories that were either created by this
            class, or manually specified in
            [`recordPath(Path)`](#recordPath(java.nio.file.Path))
            :::

            [Returns:]{.returnLabel}
            :   Set of directories

        []{#recordPath(java.nio.file.Path)}

        -   #### recordPath

            ``` methodSignature
            public void recordPath​(Path target)
            ```

            ::: block
            Ensure that we record that a path was created. This can be
            useful if for some reason a directory is created externally,
            but the list of created directories is pulled from an
            instance of
            [`DirectoryCreator`](DirectoryCreator.html "class in com.facebook.buck.util.unarchive")
            :::

            [Parameters:]{.paramLabel}
            :   `target` -

        []{#getFilesystem()}

        -   #### getFilesystem

            ``` methodSignature
            public ProjectFilesystem getFilesystem()
            ```

        []{#mkdirs(java.nio.file.Path)}

        -   #### mkdirs

            ``` methodSignature
            public void mkdirs​(Path target)
                        throws IOException
            ```

            ::: block
            Create a directory and all of its parents
            :::

            [Parameters:]{.paramLabel}
            :   `target` - The path where a directory should exist

            [Throws:]{.throwsLabel}
            :   `IOException` - If the directory could not be created

        []{#forcefullyCreateDirs(java.nio.file.Path)}

        -   #### forcefullyCreateDirs

            ``` methodSignature
            public void forcefullyCreateDirs​(Path target)
                                      throws IOException
            ```

            ::: block
            Force a directory to be created. This will delete existing
            files (not directories) if they share the name of the
            directory, including parent paths
            :::

            [Parameters:]{.paramLabel}
            :   `target` - The path where a directory should exist

            [Throws:]{.throwsLabel}
            :   `IOException` - The directory could not be created, or
                files that needed to be removed could not be removed
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
