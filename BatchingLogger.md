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
[Package]{.packageLabelInType} [com.facebook.buck.util.network](package-summary.html)
:::

## Interface BatchingLogger {#interface-batchinglogger .title title="Interface BatchingLogger"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `AbstractBatchingLogger`, `ScribeBatchingLogger`

    ------------------------------------------------------------------------

        public interface BatchingLogger

    ::: block
    Implemented by classes providing the functionality to upload log
    data in batches.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `com.google.comm      | `forceFlush()`        | ::: block             |
        | on.util.concurrent.Li |                       | Signals to upload     |
        | stenableFuture<Unit>` |                       | whatever remaining    |
        |                       |                       | information is        |
        |                       |                       | buffered.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Opti                 | `log​(String logLine)` |                       |
        | onal<com.google.commo |                       |                       |
        | n.util.concurrent.Lis |                       |                       |
        | tenableFuture<Unit>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#log(java.lang.String)}

        -   #### log

            ``` methodSignature
            Optional<com.google.common.util.concurrent.ListenableFuture<Unit>> log​(String logLine)
            ```

            [Parameters:]{.paramLabel}
            :   `logLine` - data to upload.

            [Returns:]{.returnLabel}
            :   [`Optional.empty()`](http://docs.oracle.com/javase/7/docs/api/java/util/Optional.html?is-external=true#empty() "class or interface in java.util"){.externalLink}
                if the data has merely been buffered, a
                `ListenableFuture` representing the upload otherwise.

        []{#forceFlush()}

        -   #### forceFlush

            ``` methodSignature
            com.google.common.util.concurrent.ListenableFuture<Unit> forceFlush()
            ```

            ::: block
            Signals to upload whatever remaining information is
            buffered.
            :::

            [Returns:]{.returnLabel}
            :   future representing the forced upload.
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
