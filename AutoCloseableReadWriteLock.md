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
[Package]{.packageLabelInType} [com.facebook.buck.util.concurrent](package-summary.html)
:::

## Class AutoCloseableReadWriteLock {#class-autocloseablereadwritelock .title title="Class AutoCloseableReadWriteLock"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.util.concurrent.AutoCloseableReadWriteLock

::: description
-   

    All Implemented Interfaces:
    :   `ReadWriteLock`

    ------------------------------------------------------------------------

        public class AutoCloseableReadWriteLock
        extends Object
        implements ReadWriteLock

    ::: block
    Convenience wrapper around
    [`ReentrantReadWriteLock`](http://docs.oracle.com/javase/7/docs/api/java/util/concurrent/locks/ReentrantReadWriteLock.html?is-external=true "class or interface in java.util.concurrent.locks"){.externalLink}
    that, when combined with try-with-resources pattern, automatically
    unlocks the lock once the `try` section is completed.
    Usage example:

           AutoCloseableReadWriteLock lock = new AutoCloseableReadWriteLock();
           try (AutoCloseableLock readLock = lock.readLock()) {
             // no other thread can acquire write lock while this section is running
           }
           // the readLock is automatically unlocked
         
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                      Description
          -------------------------------- -------------
          `AutoCloseableReadWriteLock()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type     Method          Description
          --------------------- --------------- -------------
          `AutoCloseableLock`   `readLock()`     
          `AutoCloseableLock`   `writeLock()`    

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

        []{#<init>()}

        -   #### AutoCloseableReadWriteLock

                public AutoCloseableReadWriteLock()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#readLock()}

        -   #### readLock

            ``` methodSignature
            public AutoCloseableLock readLock()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `readLock` in interface `ReadWriteLock`

        []{#writeLock()}

        -   #### writeLock

            ``` methodSignature
            public AutoCloseableLock writeLock()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `writeLock` in interface `ReadWriteLock`
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
