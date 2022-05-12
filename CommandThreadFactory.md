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

## Class CommandThreadFactory {#class-commandthreadfactory .title title="Class CommandThreadFactory"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.util.concurrent.CommandThreadFactory

::: description
-   

    All Implemented Interfaces:
    :   `ThreadFactory`

    ------------------------------------------------------------------------

        public class CommandThreadFactory
        extends Object
        implements ThreadFactory

    ::: block
    A ThreadFactory which associates created threads with the same
    command associated with the thread which creates the
    CommandThreadFactory.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                 Description
          ----------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `CommandThreadFactory​(String threadName,                     CommonThreadFactoryState state)`                                                                
          `CommandThreadFactory​(String threadName,                     CommonThreadFactoryState state,                     int threadPriority)`                        
          `CommandThreadFactory​(ThreadFactory threadFactory,                     CommonThreadFactoryState state)`                                                      
          `CommandThreadFactory​(ThreadFactory threadFactory,                     CommonThreadFactoryState state,                     OptionalInt optionalPriority)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                    Description
          ------------------- ------------------------- -------------
          `Thread`            `newThread​(Runnable r)`    

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

        []{#<init>(java.lang.String,com.facebook.buck.util.concurrent.CommonThreadFactoryState,int)}

        -   #### CommandThreadFactory

                public CommandThreadFactory​(String threadName,
                                            CommonThreadFactoryState state,
                                            int threadPriority)

        []{#<init>(java.lang.String,com.facebook.buck.util.concurrent.CommonThreadFactoryState)}

        -   #### CommandThreadFactory

                public CommandThreadFactory​(String threadName,
                                            CommonThreadFactoryState state)

        []{#<init>(java.util.concurrent.ThreadFactory,com.facebook.buck.util.concurrent.CommonThreadFactoryState)}

        -   #### CommandThreadFactory

                public CommandThreadFactory​(ThreadFactory threadFactory,
                                            CommonThreadFactoryState state)

        []{#<init>(java.util.concurrent.ThreadFactory,com.facebook.buck.util.concurrent.CommonThreadFactoryState,java.util.OptionalInt)}

        -   #### CommandThreadFactory

                public CommandThreadFactory​(ThreadFactory threadFactory,
                                            CommonThreadFactoryState state,
                                            OptionalInt optionalPriority)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#newThread(java.lang.Runnable)}

        -   #### newThread

            ``` methodSignature
            public Thread newThread​(Runnable r)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `newThread` in interface `ThreadFactory`
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
