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
[Package]{.packageLabelInType} [com.facebook.buck.parser](package-summary.html)
:::

## Class GenericFileParsePipeline\<T extends [FileManifest](api/FileManifest.html "interface in com.facebook.buck.parser.api")\> {#class-genericfileparsepipelinet-extends-filemanifest .title title="Class GenericFileParsePipeline"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.parser.GenericFileParsePipeline\<T\>

::: description
-   

    All Implemented Interfaces:
    :   `FileParsePipeline<T>`, `AutoCloseable`

    ```{=html}
    <!-- -->
    ```

    Direct Known Subclasses:
    :   `BuildFileRawNodeParsePipeline`, `PackageFileParsePipeline`

    ------------------------------------------------------------------------

        public class GenericFileParsePipeline<T extends FileManifest>
        extends Object
        implements FileParsePipeline<T>

    ::: block
    A pipeline that provides cached parsed results for a given file.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                                                                                                                Description
          -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `GenericFileParsePipeline​(com.facebook.buck.parser.PipelineNodeCache<AbsPath,​T> cache,                         com.facebook.buck.parser.FileParserPool<T> fileParserPool,                         com.google.common.util.concurrent.ListeningExecutorService executorService,                         BuckEventBus eventBus,                         Watchman watchman)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `void`                | `close()`             |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.c         | `getFileJo            | ::: block             |
        | ommon.util.concurrent | b​(Cell cell,          | Asynchronously obtain |
        | .ListenableFuture<T>` |   AbsPath buildFile)` | all                   |
        |                       |                       | [`TargetN             |
        |                       |                       | ode`](../core/model/t |
        |                       |                       | argetgraph/TargetNode |
        |                       |                       | .html "interface in c |
        |                       |                       | om.facebook.buck.core |
        |                       |                       | .model.targetgraph")s |
        |                       |                       | from a build file.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.parser.FileParsePipeline}

            ### Methods inherited from interface com.facebook.buck.parser.[FileParsePipeline](FileParsePipeline.html "interface in com.facebook.buck.parser")

            `getFile`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.parser.PipelineNodeCache,com.facebook.buck.parser.FileParserPool,com.google.common.util.concurrent.ListeningExecutorService,com.facebook.buck.event.BuckEventBus,com.facebook.buck.io.watchman.Watchman)}

        -   #### GenericFileParsePipeline

                public GenericFileParsePipeline​(com.facebook.buck.parser.PipelineNodeCache<AbsPath,​T> cache,
                                                com.facebook.buck.parser.FileParserPool<T> fileParserPool,
                                                com.google.common.util.concurrent.ListeningExecutorService executorService,
                                                BuckEventBus eventBus,
                                                Watchman watchman)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getFileJob(com.facebook.buck.core.cell.Cell,com.facebook.buck.core.filesystems.AbsPath)}

        -   #### getFileJob

            ``` methodSignature
            public com.google.common.util.concurrent.ListenableFuture<T> getFileJob​(Cell cell,
                                                                                    AbsPath buildFile)
                                                                             throws BuildTargetException
            ```

            ::: block
            [Description copied from
            interface: `FileParsePipeline`]{.descfrmTypeLabel}
            :::

            ::: block
            Asynchronously obtain all
            [`TargetNode`](../core/model/targetgraph/TargetNode.html "interface in com.facebook.buck.core.model.targetgraph")s
            from a build file. This will leverage previously cached raw
            contents of the file (if present) but will always loop over
            the contents, so repeated calls (with the same args) are not
            free.
            returned future may throw
            [`BuildFileParseException`](exceptions/BuildFileParseException.html "class in com.facebook.buck.parser.exceptions")
            and
            [`HumanReadableException`](../core/exceptions/HumanReadableException.html "class in com.facebook.buck.core.exceptions").
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getFileJob` in
                interface `FileParsePipeline<T extends FileManifest>`

            [Parameters:]{.paramLabel}
            :   `cell` - the
                [`Cell`](../core/cell/Cell.html "interface in com.facebook.buck.core.cell")
                that the build file belongs to.
            :   `buildFile` - absolute path to the file to process.

            [Returns:]{.returnLabel}
            :   future.

            [Throws:]{.throwsLabel}
            :   `BuildTargetException`

        []{#close()}

        -   #### close

            ``` methodSignature
            public void close()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `close` in interface `AutoCloseable`
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
