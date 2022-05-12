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
[Package]{.packageLabelInType} [com.facebook.buck.util.concurrent](package-summary.html)
:::

## Class AutoCloseableLock {#class-autocloseablelock .title title="Class AutoCloseableLock"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.util.concurrent.AutoCloseableLock

::: description
-   

    All Implemented Interfaces:
    :   `AutoCloseable`, `Lock`

    ------------------------------------------------------------------------

        public class AutoCloseableLock
        extends Object
        implements AutoCloseable, Lock
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type            Method                                       Description
          ---------------------------- -------------------------------------------- -------------
          `void`                       `close()`                                     
          `static AutoCloseableLock`   `createFor​(Lock lock)`                        
          `void`                       `lock()`                                      
          `void`                       `lockInterruptibly()`                         
          `Condition`                  `newCondition()`                              
          `boolean`                    `tryLock()`                                   
          `boolean`                    `tryLock​(long time,        TimeUnit unit)`    
          `void`                       `unlock()`                                    

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

        []{#createFor(java.util.concurrent.locks.Lock)}

        -   #### createFor

            ``` methodSignature
            public static AutoCloseableLock createFor​(Lock lock)
            ```

        []{#close()}

        -   #### close

            ``` methodSignature
            public void close()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `close` in interface `AutoCloseable`

        []{#lock()}

        -   #### lock

            ``` methodSignature
            public void lock()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `lock` in interface `Lock`

        []{#lockInterruptibly()}

        -   #### lockInterruptibly

            ``` methodSignature
            public void lockInterruptibly()
                                   throws InterruptedException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `lockInterruptibly` in interface `Lock`

            [Throws:]{.throwsLabel}
            :   `InterruptedException`

        []{#tryLock()}

        -   #### tryLock

            ``` methodSignature
            public boolean tryLock()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `tryLock` in interface `Lock`

        []{#tryLock(long,java.util.concurrent.TimeUnit)}

        -   #### tryLock

            ``` methodSignature
            public boolean tryLock​(long time,
                                   TimeUnit unit)
                            throws InterruptedException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `tryLock` in interface `Lock`

            [Throws:]{.throwsLabel}
            :   `InterruptedException`

        []{#unlock()}

        -   #### unlock

            ``` methodSignature
            public void unlock()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `unlock` in interface `Lock`

        []{#newCondition()}

        -   #### newCondition

            ``` methodSignature
            public Condition newCondition()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `newCondition` in interface `Lock`
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
