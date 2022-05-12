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
[Package]{.packageLabelInType} [com.facebook.buck.support.bgtasks](package-summary.html)
:::

## Class BackgroundTask\<T\> {#class-backgroundtaskt .title title="Class BackgroundTask"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.support.bgtasks.BackgroundTask\<T\>

::: description
-   

    ------------------------------------------------------------------------

        public abstract class BackgroundTask<T>
        extends Object

    ::: block
    Abstract class for background tasks to be run after build, e.g.
    cleanup/logging. Tasks take an action (e.g. close an event listener)
    and the arguments for that action. Tasks should be run by a
    [`BackgroundTaskManager`](BackgroundTaskManager.html "class in com.facebook.buck.support.bgtasks").
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static class `       | `Ba                   | ::: block             |
        |                       | ckgroundTask.Timeout` | Timeout object for    |
        |                       |                       | [                     |
        |                       |                       | `BackgroundTask`](Bac |
        |                       |                       | kgroundTask.html "cla |
        |                       |                       | ss in com.facebook.bu |
        |                       |                       | ck.support.bgtasks"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor          Description
          -------------------- -------------
          `BackgroundTask()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                Method                                                                                                                                            Description
          -------------------------------- ------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `static <T> BackgroundTask<T>`   `of​(String name,   TaskAction<T> action,   T actionArgs)`                                                                                          
          `static <T> BackgroundTask<T>`   `of​(String name,   TaskAction<T> action,   T actionArgs,   BackgroundTask.Timeout timeout)`                                                        
          `static <T> BackgroundTask<T>`   `of​(String name,   TaskAction<T> action,   T actionArgs,   Optional<? extends BackgroundTask.Timeout> timeout,   boolean shouldCancelOnRepeat)`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
          Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
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

        -   #### BackgroundTask

                public BackgroundTask()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#of(java.lang.String,com.facebook.buck.support.bgtasks.TaskAction,java.lang.Object)}
        []{#of(java.lang.String,com.facebook.buck.support.bgtasks.TaskAction,T)}

        -   #### of

            ``` methodSignature
            public static <T> BackgroundTask<T> of​(String name,
                                                   TaskAction<T> action,
                                                   T actionArgs)
            ```

        []{#of(java.lang.String,com.facebook.buck.support.bgtasks.TaskAction,java.lang.Object,com.facebook.buck.support.bgtasks.BackgroundTask.Timeout)}
        []{#of(java.lang.String,com.facebook.buck.support.bgtasks.TaskAction,T,com.facebook.buck.support.bgtasks.BackgroundTask.Timeout)}

        -   #### of

            ``` methodSignature
            public static <T> BackgroundTask<T> of​(String name,
                                                   TaskAction<T> action,
                                                   T actionArgs,
                                                   BackgroundTask.Timeout timeout)
            ```

        []{#of(java.lang.String,com.facebook.buck.support.bgtasks.TaskAction,java.lang.Object,java.util.Optional,boolean)}
        []{#of(java.lang.String,com.facebook.buck.support.bgtasks.TaskAction,T,java.util.Optional,boolean)}

        -   #### of

            ``` methodSignature
            public static <T> BackgroundTask<T> of​(String name,
                                                   TaskAction<T> action,
                                                   T actionArgs,
                                                   Optional<? extends BackgroundTask.Timeout> timeout,
                                                   boolean shouldCancelOnRepeat)
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
