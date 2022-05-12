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
[Package]{.packageLabelInType} [com.facebook.buck.step](package-summary.html)
:::

## Class StepRunner {#class-steprunner .title title="Class StepRunner"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.step.StepRunner

::: description
-   

    ------------------------------------------------------------------------

        public final class StepRunner
        extends Object

    ::: block
    Utility class for running
    [`Step`](Step.html "interface in com.facebook.buck.step")s
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static void`         | `runStep​(Ex           | ::: block             |
        |                       | ecutionContext contex | Runs a single         |
        |                       | t,        Step step,  | [`Step`](Step.h       |
        |                       |        Optional<Build | tml "interface in com |
        |                       | Target> buildTarget)` | .facebook.buck.step") |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

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
    -   []{#method.detail}

        ### Method Detail

        []{#runStep(com.facebook.buck.core.build.execution.context.ExecutionContext,com.facebook.buck.step.Step,java.util.Optional)}

        -   #### runStep

            ``` methodSignature
            public static void runStep​(ExecutionContext context,
                                       Step step,
                                       Optional<BuildTarget> buildTarget)
                                throws StepFailedException,
                                       InterruptedException
            ```

            ::: block
            Runs a single
            [`Step`](Step.html "interface in com.facebook.buck.step")
            :::

            [Parameters:]{.paramLabel}
            :   `context` - the
                [`ExecutionContext`](../core/build/execution/context/ExecutionContext.html "class in com.facebook.buck.core.build.execution.context")
                containing information and console logging utilities for
                the
                [`Step`](Step.html "interface in com.facebook.buck.step")
            :   `step` - the
                [`Step`](Step.html "interface in com.facebook.buck.step")
                to execute

            [Throws:]{.throwsLabel}
            :   `StepFailedException` - if the step failed
            :   `InterruptedException` - if an interrupt occurred while
                executing the
                [`Step`](Step.html "interface in com.facebook.buck.step")
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
