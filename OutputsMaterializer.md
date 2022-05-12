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

## Class OutputsMaterializer {#class-outputsmaterializer .title title="Class OutputsMaterializer"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.remoteexecution.util.OutputsMaterializer

::: description
-   

    ------------------------------------------------------------------------

        public class OutputsMaterializer
        extends Object

    ::: block
    Used for materializing outputs from the CAS.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static class `       | `Outpu                | ::: block             |
        |                       | tsMaterializer.Filesy | Simple default file   |
        |                       | stemFileMaterializer` | materializer that     |
        |                       |                       | actually materializes |
        |                       |                       | things on the         |
        |                       |                       | filesystem.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static class `       | `O                    | ::: block             |
        |                       | utputsMaterializer.Pe | Container class for   |
        |                       | ndingMaterialization` | pending               |
        |                       |                       | materialization       |
        |                       |                       | requests              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                     Description
          ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `OutputsMaterializer​(int sizeLimit,                    ExecutorService materializerService,                    AsyncBlobFetcher fetcher,                    Protocol protocol,                    BuckEventBus buckEventBus)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `com.google.comm      | `materia              | ::: block             |
        | on.util.concurrent.Li | lize​(Collection<Proto | Materialize the       |
        | stenableFuture<Unit>` | col.OutputDirectory>  | outputs of an action  |
        |                       | outputDirectories,    | into a directory.     |
        |                       |          Collection<P | :::                   |
        |                       | rotocol.OutputFile> o |                       |
        |                       | utputFiles,           |                       |
        |                       |   ContentAddressedSto |                       |
        |                       | rageClient.FileMateri |                       |
        |                       | alizer materializer)` |                       |
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

        []{#<init>(int,java.util.concurrent.ExecutorService,com.facebook.buck.remoteexecution.AsyncBlobFetcher,com.facebook.buck.remoteexecution.interfaces.Protocol,com.facebook.buck.event.BuckEventBus)}

        -   #### OutputsMaterializer

                public OutputsMaterializer​(int sizeLimit,
                                           ExecutorService materializerService,
                                           AsyncBlobFetcher fetcher,
                                           Protocol protocol,
                                           BuckEventBus buckEventBus)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#materialize(java.util.Collection,java.util.Collection,com.facebook.buck.remoteexecution.ContentAddressedStorageClient.FileMaterializer)}

        -   #### materialize

            ``` methodSignature
            public com.google.common.util.concurrent.ListenableFuture<Unit> materialize​(Collection<Protocol.OutputDirectory> outputDirectories,
                                                                                        Collection<Protocol.OutputFile> outputFiles,
                                                                                        ContentAddressedStorageClient.FileMaterializer materializer)
                                                                                 throws IOException
            ```

            ::: block
            Materialize the outputs of an action into a directory.
            :::

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
