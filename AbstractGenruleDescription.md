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
-   [Field](#field.detail) \| 
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

## Class AbstractGenruleDescription\<T extends [AbstractGenruleDescription.CommonArg](AbstractGenruleDescription.CommonArg.html "interface in com.facebook.buck.shell")\> {#class-abstractgenruledescriptiont-extends-abstractgenruledescription.commonarg .title title="Class AbstractGenruleDescription"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.shell.AbstractGenruleDescription\<T\>

::: description
-   

    All Implemented Interfaces:
    :   `ImplicitDepsInferringDescription<T>`, `BaseDescription<T>`,
        `Description<T>`, `DescriptionWithTargetGraph<T>`

    ```{=html}
    <!-- -->
    ```

    Direct Known Subclasses:
    :   `ApkGenruleDescription`, `CxxGenruleDescription`,
        `GenruleDescription`, `JarGenruleDescription`,
        `JsBundleGenruleDescription`

    ------------------------------------------------------------------------

        public abstract class AbstractGenruleDescription<T extends AbstractGenruleDescription.CommonArg>
        extends Object
        implements DescriptionWithTargetGraph<T>, ImplicitDepsInferringDescription<T>
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type     Class                                    Description
          --------------------- ---------------------------------------- -------------
          `static interface `   `AbstractGenruleDescription.CommonArg`    

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type                      Field                        Description
          -------------------------------------- ---------------------------- -------------
          `protected BuckConfig`                 `buckConfig`                  
          `protected boolean`                    `enableSandbox`               
          `protected SandboxExecutionStrategy`   `sandboxExecutionStrategy`    
          `protected ToolchainProvider`          `toolchainProvider`           

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Modifier       Constructor                                                                                                                                                                                                                                        Description
          -------------- -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `protected `   `AbstractGenruleDescription​(ToolchainProvider toolchainProvider,                           BuckConfig buckConfig,                           SandboxExecutionStrategy sandboxExecutionStrategy,                           boolean enableSandbox)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `protected boolean`   | `canExe               |                       |
        |                       | cuteRemotely​(T args)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protecte             | `createBuildRule      |                       |
        | d abstract BuildRule` | ​(BuildTarget buildTar |                       |
        |                       | get,                P |                       |
        |                       | rojectFilesystem proj |                       |
        |                       | ectFilesystem,        |                       |
        |                       |          BuildRulePar |                       |
        |                       | ams params,           |                       |
        |                       |       ActionGraphBuil |                       |
        |                       | der graphBuilder,     |                       |
        |                       |             T args,   |                       |
        |                       |               Optiona |                       |
        |                       | l<Arg> cmd,           |                       |
        |                       |       Optional<Arg> b |                       |
        |                       | ash,                O |                       |
        |                       | ptional<Arg> cmdExe)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected BuildRule` | `createBu             |                       |
        |                       | ildRule​(BuildTarget b |                       |
        |                       | uildTarget,           |                       |
        |                       |       ProjectFilesyst |                       |
        |                       | em projectFilesystem, |                       |
        |                       |                 Build |                       |
        |                       | RuleResolver resolver |                       |
        |                       | ,                T ar |                       |
        |                       | gs,                Op |                       |
        |                       | tional<Arg> cmd,      |                       |
        |                       |            Optional<A |                       |
        |                       | rg> bash,             |                       |
        |                       |     Optional<Arg> cmd |                       |
        |                       | Exe,                O |                       |
        |                       | ptional<String> outpu |                       |
        |                       | tFileName,            |                       |
        |                       |      Optional<com.goo |                       |
        |                       | gle.common.collect.Im |                       |
        |                       | mutableMap<String,​com |                       |
        |                       | .google.common.collec |                       |
        |                       | t.ImmutableSet<String |                       |
        |                       | >>> outputFileNames)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `BuildRule`           | `createBuildRule​(Buil | ::: block             |
        |                       | dRuleCreationContextW | Create a              |
        |                       | ithTargetGraph contex | [`B                   |
        |                       | t,                Bui | uildRule`](../core/ru |
        |                       | ldTarget buildTarget, | les/BuildRule.html "i |
        |                       |                 Build | nterface in com.faceb |
        |                       | RuleParams params,    | ook.buck.core.rules") |
        |                       |              T args)` | for the given         |
        |                       |                       | [`BuildRuleP          |
        |                       |                       | arams`](../core/rules |
        |                       |                       | /BuildRuleParams.html |
        |                       |                       |  "class in com.facebo |
        |                       |                       | ok.buck.core.rules"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `findDepsForT         |                       |
        |                       | argetFromConstructorA |                       |
        |                       | rgs​(BuildTarget build |                       |
        |                       | Target,               |                       |
        |                       |                       |                       |
        |                       |   CellNameResolver ce |                       |
        |                       | llRoots,              |                       |
        |                       |                       |                       |
        |                       |    T constructorArg,  |                       |
        |                       |                       |                       |
        |                       |                com.go |                       |
        |                       | ogle.common.collect.I |                       |
        |                       | mmutableCollection.Bu |                       |
        |                       | ilder<BuildTarget> ex |                       |
        |                       | traDepsBuilder,       |                       |
        |                       |                       |                       |
        |                       |           com.google. |                       |
        |                       | common.collect.Immuta |                       |
        |                       | bleCollection.Builder |                       |
        |                       | <BuildTarget> targetG |                       |
        |                       | raphOnlyDepsBuilder)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected Op         | `                     | ::: block             |
        | tional<AndroidTools>` | getAndroidToolsOption | Returns android tools |
        |                       | al​(T args,            | if `args` has         |
        |                       |              TargetCo | need_android_tools    |
        |                       | nfiguration toolchain | option set or empty   |
        |                       | TargetConfiguration)` | optional otherwise.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `protected String`    | `getGenruleType()`    |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected            | `get                  |                       |
        | Optional<com.google.c | MacroHandler​(BuildTar |                       |
        | ommon.collect.Immutab | get buildTarget,      |                       |
        | leList<MacroExpander< |            ProjectFil |                       |
        | ? extends Macro,​?>>>` | esystem filesystem,   |                       |
        |                       |               BuildRu |                       |
        |                       | leResolver resolver,  |                       |
        |                       |                Target |                       |
        |                       | Graph targetGraph,    |                       |
        |                       |              T args)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.description.BaseDescription}

            ### Methods inherited from interface com.facebook.buck.core.description.[BaseDescription](../core/description/BaseDescription.html "interface in com.facebook.buck.core.description")

            `getConfigurationDeps, getConstructorArgType`

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
    -   []{#field.detail}

        ### Field Detail

        []{#toolchainProvider}

        -   #### toolchainProvider

                protected final ToolchainProvider toolchainProvider

        []{#buckConfig}

        -   #### buckConfig

                protected final BuckConfig buckConfig

        []{#sandboxExecutionStrategy}

        -   #### sandboxExecutionStrategy

                protected final SandboxExecutionStrategy sandboxExecutionStrategy

        []{#enableSandbox}

        -   #### enableSandbox

                protected final boolean enableSandbox
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.core.toolchain.ToolchainProvider,com.facebook.buck.core.config.BuckConfig,com.facebook.buck.sandbox.SandboxExecutionStrategy,boolean)}

        -   #### AbstractGenruleDescription

                protected AbstractGenruleDescription​(ToolchainProvider toolchainProvider,
                                                     BuckConfig buckConfig,
                                                     SandboxExecutionStrategy sandboxExecutionStrategy,
                                                     boolean enableSandbox)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#createBuildRule(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.rules.BuildRuleParams,com.facebook.buck.core.rules.ActionGraphBuilder,com.facebook.buck.shell.AbstractGenruleDescription.CommonArg,java.util.Optional,java.util.Optional,java.util.Optional)}
        []{#createBuildRule(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.rules.BuildRuleParams,com.facebook.buck.core.rules.ActionGraphBuilder,T,java.util.Optional,java.util.Optional,java.util.Optional)}

        -   #### createBuildRule

            ``` methodSignature
            protected abstract BuildRule createBuildRule​(BuildTarget buildTarget,
                                                         ProjectFilesystem projectFilesystem,
                                                         BuildRuleParams params,
                                                         ActionGraphBuilder graphBuilder,
                                                         T args,
                                                         Optional<Arg> cmd,
                                                         Optional<Arg> bash,
                                                         Optional<Arg> cmdExe)
            ```

        []{#getGenruleType()}

        -   #### getGenruleType

            ``` methodSignature
            protected String getGenruleType()
            ```

            [Returns:]{.returnLabel}
            :   a
                [`String`](http://docs.oracle.com/javase/7/docs/api/java/lang/String.html?is-external=true "class or interface in java.lang"){.externalLink}
                representing the type of the genrule

        []{#canExecuteRemotely(com.facebook.buck.shell.AbstractGenruleDescription.CommonArg)}
        []{#canExecuteRemotely(T)}

        -   #### canExecuteRemotely

            ``` methodSignature
            protected boolean canExecuteRemotely​(T args)
            ```

            [Returns:]{.returnLabel}
            :   whether this genrule can use remote execution.

        []{#createBuildRule(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.rules.BuildRuleResolver,com.facebook.buck.shell.AbstractGenruleDescription.CommonArg,java.util.Optional,java.util.Optional,java.util.Optional,java.util.Optional,java.util.Optional)}
        []{#createBuildRule(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.rules.BuildRuleResolver,T,java.util.Optional,java.util.Optional,java.util.Optional,java.util.Optional,java.util.Optional)}

        -   #### createBuildRule

            ``` methodSignature
            protected BuildRule createBuildRule​(BuildTarget buildTarget,
                                                ProjectFilesystem projectFilesystem,
                                                BuildRuleResolver resolver,
                                                T args,
                                                Optional<Arg> cmd,
                                                Optional<Arg> bash,
                                                Optional<Arg> cmdExe,
                                                Optional<String> outputFileName,
                                                Optional<com.google.common.collect.ImmutableMap<String,​com.google.common.collect.ImmutableSet<String>>> outputFileNames)
            ```

        []{#getAndroidToolsOptional(com.facebook.buck.shell.AbstractGenruleDescription.CommonArg,com.facebook.buck.core.model.TargetConfiguration)}
        []{#getAndroidToolsOptional(T,com.facebook.buck.core.model.TargetConfiguration)}

        -   #### getAndroidToolsOptional

            ``` methodSignature
            protected Optional<AndroidTools> getAndroidToolsOptional​(T args,
                                                                     TargetConfiguration toolchainTargetConfiguration)
            ```

            ::: block
            Returns android tools if `args` has need_android_tools
            option set or empty optional otherwise.
            :::

        []{#getMacroHandler(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.rules.BuildRuleResolver,com.facebook.buck.core.model.targetgraph.TargetGraph,com.facebook.buck.shell.AbstractGenruleDescription.CommonArg)}
        []{#getMacroHandler(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.rules.BuildRuleResolver,com.facebook.buck.core.model.targetgraph.TargetGraph,T)}

        -   #### getMacroHandler

            ``` methodSignature
            protected Optional<com.google.common.collect.ImmutableList<MacroExpander<? extends Macro,​?>>> getMacroHandler​(BuildTarget buildTarget,
                                                                                                                                ProjectFilesystem filesystem,
                                                                                                                                BuildRuleResolver resolver,
                                                                                                                                TargetGraph targetGraph,
                                                                                                                                T args)
            ```

            [Returns:]{.returnLabel}
            :   the
                [`MacroExpander`](../rules/macros/MacroExpander.html "interface in com.facebook.buck.rules.macros")s
                which apply to the macros in this description.

        []{#createBuildRule(com.facebook.buck.core.rules.BuildRuleCreationContextWithTargetGraph,com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.rules.BuildRuleParams,com.facebook.buck.shell.AbstractGenruleDescription.CommonArg)}
        []{#createBuildRule(com.facebook.buck.core.rules.BuildRuleCreationContextWithTargetGraph,com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.rules.BuildRuleParams,T)}

        -   #### createBuildRule

            ``` methodSignature
            public BuildRule createBuildRule​(BuildRuleCreationContextWithTargetGraph context,
                                             BuildTarget buildTarget,
                                             BuildRuleParams params,
                                             T args)
            ```

            ::: block
            [Description copied from
            interface: `DescriptionWithTargetGraph`]{.descfrmTypeLabel}
            :::

            ::: block
            Create a
            [`BuildRule`](../core/rules/BuildRule.html "interface in com.facebook.buck.core.rules")
            for the given
            [`BuildRuleParams`](../core/rules/BuildRuleParams.html "class in com.facebook.buck.core.rules").
            Note that the
            [`BuildTarget`](../core/model/BuildTarget.html "class in com.facebook.buck.core.model")
            referred to in the `params` contains the
            [`Flavor`](../core/model/Flavor.html "interface in com.facebook.buck.core.model")
            to create.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `createBuildRule` in
                interface `DescriptionWithTargetGraph<T extends AbstractGenruleDescription.CommonArg>`
            :   `args` - A constructor argument, of type as returned by
                [`BaseDescription.getConstructorArgType()`](../core/description/BaseDescription.html#getConstructorArgType()).

            [Returns:]{.returnLabel}
            :   The
                [`BuildRule`](../core/rules/BuildRule.html "interface in com.facebook.buck.core.rules")
                that describes the default flavour of the rule being
                described.

        []{#findDepsForTargetFromConstructorArgs(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.cell.nameresolver.CellNameResolver,com.facebook.buck.shell.AbstractGenruleDescription.CommonArg,com.google.common.collect.ImmutableCollection.Builder,com.google.common.collect.ImmutableCollection.Builder)}
        []{#findDepsForTargetFromConstructorArgs(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.cell.nameresolver.CellNameResolver,T,com.google.common.collect.ImmutableCollection.Builder,com.google.common.collect.ImmutableCollection.Builder)}

        -   #### findDepsForTargetFromConstructorArgs

            ``` methodSignature
            public void findDepsForTargetFromConstructorArgs​(BuildTarget buildTarget,
                                                             CellNameResolver cellRoots,
                                                             T constructorArg,
                                                             com.google.common.collect.ImmutableCollection.Builder<BuildTarget> extraDepsBuilder,
                                                             com.google.common.collect.ImmutableCollection.Builder<BuildTarget> targetGraphOnlyDepsBuilder)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `findDepsForTargetFromConstructorArgs` in
                interface `ImplicitDepsInferringDescription<T extends AbstractGenruleDescription.CommonArg>`
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
-   [Field](#field.detail) \| 
-   [Constr](#constructor.detail) \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
