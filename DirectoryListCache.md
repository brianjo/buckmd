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

## Class DirectoryListCache {#class-directorylistcache .title title="Class DirectoryListCache"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.files.DirectoryListCache

::: description
-   

    All Implemented Interfaces:
    :   `GraphEngineCache<DirectoryListKey,​DirectoryList>`

    ------------------------------------------------------------------------

        public class DirectoryListCache
        extends Object
        implements GraphEngineCache<DirectoryListKey,​DirectoryList>

    ::: block
    Stores a list of files and subfolders per each folder
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static class `       | `DirectoryL           | ::: block             |
        |                       | istCache.Invalidator` | Subscribes to         |
        |                       |                       | watchman event and    |
        |                       |                       | invalidates internal  |
        |                       |                       | state of a provided   |
        |                       |                       | [`D                   |
        |                       |                       | irectoryListCache`](D |
        |                       |                       | irectoryListCache.htm |
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
        | `Opt                  | `get​(D                | ::: block             |
        | ional<DirectoryList>` | irectoryListKey key)` | Optionally returns    |
        |                       |                       | the cached result     |
        |                       |                       | given the key         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `DirectoryL           | `getInvalidator()`    |                       |
        | istCache.Invalidator` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `stati                | `of​(Path rootPath)`   | ::: block             |
        | c DirectoryListCache` |                       | Create a new instance |
        |                       |                       | of                    |
        |                       |                       | [`D                   |
        |                       |                       | irectoryListCache`](D |
        |                       |                       | irectoryListCache.htm |
        |                       |                       | l "class in com.faceb |
        |                       |                       | ook.buck.core.files") |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `put​(DirectoryLis     | ::: block             |
        |                       | tKey key,    Director | Offers the given key  |
        |                       | yList directoryList)` | and value for caching |
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
            public static DirectoryListCache of​(Path rootPath)
            ```

            ::: block
            Create a new instance of
            [`DirectoryListCache`](DirectoryListCache.html "class in com.facebook.buck.core.files")
            :::

            [Parameters:]{.paramLabel}
            :   `rootPath` - Absolute path to the root folder for which
                files and subfolders are cached

        []{#get(com.facebook.buck.core.files.DirectoryListKey)}

        -   #### get

            ``` methodSignature
            public Optional<DirectoryList> get​(DirectoryListKey key)
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
                interface `GraphEngineCache<DirectoryListKey,​DirectoryList>`

            [Parameters:]{.paramLabel}
            :   `key` - The desired key

            [Returns:]{.returnLabel}
            :   the result if cached, otherwise an empty Optional

        []{#put(com.facebook.buck.core.files.DirectoryListKey,com.facebook.buck.core.files.DirectoryList)}

        -   #### put

            ``` methodSignature
            public void put​(DirectoryListKey key,
                            DirectoryList directoryList)
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
                interface `GraphEngineCache<DirectoryListKey,​DirectoryList>`

            [Parameters:]{.paramLabel}
            :   `key` - the key to cache
            :   `directoryList` - the value to cache

        []{#getInvalidator()}

        -   #### getInvalidator

            ``` methodSignature
            public DirectoryListCache.Invalidator getInvalidator()
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
