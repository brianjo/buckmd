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
-   Method

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

## Class BuildFileRawNodeParsePipeline {#class-buildfilerawnodeparsepipeline .title title="Class BuildFileRawNodeParsePipeline"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.parser.GenericFileParsePipeline](GenericFileParsePipeline.html "class in com.facebook.buck.parser")\<[BuildFileManifest](api/BuildFileManifest.html "class in com.facebook.buck.parser.api")\>

    -   -   com.facebook.buck.parser.BuildFileRawNodeParsePipeline

::: description
-   

    All Implemented Interfaces:
    :   `FileParsePipeline<BuildFileManifest>`, `AutoCloseable`

    ------------------------------------------------------------------------

        public class BuildFileRawNodeParsePipeline
        extends GenericFileParsePipeline<BuildFileManifest>

    ::: block
    A pipeline that provides a
    [`BuildFileManifest`](api/BuildFileManifest.html "class in com.facebook.buck.parser.api")
    for a given build file.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                                                                                                                                                                              Description
          ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `BuildFileRawNodeParsePipeline​(com.facebook.buck.parser.PipelineNodeCache<AbsPath,​BuildFileManifest> cache,                              com.facebook.buck.parser.ProjectBuildFileParserPool projectBuildFileParserPool,                              com.google.common.util.concurrent.ListeningExecutorService executorService,                              BuckEventBus eventBus,                              Watchman watchman)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        -   []{#methods.inherited.from.class.com.facebook.buck.parser.GenericFileParsePipeline}

            ### Methods inherited from class com.facebook.buck.parser.[GenericFileParsePipeline](GenericFileParsePipeline.html "class in com.facebook.buck.parser")

            `close, getFileJob`

        ```{=html}
        <!-- -->
        ```
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

        []{#<init>(com.facebook.buck.parser.PipelineNodeCache,com.facebook.buck.parser.ProjectBuildFileParserPool,com.google.common.util.concurrent.ListeningExecutorService,com.facebook.buck.event.BuckEventBus,com.facebook.buck.io.watchman.Watchman)}

        -   #### BuildFileRawNodeParsePipeline

                public BuildFileRawNodeParsePipeline​(com.facebook.buck.parser.PipelineNodeCache<AbsPath,​BuildFileManifest> cache,
                                                     com.facebook.buck.parser.ProjectBuildFileParserPool projectBuildFileParserPool,
                                                     com.google.common.util.concurrent.ListeningExecutorService executorService,
                                                     BuckEventBus eventBus,
                                                     Watchman watchman)
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
-   Method

</div>

[]{#skip.navbar.bottom}
:::
