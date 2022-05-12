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
[Package]{.packageLabelInType} [com.facebook.buck.sandbox.impl](package-summary.html)
:::

## Class PlatformSandboxExecutionStrategyFactory {#class-platformsandboxexecutionstrategyfactory .title title="Class PlatformSandboxExecutionStrategyFactory"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.sandbox.impl.PlatformSandboxExecutionStrategyFactory

::: description
-   

    All Implemented Interfaces:
    :   `SandboxExecutionStrategyFactory`

    ------------------------------------------------------------------------

        public class PlatformSandboxExecutionStrategyFactory
        extends Object
        implements SandboxExecutionStrategyFactory

    ::: block
    Creates
    [`SandboxExecutionStrategyFactory`](../SandboxExecutionStrategyFactory.html "interface in com.facebook.buck.sandbox")
    using the information about the current platform.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                   Description
          --------------------------------------------- -------------
          `PlatformSandboxExecutionStrategyFactory()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `Sand                 | `create               | ::: block             |
        | boxExecutionStrategy` | ​(ProcessExecutor proc | Creates a             |
        |                       | essExecutor,       Bu | [`SandboxExecutionS   |
        |                       | ckConfig buckConfig)` | trategy`](../SandboxE |
        |                       |                       | xecutionStrategy.html |
        |                       |                       |  "interface in com.fa |
        |                       |                       | cebook.buck.sandbox") |
        |                       |                       | using the provided    |
        |                       |                       | process executor and  |
        |                       |                       | configuration.        |
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

        []{#<init>()}

        -   #### PlatformSandboxExecutionStrategyFactory

                public PlatformSandboxExecutionStrategyFactory()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#create(com.facebook.buck.util.ProcessExecutor,com.facebook.buck.core.config.BuckConfig)}

        -   #### create

            ``` methodSignature
            public SandboxExecutionStrategy create​(ProcessExecutor processExecutor,
                                                   BuckConfig buckConfig)
            ```

            ::: block
            [Description copied from
            interface: `SandboxExecutionStrategyFactory`]{.descfrmTypeLabel}
            :::

            ::: block
            Creates a
            [`SandboxExecutionStrategy`](../SandboxExecutionStrategy.html "interface in com.facebook.buck.sandbox")
            using the provided process executor and configuration.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `create` in interface `SandboxExecutionStrategyFactory`
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
