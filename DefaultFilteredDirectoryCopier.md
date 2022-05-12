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
[Package]{.packageLabelInType} [com.facebook.buck.util](package-summary.html)
:::

## Class DefaultFilteredDirectoryCopier {#class-defaultfiltereddirectorycopier .title title="Class DefaultFilteredDirectoryCopier"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.util.DefaultFilteredDirectoryCopier

::: description
-   

    All Implemented Interfaces:
    :   `FilteredDirectoryCopier`

    ------------------------------------------------------------------------

        public class DefaultFilteredDirectoryCopier
        extends Object
        implements FilteredDirectoryCopier

    ::: block
    This class allows the creation of copies of multiple directories,
    while filtering out files which do not match a specified predicate.
    Current caveats:

    -   Existing content in destination directories is deleted.
    -   Empty directories will not be created.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `void`                | `c                    | ::: block             |
        |                       | opyDir​(ProjectFilesys | Creates a filtered    |
        |                       | tem filesystem,       | copy of a directory.  |
        |                       |   Path srcDir,        | :::                   |
        |                       |  Path destDir,        |                       |
        |                       |  java.util.function.P |                       |
        |                       | redicate<Path> pred)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `copyDirs             | ::: block             |
        |                       | ​(ProjectFilesystem fi | Copies multiple       |
        |                       | lesystem,         Map | directories while     |
        |                       | <Path,​Path> sourcesTo | filtering out         |
        |                       | Destinations,         | individual files      |
        |                       |  java.util.function.P | which fail a          |
        |                       | redicate<Path> pred)` | predicate.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static DefaultFil    | `getInstance()`       |                       |
        | teredDirectoryCopier` |                       |                       |
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
    -   []{#method.detail}

        ### Method Detail

        []{#getInstance()}

        -   #### getInstance

            ``` methodSignature
            public static DefaultFilteredDirectoryCopier getInstance()
            ```

        []{#copyDirs(com.facebook.buck.io.filesystem.ProjectFilesystem,java.util.Map,java.util.function.Predicate)}

        -   #### copyDirs

            ``` methodSignature
            public void copyDirs​(ProjectFilesystem filesystem,
                                 Map<Path,​Path> sourcesToDestinations,
                                 java.util.function.Predicate<Path> pred)
                          throws IOException
            ```

            ::: block
            [Description copied from
            interface: `FilteredDirectoryCopier`]{.descfrmTypeLabel}
            :::

            ::: block
            Copies multiple directories while filtering out individual
            files which fail a predicate.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `copyDirs` in interface `FilteredDirectoryCopier`
            :   `sourcesToDestinations` - mapping from source to
                destination directories
            :   `pred` - predicate to test against

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#copyDir(com.facebook.buck.io.filesystem.ProjectFilesystem,java.nio.file.Path,java.nio.file.Path,java.util.function.Predicate)}

        -   #### copyDir

            ``` methodSignature
            public void copyDir​(ProjectFilesystem filesystem,
                                Path srcDir,
                                Path destDir,
                                java.util.function.Predicate<Path> pred)
                         throws IOException
            ```

            ::: block
            [Description copied from
            interface: `FilteredDirectoryCopier`]{.descfrmTypeLabel}
            :::

            ::: block
            Creates a filtered copy of a directory.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `copyDir` in interface `FilteredDirectoryCopier`
            :   `srcDir` - source directory
            :   `destDir` - destination directory
            :   `pred` - a predicate to determine which files should be
                copied.

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
