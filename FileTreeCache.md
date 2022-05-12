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
-   [Nested](#nested.class.summary) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.core.files](package-summary.html)
:::

## Class FileTreeCache {#class-filetreecache .title title="Class FileTreeCache"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.files.FileTreeCache

::: description
-   

    All Implemented Interfaces:
    :   `GraphEngineCache<FileTreeKey,​FileTree>`

    ------------------------------------------------------------------------

        public class FileTreeCache
        extends Object
        implements GraphEngineCache<FileTreeKey,​FileTree>

    ::: block
    Stores a recursive file tree
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static class `       | `FileT                | ::: block             |
        |                       | reeCache.Invalidator` | Subscribes to         |
        |                       |                       | watchman event and    |
        |                       |                       | invalidates internal  |
        |                       |                       | state of a provided   |
        |                       |                       | [`FileTreeCach        |
        |                       |                       | e`](FileTreeCache.htm |
        |                       |                       | l "class in com.faceb |
        |                       |                       | ook.buck.core.files") |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `Optional<FileTree>`  | `                     | ::: block             |
        |                       | get​(FileTreeKey key)` | Optionally returns    |
        |                       |                       | the cached result     |
        |                       |                       | given the key         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `FileT                | `getInvalidator()`    |                       |
        | reeCache.Invalidator` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `of​(Path rootPath)`   | ::: block             |
        | static FileTreeCache` |                       | Create a new instance |
        |                       |                       | of                    |
        |                       |                       | [`FileTreeCach        |
        |                       |                       | e`](FileTreeCache.htm |
        |                       |                       | l "class in com.faceb |
        |                       |                       | ook.buck.core.files") |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `p                    | ::: block             |
        |                       | ut​(FileTreeKey key,   | Offers the given key  |
        |                       |   FileTree fileTree)` | and value for caching |
        |                       |                       | :::                   |
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

        []{#of(java.nio.file.Path)}

        -   #### of

            ``` methodSignature
            public static FileTreeCache of​(Path rootPath)
            ```

            ::: block
            Create a new instance of
            [`FileTreeCache`](FileTreeCache.html "class in com.facebook.buck.core.files")
            :::

            [Parameters:]{.paramLabel}
            :   `rootPath` - Absolute path to the root folder for which
                files and subfolders are cached, this is usually the
                root path of the cell

        []{#get(com.facebook.buck.core.files.FileTreeKey)}

        -   #### get

            ``` methodSignature
            public Optional<FileTree> get​(FileTreeKey key)
            ```

            ::: block
            [Description copied from
            interface: `GraphEngineCache`]{.descfrmTypeLabel}
            :::

            ::: block
            Optionally returns the cached result given the key
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `get` in
                interface `GraphEngineCache<FileTreeKey,​FileTree>`

            [Parameters:]{.paramLabel}
            :   `key` - The desired key

            [Returns:]{.returnLabel}
            :   the result if cached, otherwise an empty Optional

        []{#put(com.facebook.buck.core.files.FileTreeKey,com.facebook.buck.core.files.FileTree)}

        -   #### put

            ``` methodSignature
            public void put​(FileTreeKey key,
                            FileTree fileTree)
            ```

            ::: block
            [Description copied from
            interface: `GraphEngineCache`]{.descfrmTypeLabel}
            :::

            ::: block
            Offers the given key and value for caching
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `put` in
                interface `GraphEngineCache<FileTreeKey,​FileTree>`

            [Parameters:]{.paramLabel}
            :   `key` - the key to cache
            :   `fileTree` - the value to cache

        []{#getInvalidator()}

        -   #### getInvalidator

            ``` methodSignature
            public FileTreeCache.Invalidator getInvalidator()
            ```

            [Returns:]{.returnLabel}
            :   class that listens to watchman events and invalidates
                internal cache state
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
-   [Nested](#nested.class.summary) \| 
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
