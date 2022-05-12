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
-   Field \| 
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   [Constr](#constructor.detail) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.remoteexecution.util](package-summary.html)
:::

## Class MultiThreadedBlobUploader {#class-multithreadedblobuploader .title title="Class MultiThreadedBlobUploader"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.remoteexecution.util.MultiThreadedBlobUploader

::: description
-   

    ------------------------------------------------------------------------

        public class MultiThreadedBlobUploader
        extends Object

    ::: block
    A simple multi-threaded blob uploader for uploading inputs/outputs
    to the CAS.
    Before uploading a file, the uploader will check if the CAS already
    contains it.

    All upload requests get added to a queue for the \"missing check\".
    Work threads will pull up to missingCheckLimit items off this queue
    and send a request to the CAS to find which it does/doesn\'t
    contain. Any that are missing will be added to a queue to be
    uploaded. Work threads will then pull those off and upload them.
    When the upload is finished, the future for that digest will be
    fulfilled.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static class `       | `MultiThre            | ::: block             |
        |                       | adedBlobUploader.Corr | An exception that     |
        |                       | uptArtifactException` | indicates that an     |
        |                       |                       | upload failed because |
        |                       |                       | the artifact was      |
        |                       |                       | corrupted.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                   Description
          ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `MultiThreadedBlobUploader​(int missingCheckLimit,                          int uploadSizeLimit,                          ExecutorService uploadService,                          CasBlobUploader delegate)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `com.google.comm      | `addMis               | ::: block             |
        | on.util.concurrent.Li | sing​(java.util.stream | Uploads missing items |
        | stenableFuture<Unit>` | .Stream<UploadDataSup | to the CAS.           |
        |                       | plier> dataSupplier)` | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `containsDigest​(Pro   |                       |
        |                       | tocol.Digest digest)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
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
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(int,int,java.util.concurrent.ExecutorService,com.facebook.buck.remoteexecution.CasBlobUploader)}

        -   #### MultiThreadedBlobUploader

                public MultiThreadedBlobUploader​(int missingCheckLimit,
                                                 int uploadSizeLimit,
                                                 ExecutorService uploadService,
                                                 CasBlobUploader delegate)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#containsDigest(com.facebook.buck.remoteexecution.interfaces.Protocol.Digest)}

        -   #### containsDigest

            ``` methodSignature
            public boolean containsDigest​(Protocol.Digest digest)
            ```

        []{#addMissing(java.util.stream.Stream)}

        -   #### addMissing

            ``` methodSignature
            public com.google.common.util.concurrent.ListenableFuture<Unit> addMissing​(java.util.stream.Stream<UploadDataSupplier> dataSupplier)
            ```

            ::: block
            Uploads missing items to the CAS.
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
-   [Nested](#nested.class.summary) \| 
-   Field \| 
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   [Constr](#constructor.detail) \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
