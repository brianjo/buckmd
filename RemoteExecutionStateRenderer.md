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
[Package]{.packageLabelInType} [com.facebook.buck.event.listener](package-summary.html)
:::

## Class RemoteExecutionStateRenderer {#class-remoteexecutionstaterenderer .title title="Class RemoteExecutionStateRenderer"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.event.listener.RemoteExecutionStateRenderer

::: description
-   

    All Implemented Interfaces:
    :   `MultiStateRenderer`

    ------------------------------------------------------------------------

        public class RemoteExecutionStateRenderer
        extends Object
        implements MultiStateRenderer

    ::: block
    A renderer for creating remote execution related lines on the
    console.
    Maintains an internal mapping of build targets and their associated
    [`RemoteExecutionActionEvent.Started`](../../remoteexecution/event/RemoteExecutionActionEvent.Started.html "class in com.facebook.buck.remoteexecution.event")
    at a particular instant in time defined by
    [`currentTimeMillis`](#currentTimeMillis). The mapping is ordered
    and immutable, and each map entry\'s index in the total ordering is
    treated as an ID. Targets that have not been executing long enough
    are ignored.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  Description
          -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `RemoteExecutionStateRenderer​(Ansi ansi,                             java.util.function.Function<Long,​String> formatTimeFunction,                             long currentTimeMillis,                             int outputMaxColumns,                             long minimumDurationMillis,                             int maxConcurrentExecutions,                             com.google.common.collect.ImmutableList<RemoteExecutionActionEvent.Started> remotelyBuildingTargets)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                 Method                               Description
          ------------------------------------------------- ------------------------------------ -------------
          `String`                                          `getExecutorCollectionLabel()`        
          `int`                                             `getExecutorCount()`                  
          `com.google.common.collect.ImmutableList<Long>`   `getSortedIds​(boolean unused)`        
          `String`                                          `renderShortStatus​(long targetId)`    
          `String`                                          `renderStatusLine​(long targetId)`     

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

        []{#<init>(com.facebook.buck.util.Ansi,java.util.function.Function,long,int,long,int,com.google.common.collect.ImmutableList)}

        -   #### RemoteExecutionStateRenderer

                public RemoteExecutionStateRenderer​(Ansi ansi,
                                                    java.util.function.Function<Long,​String> formatTimeFunction,
                                                    long currentTimeMillis,
                                                    int outputMaxColumns,
                                                    long minimumDurationMillis,
                                                    int maxConcurrentExecutions,
                                                    com.google.common.collect.ImmutableList<RemoteExecutionActionEvent.Started> remotelyBuildingTargets)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getExecutorCollectionLabel()}

        -   #### getExecutorCollectionLabel

            ``` methodSignature
            public String getExecutorCollectionLabel()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getExecutorCollectionLabel` in
                interface `MultiStateRenderer`

        []{#getExecutorCount()}

        -   #### getExecutorCount

            ``` methodSignature
            public int getExecutorCount()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getExecutorCount` in interface `MultiStateRenderer`

        []{#getSortedIds(boolean)}

        -   #### getSortedIds

            ``` methodSignature
            public com.google.common.collect.ImmutableList<Long> getSortedIds​(boolean unused)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getSortedIds` in interface `MultiStateRenderer`

        []{#renderStatusLine(long)}

        -   #### renderStatusLine

            ``` methodSignature
            public String renderStatusLine​(long targetId)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `renderStatusLine` in interface `MultiStateRenderer`

        []{#renderShortStatus(long)}

        -   #### renderShortStatus

            ``` methodSignature
            public String renderShortStatus​(long targetId)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `renderShortStatus` in interface `MultiStateRenderer`
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
