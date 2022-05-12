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
[Package]{.packageLabelInType} [com.facebook.buck.jvm.java](package-summary.html)
:::

## Class JarGenruleDescription {#class-jargenruledescription .title title="Class JarGenruleDescription"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.shell.AbstractGenruleDescription](../../shell/AbstractGenruleDescription.html "class in com.facebook.buck.shell")\<[JarGenruleDescriptionArg](JarGenruleDescriptionArg.html "class in com.facebook.buck.jvm.java")\>

    -   -   com.facebook.buck.jvm.java.JarGenruleDescription

::: description
-   

    All Implemented Interfaces:
    :   `ImplicitDepsInferringDescription<JarGenruleDescriptionArg>`,
        `BaseDescription<JarGenruleDescriptionArg>`,
        `Description<JarGenruleDescriptionArg>`,
        `DescriptionWithTargetGraph<JarGenruleDescriptionArg>`

    ------------------------------------------------------------------------

        public class JarGenruleDescription
        extends AbstractGenruleDescription<JarGenruleDescriptionArg>
        implements ImplicitDepsInferringDescription<JarGenruleDescriptionArg>

    ::: block
    Based on
    [`GenruleDescription`](../../shell/GenruleDescription.html "class in com.facebook.buck.shell")
    except specialized to produce a jar.
    The produced jar behaves similarly to a jar produced by java_binary,
    which means it can be executed by `buck run` or using the `$(exe )`
    macro.
    :::
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

          Constructor                                                                                                                                                                    Description
          ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ -------------
          `JarGenruleDescription​(ToolchainProvider toolchainProvider,                      BuckConfig config,                      SandboxExecutionStrategy sandboxExecutionStrategy)`    

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
        |                       |           JarGenruleD |                       |
        |                       | escriptionArg args,   |                       |
        |                       |               Optiona |                       |
        |                       | l<Arg> cmd,           |                       |
        |                       |       Optional<Arg> b |                       |
        |                       | ash,                O |                       |
        |                       | ptional<Arg> cmdExe)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `findDepsForTar       |                       |
        |                       | getFromConstructorArg |                       |
        |                       | s​(BuildTarget buildTa |                       |
        |                       | rget,                 |                       |
        |                       |                       |                       |
        |                       | CellNameResolver cell |                       |
        |                       | Roots,                |                       |
        |                       |                       |                       |
        |                       |  JarGenruleDescriptio |                       |
        |                       | nArg constructorArg,  |                       |
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
        | `Class<JarGe          | `get                  | ::: block             |
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

            ### Methods inherited from class com.facebook.buck.shell.[AbstractGenruleDescription](../../shell/AbstractGenruleDescription.html "class in com.facebook.buck.shell")

            `canExecuteRemotely, createBuildRule, createBuildRule, getAndroidToolsOptional, getGenruleType, getMacroHandler`

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

            `producesCacheableSubgraph`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.core.toolchain.ToolchainProvider,com.facebook.buck.core.config.BuckConfig,com.facebook.buck.sandbox.SandboxExecutionStrategy)}

        -   #### JarGenruleDescription

                public JarGenruleDescription​(ToolchainProvider toolchainProvider,
                                             BuckConfig config,
                                             SandboxExecutionStrategy sandboxExecutionStrategy)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getConstructorArgType()}

        -   #### getConstructorArgType

            ``` methodSignature
            public Class<JarGenruleDescriptionArg> getConstructorArgType()
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
                interface `BaseDescription<JarGenruleDescriptionArg>`

        []{#createBuildRule(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.rules.BuildRuleParams,com.facebook.buck.core.rules.ActionGraphBuilder,com.facebook.buck.jvm.java.JarGenruleDescriptionArg,java.util.Optional,java.util.Optional,java.util.Optional)}

        -   #### createBuildRule

            ``` methodSignature
            protected BuildRule createBuildRule​(BuildTarget buildTarget,
                                                ProjectFilesystem projectFilesystem,
                                                BuildRuleParams params,
                                                ActionGraphBuilder graphBuilder,
                                                JarGenruleDescriptionArg args,
                                                Optional<Arg> cmd,
                                                Optional<Arg> bash,
                                                Optional<Arg> cmdExe)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `createBuildRule` in
                class `AbstractGenruleDescription<JarGenruleDescriptionArg>`

        []{#findDepsForTargetFromConstructorArgs(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.cell.nameresolver.CellNameResolver,com.facebook.buck.jvm.java.JarGenruleDescriptionArg,com.google.common.collect.ImmutableCollection.Builder,com.google.common.collect.ImmutableCollection.Builder)}

        -   #### findDepsForTargetFromConstructorArgs

            ``` methodSignature
            public void findDepsForTargetFromConstructorArgs​(BuildTarget buildTarget,
                                                             CellNameResolver cellRoots,
                                                             JarGenruleDescriptionArg constructorArg,
                                                             com.google.common.collect.ImmutableCollection.Builder<BuildTarget> extraDepsBuilder,
                                                             com.google.common.collect.ImmutableCollection.Builder<BuildTarget> targetGraphOnlyDepsBuilder)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `findDepsForTargetFromConstructorArgs` in
                interface `ImplicitDepsInferringDescription<JarGenruleDescriptionArg>`

            [Overrides:]{.overrideSpecifyLabel}
            :   `findDepsForTargetFromConstructorArgs` in
                class `AbstractGenruleDescription<JarGenruleDescriptionArg>`
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
