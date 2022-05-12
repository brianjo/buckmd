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
[Package]{.packageLabelInType} [com.facebook.buck.sandbox.darwin](package-summary.html)
:::

## Class DarwinSandboxExecutionStrategy {#class-darwinsandboxexecutionstrategy .title title="Class DarwinSandboxExecutionStrategy"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.sandbox.darwin.DarwinSandboxExecutionStrategy

::: description
-   

    All Implemented Interfaces:
    :   `SandboxExecutionStrategy`

    ------------------------------------------------------------------------

        public class DarwinSandboxExecutionStrategy
        extends Object
        implements SandboxExecutionStrategy

    ::: block
    [`SandboxExecutionStrategy`](../SandboxExecutionStrategy.html "interface in com.facebook.buck.sandbox")
    for OS X sandbox.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                    Description
          ------------------------------------------------------------------------------------------------------------------------------ -------------
          `DarwinSandboxExecutionStrategy​(ProcessExecutor processExecutor,                               SandboxConfig sandboxConfig)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `ProgramRunner`       | `c                    | ::: block             |
        |                       | reateSandboxProgramRu | Creates a new         |
        |                       | nner​(SandboxPropertie | [`ProgramRu           |
        |                       | s sandboxProperties)` | nner`](../../shell/pr |
        |                       |                       | ogramrunner/ProgramRu |
        |                       |                       | nner.html "interface  |
        |                       |                       | in com.facebook.buck. |
        |                       |                       | shell.programrunner") |
        |                       |                       | to run a specific     |
        |                       |                       | program in a sandbox. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isSandboxEnabled()`  |                       |
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

        []{#<init>(com.facebook.buck.util.ProcessExecutor,com.facebook.buck.sandbox.SandboxConfig)}

        -   #### DarwinSandboxExecutionStrategy

                public DarwinSandboxExecutionStrategy​(ProcessExecutor processExecutor,
                                                      SandboxConfig sandboxConfig)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#isSandboxEnabled()}

        -   #### isSandboxEnabled

            ``` methodSignature
            public boolean isSandboxEnabled()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `isSandboxEnabled` in
                interface `SandboxExecutionStrategy`

            [Returns:]{.returnLabel}
            :   when sandboxing is supported by the platform and it\'s
                enabled

        []{#createSandboxProgramRunner(com.facebook.buck.sandbox.SandboxProperties)}

        -   #### createSandboxProgramRunner

            ``` methodSignature
            public ProgramRunner createSandboxProgramRunner​(SandboxProperties sandboxProperties)
            ```

            ::: block
            [Description copied from
            interface: `SandboxExecutionStrategy`]{.descfrmTypeLabel}
            :::

            ::: block
            Creates a new
            [`ProgramRunner`](../../shell/programrunner/ProgramRunner.html "interface in com.facebook.buck.shell.programrunner")
            to run a specific program in a sandbox.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `createSandboxProgramRunner` in
                interface `SandboxExecutionStrategy`

            [Parameters:]{.paramLabel}
            :   `sandboxProperties` - describes the particular execution
                of a sandboxed processes.
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
