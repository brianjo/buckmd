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
[Package]{.packageLabelInType} [com.facebook.buck.support.build.report](package-summary.html)
:::

## Class RequestUploader {#class-requestuploader .title title="Class RequestUploader"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.support.build.report.RequestUploader

::: description
-   

    ------------------------------------------------------------------------

        public class RequestUploader
        extends Object

    ::: block
    RequestUploader is only concerned with uploading and handling a
    request of type `  RequestBody` related to a buildId.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `String`              | `getBuildId()`        |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.facebook         | `uploa                |                       |
        | .buck.support.build.r | dRequest​(okhttp3.Requ |                       |
        | eport.UploadResponse` | estBody requestBody)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.facebook         | `u                    | ::: block             |
        | .buck.support.build.r | ploadRequest​(okhttp3. | Uploads the request   |
        | eport.UploadResponse` | RequestBody requestBo | to the build report   |
        |                       | dy,              com. | endpoint, adding      |
        |                       | google.common.collect | extra `queryParams`   |
        |                       | .ImmutableMap<String, | to the url.           |
        |                       | ​String> queryParams)` | :::                   |
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
    -   []{#method.detail}

        ### Method Detail

        []{#getBuildId()}

        -   #### getBuildId

            ``` methodSignature
            public String getBuildId()
            ```

        []{#uploadRequest(okhttp3.RequestBody)}

        -   #### uploadRequest

            ``` methodSignature
            public com.facebook.buck.support.build.report.UploadResponse uploadRequest​(okhttp3.RequestBody requestBody)
                                                                                throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#uploadRequest(okhttp3.RequestBody,com.google.common.collect.ImmutableMap)}

        -   #### uploadRequest

            ``` methodSignature
            public com.facebook.buck.support.build.report.UploadResponse uploadRequest​(okhttp3.RequestBody requestBody,
                                                                                       com.google.common.collect.ImmutableMap<String,​String> queryParams)
                                                                                throws IOException
            ```

            ::: block
            Uploads the request to the build report endpoint, adding
            extra `queryParams` to the url.
            :::

            [Throws:]{.throwsLabel}
            :   `IOException` - in case of a http error
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
