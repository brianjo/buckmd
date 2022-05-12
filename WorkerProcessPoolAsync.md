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
[Package]{.packageLabelInType} [com.facebook.buck.worker](package-summary.html)
:::

## Class WorkerProcessPoolAsync {#class-workerprocesspoolasync .title title="Class WorkerProcessPoolAsync"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.worker.WorkerProcessPoolAsync

::: description
-   

    All Implemented Interfaces:
    :   `WorkerProcessPool`, `Closeable`, `AutoCloseable`

    ------------------------------------------------------------------------

        public class WorkerProcessPoolAsync
        extends Object
        implements WorkerProcessPool
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                       Description
          ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `WorkerProcessPoolAsync​(int maxRequests,                       com.google.common.hash.HashCode poolHash,                       ThrowingSupplier<WorkerProcess,​IOException> startWorkerProcess)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                       Method                                Description
          ----------------------------------------------------------------------- ------------------------------------- -------------
          `void`                                                                  `close()`                              
          `int`                                                                   `getCapacity()`                        
          `com.google.common.hash.HashCode`                                       `getPoolHash()`                        
          `com.google.common.util.concurrent.ListenableFuture<WorkerJobResult>`   `submitJob​(String expandedJobArgs)`    

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

        []{#<init>(int,com.google.common.hash.HashCode,com.facebook.buck.util.function.ThrowingSupplier)}

        -   #### WorkerProcessPoolAsync

                public WorkerProcessPoolAsync​(int maxRequests,
                                              com.google.common.hash.HashCode poolHash,
                                              ThrowingSupplier<WorkerProcess,​IOException> startWorkerProcess)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getPoolHash()}

        -   #### getPoolHash

            ``` methodSignature
            public com.google.common.hash.HashCode getPoolHash()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getPoolHash` in interface `WorkerProcessPool`

        []{#getCapacity()}

        -   #### getCapacity

            ``` methodSignature
            public int getCapacity()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getCapacity` in interface `WorkerProcessPool`

        []{#submitJob(java.lang.String)}

        -   #### submitJob

            ``` methodSignature
            public com.google.common.util.concurrent.ListenableFuture<WorkerJobResult> submitJob​(String expandedJobArgs)
                                                                                          throws IOException,
                                                                                                 InterruptedException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `submitJob` in interface `WorkerProcessPool`

            [Throws:]{.throwsLabel}
            :   `IOException`
            :   `InterruptedException`

        []{#close()}

        -   #### close

            ``` methodSignature
            public void close()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `close` in interface `AutoCloseable`

            [Specified by:]{.overrideSpecifyLabel}
            :   `close` in interface `Closeable`

            [Specified by:]{.overrideSpecifyLabel}
            :   `close` in interface `WorkerProcessPool`
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