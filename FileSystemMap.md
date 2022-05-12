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
[Package]{.packageLabelInType} [com.facebook.buck.util.filesystem](package-summary.html)
:::

## Class FileSystemMap\<T\> {#class-filesystemmapt .title title="Class FileSystemMap"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.util.filesystem.FileSystemMap\<T\>

::: description
-   

    [Type Parameters:]{.paramLabel}
    :   `T` - The type to associate with a specific path.

    ------------------------------------------------------------------------

        public class FileSystemMap<T>
        extends Object

    ::: block
    This class implements a map for a filesystem structure relying on a
    prefix tree. The trie only supports relative paths for now, but an
    effort can be made in order to let it support absolute paths if
    needed. Every intermediate or leaf node of the trie is a folder/file
    which may be associated with a value. It\'s worth noting that adding
    a value for path foo/bar/file.txt will add intermediate nodes for
    foo and foo/bar but not values. The value is associated with the
    specified path and not with its ancestors. Invalidating one of the
    leaves or intermediate nodes will cause its parent and its ancestors
    to be invalidated as well: this operation consists in removing the
    leaf from its parent children and setting the value of all its
    ancestors to null. If the removal of the target leaf leaves an empty
    branch (a stump), that is removed as well in order to keep the
    prefix tree as slim as possible.
    This class is thread safe in its public methods: concurrent calls to
    the trie will have the exclusiveness in write/remove operations,
    while allowing parallel reads to the whole data structure: an
    attempt could be made to make the trie more concurrent by locking
    branches of the trie instead of the whole object, although that will
    require some thought around how to grant parallel writes.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static interface `   | `FileSyst             | ::: block             |
        |                       | emMap.ValueLoader<T>` | Wrapper class that    |
        |                       |                       | implements a method   |
        |                       |                       | for loading a value   |
        |                       |                       | in the leaves of the  |
        |                       |                       | trie.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                       Description
          ------------------------------------------------------------------------------------------------- -------------
          `FileSystemMap​(FileSystemMap.ValueLoader<T> loader,              ProjectFilesystem filesystem)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `com.g                | `asMap()`             | ::: block             |
        | oogle.common.collect. |                       | Returns a copy of the |
        | ImmutableMap<Path,​T>` |                       | leaves stored in the  |
        |                       |                       | trie as a map.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `T`                   | `get​(Path path)`      | ::: block             |
        |                       |                       | Gets the value        |
        |                       |                       | associated with the   |
        |                       |                       | given path.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `T`                   | `get                  | ::: block             |
        |                       | IfPresent​(Path path)` | Gets the value        |
        |                       |                       | associated with the   |
        |                       |                       | given path, if found, |
        |                       |                       | or \`null\`           |
        |                       |                       | otherwise.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `put​(Pa               | ::: block             |
        |                       | th path,    T value)` | Puts a path and a     |
        |                       |                       | value into the map.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `remove​(Path path)`   | ::: block             |
        |                       |                       | Removes the given     |
        |                       |                       | path.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `removeAll()`         | ::: block             |
        |                       |                       | Empties the trie      |
        |                       |                       | leaving only the root |
        |                       |                       | node available.       |
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

        []{#<init>(com.facebook.buck.util.filesystem.FileSystemMap.ValueLoader,com.facebook.buck.io.filesystem.ProjectFilesystem)}

        -   #### FileSystemMap

                public FileSystemMap​(FileSystemMap.ValueLoader<T> loader,
                                     ProjectFilesystem filesystem)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#put(java.nio.file.Path,java.lang.Object)}
        []{#put(java.nio.file.Path,T)}

        -   #### put

            ``` methodSignature
            public void put​(Path path,
                            T value)
            ```

            ::: block
            Puts a path and a value into the map.
            :::

            [Parameters:]{.paramLabel}
            :   `path` - The path to store.
            :   `value` - The value to associate to the given path.

        []{#remove(java.nio.file.Path)}

        -   #### remove

            ``` methodSignature
            public void remove​(Path path)
            ```

            ::: block
            Removes the given path.
            Removing a path involves the following:

            -   all the child nodes of the given path are discarded as
                well.
            -   all the paths upstream lose their value.
            -   each path upstream will be removed if after the removal
                of the leaf the node is left with no children (that is,
                it has become a stump).
            :::

            [Parameters:]{.paramLabel}
            :   `path` - The path specifying the branch to remove.

        []{#removeAll()}

        -   #### removeAll

            ``` methodSignature
            public void removeAll()
            ```

            ::: block
            Empties the trie leaving only the root node available.
            :::

        []{#get(java.nio.file.Path)}

        -   #### get

            ``` methodSignature
            public T get​(Path path)
            ```

            ::: block
            Gets the value associated with the given path.
            :::

            [Parameters:]{.paramLabel}
            :   `path` - The path to fetch.

            [Returns:]{.returnLabel}
            :   The value associated with the path.

        []{#getIfPresent(java.nio.file.Path)}

        -   #### getIfPresent

            ``` methodSignature
            @Nullable
            public T getIfPresent​(Path path)
            ```

            ::: block
            Gets the value associated with the given path, if found, or
            \`null\` otherwise.
            :::

            [Parameters:]{.paramLabel}
            :   `path` - The path to fetch.

            [Returns:]{.returnLabel}
            :   The value associated with the path.

        []{#asMap()}

        -   #### asMap

            ``` methodSignature
            public com.google.common.collect.ImmutableMap<Path,​T> asMap()
            ```

            ::: block
            Returns a copy of the leaves stored in the trie as a map.
            N.B.: this is quite an expensive call to make, so use it
            wisely.
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
-   [Nested](#nested.class.summary) \| 
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
