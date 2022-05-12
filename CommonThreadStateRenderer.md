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

## Class CommonThreadStateRenderer {#class-commonthreadstaterenderer .title title="Class CommonThreadStateRenderer"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.event.listener.CommonThreadStateRenderer

::: description
-   

    ------------------------------------------------------------------------

        public class CommonThreadStateRenderer
        extends Object

    ::: block
    Renders the per thread information line during build phase on super
    console
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                                                                                                                        Description
          ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `CommonThreadStateRenderer​(Ansi ansi,                          java.util.function.Function<Long,​String> formatTimeFunction,                          long currentTimeMs,                          int outputMaxColumns,                          com.google.common.collect.ImmutableMap<Long,​com.facebook.buck.event.listener.ThreadRenderingInformation> threadInformationMap)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `com.                 | `getSortedThreadIds   |                       |
        | google.common.collect | ​(boolean sortByTime)` |                       |
        | .ImmutableList<Long>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `getThreadCount()`    |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `renderLine​(O         |                       |
        |                       | ptional<BuildTarget>  |                       |
        |                       | buildTarget,          |                       |
        |                       |   Optional<? extends  |                       |
        |                       | AbstractBuckEvent> st |                       |
        |                       | artEvent,           O |                       |
        |                       | ptional<? extends Lea |                       |
        |                       | fEvent> runningStep,  |                       |
        |                       |           Optional<St |                       |
        |                       | ring> stepCategory,   |                       |
        |                       |          Optional<Str |                       |
        |                       | ing> placeholderStepI |                       |
        |                       | nformation,           |                       |
        |                       |  long elapsedTimeMs)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `renderS              | ::: block             |
        |                       | hortStatus​(boolean is | Returns a compressed  |
        |                       | Active,               | version of            |
        |                       |     boolean renderSub | `renderLine`.         |
        |                       | tle,                  | :::                   |
        |                       |  long elapsedTimeMs)` |                       |
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

        []{#<init>(com.facebook.buck.util.Ansi,java.util.function.Function,long,int,com.google.common.collect.ImmutableMap)}

        -   #### CommonThreadStateRenderer

                public CommonThreadStateRenderer​(Ansi ansi,
                                                 java.util.function.Function<Long,​String> formatTimeFunction,
                                                 long currentTimeMs,
                                                 int outputMaxColumns,
                                                 com.google.common.collect.ImmutableMap<Long,​com.facebook.buck.event.listener.ThreadRenderingInformation> threadInformationMap)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getThreadCount()}

        -   #### getThreadCount

            ``` methodSignature
            public int getThreadCount()
            ```

        []{#getSortedThreadIds(boolean)}

        -   #### getSortedThreadIds

            ``` methodSignature
            public com.google.common.collect.ImmutableList<Long> getSortedThreadIds​(boolean sortByTime)
            ```

        []{#renderLine(java.util.Optional,java.util.Optional,java.util.Optional,java.util.Optional,java.util.Optional,long)}

        -   #### renderLine

            ``` methodSignature
            public String renderLine​(Optional<BuildTarget> buildTarget,
                                     Optional<? extends AbstractBuckEvent> startEvent,
                                     Optional<? extends LeafEvent> runningStep,
                                     Optional<String> stepCategory,
                                     Optional<String> placeholderStepInformation,
                                     long elapsedTimeMs)
            ```

        []{#renderShortStatus(boolean,boolean,long)}

        -   #### renderShortStatus

            ``` methodSignature
            public String renderShortStatus​(boolean isActive,
                                            boolean renderSubtle,
                                            long elapsedTimeMs)
            ```

            ::: block
            Returns a compressed version of `renderLine`.
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
