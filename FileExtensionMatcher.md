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

## Class FileExtensionMatcher {#class-fileextensionmatcher .title title="Class FileExtensionMatcher"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.io.filesystem.FileExtensionMatcher

::: description
-   

    All Implemented Interfaces:
    :   `PathMatcher`, `PathMatcher`

    ------------------------------------------------------------------------

        public class FileExtensionMatcher
        extends Object
        implements PathMatcher

    ::: block
    Matcher that matches file paths with specific extension.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `boolean`             | `                     |                       |
        |                       | equals​(Object other)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getPathOrGlob()`     | ::: block             |
        |                       |                       | Returns a path or     |
        |                       |                       | glob pattern          |
        |                       |                       | identifying paths     |
        |                       |                       | that should be        |
        |                       |                       | matched by this       |
        |                       |                       | matcher.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `hashCode()`          |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `matches​(Path path)`  |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static               | `                     |                       |
        | FileExtensionMatcher` | of​(String extension)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `toString()`          |                       |
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

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, finalize, getClass, notify, notifyAll, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#equals(java.lang.Object)}

        -   #### equals

            ``` methodSignature
            public boolean equals​(Object other)
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `equals` in class `Object`

        []{#hashCode()}

        -   #### hashCode

            ``` methodSignature
            public int hashCode()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `hashCode` in class `Object`

        []{#toString()}

        -   #### toString

            ``` methodSignature
            public String toString()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `toString` in class `Object`

        []{#matches(java.nio.file.Path)}

        -   #### matches

            ``` methodSignature
            public boolean matches​(Path path)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `matches` in interface `PathMatcher`

        []{#toWatchmanMatchQuery(java.util.Set)}

        -   #### toWatchmanMatchQuery

            ``` methodSignature
            public com.google.common.collect.ImmutableList<?> toWatchmanMatchQuery​(Set<Capability> capabilities)
            ```

            ::: block
            [Description copied from
            interface: `PathMatcher`]{.descfrmTypeLabel}
            :::

            ::: block
            Transforms this matcher into a Watchman match query
            arguments matching the same set of paths as this matcher.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `toWatchmanMatchQuery` in interface `PathMatcher`

        []{#getPathOrGlob()}

        -   #### getPathOrGlob

            ``` methodSignature
            public String getPathOrGlob()
            ```

            ::: block
            [Description copied from
            interface: `PathMatcher`]{.descfrmTypeLabel}
            :::

            ::: block
            Returns a path or glob pattern identifying paths that should
            be matched by this matcher.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getPathOrGlob` in interface `PathMatcher`

        []{#of(java.lang.String)}

        -   #### of

            ``` methodSignature
            public static FileExtensionMatcher of​(String extension)
            ```

            [Returns:]{.returnLabel}
            :   The matcher for paths that have `extension` as an
                extension.
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
