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
[Package]{.packageLabelInType} [com.facebook.buck.file.downloader](package-summary.html)
:::

## Interface Downloader {#interface-downloader .title title="Interface Downloader"}
:::

::: contentContainer
::: description
-   

    All Superinterfaces:
    :   `Toolchain`

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `ExplodingDownloader`, `HttpDownloader`,
        `OnDiskMavenDownloader`, `RemoteMavenDownloader`,
        `RetryingDownloader`, `StackedDownloader`

    ------------------------------------------------------------------------

        public interface Downloader
        extends Toolchain
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type   Field            Description
          ------------------- ---------------- -------------
          `static String`     `DEFAULT_NAME`    

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `boolean`             | `fetch​(BuckEventBus   | ::: block             |
        |                       | eventBus,      URI ur | Download the given    |
        |                       | i,      Path output)` | URL and, upon a       |
        |                       |                       | successful download,  |
        |                       |                       | place it in `output`. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `default String`      | `getName()`           |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
        .tableTab}[[Default
        Methods](javascript:show(16);)[ ]{.tabEnd}]{#t5 .tableTab}
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#field.detail}

        ### Field Detail

        []{#DEFAULT_NAME}

        -   #### DEFAULT_NAME

                static final String DEFAULT_NAME

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.file.downloader.Downloader.DEFAULT_NAME)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#fetch(com.facebook.buck.event.BuckEventBus,java.net.URI,java.nio.file.Path)}

        -   #### fetch

            ``` methodSignature
            boolean fetch​(BuckEventBus eventBus,
                          URI uri,
                          Path output)
                   throws IOException
            ```

            ::: block
            Download the given URL and, upon a successful download,
            place it in `output`. Note that if a `Downloader` can\'t
            handle the
            [`URI.scheme`](http://docs.oracle.com/javase/7/docs/api/java/net/URI.html?is-external=true#scheme "class or interface in java.net"){.externalLink}
            then `false` will be returned.
            :::

            [Returns:]{.returnLabel}
            :   Whether or not the download succeeded.

            [Throws:]{.throwsLabel}
            :   `IOException` - Should an exception be thrown when
                downloading.

        []{#getName()}

        -   #### getName

            ``` methodSignature
            default String getName()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getName` in interface `Toolchain`
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
