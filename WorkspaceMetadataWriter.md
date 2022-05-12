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
[Package]{.packageLabelInType} [com.facebook.buck.features.apple.common](package-summary.html)
:::

## Class WorkspaceMetadataWriter {#class-workspacemetadatawriter .title title="Class WorkspaceMetadataWriter"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.features.apple.common.WorkspaceMetadataWriter

::: description
-   

    ------------------------------------------------------------------------

        public class WorkspaceMetadataWriter
        extends Object

    ::: block
    Writes workspace metadata information to a json file.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                                                                                                                                        Description
          -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `WorkspaceMetadataWriter​(String projectVersion,                        com.google.common.collect.ImmutableSet<BuildTarget> requiredBuildTargets,                        com.google.common.collect.ImmutableSet<Path> xcconfigPaths,                        com.google.common.collect.ImmutableList<CopyInXcode> filesToCopyInXcode,                        ProjectFilesystem projectFilesystem)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `void`                | `w                    | ::: block             |
        |                       | riteToWorkspaceAtPath | Writes the metadata   |
        |                       | ​(Path workspacePath)` | information to the    |
        |                       |                       | workspace at the      |
        |                       |                       | input path.           |
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

        []{#<init>(java.lang.String,com.google.common.collect.ImmutableSet,com.google.common.collect.ImmutableSet,com.google.common.collect.ImmutableList,com.facebook.buck.io.filesystem.ProjectFilesystem)}

        -   #### WorkspaceMetadataWriter

                public WorkspaceMetadataWriter​(String projectVersion,
                                               com.google.common.collect.ImmutableSet<BuildTarget> requiredBuildTargets,
                                               com.google.common.collect.ImmutableSet<Path> xcconfigPaths,
                                               com.google.common.collect.ImmutableList<CopyInXcode> filesToCopyInXcode,
                                               ProjectFilesystem projectFilesystem)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#writeToWorkspaceAtPath(java.nio.file.Path)}

        -   #### writeToWorkspaceAtPath

            ``` methodSignature
            public void writeToWorkspaceAtPath​(Path workspacePath)
                                        throws IOException
            ```

            ::: block
            Writes the metadata information to the workspace at the
            input path.
            :::

            [Parameters:]{.paramLabel}
            :   `workspacePath` - The workspace path to write to.

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
