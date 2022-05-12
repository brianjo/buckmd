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

## Class FileTreeFileNameIterator {#class-filetreefilenameiterator .title title="Class FileTreeFileNameIterator"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.files.FileTreeFileNameIterator

::: description
-   

    All Implemented Interfaces:
    :   `Iterator<Path>`

    ------------------------------------------------------------------------

        public class FileTreeFileNameIterator
        extends Object
        implements Iterator<Path>

    ::: block
    Iterator which recursively traverses
    [`FileTree`](FileTree.html "class in com.facebook.buck.core.files")
    searching for specific file name Returns relative Path of that file
    including file name itself This type of iterator is useful for
    finding all build files under some path
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `boolean`             | `hasNext()`           |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Path`                | `next()`              |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static File          | `of​(FileTree fileTree | ::: block             |
        | TreeFileNameIterator` | ,   String fileName)` | Create new instance   |
        |                       |                       | of                    |
        |                       |                       | [`FileTreeFileN       |
        |                       |                       | ameIterator`](FileTre |
        |                       |                       | eFileNameIterator.htm |
        |                       |                       | l "class in com.faceb |
        |                       |                       | ook.buck.core.files") |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `s                    | `ofIterable​(File      | ::: block             |
        | tatic Iterable<Path>` | Tree fileTree,        | Create new instance   |
        |                       |     String fileName)` | of                    |
        |                       |                       | [`FileTreeFileN       |
        |                       |                       | ameIterator`](FileTre |
        |                       |                       | eFileNameIterator.htm |
        |                       |                       | l "class in com.faceb |
        |                       |                       | ook.buck.core.files") |
        |                       |                       | and return it as      |
        |                       |                       | [`Iterable`](http:    |
        |                       |                       | //docs.oracle.com/jav |
        |                       |                       | ase/7/docs/api/java/l |
        |                       |                       | ang/Iterable.html?is- |
        |                       |                       | external=true "class  |
        |                       |                       | or interface in java. |
        |                       |                       | lang"){.externalLink} |
        |                       |                       | which can be used in  |
        |                       |                       | for loop              |
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

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.util.Iterator}

            ### Methods inherited from interface java.util.[Iterator](http://docs.oracle.com/javase/7/docs/api/java/util/Iterator.html?is-external=true "class or interface in java.util"){.externalLink}

            `forEachRemaining, remove`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#of(com.facebook.buck.core.files.FileTree,java.lang.String)}

        -   #### of

            ``` methodSignature
            public static FileTreeFileNameIterator of​(FileTree fileTree,
                                                      String fileName)
            ```

            ::: block
            Create new instance of
            [`FileTreeFileNameIterator`](FileTreeFileNameIterator.html "class in com.facebook.buck.core.files")
            :::

            [Parameters:]{.paramLabel}
            :   `fileTree` - File tree to recursively iterate
            :   `fileName` - File name to search for, for example
                \"BUCK\"

        []{#ofIterable(com.facebook.buck.core.files.FileTree,java.lang.String)}

        -   #### ofIterable

            ``` methodSignature
            public static Iterable<Path> ofIterable​(FileTree fileTree,
                                                    String fileName)
            ```

            ::: block
            Create new instance of
            [`FileTreeFileNameIterator`](FileTreeFileNameIterator.html "class in com.facebook.buck.core.files")
            and return it as
            [`Iterable`](http://docs.oracle.com/javase/7/docs/api/java/lang/Iterable.html?is-external=true "class or interface in java.lang"){.externalLink}
            which can be used in for loop
            :::

            [Parameters:]{.paramLabel}
            :   `fileTree` - File tree to recursively iterate
            :   `fileName` - File name to search for, for example
                \"BUCK\"

        []{#hasNext()}

        -   #### hasNext

            ``` methodSignature
            public boolean hasNext()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `hasNext` in interface `Iterator<Path>`

        []{#next()}

        -   #### next

            ``` methodSignature
            public Path next()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `next` in interface `Iterator<Path>`
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
