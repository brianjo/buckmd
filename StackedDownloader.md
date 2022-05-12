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
-   [Field](#field.summary) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.file.downloader.impl](package-summary.html)
:::

## Class StackedDownloader {#class-stackeddownloader .title title="Class StackedDownloader"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.file.downloader.impl.StackedDownloader

::: description
-   

    All Implemented Interfaces:
    :   `Toolchain`, `Downloader`

    ------------------------------------------------------------------------

        public class StackedDownloader
        extends Object
        implements Downloader

    ::: block
    A
    [`Downloader`](../Downloader.html "interface in com.facebook.buck.file.downloader")
    which is composed of many other downloaders. When asked to download
    a resource, these are each called in order until one succeeds or the
    final one fails.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        -   []{#fields.inherited.from.class.com.facebook.buck.file.downloader.Downloader}

            ### Fields inherited from interface com.facebook.buck.file.downloader.[Downloader](../Downloader.html "interface in com.facebook.buck.file.downloader")

            `DEFAULT_NAME`
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static Downloader`   | `createFr             |                       |
        |                       | omConfig​(BuckConfig c |                       |
        |                       | onfig,                |                       |
        |                       |   ToolchainProvider t |                       |
        |                       | oolchainProvider,     |                       |
        |                       |              TargetCo |                       |
        |                       | nfiguration toolchain |                       |
        |                       | TargetConfiguration)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `fetch​(BuckEventBus   | ::: block             |
        |                       | eventBus,      URI ur | Download the given    |
        |                       | i,      Path output)` | URL and, upon a       |
        |                       |                       | successful download,  |
        |                       |                       | place it in `output`. |
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
        -   []{#methods.inherited.from.class.com.facebook.buck.file.downloader.Downloader}

            ### Methods inherited from interface com.facebook.buck.file.downloader.[Downloader](../Downloader.html "interface in com.facebook.buck.file.downloader")

            `getName`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#createFromConfig(com.facebook.buck.core.config.BuckConfig,com.facebook.buck.core.toolchain.ToolchainProvider,com.facebook.buck.core.model.TargetConfiguration)}

        -   #### createFromConfig

            ``` methodSignature
            public static Downloader createFromConfig​(BuckConfig config,
                                                      ToolchainProvider toolchainProvider,
                                                      TargetConfiguration toolchainTargetConfiguration)
            ```

        []{#fetch(com.facebook.buck.event.BuckEventBus,java.net.URI,java.nio.file.Path)}

        -   #### fetch

            ``` methodSignature
            public boolean fetch​(BuckEventBus eventBus,
                                 URI uri,
                                 Path output)
            ```

            ::: block
            [Description copied from
            interface: `Downloader`]{.descfrmTypeLabel}
            :::

            ::: block
            Download the given URL and, upon a successful download,
            place it in `output`. Note that if a `Downloader` can\'t
            handle the
            [`URI.scheme`](http://docs.oracle.com/javase/7/docs/api/java/net/URI.html?is-external=true#scheme "class or interface in java.net"){.externalLink}
            then `false` will be returned.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `fetch` in interface `Downloader`

            [Returns:]{.returnLabel}
            :   Whether or not the download succeeded.
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
-   [Field](#field.summary) \| 
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
