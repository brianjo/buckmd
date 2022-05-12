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
[Package]{.packageLabelInType} [com.facebook.buck.skylark.io.impl](package-summary.html)
:::

## Class HybridGlobberFactory {#class-hybridglobberfactory .title title="Class HybridGlobberFactory"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.skylark.io.impl.HybridGlobberFactory

::: description
-   

    All Implemented Interfaces:
    :   `GlobberFactory`

    ------------------------------------------------------------------------

        public class HybridGlobberFactory
        extends Object
        implements GlobberFactory

    ::: block
    Provides instances of
    [`HybridGlobber`](HybridGlobber.html "class in com.facebook.buck.skylark.io.impl").
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `Globber`             | `create​(com.goo       |                       |
        |                       | gle.devtools.build.li |                       |
        |                       | b.vfs.Path basePath)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getWatchmanRelativ   | ::: block             |
        | Optional<com.facebook | izedFinalPath​(com.goo | Ask Watchman to get   |
        | .buck.skylark.io.impl | gle.devtools.build.li | the final path for a  |
        | .HybridGlobberFactory | b.vfs.Path filePath)` | file, following links |
        | .WatchProjectResult>` |                       | (and ReparsePoints on |
        |                       |                       | Windows).             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static               | `using​(Watchm         |                       |
        | HybridGlobberFactory` | anClient watchmanClie |                       |
        |                       | nt,      SyncCookieSt |                       |
        |                       | ate syncCookieState,  |                       |
        |                       |      Path projectRoot |                       |
        |                       | ,      com.google.com |                       |
        |                       | mon.collect.Immutable |                       |
        |                       | Map<AbsPath,​ProjectWa |                       |
        |                       | tch> projectWatches)` |                       |
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

        []{#getWatchmanRelativizedFinalPath(com.google.devtools.build.lib.vfs.Path)}

        -   #### getWatchmanRelativizedFinalPath

            ``` methodSignature
            public Optional<com.facebook.buck.skylark.io.impl.HybridGlobberFactory.WatchProjectResult> getWatchmanRelativizedFinalPath​(com.google.devtools.build.lib.vfs.Path filePath)
                                                                                                                                throws IOException,
                                                                                                                                       InterruptedException
            ```

            ::: block
            Ask Watchman to get the final path for a file, following
            links (and ReparsePoints on Windows).
            :::

            [Parameters:]{.paramLabel}
            :   `filePath` - the path for which we want to get the final
                path.

            [Returns:]{.returnLabel}
            :   the inal path from Watchman for `filePath`, if Watchman
                is possible to calculate and `Optional.empty()`
                otherwise.

            [Throws:]{.throwsLabel}
            :   `IOException`
            :   `InterruptedException`

        []{#create(com.google.devtools.build.lib.vfs.Path)}

        -   #### create

            ``` methodSignature
            public Globber create​(com.google.devtools.build.lib.vfs.Path basePath)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `create` in interface `GlobberFactory`

        []{#using(com.facebook.buck.io.watchman.WatchmanClient,com.facebook.buck.skylark.io.impl.SyncCookieState,java.nio.file.Path,com.google.common.collect.ImmutableMap)}

        -   #### using

            ``` methodSignature
            public static HybridGlobberFactory using​(WatchmanClient watchmanClient,
                                                     SyncCookieState syncCookieState,
                                                     Path projectRoot,
                                                     com.google.common.collect.ImmutableMap<AbsPath,​ProjectWatch> projectWatches)
            ```
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
