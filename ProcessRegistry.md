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
-   [Nested](#nested.class.summary) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.util](package-summary.html)
:::

## Class ProcessRegistry {#class-processregistry .title title="Class ProcessRegistry"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.util.ProcessRegistry

::: description
-   

    ------------------------------------------------------------------------

        public class ProcessRegistry
        extends Object

    ::: block
    A singleton helper class for process registration.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static interface `   | `ProcessRegistry.Pro  | ::: block             |
        |                       | cessRegisterCallback` | A callback to be      |
        |                       |                       | called upon           |
        |                       |                       | registering a         |
        |                       |                       | process.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `st                   | `getInstance()`       | ::: block             |
        | atic ProcessRegistry` |                       | Gets the singleton    |
        |                       |                       | instance of this      |
        |                       |                       | class.                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `register             | ::: block             |
        |                       | Process​(Object proces | Registers the process |
        |                       | s,                Pro | and notifies the      |
        |                       | cessExecutorParams pa | subscribers.          |
        |                       | rams,                 | :::                   |
        |                       | com.google.common.col |                       |
        |                       | lect.ImmutableMap<Str |                       |
        |                       | ing,​String> context)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `subscribe​(Pr         | ::: block             |
        |                       | ocessRegistry.Process | Subscribes the        |
        |                       | RegisterCallback proc | process register      |
        |                       | essRegisterCallback)` | callback.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `unsubscribe​(Pr       | ::: block             |
        |                       | ocessRegistry.Process | Unsubscribes the      |
        |                       | RegisterCallback proc | process register      |
        |                       | essRegisterCallback)` | callback.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

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

        []{#getInstance()}

        -   #### getInstance

            ``` methodSignature
            public static ProcessRegistry getInstance()
            ```

            ::: block
            Gets the singleton instance of this class.
            :::

        []{#subscribe(com.facebook.buck.util.ProcessRegistry.ProcessRegisterCallback)}

        -   #### subscribe

            ``` methodSignature
            public void subscribe​(ProcessRegistry.ProcessRegisterCallback processRegisterCallback)
            ```

            ::: block
            Subscribes the process register callback.
            :::

        []{#unsubscribe(com.facebook.buck.util.ProcessRegistry.ProcessRegisterCallback)}

        -   #### unsubscribe

            ``` methodSignature
            public void unsubscribe​(ProcessRegistry.ProcessRegisterCallback processRegisterCallback)
            ```

            ::: block
            Unsubscribes the process register callback.
            :::

        []{#registerProcess(java.lang.Object,com.facebook.buck.util.ProcessExecutorParams,com.google.common.collect.ImmutableMap)}

        -   #### registerProcess

            ``` methodSignature
            public void registerProcess​(Object process,
                                        ProcessExecutorParams params,
                                        com.google.common.collect.ImmutableMap<String,​String> context)
            ```

            ::: block
            Registers the process and notifies the subscribers.
            :::
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
-   [Nested](#nested.class.summary) \| 
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
