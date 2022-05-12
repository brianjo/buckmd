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

## Class BuckJavacTaskListenerProxy {#class-buckjavactasklistenerproxy .title title="Class BuckJavacTaskListenerProxy"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.jvm.java.plugin.adapter.BuckJavacTaskListenerProxy

::: description
-   

    All Implemented Interfaces:
    :   `com.sun.source.util.TaskListener`

    ------------------------------------------------------------------------

        public class BuckJavacTaskListenerProxy
        extends Object
        implements com.sun.source.util.TaskListener

    ::: block
    Implements `TaskListener` by proxying calls to an inner
    [`BuckJavacTaskListener`](../api/BuckJavacTaskListener.html "interface in com.facebook.buck.jvm.java.plugin.api").
    This is the bridge that allows us to implement `TaskListener`s in
    Buck itself.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                            Description
          ---------------------------------------------------------------------- -------------
          `BuckJavacTaskListenerProxy​(BuckJavacTaskListener buckSideListener)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                                        Description
          ------------------- --------------------------------------------- -------------
          `void`              `finished​(com.sun.source.util.TaskEvent e)`    
          `void`              `started​(com.sun.source.util.TaskEvent e)`     

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

        []{#<init>(com.facebook.buck.jvm.java.plugin.api.BuckJavacTaskListener)}

        -   #### BuckJavacTaskListenerProxy

                public BuckJavacTaskListenerProxy​(BuckJavacTaskListener buckSideListener)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#started(com.sun.source.util.TaskEvent)}

        -   #### started

            ``` methodSignature
            public void started​(com.sun.source.util.TaskEvent e)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `started` in
                interface `com.sun.source.util.TaskListener`

        []{#finished(com.sun.source.util.TaskEvent)}

        -   #### finished

            ``` methodSignature
            public void finished​(com.sun.source.util.TaskEvent e)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `finished` in
                interface `com.sun.source.util.TaskListener`
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
