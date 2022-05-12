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
[Package]{.packageLabelInType} [com.facebook.buck.features.js](package-summary.html)
:::

## Class JsBundleGenruleDescription {#class-jsbundlegenruledescription .title title="Class JsBundleGenruleDescription"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.shell.AbstractGenruleDescription](../../shell/AbstractGenruleDescription.html "class in com.facebook.buck.shell")\<[JsBundleGenruleDescriptionArg](JsBundleGenruleDescriptionArg.html "class in com.facebook.buck.features.js")\>

    -   -   com.facebook.buck.features.js.JsBundleGenruleDescription

::: description
-   

    All Implemented Interfaces:
    :   `HasAppleBundleResourcesDescription<JsBundleGenruleDescriptionArg>`,
        `ImplicitDepsInferringDescription<JsBundleGenruleDescriptionArg>`,
        `BaseDescription<JsBundleGenruleDescriptionArg>`,
        `Description<JsBundleGenruleDescriptionArg>`, `Flavored`,
        `DescriptionWithTargetGraph<JsBundleGenruleDescriptionArg>`,
        `JsBundleOutputsDescription<JsBundleGenruleDescriptionArg>`

    ------------------------------------------------------------------------

        public class JsBundleGenruleDescription
        extends AbstractGenruleDescription<JsBundleGenruleDescriptionArg>
        implements Flavored, HasAppleBundleResourcesDescription<JsBundleGenruleDescriptionArg>, JsBundleOutputsDescription<JsBundleGenruleDescriptionArg>
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        -   []{#nested.classes.inherited.from.class.com.facebook.buck.shell.AbstractGenruleDescription}

            ### Nested classes/interfaces inherited from class com.facebook.buck.shell.[AbstractGenruleDescription](../../shell/AbstractGenruleDescription.html "class in com.facebook.buck.shell")

            `AbstractGenruleDescription.CommonArg`
    :::

    ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        -   []{#fields.inherited.from.class.com.facebook.buck.shell.AbstractGenruleDescription}

            ### Fields inherited from class com.facebook.buck.shell.[AbstractGenruleDescription](../../shell/AbstractGenruleDescription.html "class in com.facebook.buck.shell")

            `buckConfig, enableSandbox, sandboxExecutionStrategy, toolchainProvider`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                   Description
          --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `JsBundleGenruleDescription​(ToolchainProvider toolchainProvider,                           BuckConfig config,                           SandboxExecutionStrategy sandboxExecutionStrategy)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `void`                | `addAppleBund         |                       |
        |                       | leResources​(AppleBund |                       |
        |                       | leResources.Builder b |                       |
        |                       | uilder,               |                       |
        |                       |           TargetNode< |                       |
        |                       | JsBundleGenruleDescri |                       |
        |                       | ptionArg> targetNode, |                       |
        |                       |                       |                       |
        |                       |    ProjectFilesystem  |                       |
        |                       | filesystem,           |                       |
        |                       |               BuildRu |                       |
        |                       | leResolver resolver)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected BuildRule` | `c                    |                       |
        |                       | reateBuildRule​(BuildT |                       |
        |                       | arget buildTarget,    |                       |
        |                       |              ProjectF |                       |
        |                       | ilesystem projectFile |                       |
        |                       | system,               |                       |
        |                       |   BuildRuleParams par |                       |
        |                       | ams,                A |                       |
        |                       | ctionGraphBuilder gra |                       |
        |                       | phBuilder,            |                       |
        |                       |      JsBundleGenruleD |                       |
        |                       | escriptionArg args,   |                       |
        |                       |               Optiona |                       |
        |                       | l<Arg> cmd,           |                       |
        |                       |       Optional<Arg> b |                       |
        |                       | ash,                O |                       |
        |                       | ptional<Arg> cmdExe)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Opt                  | `f                    |                       |
        | ional<com.google.comm | lavorDomains​(TargetCo |                       |
        | on.collect.ImmutableS | nfiguration toolchain |                       |
        | et<FlavorDomain<?>>>` | TargetConfiguration)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Class<JsBundleGe     | `get                  | ::: block             |
        | nruleDescriptionArg>` | ConstructorArgType()` | The type of the       |
        |                       |                       | constructor argument  |
        |                       |                       | that is used by this  |
        |                       |                       | description to create |
        |                       |                       | a rule                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `h                    |                       |
        |                       | asFlavors​(com.google. |                       |
        |                       | common.collect.Immuta |                       |
        |                       | bleSet<Flavor> flavor |                       |
        |                       | s,           TargetCo |                       |
        |                       | nfiguration toolchain |                       |
        |                       | TargetConfiguration)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.shell.AbstractGenruleDescription}

            ### Methods inherited from class com.facebook.buck.shell.[AbstractGenruleDescription](../../shell/AbstractGenruleDescription.html "class in com.facebook.buck.shell")

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

            ### Methods inherited from interface com.facebook.buck.core.description.[BaseDescription](../../core/description/BaseDescription.html "interface in com.facebook.buck.core.description")

            `getConfigurationDeps`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.DescriptionWithTargetGraph}

            ### Methods inherited from interface com.facebook.buck.core.rules.[DescriptionWithTargetGraph](../../core/rules/DescriptionWithTargetGraph.html "interface in com.facebook.buck.core.rules")

            `createBuildRule, producesCacheableSubgraph`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.core.toolchain.ToolchainProvider,com.facebook.buck.core.config.BuckConfig,com.facebook.buck.sandbox.SandboxExecutionStrategy)}

        -   #### JsBundleGenruleDescription

                public JsBundleGenruleDescription​(ToolchainProvider toolchainProvider,
                                                  BuckConfig config,
                                                  SandboxExecutionStrategy sandboxExecutionStrategy)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getConstructorArgType()}

        -   #### getConstructorArgType

            ``` methodSignature
            public Class<JsBundleGenruleDescriptionArg> getConstructorArgType()
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
                interface `BaseDescription<JsBundleGenruleDescriptionArg>`

        []{#createBuildRule(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.rules.BuildRuleParams,com.facebook.buck.core.rules.ActionGraphBuilder,com.facebook.buck.features.js.JsBundleGenruleDescriptionArg,java.util.Optional,java.util.Optional,java.util.Optional)}

        -   #### createBuildRule

            ``` methodSignature
            protected BuildRule createBuildRule​(BuildTarget buildTarget,
                                                ProjectFilesystem projectFilesystem,
                                                BuildRuleParams params,
                                                ActionGraphBuilder graphBuilder,
                                                JsBundleGenruleDescriptionArg args,
                                                Optional<Arg> cmd,
                                                Optional<Arg> bash,
                                                Optional<Arg> cmdExe)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `createBuildRule` in
                class `AbstractGenruleDescription<JsBundleGenruleDescriptionArg>`

        []{#addAppleBundleResources(com.facebook.buck.apple.AppleBundleResources.Builder,com.facebook.buck.core.model.targetgraph.TargetNode,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.rules.BuildRuleResolver)}

        -   #### addAppleBundleResources

            ``` methodSignature
            public void addAppleBundleResources​(AppleBundleResources.Builder builder,
                                                TargetNode<JsBundleGenruleDescriptionArg> targetNode,
                                                ProjectFilesystem filesystem,
                                                BuildRuleResolver resolver)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `addAppleBundleResources` in
                interface `HasAppleBundleResourcesDescription<JsBundleGenruleDescriptionArg>`

        []{#hasFlavors(com.google.common.collect.ImmutableSet,com.facebook.buck.core.model.TargetConfiguration)}

        -   #### hasFlavors

            ``` methodSignature
            public boolean hasFlavors​(com.google.common.collect.ImmutableSet<Flavor> flavors,
                                      TargetConfiguration toolchainTargetConfiguration)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `hasFlavors` in interface `Flavored`

            [Parameters:]{.paramLabel}
            :   `flavors` - The set of
                [`Flavor`](../../core/model/Flavor.html "interface in com.facebook.buck.core.model")s
                to consider. All must match.

            [Returns:]{.returnLabel}
            :   Whether a
                [`BuildRule`](../../core/rules/BuildRule.html "interface in com.facebook.buck.core.rules")
                of the given
                [`Flavor`](../../core/model/Flavor.html "interface in com.facebook.buck.core.model")
                can be created.

        []{#flavorDomains(com.facebook.buck.core.model.TargetConfiguration)}

        -   #### flavorDomains

            ``` methodSignature
            public Optional<com.google.common.collect.ImmutableSet<FlavorDomain<?>>> flavorDomains​(TargetConfiguration toolchainTargetConfiguration)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `flavorDomains` in interface `Flavored`
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
