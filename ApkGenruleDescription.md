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
-   [Field](#field.summary) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.android](package-summary.html)
:::

## Class ApkGenruleDescription {#class-apkgenruledescription .title title="Class ApkGenruleDescription"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.shell.AbstractGenruleDescription](../shell/AbstractGenruleDescription.html "class in com.facebook.buck.shell")\<[ApkGenruleDescriptionArg](ApkGenruleDescriptionArg.html "class in com.facebook.buck.android")\>

    -   -   com.facebook.buck.android.ApkGenruleDescription

::: description
-   

    All Implemented Interfaces:
    :   `ImplicitDepsInferringDescription<ApkGenruleDescriptionArg>`,
        `BaseDescription<ApkGenruleDescriptionArg>`,
        `Description<ApkGenruleDescriptionArg>`,
        `DescriptionWithTargetGraph<ApkGenruleDescriptionArg>`

    ------------------------------------------------------------------------

        public class ApkGenruleDescription
        extends AbstractGenruleDescription<ApkGenruleDescriptionArg>
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        -   []{#nested.classes.inherited.from.class.com.facebook.buck.shell.AbstractGenruleDescription}

            ### Nested classes/interfaces inherited from class com.facebook.buck.shell.[AbstractGenruleDescription](../shell/AbstractGenruleDescription.html "class in com.facebook.buck.shell")

            `AbstractGenruleDescription.CommonArg`
    :::

    ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        -   []{#fields.inherited.from.class.com.facebook.buck.shell.AbstractGenruleDescription}

            ### Fields inherited from class com.facebook.buck.shell.[AbstractGenruleDescription](../shell/AbstractGenruleDescription.html "class in com.facebook.buck.shell")

            `buckConfig, enableSandbox, sandboxExecutionStrategy, toolchainProvider`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                    Description
          ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ -------------
          `ApkGenruleDescription​(ToolchainProvider toolchainProvider,                      BuckConfig config,                      SandboxExecutionStrategy sandboxExecutionStrategy)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `protected BuildRule` | `createBuildRule​(B    |                       |
        |                       | uildTarget buildTarge |                       |
        |                       | t,                Pro |                       |
        |                       | jectFilesystem projec |                       |
        |                       | tFilesystem,          |                       |
        |                       |        BuildRuleParam |                       |
        |                       | s params,             |                       |
        |                       |     ActionGraphBuilde |                       |
        |                       | r graphBuilder,       |                       |
        |                       |           ApkGenruleD |                       |
        |                       | escriptionArg args,   |                       |
        |                       |               Optiona |                       |
        |                       | l<Arg> cmd,           |                       |
        |                       |       Optional<Arg> b |                       |
        |                       | ash,                O |                       |
        |                       | ptional<Arg> cmdExe)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Class<ApkGe          | `get                  | ::: block             |
        | nruleDescriptionArg>` | ConstructorArgType()` | The type of the       |
        |                       |                       | constructor argument  |
        |                       |                       | that is used by this  |
        |                       |                       | description to create |
        |                       |                       | a rule                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.shell.AbstractGenruleDescription}

            ### Methods inherited from class com.facebook.buck.shell.[AbstractGenruleDescription](../shell/AbstractGenruleDescription.html "class in com.facebook.buck.shell")

            `canExecuteRemotely, createBuildRule, createBuildRule, findDepsForTargetFromConstructorArgs, getAndroidToolsOptional, getGenruleType, getMacroHandler`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.description.BaseDescription}

            ### Methods inherited from interface com.facebook.buck.core.description.[BaseDescription](../core/description/BaseDescription.html "interface in com.facebook.buck.core.description")

            `getConfigurationDeps`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.DescriptionWithTargetGraph}

            ### Methods inherited from interface com.facebook.buck.core.rules.[DescriptionWithTargetGraph](../core/rules/DescriptionWithTargetGraph.html "interface in com.facebook.buck.core.rules")

            `producesCacheableSubgraph`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.core.toolchain.ToolchainProvider,com.facebook.buck.core.config.BuckConfig,com.facebook.buck.sandbox.SandboxExecutionStrategy)}

        -   #### ApkGenruleDescription

                public ApkGenruleDescription​(ToolchainProvider toolchainProvider,
                                             BuckConfig config,
                                             SandboxExecutionStrategy sandboxExecutionStrategy)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getConstructorArgType()}

        -   #### getConstructorArgType

            ``` methodSignature
            public Class<ApkGenruleDescriptionArg> getConstructorArgType()
            ```

            ::: block
            [Description copied from
            interface: `BaseDescription`]{.descfrmTypeLabel}
            :::

            ::: block
            The type of the constructor argument that is used by this
            description to create a rule
            :::

        []{#createBuildRule(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.rules.BuildRuleParams,com.facebook.buck.core.rules.ActionGraphBuilder,com.facebook.buck.android.ApkGenruleDescriptionArg,java.util.Optional,java.util.Optional,java.util.Optional)}

        -   #### createBuildRule

            ``` methodSignature
            protected BuildRule createBuildRule​(BuildTarget buildTarget,
                                                ProjectFilesystem projectFilesystem,
                                                BuildRuleParams params,
                                                ActionGraphBuilder graphBuilder,
                                                ApkGenruleDescriptionArg args,
                                                Optional<Arg> cmd,
                                                Optional<Arg> bash,
                                                Optional<Arg> cmdExe)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `createBuildRule` in
                class `AbstractGenruleDescription<ApkGenruleDescriptionArg>`
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
-   [Field](#field.summary) \| 
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
