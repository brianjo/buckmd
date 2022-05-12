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
-   [Field](#field.summary) \| 
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.io.file](package-summary.html)
:::

## Class PathListing {#class-pathlisting .title title="Class PathListing"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.io.file.PathListing

::: description
-   

    ------------------------------------------------------------------------

        public class PathListing
        extends Object

    ::: block
    Utility class to list files which match a pattern, applying ordering
    and filtering.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static class `       | `Pa                   | ::: block             |
        |                       | thListing.FilterMode` | Whether to include    |
        |                       |                       | files which match the |
        |                       |                       | filter, or exclude    |
        |                       |                       | them.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static interface `   | `PathListing.Pat      | ::: block             |
        |                       | hModifiedTimeFetcher` | Fetches last-modified |
        |                       |                       | time from a path.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Field                 | Description           |
        +=======================+=======================+=======================+
        | `s                    | `GE                   | ::: block             |
        | tatic PathListing.Pat | T_PATH_MODIFIED_TIME` | Uses                  |
        | hModifiedTimeFetcher` |                       | `Files.g              |
        |                       |                       | etLastModifiedTime()` |
        |                       |                       | to get the last       |
        |                       |                       | modified time for a   |
        |                       |                       | Path.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static com.googl     | `lis                  | ::: block             |
        | e.common.collect.Immu | tMatchingPaths​(Path p | Lists matching paths  |
        | tableSortedSet<Path>` | athToGlob,            | in descending         |
        |                       |        String globPat | modified time order.  |
        |                       | tern,                 | :::                   |
        |                       |   PathListing.PathMod |                       |
        |                       | ifiedTimeFetcher path |                       |
        |                       | ModifiedTimeFetcher)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static com.googl     | `listM                | ::: block             |
        | e.common.collect.Immu | atchingPathsWithFilte | Lists paths in        |
        | tableSortedSet<Path>` | rs​(Path pathToGlob,   | descending modified   |
        |                       |                       | time order, excluding |
        |                       |       String globPatt | any paths which bring |
        |                       | ern,                  | the number of files   |
        |                       |             PathListi | over `maxNumPaths` or |
        |                       | ng.PathModifiedTimeFe | over                  |
        |                       | tcher pathModifiedTim | `totalSizeFilter`     |
        |                       | eFetcher,             | bytes in size.        |
        |                       |                  Path | :::                   |
        |                       | Listing.FilterMode fi |                       |
        |                       | lterMode,             |                       |
        |                       |                  Opti |                       |
        |                       | onalInt maxPathsFilte |                       |
        |                       | r,                    |                       |
        |                       |           Optional<Lo |                       |
        |                       | ng> totalSizeFilter)` |                       |
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
    -   []{#field.detail}

        ### Field Detail

        []{#GET_PATH_MODIFIED_TIME}

        -   #### GET_PATH_MODIFIED_TIME

                public static final PathListing.PathModifiedTimeFetcher GET_PATH_MODIFIED_TIME

            ::: block
            Uses `Files.getLastModifiedTime()` to get the last modified
            time for a Path.
            :::
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#listMatchingPaths(java.nio.file.Path,java.lang.String,com.facebook.buck.io.file.PathListing.PathModifiedTimeFetcher)}

        -   #### listMatchingPaths

            ``` methodSignature
            public static com.google.common.collect.ImmutableSortedSet<Path> listMatchingPaths​(Path pathToGlob,
                                                                                               String globPattern,
                                                                                               PathListing.PathModifiedTimeFetcher pathModifiedTimeFetcher)
                                                                                        throws IOException
            ```

            ::: block
            Lists matching paths in descending modified time order.
            :::

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#listMatchingPathsWithFilters(java.nio.file.Path,java.lang.String,com.facebook.buck.io.file.PathListing.PathModifiedTimeFetcher,com.facebook.buck.io.file.PathListing.FilterMode,java.util.OptionalInt,java.util.Optional)}

        -   #### listMatchingPathsWithFilters

            ``` methodSignature
            public static com.google.common.collect.ImmutableSortedSet<Path> listMatchingPathsWithFilters​(Path pathToGlob,
                                                                                                          String globPattern,
                                                                                                          PathListing.PathModifiedTimeFetcher pathModifiedTimeFetcher,
                                                                                                          PathListing.FilterMode filterMode,
                                                                                                          OptionalInt maxPathsFilter,
                                                                                                          Optional<Long> totalSizeFilter)
                                                                                                   throws IOException
            ```

            ::: block
            Lists paths in descending modified time order, excluding any
            paths which bring the number of files over `maxNumPaths` or
            over `totalSizeFilter` bytes in size.
            :::

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
-   [Field](#field.summary) \| 
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
-   Constr \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
