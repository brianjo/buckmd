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
-   [Field](#field.summary) \| 
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
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

## Class StepFailedException {#class-stepfailedexception .title title="Class StepFailedException"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [java.lang.Throwable](http://docs.oracle.com/javase/7/docs/api/java/lang/Throwable.html?is-external=true "class or interface in java.lang"){.externalLink}

    -   -   [java.lang.Exception](http://docs.oracle.com/javase/7/docs/api/java/lang/Exception.html?is-external=true "class or interface in java.lang"){.externalLink}

        -   -   com.facebook.buck.step.StepFailedException

::: description
-   

    All Implemented Interfaces:
    :   `ExceptionWithContext`, `WrapsException`, `Serializable`

    ------------------------------------------------------------------------

        public class StepFailedException
        extends Exception
        implements WrapsException, ExceptionWithContext

    [See Also:]{.seeLabel}
    :   [Serialized
        Form](../../../../serialized-form.html#com.facebook.buck.step.StepFailedException)
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type        Field                Description
          ------------------------ -------------------- -------------
          `protected static int`   `KEEP_FIRST_CHARS`    

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static               | `cre                  | ::: block             |
        |  StepFailedException` | ateForFailingStepWith | Creates a             |
        |                       | ExitCode​(Step step,   | StepFailedException   |
        |                       |                       | based on a            |
        |                       |           ExecutionCo | StepExecutionResult.  |
        |                       | ntext context,        | :::                   |
        |                       |                       |                       |
        |                       |      StepExecutionRes |                       |
        |                       | ult executionResult)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static               | `createForFailingSte  | ::: block             |
        |  StepFailedException` | pWithExitCode​(Step st | Same as above but     |
        |                       | ep,                   | includes RE action    |
        |                       |                Execut | metadata              |
        |                       | ionContext context,   | :::                   |
        |                       |                       |                       |
        |                       |           StepExecuti |                       |
        |                       | onResult executionRes |                       |
        |                       | ult,                  |                       |
        |                       |                 com.f |                       |
        |                       | acebook.buck.remoteex |                       |
        |                       | ecution.proto.RemoteE |                       |
        |                       | xecutionMetadata remo |                       |
        |                       | teExecutionMetadata)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `getContext()`        |                       |
        +-----------------------+-----------------------+-----------------------+
        | `OptionalInt`         | `getExitCode()`       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getMessage()`        |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<co          | `getRemot             |                       |
        | m.facebook.buck.remot | eExecutionMetadata()` |                       |
        | eexecution.proto.Remo |                       |                       |
        | teExecutionMetadata>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Step`                | `getStep()`           |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Throwable}

            ### Methods inherited from class java.lang.[Throwable](http://docs.oracle.com/javase/7/docs/api/java/lang/Throwable.html?is-external=true "class or interface in java.lang"){.externalLink}

            `addSuppressed, fillInStackTrace, getCause, getLocalizedMessage, getStackTrace, getSuppressed, initCause, printStackTrace, printStackTrace, printStackTrace, setStackTrace, toString`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#field.detail}

        ### Field Detail

        []{#KEEP_FIRST_CHARS}

        -   #### KEEP_FIRST_CHARS

                protected static final int KEEP_FIRST_CHARS

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../constant-values.html#com.facebook.buck.step.StepFailedException.KEEP_FIRST_CHARS)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getMessage()}

        -   #### getMessage

            ``` methodSignature
            public String getMessage()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `getMessage` in class `Throwable`

        []{#createForFailingStepWithExitCode(com.facebook.buck.step.Step,com.facebook.buck.core.build.execution.context.ExecutionContext,com.facebook.buck.step.StepExecutionResult)}

        -   #### createForFailingStepWithExitCode

            ``` methodSignature
            public static StepFailedException createForFailingStepWithExitCode​(Step step,
                                                                               ExecutionContext context,
                                                                               StepExecutionResult executionResult)
            ```

            ::: block
            Creates a StepFailedException based on a
            StepExecutionResult.
            :::

        []{#createForFailingStepWithExitCode(com.facebook.buck.step.Step,com.facebook.buck.core.build.execution.context.ExecutionContext,com.facebook.buck.step.StepExecutionResult,com.facebook.buck.remoteexecution.proto.RemoteExecutionMetadata)}

        -   #### createForFailingStepWithExitCode

            ``` methodSignature
            public static StepFailedException createForFailingStepWithExitCode​(Step step,
                                                                               ExecutionContext context,
                                                                               StepExecutionResult executionResult,
                                                                               com.facebook.buck.remoteexecution.proto.RemoteExecutionMetadata remoteExecutionMetadata)
            ```

            ::: block
            Same as above but includes RE action metadata
            :::

        []{#getStep()}

        -   #### getStep

            ``` methodSignature
            public Step getStep()
            ```

        []{#getExitCode()}

        -   #### getExitCode

            ``` methodSignature
            public OptionalInt getExitCode()
            ```

        []{#getRemoteExecutionMetadata()}

        -   #### getRemoteExecutionMetadata

            ``` methodSignature
            public Optional<com.facebook.buck.remoteexecution.proto.RemoteExecutionMetadata> getRemoteExecutionMetadata()
            ```

        []{#getContext()}

        -   #### getContext

            ``` methodSignature
            public Optional<String> getContext()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getContext` in interface `ExceptionWithContext`
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
-   [Field](#field.summary) \| 
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
-   Constr \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
