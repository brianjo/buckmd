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
[Package]{.packageLabelInType} [com.facebook.buck.shell](package-summary.html)
:::

## Class GenruleDescription {#class-genruledescription .title title="Class GenruleDescription"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.shell.AbstractGenruleDescription](AbstractGenruleDescription.html "class in com.facebook.buck.shell")\<[GenruleDescriptionArg](GenruleDescriptionArg.html "class in com.facebook.buck.shell")\>

    -   -   com.facebook.buck.shell.GenruleDescription

::: description
-   

    All Implemented Interfaces:
    :   `ImplicitDepsInferringDescription<GenruleDescriptionArg>`,
        `BaseDescription<GenruleDescriptionArg>`,
        `Description<GenruleDescriptionArg>`,
        `DescriptionWithTargetGraph<GenruleDescriptionArg>`,
        `VersionRoot<GenruleDescriptionArg>`

    ------------------------------------------------------------------------

        public class GenruleDescription
        extends AbstractGenruleDescription<GenruleDescriptionArg>
        implements VersionRoot<GenruleDescriptionArg>
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        -   []{#nested.classes.inherited.from.class.com.facebook.buck.shell.AbstractGenruleDescription}

            ### Nested classes/interfaces inherited from class com.facebook.buck.shell.[AbstractGenruleDescription](AbstractGenruleDescription.html "class in com.facebook.buck.shell")

            `AbstractGenruleDescription.CommonArg`
    :::

    ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        -   []{#fields.inherited.from.class.com.facebook.buck.shell.AbstractGenruleDescription}

            ### Fields inherited from class com.facebook.buck.shell.[AbstractGenruleDescription](AbstractGenruleDescription.html "class in com.facebook.buck.shell")

            `buckConfig, enableSandbox, sandboxExecutionStrategy, toolchainProvider`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                               Description
          ------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `GenruleDescription​(ToolchainProvider toolchainProvider,                   BuckConfig buckConfig,                   SandboxExecutionStrategy sandboxExecutionStrategy)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `protected BuildRule` | `createBuildRul       |                       |
        |                       | e​(BuildTarget buildTa |                       |
        |                       | rget,                 |                       |
        |                       | ProjectFilesystem pro |                       |
        |                       | jectFilesystem,       |                       |
        |                       |           BuildRulePa |                       |
        |                       | rams params,          |                       |
        |                       |        ActionGraphBui |                       |
        |                       | lder graphBuilder,    |                       |
        |                       |              GenruleD |                       |
        |                       | escriptionArg args,   |                       |
        |                       |               Optiona |                       |
        |                       | l<Arg> cmd,           |                       |
        |                       |       Optional<Arg> b |                       |
        |                       | ash,                O |                       |
        |                       | ptional<Arg> cmdExe)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Class<Ge             | `get                  | ::: block             |
        | nruleDescriptionArg>` | ConstructorArgType()` | The type of the       |
        |                       |                       | constructor argument  |
        |                       |                       | that is used by this  |
        |                       |                       | description to create |
        |                       |                       | a rule                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `produce              | ::: block             |
        |                       | sCacheableSubgraph()` | Whether or not the    |
        |                       |                       | build rule subgraph   |
        |                       |                       | produced by this      |
        |                       |                       | `Description` is safe |
        |                       |                       | to cache in           |
        |                       |                       | [`Incre               |
        |                       |                       | mentalActionGraphGene |
        |                       |                       | rator`](../core/model |
        |                       |                       | /actiongraph/computat |
        |                       |                       | ion/IncrementalAction |
        |                       |                       | GraphGenerator.html " |
        |                       |                       | class in com.facebook |
        |                       |                       | .buck.core.model.acti |
        |                       |                       | ongraph.computation") |
        |                       |                       | for incremental       |
        |                       |                       | action graph          |
        |                       |                       | generation.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.shell.AbstractGenruleDescription}

            ### Methods inherited from class com.facebook.buck.shell.[AbstractGenruleDescription](AbstractGenruleDescription.html "class in com.facebook.buck.shell")

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

            `createBuildRule`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.versions.VersionRoot}

            ### Methods inherited from interface com.facebook.buck.versions.[VersionRoot](../versions/VersionRoot.html "interface in com.facebook.buck.versions")

            `isVersionRoot`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.core.toolchain.ToolchainProvider,com.facebook.buck.core.config.BuckConfig,com.facebook.buck.sandbox.SandboxExecutionStrategy)}

        -   #### GenruleDescription

                public GenruleDescription​(ToolchainProvider toolchainProvider,
                                          BuckConfig buckConfig,
                                          SandboxExecutionStrategy sandboxExecutionStrategy)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getConstructorArgType()}

        -   #### getConstructorArgType

            ``` methodSignature
            public Class<GenruleDescriptionArg> getConstructorArgType()
            ```

            ::: block
            [Description copied from
            interface: `BaseDescription`]{.descfrmTypeLabel}
            :::

            ::: block
            The type of the constructor argument that is used by this
            description to create a rule
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getConstructorArgType` in
                interface `BaseDescription<GenruleDescriptionArg>`

        []{#createBuildRule(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.rules.BuildRuleParams,com.facebook.buck.core.rules.ActionGraphBuilder,com.facebook.buck.shell.GenruleDescriptionArg,java.util.Optional,java.util.Optional,java.util.Optional)}

        -   #### createBuildRule

            ``` methodSignature
            protected BuildRule createBuildRule​(BuildTarget buildTarget,
                                                ProjectFilesystem projectFilesystem,
                                                BuildRuleParams params,
                                                ActionGraphBuilder graphBuilder,
                                                GenruleDescriptionArg args,
                                                Optional<Arg> cmd,
                                                Optional<Arg> bash,
                                                Optional<Arg> cmdExe)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `createBuildRule` in
                class `AbstractGenruleDescription<GenruleDescriptionArg>`

        []{#producesCacheableSubgraph()}

        -   #### producesCacheableSubgraph

            ``` methodSignature
            public boolean producesCacheableSubgraph()
            ```

            ::: block
            [Description copied from
            interface: `DescriptionWithTargetGraph`]{.descfrmTypeLabel}
            :::

            ::: block
            Whether or not the build rule subgraph produced by this
            `Description` is safe to cache in
            [`IncrementalActionGraphGenerator`](../core/model/actiongraph/computation/IncrementalActionGraphGenerator.html "class in com.facebook.buck.core.model.actiongraph.computation")
            for incremental action graph generation.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `producesCacheableSubgraph` in
                interface `Description<GenruleDescriptionArg>`

            [Specified by:]{.overrideSpecifyLabel}
            :   `producesCacheableSubgraph` in
                interface `DescriptionWithTargetGraph<GenruleDescriptionArg>`
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
