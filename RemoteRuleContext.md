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

## Class RemoteRuleContext {#class-remoterulecontext .title title="Class RemoteRuleContext"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.rules.modern.builders.RemoteRuleContext

::: description
-   

    ------------------------------------------------------------------------

        public class RemoteRuleContext
        extends Object

    ::: block
    This holds information about rule states.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                   Description
          ----------------------------------------------------------------------------- -------------
          `RemoteRuleContext​(BuckEventBus eventBus,                  BuildRule rule)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `void`                | `canc                 | ::: block             |
        |                       | el​(Throwable reason)` | Call when action has  |
        |                       |                       | been cancelled.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Scope`               | `enterState​(Remote    | ::: block             |
        |                       | ExecutionActionEvent. | Called when Action    |
        |                       | State state,          | state is changed.     |
        |                       |   Optional<Protocol.D | :::                   |
        |                       | igest> actionDigest)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Throwable`           | `getCancelReason()`   | ::: block             |
        |                       |                       | Get Throwable which   |
        |                       |                       | caused action to      |
        |                       |                       | cancel.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isCancelled()`       | ::: block             |
        |                       |                       | Whether action has    |
        |                       |                       | been cancelled.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `onCance              | ::: block             |
        |                       | llation​(java.util.fun | Action has been       |
        |                       | ction.Consumer<Throwa | cancelled.            |
        |                       | ble> cancelCallback)` | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `tryStart()`          | ::: block             |
        |                       |                       | Call Try Start to set |
        |                       |                       | the guard.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

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

        []{#<init>(com.facebook.buck.event.BuckEventBus,com.facebook.buck.core.rules.BuildRule)}

        -   #### RemoteRuleContext

                public RemoteRuleContext​(BuckEventBus eventBus,
                                         BuildRule rule)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#isCancelled()}

        -   #### isCancelled

            ``` methodSignature
            public boolean isCancelled()
            ```

            ::: block
            Whether action has been cancelled.
            :::

        []{#getCancelReason()}

        -   #### getCancelReason

            ``` methodSignature
            public Throwable getCancelReason()
            ```

            ::: block
            Get Throwable which caused action to cancel.
            :::

        []{#cancel(java.lang.Throwable)}

        -   #### cancel

            ``` methodSignature
            public void cancel​(Throwable reason)
            ```

            ::: block
            Call when action has been cancelled.
            :::

        []{#tryStart()}

        -   #### tryStart

            ``` methodSignature
            public boolean tryStart()
            ```

            ::: block
            Call Try Start to set the guard.
            :::

        []{#onCancellation(java.util.function.Consumer)}

        -   #### onCancellation

            ``` methodSignature
            public void onCancellation​(java.util.function.Consumer<Throwable> cancelCallback)
            ```

            ::: block
            Action has been cancelled.
            :::

        []{#enterState(com.facebook.buck.remoteexecution.event.RemoteExecutionActionEvent.State,java.util.Optional)}

        -   #### enterState

            ``` methodSignature
            public Scope enterState​(RemoteExecutionActionEvent.State state,
                                    Optional<Protocol.Digest> actionDigest)
            ```

            ::: block
            Called when Action state is changed.
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
