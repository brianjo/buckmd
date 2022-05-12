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
[Package]{.packageLabelInType} [com.facebook.buck.edenfs](package-summary.html)
:::

## Class EdenClientPool {#class-edenclientpool .title title="Class EdenClientPool"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.edenfs.EdenClientPool

::: description
-   

    ------------------------------------------------------------------------

        public final class EdenClientPool
        extends Object

    ::: block
    A pool of
    [`EdenClient`](EdenClient.html "interface in com.facebook.buck.edenfs")
    objects.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                   Method                                                     Description
          ----------------------------------- ---------------------------------------------------------- -------------
          `EdenClient`                        `getClient()`                                               
          `static Optional<EdenClientPool>`   `newInstanceFromSocket​(Path socketFile)`                    
          `static Optional<EdenClientPool>`   `tryToCreateEdenClientPool​(Path directoryInEdenFsMount)`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
          Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
          .tableTab}[[Instance
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

        []{#getClient()}

        -   #### getClient

            ``` methodSignature
            public EdenClient getClient()
            ```

            [Returns:]{.returnLabel}
            :   an
                [`EdenClient`](EdenClient.html "interface in com.facebook.buck.edenfs")
                that must be used on the same thread that requested it.

        []{#tryToCreateEdenClientPool(java.nio.file.Path)}

        -   #### tryToCreateEdenClientPool

            ``` methodSignature
            public static Optional<EdenClientPool> tryToCreateEdenClientPool​(Path directoryInEdenFsMount)
            ```

        []{#newInstanceFromSocket(java.nio.file.Path)}

        -   #### newInstanceFromSocket

            ``` methodSignature
            public static Optional<EdenClientPool> newInstanceFromSocket​(Path socketFile)
            ```
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
