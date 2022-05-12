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
[Package]{.packageLabelInType} [com.facebook.buck.core.files](package-summary.html)
:::

## Class FileTree {#class-filetree .title title="Class FileTree"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.files.FileTree

::: description
-   

    All Implemented Interfaces:
    :   `ComputeResult`

    ------------------------------------------------------------------------

        public abstract class FileTree
        extends Object
        implements ComputeResult

    ::: block
    Has information about files and folders at some directory
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor    Description
          -------------- -------------
          `FileTree()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `                     | `getChildren()`       | ::: block             |
        | abstract com.google.c |                       | File trees of all     |
        | ommon.collect.Immutab |                       | subfolders            |
        | leMap<Path,​FileTree>` |                       | recursively           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ab                   | `getDirectoryList()`  | ::: block             |
        | stract DirectoryList` |                       | List of files,        |
        |                       |                       | folders and symlinks  |
        |                       |                       | in the desired        |
        |                       |                       | directory             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `abstract Path`       | `getPath()`           | ::: block             |
        |                       |                       | Relative path to this |
        |                       |                       | instance from some    |
        |                       |                       | root, usually cell    |
        |                       |                       | root                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}

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

        -   #### FileTree

                public FileTree()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getPath()}

        -   #### getPath

            ``` methodSignature
            public abstract Path getPath()
            ```

            ::: block
            Relative path to this instance from some root, usually cell
            root
            :::

        []{#getDirectoryList()}

        -   #### getDirectoryList

            ``` methodSignature
            public abstract DirectoryList getDirectoryList()
            ```

            ::: block
            List of files, folders and symlinks in the desired directory
            :::

        []{#getChildren()}

        -   #### getChildren

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableMap<Path,​FileTree> getChildren()
            ```

            ::: block
            File trees of all subfolders recursively
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
