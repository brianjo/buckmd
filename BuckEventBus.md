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
[Package]{.packageLabelInType} [com.facebook.buck.event](package-summary.html)
:::

## Interface BuckEventBus {#interface-buckeventbus .title title="Interface BuckEventBus"}
:::

::: contentContainer
::: description
-   

    All Superinterfaces:
    :   `AutoCloseable`, `Closeable`, `EventDispatcher`

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `DefaultBuckEventBus`

    ------------------------------------------------------------------------

        public interface BuckEventBus
        extends Closeable, EventDispatcher

    ::: block
    Thin wrapper around guava event bus.
    This interface exists only to break circular Buck target
    dependencies.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `BuildId`             | `getBuildId()`        |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `reg                  | ::: block             |
        |                       | ister​(Object object)` | Register a listener   |
        |                       |                       | to process events     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `unreg                | ::: block             |
        |                       | ister​(Object object)` | Remove a listener     |
        |                       |                       | previously specified  |
        |                       |                       | with `register()`     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `wait                 | ::: block             |
        |                       | Events​(long timeout)` | Wait for all          |
        |                       |                       | currently running     |
        |                       |                       | events to dispatch    |
        |                       |                       | and finish executing  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}

        -   []{#methods.inherited.from.class.java.io.Closeable}

            ### Methods inherited from interface java.io.[Closeable](http://docs.oracle.com/javase/7/docs/api/java/io/Closeable.html?is-external=true "class or interface in java.io"){.externalLink}

            `close`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.event.EventDispatcher}

            ### Methods inherited from interface com.facebook.buck.event.[EventDispatcher](EventDispatcher.html "interface in com.facebook.buck.event")

            `post, post, postWithoutConfiguring, timestamp`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getBuildId()}

        -   #### getBuildId

            ``` methodSignature
            BuildId getBuildId()
            ```

        []{#register(java.lang.Object)}

        -   #### register

            ``` methodSignature
            void register​(Object object)
            ```

            ::: block
            Register a listener to process events
            :::

        []{#unregister(java.lang.Object)}

        -   #### unregister

            ``` methodSignature
            void unregister​(Object object)
            ```

            ::: block
            Remove a listener previously specified with `register()`
            :::

        []{#waitEvents(long)}

        -   #### waitEvents

            ``` methodSignature
            boolean waitEvents​(long timeout)
            ```

            ::: block
            Wait for all currently running events to dispatch and finish
            executing
            :::

            [Parameters:]{.paramLabel}
            :   `timeout` - Time in milliseconds to wait for completion,
                if timeout is not greater than 0 then it will wait
                indefinitely

            [Returns:]{.returnLabel}
            :   true if all events were handled and false if timeout was
                hit
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
