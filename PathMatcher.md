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
[Package]{.packageLabelInType} [com.facebook.buck.io.filesystem](package-summary.html)
:::

## Interface PathMatcher {#interface-pathmatcher .title title="Interface PathMatcher"}
:::

::: contentContainer
::: description
-   

    All Superinterfaces:
    :   `PathMatcher`

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `ExactPathMatcher`, `FileExtensionMatcher`,
        `GlobPatternMatcher`, `RecursiveFileMatcher`

    ------------------------------------------------------------------------

        public interface PathMatcher
        extends PathMatcher

    ::: block
    A contract for matching
    [`Path`](http://docs.oracle.com/javase/7/docs/api/java/nio/file/Path.html?is-external=true "class or interface in java.nio.file"){.externalLink}s.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `String`              | `getPathOrGlob()`     | ::: block             |
        |                       |                       | Returns a path or     |
        |                       |                       | glob pattern          |
        |                       |                       | identifying paths     |
        |                       |                       | that should be        |
        |                       |                       | matched by this       |
        |                       |                       | matcher.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `c                    | `toWatchma            | ::: block             |
        | om.google.common.coll | nMatchQuery​(Set<Capab | Transforms this       |
        | ect.ImmutableList<?>` | ility> capabilities)` | matcher into a        |
        |                       |                       | Watchman match query  |
        |                       |                       | arguments matching    |
        |                       |                       | the same set of paths |
        |                       |                       | as this matcher.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}

        -   []{#methods.inherited.from.class.java.nio.file.PathMatcher}

            ### Methods inherited from interface java.nio.file.[PathMatcher](http://docs.oracle.com/javase/7/docs/api/java/nio/file/PathMatcher.html?is-external=true "class or interface in java.nio.file"){.externalLink}

            `matches`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#toWatchmanMatchQuery(java.util.Set)}

        -   #### toWatchmanMatchQuery

            ``` methodSignature
            com.google.common.collect.ImmutableList<?> toWatchmanMatchQuery​(Set<Capability> capabilities)
            ```

            ::: block
            Transforms this matcher into a Watchman match query
            arguments matching the same set of paths as this matcher.
            :::

        []{#getPathOrGlob()}

        -   #### getPathOrGlob

            ``` methodSignature
            String getPathOrGlob()
            ```

            ::: block
            Returns a path or glob pattern identifying paths that should
            be matched by this matcher.
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
