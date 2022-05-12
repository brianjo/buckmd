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
[Package]{.packageLabelInType} [com.facebook.buck.util](package-summary.html)
:::

## Class ProcessResourceConsumption {#class-processresourceconsumption .title title="Class ProcessResourceConsumption"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.util.ProcessResourceConsumption

::: description
-   

    ------------------------------------------------------------------------

        public abstract class ProcessResourceConsumption
        extends Object

    ::: block
    Represents resource consumption counters of a
    [`Process`](http://docs.oracle.com/javase/7/docs/api/java/lang/Process.html?is-external=true "class or interface in java.lang"){.externalLink}.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                      Description
          -------------------------------- -------------
          `ProcessResourceConsumption()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                     Method                                                                                                                                                              Description
          ------------------------------------- ------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `abstract long`                       `getCpuReal()`                                                                                                                                                       
          `abstract long`                       `getCpuSys()`                                                                                                                                                        
          `abstract long`                       `getCpuTotal()`                                                                                                                                                      
          `abstract long`                       `getCpuUser()`                                                                                                                                                       
          `abstract long`                       `getIoBytesRead()`                                                                                                                                                   
          `abstract long`                       `getIoBytesWritten()`                                                                                                                                                
          `abstract long`                       `getIoTotal()`                                                                                                                                                       
          `abstract long`                       `getMemResident()`                                                                                                                                                   
          `abstract long`                       `getMemSize()`                                                                                                                                                       
          `static ProcessResourceConsumption`   `getPeak​(ProcessResourceConsumption r1,        ProcessResourceConsumption r2)`                                                                                       
          `static ProcessResourceConsumption`   `getTotal​(ProcessResourceConsumption r1,         ProcessResourceConsumption r2)`                                                                                     
          `static ProcessResourceConsumption`   `of​(long memResident,   long memSize,   long cpuReal,   long cpuUser,   long cpuSys,   long cpuTotal,   long ioBytesRead,   long ioBytesWritten,   long ioTotal)`    

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

        -   #### ProcessResourceConsumption

                public ProcessResourceConsumption()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getMemResident()}

        -   #### getMemResident

            ``` methodSignature
            public abstract long getMemResident()
            ```

        []{#getMemSize()}

        -   #### getMemSize

            ``` methodSignature
            public abstract long getMemSize()
            ```

        []{#getCpuReal()}

        -   #### getCpuReal

            ``` methodSignature
            public abstract long getCpuReal()
            ```

        []{#getCpuUser()}

        -   #### getCpuUser

            ``` methodSignature
            public abstract long getCpuUser()
            ```

        []{#getCpuSys()}

        -   #### getCpuSys

            ``` methodSignature
            public abstract long getCpuSys()
            ```

        []{#getCpuTotal()}

        -   #### getCpuTotal

            ``` methodSignature
            public abstract long getCpuTotal()
            ```

        []{#getIoBytesRead()}

        -   #### getIoBytesRead

            ``` methodSignature
            public abstract long getIoBytesRead()
            ```

        []{#getIoBytesWritten()}

        -   #### getIoBytesWritten

            ``` methodSignature
            public abstract long getIoBytesWritten()
            ```

        []{#getIoTotal()}

        -   #### getIoTotal

            ``` methodSignature
            public abstract long getIoTotal()
            ```

        []{#getPeak(com.facebook.buck.util.ProcessResourceConsumption,com.facebook.buck.util.ProcessResourceConsumption)}

        -   #### getPeak

            ``` methodSignature
            @Nullable
            public static ProcessResourceConsumption getPeak​(@Nullable
                                                             ProcessResourceConsumption r1,
                                                             @Nullable
                                                             ProcessResourceConsumption r2)
            ```

        []{#getTotal(com.facebook.buck.util.ProcessResourceConsumption,com.facebook.buck.util.ProcessResourceConsumption)}

        -   #### getTotal

            ``` methodSignature
            @Nullable
            public static ProcessResourceConsumption getTotal​(@Nullable
                                                              ProcessResourceConsumption r1,
                                                              @Nullable
                                                              ProcessResourceConsumption r2)
            ```

        []{#of(long,long,long,long,long,long,long,long,long)}

        -   #### of

            ``` methodSignature
            public static ProcessResourceConsumption of​(long memResident,
                                                        long memSize,
                                                        long cpuReal,
                                                        long cpuUser,
                                                        long cpuSys,
                                                        long cpuTotal,
                                                        long ioBytesRead,
                                                        long ioBytesWritten,
                                                        long ioTotal)
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
