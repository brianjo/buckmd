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
[Package]{.packageLabelInType} [com.facebook.buck.android.exopackage](package-summary.html)
:::

## Class ExopackageSymlinkTree {#class-exopackagesymlinktree .title title="Class ExopackageSymlinkTree"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.android.exopackage.ExopackageSymlinkTree

::: description
-   

    ------------------------------------------------------------------------

        public class ExopackageSymlinkTree
        extends Object

    ::: block
    Support out-of-process exopackage installation by creating a symlink
    tree mirroring the desired on-device layout. This allows an external
    process to call \`adb push\` or the equivalent without any knowledge
    of the internals of exo-install (or a dependency on the implementing
    code)
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                 Description
          --------------------------- -------------
          `ExopackageSymlinkTree()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static void`         | `creat                | ::: block             |
        |                       | eSymlinkTree​(String p | Create a symlink tree |
        |                       | ackageName,           | rooted at rootPath    |
        |                       |         ExopackageInf | which contains a      |
        |                       | o exoInfo,            | mirror of what should |
        |                       |        SourcePathReso | appear on the device  |
        |                       | lverAdapter pathResol | as a result of an     |
        |                       | ver,                  | exopackage            |
        |                       |  ProjectFilesystem fi | installation.         |
        |                       | lesystem,             | :::                   |
        |                       |       Path rootPath)` |                       |
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
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### ExopackageSymlinkTree

                public ExopackageSymlinkTree()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#createSymlinkTree(java.lang.String,com.facebook.buck.android.exopackage.ExopackageInfo,com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter,com.facebook.buck.io.filesystem.ProjectFilesystem,java.nio.file.Path)}

        -   #### createSymlinkTree

            ``` methodSignature
            public static void createSymlinkTree​(String packageName,
                                                 ExopackageInfo exoInfo,
                                                 SourcePathResolverAdapter pathResolver,
                                                 ProjectFilesystem filesystem,
                                                 Path rootPath)
                                          throws IOException
            ```

            ::: block
            Create a symlink tree rooted at rootPath which contains a
            mirror of what should appear on the device as a result of an
            exopackage installation.
            :::

            [Parameters:]{.paramLabel}
            :   `packageName` -
            :   `exoInfo` - the exopackage info for the app which will
                be installed
            :   `pathResolver` - needed to convert the exoInfo
                SourcePaths into real Paths
            :   `filesystem` - need to write files/create
                symlinks/access paths
            :   `rootPath` - location where the resulting symlink tree
                will be rooted

            [Throws:]{.throwsLabel}
            :   `IOException` - if the symlink tree or any of its files
                cannot be written
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
