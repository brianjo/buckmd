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

-   [Overview](../../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../index-all.html)
-   [Help](../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.jvm.java.plugin.adapter](package-summary.html)
:::

## Class TaskListenerProxy {#class-tasklistenerproxy .title title="Class TaskListenerProxy"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.jvm.java.plugin.adapter.TaskListenerProxy

::: description
-   

    All Implemented Interfaces:
    :   `BuckJavacTaskListener`

    ------------------------------------------------------------------------

        public class TaskListenerProxy
        extends Object
        implements BuckJavacTaskListener

    ::: block
    Implements
    [`BuckJavacTaskListener`](../api/BuckJavacTaskListener.html "interface in com.facebook.buck.jvm.java.plugin.api")
    by proxying calls to an inner `TaskListener`. This is the bridge
    that allows Buck to call `TaskListener`s that are loaded in the
    compiler\'s
    [`ClassLoader`](http://docs.oracle.com/javase/7/docs/api/java/lang/ClassLoader.html?is-external=true "class or interface in java.lang"){.externalLink}.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                Description
          ------------------------------------------ -------------
          `TaskListenerProxy​(Object taskListener)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                    Method                          Description
          ------------------------------------ ------------------------------- -------------
          `void`                               `finished​(TaskEventMirror e)`    
          `com.sun.source.util.TaskListener`   `getInner()`                     
          `void`                               `started​(TaskEventMirror e)`     

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

        []{#<init>(java.lang.Object)}

        -   #### TaskListenerProxy

                public TaskListenerProxy​(Object taskListener)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getInner()}

        -   #### getInner

            ``` methodSignature
            public com.sun.source.util.TaskListener getInner()
            ```

        []{#started(com.facebook.buck.jvm.java.plugin.api.TaskEventMirror)}

        -   #### started

            ``` methodSignature
            public void started​(TaskEventMirror e)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `started` in interface `BuckJavacTaskListener`

        []{#finished(com.facebook.buck.jvm.java.plugin.api.TaskEventMirror)}

        -   #### finished

            ``` methodSignature
            public void finished​(TaskEventMirror e)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `finished` in interface `BuckJavacTaskListener`
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

-   [Overview](../../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../index-all.html)
-   [Help](../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../allclasses.html)

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
