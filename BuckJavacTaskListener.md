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
[Package]{.packageLabelInType} [com.facebook.buck.jvm.java.plugin.api](package-summary.html)
:::

## Interface BuckJavacTaskListener {#interface-buckjavactasklistener .title title="Interface BuckJavacTaskListener"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `TaskListenerProxy`, `TracingTaskListener`

    ------------------------------------------------------------------------

        public interface BuckJavacTaskListener

    ::: block
    Listens to events coming from the Java compiler. This is analogous
    to `TaskListener`, but loads in Buck\'s
    [`ClassLoader`](http://docs.oracle.com/javase/7/docs/api/java/lang/ClassLoader.html?is-external=true "class or interface in java.lang"){.externalLink}
    instead of the compiler\'s.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                Method                                                                                      Description
          -------------------------------- ------------------------------------------------------------------------------------------- -------------
          `void`                           `finished​(TaskEventMirror e)`                                                                
          `void`                           `started​(TaskEventMirror e)`                                                                 
          `static BuckJavacTaskListener`   `wrapRealTaskListener​(PluginClassLoader loader,                     Object taskListener)`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
          Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
          .tableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Abstract
          Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#wrapRealTaskListener(com.facebook.buck.jvm.java.plugin.api.PluginClassLoader,java.lang.Object)}

        -   #### wrapRealTaskListener

            ``` methodSignature
            static BuckJavacTaskListener wrapRealTaskListener​(PluginClassLoader loader,
                                                              Object taskListener)
            ```

        []{#started(com.facebook.buck.jvm.java.plugin.api.TaskEventMirror)}

        -   #### started

            ``` methodSignature
            void started​(TaskEventMirror e)
            ```

        []{#finished(com.facebook.buck.jvm.java.plugin.api.TaskEventMirror)}

        -   #### finished

            ``` methodSignature
            void finished​(TaskEventMirror e)
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
