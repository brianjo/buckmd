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
[Package]{.packageLabelInType} [com.facebook.buck.remoteexecution.util](package-summary.html)
:::

## Class OutputsMaterializer.PendingMaterialization {#class-outputsmaterializer.pendingmaterialization .title title="Class OutputsMaterializer.PendingMaterialization"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.remoteexecution.util.OutputsMaterializer.PendingMaterialization

::: description
-   

    Enclosing class:
    :   [OutputsMaterializer](OutputsMaterializer.html "class in com.facebook.buck.remoteexecution.util")

    ------------------------------------------------------------------------

        public static class OutputsMaterializer.PendingMaterialization
        extends Object

    ::: block
    Container class for pending materialization requests
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type                                          Field            Description
          ---------------------------------------------------------- ---------------- -------------
          `Protocol.Digest`                                          `digest`          
          `com.google.common.util.concurrent.SettableFuture<Unit>`   `future`          
          `boolean`                                                  `isExecutable`    
          `ContentAddressedStorageClient.FileMaterializer`           `materializer`    
          `Path`                                                     `path`            

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#field.detail}

        ### Field Detail

        []{#materializer}

        -   #### materializer

                public final ContentAddressedStorageClient.FileMaterializer materializer

        []{#digest}

        -   #### digest

                public final Protocol.Digest digest

        []{#isExecutable}

        -   #### isExecutable

                public final boolean isExecutable

        []{#path}

        -   #### path

                public final Path path

        []{#future}

        -   #### future

                public final com.google.common.util.concurrent.SettableFuture<Unit> future
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
-   Method

</div>

[]{#skip.navbar.bottom}
:::
