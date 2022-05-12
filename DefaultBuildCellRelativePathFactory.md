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
[Package]{.packageLabelInType} [com.facebook.buck.rules.modern](package-summary.html)
:::

## Class DefaultBuildCellRelativePathFactory {#class-defaultbuildcellrelativepathfactory .title title="Class DefaultBuildCellRelativePathFactory"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.rules.modern.DefaultBuildCellRelativePathFactory

::: description
-   

    All Implemented Interfaces:
    :   `BuildCellRelativePathFactory`

    ------------------------------------------------------------------------

        public class DefaultBuildCellRelativePathFactory
        extends Object
        implements BuildCellRelativePathFactory
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                          Description
          -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `DefaultBuildCellRelativePathFactory​(Path buildCellRootPath,                                    ProjectFilesystem filesystem,                                    Optional<OutputPathResolver> outputPathResolver)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `B                    | `from​(Ou              | ::: block             |
        | uildCellRelativePath` | tputPath outputPath)` | Converts an           |
        |                       |                       | OutputPath to a       |
        |                       |                       | B                     |
        |                       |                       | uildCellRelativePath. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `B                    | `from​(Path bu         | ::: block             |
        | uildCellRelativePath` | ildableRelativePath)` | Converts a Path       |
        |                       |                       | relative to the       |
        |                       |                       | Buildable\'s          |
        |                       |                       | ProjectFilesystem to  |
        |                       |                       | a                     |
        |                       |                       | B                     |
        |                       |                       | uildCellRelativePath. |
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

        []{#<init>(java.nio.file.Path,com.facebook.buck.io.filesystem.ProjectFilesystem,java.util.Optional)}

        -   #### DefaultBuildCellRelativePathFactory

                public DefaultBuildCellRelativePathFactory​(Path buildCellRootPath,
                                                           ProjectFilesystem filesystem,
                                                           Optional<OutputPathResolver> outputPathResolver)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#from(java.nio.file.Path)}

        -   #### from

            ``` methodSignature
            public BuildCellRelativePath from​(Path buildableRelativePath)
            ```

            ::: block
            [Description copied from
            interface: `BuildCellRelativePathFactory`]{.descfrmTypeLabel}
            :::

            ::: block
            Converts a Path relative to the Buildable\'s
            ProjectFilesystem to a BuildCellRelativePath.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `from` in interface `BuildCellRelativePathFactory`

        []{#from(com.facebook.buck.rules.modern.OutputPath)}

        -   #### from

            ``` methodSignature
            public BuildCellRelativePath from​(OutputPath outputPath)
            ```

            ::: block
            [Description copied from
            interface: `BuildCellRelativePathFactory`]{.descfrmTypeLabel}
            :::

            ::: block
            Converts an OutputPath to a BuildCellRelativePath.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `from` in interface `BuildCellRelativePathFactory`
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
