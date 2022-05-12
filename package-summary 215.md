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
-   Package
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

[]{#skip.navbar.top}
:::
:::

::: navPadding
 
:::
:::

::: {role="main"}
::: header
# Package com.facebook.buck.skylark.io.impl {#package-com.facebook.buck.skylark.io.impl .title title="Package"}
:::

::: contentContainer
-   +-----------------------------------+-----------------------------------+
    | Class                             | Description                       |
    +===================================+===================================+
    | [CachingGlobber]                  | ::: block                         |
    | (CachingGlobber.html "class in co | [`Glob                            |
    | m.facebook.buck.skylark.io.impl") | ber`](../Globber.html "interface  |
    |                                   | in com.facebook.buck.skylark.io") |
    |                                   | implementation that caches        |
    |                                   | expanded paths from previous      |
    |                                   | invocations and reuses them in    |
    |                                   | case the glob with same           |
    |                                   | [`Gl                              |
    |                                   | obSpec`](../GlobSpec.html "class  |
    |                                   | in com.facebook.buck.skylark.io") |
    |                                   | is requested again.               |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [HybridGlobber                    | ::: block                         |
    | ](HybridGlobber.html "class in co | A                                 |
    | m.facebook.buck.skylark.io.impl") | [`Glob                            |
    |                                   | ber`](../Globber.html "interface  |
    |                                   | in com.facebook.buck.skylark.io") |
    |                                   | implementation that tries to use  |
    |                                   | Watchman if it\'s available and   |
    |                                   | falls back to a fallback globber, |
    |                                   | in case Watchman query cannot be  |
    |                                   | fulfilled.                        |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [HybridGlobberFactory](Hybri      | ::: block                         |
    | dGlobberFactory.html "class in co | Provides instances of             |
    | m.facebook.buck.skylark.io.impl") | [`HybridGlobber`]                 |
    |                                   | (HybridGlobber.html "class in com |
    |                                   | .facebook.buck.skylark.io.impl"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [NativeGlobber                    | ::: block                         |
    | ](NativeGlobber.html "class in co | A Java native glob function       |
    | m.facebook.buck.skylark.io.impl") | implementation that allows        |
    |                                   | resolving file paths based on     |
    |                                   | include patterns (file patterns   |
    |                                   | that should be returned) minus    |
    |                                   | exclude patterns (file patterns   |
    |                                   | that should be excluded from the  |
    |                                   | resulting set).                   |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [SyncCookieState](                | ::: block                         |
    | SyncCookieState.html "class in co | Process-wide state used to enable |
    | m.facebook.buck.skylark.io.impl") | Watchman sync cookies only on the |
    |                                   | first query issued.               |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [WatchmanGlobber](                | ::: block                         |
    | WatchmanGlobber.html "class in co | An implementation of globbing     |
    | m.facebook.buck.skylark.io.impl") | functionality that allows         |
    |                                   | resolving file paths based on     |
    |                                   | include patterns (file patterns   |
    |                                   | that should be returned) minus    |
    |                                   | exclude patterns (file patterns   |
    |                                   | that should be excluded from the  |
    |                                   | resulting set) using Watchman     |
    |                                   | tool for improved performance.    |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+

    : Class Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Enum                              | Description                       |
    +===================================+===================================+
    | [WatchmanGlobber.Option](Watchm   | ::: block                         |
    | anGlobber.Option.html "enum in co | Watchman options to use when      |
    | m.facebook.buck.skylark.io.impl") | globbing.                         |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+

    : Enum Summary[ ]{.tabEnd}
:::
:::

::: bottomNav
[]{#navbar.bottom}

::: skipNav
[Skip navigation links](#skip.navbar.bottom "Skip navigation links")
:::

[]{#navbar.bottom.firstrow}

-   [Overview](../../../../../../index.html)
-   Package
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

[]{#skip.navbar.bottom}
:::
