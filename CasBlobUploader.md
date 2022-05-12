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

-   [Overview](../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../deprecated-list.html)
-   [Index](../../../../index-all.html)
-   [Help](../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.remoteexecution](package-summary.html)
:::

## Interface CasBlobUploader {#interface-casblobuploader .title title="Interface CasBlobUploader"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `GrpcCasBlobUploader`

    ------------------------------------------------------------------------

        public interface CasBlobUploader

    ::: block
    Interface used to upload inputs/outputs to the CAS.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Interface             | Description           |
        +=======================+=======================+=======================+
        | `static class `       | `CasBlobU             | ::: block             |
        |                       | ploader.UploadResult` | Result (status/error  |
        |                       |                       | message) of an        |
        |                       |                       | upload.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                         Method                                                                                  Description
          ------------------------------------------------------------------------- --------------------------------------------------------------------------------------- -------------
          `com.google.common.collect.ImmutableList<CasBlobUploader.UploadResult>`   `batchUpdateBlobs​(com.google.common.collect.ImmutableList<UploadDataSupplier> build)`    
          `com.google.common.collect.ImmutableSet<String>`                          `getMissingHashes​(Set<Protocol.Digest> requiredDigests)`                                 
          `CasBlobUploader.UploadResult`                                            `uploadFromStream​(UploadDataSupplier build)`                                             

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

        []{#getMissingHashes(java.util.Set)}

        -   #### getMissingHashes

            ``` methodSignature
            com.google.common.collect.ImmutableSet<String> getMissingHashes​(Set<Protocol.Digest> requiredDigests)
                                                                     throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#batchUpdateBlobs(com.google.common.collect.ImmutableList)}

        -   #### batchUpdateBlobs

            ``` methodSignature
            com.google.common.collect.ImmutableList<CasBlobUploader.UploadResult> batchUpdateBlobs​(com.google.common.collect.ImmutableList<UploadDataSupplier> build)
                                                                                            throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#uploadFromStream(com.facebook.buck.remoteexecution.UploadDataSupplier)}

        -   #### uploadFromStream

            ``` methodSignature
            CasBlobUploader.UploadResult uploadFromStream​(UploadDataSupplier build)
                                                   throws IOException
            ```

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

-   [Overview](../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../deprecated-list.html)
-   [Index](../../../../index-all.html)
-   [Help](../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../allclasses.html)

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
