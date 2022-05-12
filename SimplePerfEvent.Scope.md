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

## Interface SimplePerfEvent.Scope {#interface-simpleperfevent.scope .title title="Interface SimplePerfEvent.Scope"}
:::

::: contentContainer
::: description
-   

    All Superinterfaces:
    :   `AutoCloseable`

    ```{=html}
    <!-- -->
    ```

    Enclosing class:
    :   [SimplePerfEvent](SimplePerfEvent.html "class in com.facebook.buck.event")

    ------------------------------------------------------------------------

        public static interface SimplePerfEvent.Scope
        extends AutoCloseable

    ::: block
    Represents the scope within which a particular performance operation
    is taking place.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `void`                | `appendFinishedInf    | ::: block             |
        |                       | o​(String k1,          | Appends information   |
        |                       |           Object v1)` | to the finished event |
        |                       |                       | which will be sent    |
        |                       |                       | when control exits    |
        |                       |                       | the scope.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `close()`             |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `incrementFinis       | ::: block             |
        |                       | hedCounter​(String key | Increments a counter  |
        |                       | ,                     | that will be appended |
        |                       |      long increment)` | to the finished       |
        |                       |                       | event.                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `upda                 | ::: block             |
        |                       | te​(com.google.common. | Creates and sends an  |
        |                       | collect.ImmutableMap< | event which indicates |
        |                       | String,​Object> info)` | an update in state of |
        |                       |                       | the scope.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `update​(String        | ::: block             |
        |                       | k1,       Object v1)` | Convenience wrapper   |
        |                       |                       | for                   |
        |                       |                       | [`update(Im           |
        |                       |                       | mutableMap)`](#update |
        |                       |                       | (com.google.common.co |
        |                       |                       | llect.ImmutableMap)). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `update               | ::: block             |
        |                       | ​(String k1,       Obj | Convenience wrapper   |
        |                       | ect v1,       String  | for                   |
        |                       | k2,       Object v2)` | [`update(Im           |
        |                       |                       | mutableMap)`](#update |
        |                       |                       | (com.google.common.co |
        |                       |                       | llect.ImmutableMap)). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#update(com.google.common.collect.ImmutableMap)}

        -   #### update

            ``` methodSignature
            void update​(com.google.common.collect.ImmutableMap<String,​Object> info)
            ```

            ::: block
            Creates and sends an event which indicates an update in
            state of the scope. Every invocation creates and sends a new
            event.
            :::

            [Parameters:]{.paramLabel}
            :   `info` - Any additional information to be saved with the
                event. This will be serialized and potentially sent over
                the wire, so please keep this small.

        []{#update(java.lang.String,java.lang.Object)}

        -   #### update

            ``` methodSignature
            void update​(String k1,
                        Object v1)
            ```

            ::: block
            Convenience wrapper for
            [`update(ImmutableMap)`](#update(com.google.common.collect.ImmutableMap)).
            :::

        []{#update(java.lang.String,java.lang.Object,java.lang.String,java.lang.Object)}

        -   #### update

            ``` methodSignature
            void update​(String k1,
                        Object v1,
                        String k2,
                        Object v2)
            ```

            ::: block
            Convenience wrapper for
            [`update(ImmutableMap)`](#update(com.google.common.collect.ImmutableMap)).
            :::

        []{#appendFinishedInfo(java.lang.String,java.lang.Object)}

        -   #### appendFinishedInfo

            ``` methodSignature
            void appendFinishedInfo​(String k1,
                                    Object v1)
            ```

            ::: block
            Appends information to the finished event which will be sent
            when control exits the scope.
            :::

            [Parameters:]{.paramLabel}
            :   `k1` - name of the value to be stored with the event.
            :   `v1` - value to be stored. This will be serialized and
                potentially sent over the wire, so please keep this
                small.

        []{#incrementFinishedCounter(java.lang.String,long)}

        -   #### incrementFinishedCounter

            ``` methodSignature
            void incrementFinishedCounter​(String key,
                                          long increment)
            ```

            ::: block
            Increments a counter that will be appended to the finished
            event.
            :::

        []{#close()}

        -   #### close

            ``` methodSignature
            void close()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `close` in interface `AutoCloseable`
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
