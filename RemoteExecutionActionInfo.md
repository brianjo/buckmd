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
[Package]{.packageLabelInType} [com.facebook.buck.rules.modern.builders](package-summary.html)
:::

## Class RemoteExecutionActionInfo {#class-remoteexecutionactioninfo .title title="Class RemoteExecutionActionInfo"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.rules.modern.builders.RemoteExecutionActionInfo

::: description
-   

    ------------------------------------------------------------------------

        public abstract class RemoteExecutionActionInfo
        extends Object

    ::: block
    This includes all the information needed to run a remote execution
    command.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                     Description
          ------------------------------- -------------
          `RemoteExecutionActionInfo()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                        Method                                                                                                                                                                      Description
          ------------------------------------------------------------------------ --------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `abstract Protocol.Digest`                                               `getActionDigest()`                                                                                                                                                          
          `abstract Iterable<? extends Path>`                                      `getOutputs()`                                                                                                                                                               
          `abstract com.google.common.collect.ImmutableList<UploadDataSupplier>`   `getRequiredData()`                                                                                                                                                          
          `abstract long`                                                          `getTotalInputSize()`                                                                                                                                                        
          `static RemoteExecutionActionInfo`                                       `of​(Protocol.Digest actionDigest,   com.google.common.collect.ImmutableList<UploadDataSupplier> requiredData,   long totalInputSize,   Iterable<? extends Path> outputs)`    
          `RemoteExecutionActionInfo`                                              `withRequiredData​(com.google.common.collect.ImmutableList<UploadDataSupplier> data)`                                                                                         

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
          Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
          .tableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Abstract
          Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
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

        []{#<init>()}

        -   #### RemoteExecutionActionInfo

                public RemoteExecutionActionInfo()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getActionDigest()}

        -   #### getActionDigest

            ``` methodSignature
            public abstract Protocol.Digest getActionDigest()
            ```

        []{#getRequiredData()}

        -   #### getRequiredData

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableList<UploadDataSupplier> getRequiredData()
            ```

        []{#getTotalInputSize()}

        -   #### getTotalInputSize

            ``` methodSignature
            public abstract long getTotalInputSize()
            ```

        []{#getOutputs()}

        -   #### getOutputs

            ``` methodSignature
            public abstract Iterable<? extends Path> getOutputs()
            ```

        []{#withRequiredData(com.google.common.collect.ImmutableList)}

        -   #### withRequiredData

            ``` methodSignature
            public RemoteExecutionActionInfo withRequiredData​(com.google.common.collect.ImmutableList<UploadDataSupplier> data)
            ```

        []{#of(com.facebook.buck.remoteexecution.interfaces.Protocol.Digest,com.google.common.collect.ImmutableList,long,java.lang.Iterable)}

        -   #### of

            ``` methodSignature
            public static RemoteExecutionActionInfo of​(Protocol.Digest actionDigest,
                                                       com.google.common.collect.ImmutableList<UploadDataSupplier> requiredData,
                                                       long totalInputSize,
                                                       Iterable<? extends Path> outputs)
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
