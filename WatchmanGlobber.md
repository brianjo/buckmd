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
[Package]{.packageLabelInType} [com.facebook.buck.skylark.io.impl](package-summary.html)
:::

## Class WatchmanGlobber {#class-watchmanglobber .title title="Class WatchmanGlobber"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.skylark.io.impl.WatchmanGlobber

::: description
-   

    ------------------------------------------------------------------------

        public class WatchmanGlobber
        extends Object

    ::: block
    An implementation of globbing functionality that allows resolving
    file paths based on include patterns (file patterns that should be
    returned) minus exclude patterns (file patterns that should be
    excluded from the resulting set) using Watchman tool for improved
    performance.
    The implementation is mostly compatible with glob_watchman.py and as
    such differs from the
    [`NativeGlobber`](NativeGlobber.html "class in com.facebook.buck.skylark.io.impl")
    in certain ways:

    -   does not fail for patterns that cannot possibly match
    -   does not collapse multiple slashes
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static class `       | `Wa                   | ::: block             |
        |                       | tchmanGlobber.Option` | Watchman options to   |
        |                       |                       | use when globbing.    |
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
        | `st                   | `create               | ::: block             |
        | atic WatchmanGlobber` | ​(WatchmanClient watch | Factory method for    |
        |                       | manClient,       Sync | creating              |
        |                       | CookieState syncCooki | [`                    |
        |                       | eState,       String  | WatchmanGlobber`](Wat |
        |                       | basePath,       Strin | chmanGlobber.html "cl |
        |                       | g watchmanWatchRoot)` | ass in com.facebook.b |
        |                       |                       | uck.skylark.io.impl") |
        |                       |                       | instances.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<com.go      | `run​(Collec           |                       |
        | ogle.common.collect.I | tion<String> include, |                       |
        | mmutableSet<String>>` |     Collection<String |                       |
        |                       | > exclude,    boolean |                       |
        |                       |  excludeDirectories)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<com.go      | `run​(Collectio        |                       |
        | ogle.common.collect.I | n<String> include,    |                       |
        | mmutableSet<String>>` |  Collection<String> e |                       |
        |                       | xclude,    WatchmanGl |                       |
        |                       | obber.Option option)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<com.go      | `ru                   |                       |
        | ogle.common.collect.I | n​(Collection<String>  |                       |
        | mmutableSet<String>>` | include,    Collectio |                       |
        |                       | n<String> exclude,    |                       |
        |                       |  EnumSet<WatchmanGlob |                       |
        |                       | ber.Option> options)` |                       |
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

        []{#run(java.util.Collection,java.util.Collection,boolean)}

        -   #### run

            ``` methodSignature
            public Optional<com.google.common.collect.ImmutableSet<String>> run​(Collection<String> include,
                                                                                Collection<String> exclude,
                                                                                boolean excludeDirectories)
                                                                         throws IOException,
                                                                                InterruptedException
            ```

            [Parameters:]{.paramLabel}
            :   `include` - File patterns that should be included in the
                resulting set.
            :   `exclude` - File patterns that should be excluded from
                the resulting set.
            :   `excludeDirectories` - Whether directories should be
                excluded from the resulting set.

            [Returns:]{.returnLabel}
            :   The set of paths resolved using include patterns minus
                paths excluded by exclude patterns.

            [Throws:]{.throwsLabel}
            :   `IOException`
            :   `InterruptedException`

            [See Also:]{.seeLabel}
            :   [`run(Collection, Collection, EnumSet)`](#run(java.util.Collection,java.util.Collection,java.util.EnumSet))

        []{#run(java.util.Collection,java.util.Collection,com.facebook.buck.skylark.io.impl.WatchmanGlobber.Option)}

        -   #### run

            ``` methodSignature
            public Optional<com.google.common.collect.ImmutableSet<String>> run​(Collection<String> include,
                                                                                Collection<String> exclude,
                                                                                WatchmanGlobber.Option option)
                                                                         throws IOException,
                                                                                InterruptedException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`
            :   `InterruptedException`

        []{#run(java.util.Collection,java.util.Collection,java.util.EnumSet)}

        -   #### run

            ``` methodSignature
            public Optional<com.google.common.collect.ImmutableSet<String>> run​(Collection<String> include,
                                                                                Collection<String> exclude,
                                                                                EnumSet<WatchmanGlobber.Option> options)
                                                                         throws IOException,
                                                                                InterruptedException,
                                                                                WatchmanQueryFailedException
            ```

            [Parameters:]{.paramLabel}
            :   `include` - File patterns that should be included in the
                resulting set.
            :   `exclude` - File patterns that should be excluded from
                the resulting set.
            :   `options` - Customizations for matching behavior.

            [Returns:]{.returnLabel}
            :   The set of paths resolved using include patterns minus
                paths excluded by exclude patterns.

            [Throws:]{.throwsLabel}
            :   `WatchmanQueryFailedException` - Watchman returned an
                error response.
            :   `IOException`
            :   `InterruptedException`

        []{#create(com.facebook.buck.io.watchman.WatchmanClient,com.facebook.buck.skylark.io.impl.SyncCookieState,java.lang.String,java.lang.String)}

        -   #### create

            ``` methodSignature
            public static WatchmanGlobber create​(WatchmanClient watchmanClient,
                                                 SyncCookieState syncCookieState,
                                                 String basePath,
                                                 String watchmanWatchRoot)
            ```

            ::: block
            Factory method for creating
            [`WatchmanGlobber`](WatchmanGlobber.html "class in com.facebook.buck.skylark.io.impl")
            instances.
            :::

            [Parameters:]{.paramLabel}
            :   `basePath` - The base path relative to which paths
                matching glob patterns will be resolved.
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
