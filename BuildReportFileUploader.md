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
[Package]{.packageLabelInType} [com.facebook.buck.support.build.report](package-summary.html)
:::

## Class BuildReportFileUploader {#class-buildreportfileuploader .title title="Class BuildReportFileUploader"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.support.build.report.BuildReportFileUploader

::: description
-   

    ------------------------------------------------------------------------

        public class BuildReportFileUploader
        extends Object

    ::: block
    A general way to upload any file to the build report endpoint
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                       Description
          ----------------------------------------------------------------------------------------------------------------- -------------
          `BuildReportFileUploader​(URL url,                        long timeout,                        BuildId buildId)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                         Method                                                                   Description
          --------------------------------------------------------- ------------------------------------------------------------------------ -------------
          `com.facebook.buck.support.build.report.UploadResponse`   `uploadDiffFile​(InputStream inputStream)`                                 
          `void`                                                    `uploadFile​(Path buildReportFilePath,           String traceFileKind)`    

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

        []{#<init>(java.net.URL,long,com.facebook.buck.core.model.BuildId)}

        -   #### BuildReportFileUploader

                public BuildReportFileUploader​(URL url,
                                               long timeout,
                                               BuildId buildId)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#uploadFile(java.nio.file.Path,java.lang.String)}

        -   #### uploadFile

            ``` methodSignature
            public void uploadFile​(Path buildReportFilePath,
                                   String traceFileKind)
            ```

            [Parameters:]{.paramLabel}
            :   `buildReportFilePath` - is the file to upload
            :   `traceFileKind` - is the type of file to associate it
                correctly to the build in the server

        []{#uploadDiffFile(java.io.InputStream)}

        -   #### uploadDiffFile

            ``` methodSignature
            public com.facebook.buck.support.build.report.UploadResponse uploadDiffFile​(InputStream inputStream)
                                                                                 throws IOException
            ```

            [Parameters:]{.paramLabel}
            :   `inputStream` - that has an input stream containing the
                output of \`hg export\` command see
                [`HgCmdLineInterface`](../../../util/versioncontrol/HgCmdLineInterface.html "class in com.facebook.buck.util.versioncontrol")
                for more info.

            [Returns:]{.returnLabel}
            :   the endpoints\' response

            [Throws:]{.throwsLabel}
            :   `IOException` - when an error occurs while executing the
                http call
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
