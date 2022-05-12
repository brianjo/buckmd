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
[Package]{.packageLabelInType} [com.facebook.buck.rules.modern](package-summary.html)
:::

## Class ModernBuildRule\<T extends [Buildable](Buildable.html "interface in com.facebook.buck.rules.modern")\> {#class-modernbuildrulet-extends-buildable .title title="Class ModernBuildRule"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.core.rules.impl.AbstractBuildRule](../../core/rules/impl/AbstractBuildRule.html "class in com.facebook.buck.core.rules.impl")

    -   -   com.facebook.buck.rules.modern.ModernBuildRule\<T\>

::: description
-   

    All Implemented Interfaces:
    :   `BuildEngineAction`, `AllowsNonAnnotatedFields`,
        `SupportsInputBasedRuleKey`, `BuildRule`, `HasNameAndType`,
        `Comparable<BuildRule>`

    ```{=html}
    <!-- -->
    ```

    Direct Known Subclasses:
    :   `Aapt2Compile`, `Archive`, `BaseGenrule`, `CalculateClassAbi`,
        `CalculateSourceAbiFromLibraryTarget`, `CxxLink`,
        `CxxPreprocessAndCompile`, `CxxThinLTOIndex`, `CxxThinLTOOpt`,
        `DexProducedFromJavaLibrary`, `Filegroup`, `InferNullsafe`,
        `JsFile`, `JsLibrary`, `MachoDylibStubRule`,
        `MergeThirdPartyJarResources`, `PipelinedModernBuildRule`,
        `PythonCompileRule`, `RustCompileRule`, `SplitUberRDotJavaJar`,
        `StripLinkable`, `UnitTestOptions`, `WriteFileHashCode`, `Zip`

    ------------------------------------------------------------------------

        public class ModernBuildRule<T extends Buildable>
        extends AbstractBuildRule
        implements SupportsInputBasedRuleKey

    ::: block
    ModernBuildRule wraps a Buildable into something that implements
    BuildRule (and various other interfaces used by the build engine).
    Most of the overridden methods from BuildRule/AbstractBuildRule are
    intentionally final to keep users on the safe path.
    Deps, outputs, inputs and rulekeys are derived from the fields of
    the
    [`Buildable`](Buildable.html "interface in com.facebook.buck.rules.modern").

    For simple ModernBuildRules (e.g. those that don\'t have any fields
    that can\'t be added to the rulekey), the build rule class itself
    can (and should) implement Buildable. In this case, the constructor
    taking a `Class<T>` should be used.

    Example:

         class WriteData extends ModernBuildRule<WriteData> implements Buildable {
           final String data;
           public WriteData(
               SourcePathRuleFinder ruleFinder,
               BuildTarget buildTarget,
               ProjectFilesystem projectFilesystem,
               String data) {
             super(buildTarget, projectFilesystem, ruleFinder, WriteData.class);
             this.data = data;
           }

           ...
         }
         

    Some BuildRules contain more information than just that added to the
    rulekey and used for getBuildSteps(). For these rules, the part used
    for getBuildSteps should be split out into its own implementation of
    Buildable.

    Example:

         class CopyData extends ModernBuildRule<CopyData.Impl> implements Buildable {
           BuildRule other;
           public WriteData(
               SourcePathRuleFinder ruleFinder,
               BuildTarget buildTarget,
               ProjectFilesystem projectFilesystem,
               BuildRule other) {
             super(buildTarget, projectFilesystem, ruleFinder, new Impl("hello"));
             this.other = other;
           }

           private static class Impl implements Buildable {
             ...
           }
           ...
         }
         
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Modifier       Constructor                                                                                                                                                           Description
          -------------- --------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `protected `   `ModernBuildRule​(BuildTarget buildTarget,                ProjectFilesystem filesystem,                SourcePathRuleFinder finder,                Class<T> clazz)`     
          `protected `   `ModernBuildRule​(BuildTarget buildTarget,                ProjectFilesystem filesystem,                SourcePathRuleFinder ruleFinder,                T buildable)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `int`                 | `compa                |                       |
        |                       | reTo​(BuildRule that)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `T`                   | `getBuildable()`      |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected s          | `getBuildCellPa       |                       |
        | tatic DefaultBuildCel | thFactory​(BuildContex |                       |
        | lRelativePathFactory` | t context,            |                       |
        |                       |              ProjectF |                       |
        |                       | ilesystem filesystem, |                       |
        |                       |                       |                       |
        |                       |    OutputPathResolver |                       |
        |                       |  outputPathResolver)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.com       | `getBuildDeps()`      |                       |
        | mon.collect.Immutable |                       |                       |
        | SortedSet<BuildRule>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.                 | `                     |                       |
        | google.common.collect | getBuildSteps​(BuildCo |                       |
        | .ImmutableList<Step>` | ntext context,        |                       |
        |                       |        BuildableConte |                       |
        |                       | xt buildableContext)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `OutputPathResolver`  | `get                  | ::: block             |
        |                       | OutputPathResolver()` | This field could be   |
        |                       |                       | used unsafely, most   |
        |                       |                       | ModernBuildRule       |
        |                       |                       | should never need     |
        |                       |                       | this directly and it  |
        |                       |                       | should only be used   |
        |                       |                       | within the            |
        |                       |                       | getBuildSteps() call. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static void`         | `getSetupStepsF       | ::: block             |
        |                       | orBuildable​(BuildCont | Gets the steps for    |
        |                       | ext context,          | preparing the output  |
        |                       |                  Proj | directories of the    |
        |                       | ectFilesystem filesys | build rule.           |
        |                       | tem,                  | :::                   |
        |                       |          Iterable<Pat |                       |
        |                       | h> outputs,           |                       |
        |                       |                 com.g |                       |
        |                       | oogle.common.collect. |                       |
        |                       | ImmutableList.Builder |                       |
        |                       | <Step> stepBuilder,   |                       |
        |                       |                       |                       |
        |                       |    OutputPathResolver |                       |
        |                       |  outputPathResolver)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected B          | `getSourcePath​(Ou     | ::: block             |
        | uildTargetSourcePath` | tputPath outputPath)` | This should only be   |
        |                       |                       | exposed to            |
        |                       |                       | implementations of    |
        |                       |                       | the ModernBuildRule,  |
        |                       |                       | not of the Buildable. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `prot                 | `getSource            | ::: block             |
        | ected com.google.comm | Paths​(Collection<Outp | Same as               |
        | on.collect.ImmutableS | utPath> outputPaths)` | [`getSourcePath       |
        | ortedSet<SourcePath>` |                       | (com.facebook.buck.ru |
        |                       |                       | les.modern.OutputPath |
        |                       |                       | )`](#getSourcePath(co |
        |                       |                       | m.facebook.buck.rules |
        |                       |                       | .modern.OutputPath)), |
        |                       |                       | but takes multiple    |
        |                       |                       | [`OutputPa            |
        |                       |                       | th`](OutputPath.html  |
        |                       |                       | "class in com.faceboo |
        |                       |                       | k.buck.rules.modern") |
        |                       |                       | instances and returns |
        |                       |                       | multiple              |
        |                       |                       | [`SourcePath`](../    |
        |                       |                       | ../core/sourcepath/So |
        |                       |                       | urcePath.html "interf |
        |                       |                       | ace in com.facebook.b |
        |                       |                       | uck.core.sourcepath") |
        |                       |                       | instances.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `SourcePath`          | `get                  |                       |
        |                       | SourcePathToOutput()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static void`         | `injectFi             | ::: block             |
        |                       | eldsIfNecessary​(Proje | Allows injecting the  |
        |                       | ctFilesystem filesyst | AbstractBuildRule     |
        |                       | em,                   | fields into a         |
        |                       |       BuildTarget tar | Buildable after       |
        |                       | get,                  | construction.         |
        |                       |        Buildable buil | :::                   |
        |                       | dable,                |                       |
        |                       |          SourcePathRu |                       |
        |                       | leFinder ruleFinder)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `inputBas             |                       |
        |                       | edRuleKeyIsEnabled()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `recordO              | ::: block             |
        |                       | utputs​(BuildableConte | Records the outputs   |
        |                       | xt buildableContext)` | of this buildrule.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static <T extend     | `recordOutputs​(Bui    | ::: block             |
        | s AddsToRuleKey>void` | ldableContext buildab | Records the outputs   |
        |                       | leContext,            | of this buildrule.    |
        |                       |    OutputPathResolver | :::                   |
        |                       |  outputPathResolver,  |                       |
        |                       |              ClassInf |                       |
        |                       | o<T> classInfo,       |                       |
        |                       |         T buildable)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static <T extend     | `r                    | ::: block             |
        | s AddsToRuleKey>void` | ecordOutputs​(Buildabl | Records the outputs   |
        |                       | eContext buildableCon | of this buildrule.    |
        |                       | text,              Ou | :::                   |
        |                       | tputPathResolver outp |                       |
        |                       | utPathResolver,       |                       |
        |                       |         T buildable)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static <T e          | `stepsForBuil         | ::: block             |
        | xtends Buildable>com. | dable​(BuildContext co | Return the steps for  |
        | google.common.collect | ntext,                | a buildable.          |
        | .ImmutableList<Step>` |    T buildable,       | :::                   |
        |                       |             ProjectFi |                       |
        |                       | lesystem filesystem,  |                       |
        |                       |                  Buil |                       |
        |                       | dTarget buildTarget)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static <T e          | `stepsForBui          | ::: block             |
        | xtends Buildable>com. | ldable​(BuildContext c | Returns the build     |
        | google.common.collect | ontext,               | steps for the         |
        | .ImmutableList<Step>` |     T buildable,      | Buildable.            |
        |                       |              ProjectF | :::                   |
        |                       | ilesystem filesystem, |                       |
        |                       |                   Bui |                       |
        |                       | ldTarget buildTarget, |                       |
        |                       |                   Ite |                       |
        |                       | rable<Path> outputs)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `updateBuildRul       | ::: block             |
        |                       | eResolver​(BuildRuleRe | Updates the           |
        |                       | solver ruleResolver)` | BuildRuleResolver and |
        |                       |                       | associated objects    |
        |                       |                       | for this build rule.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.impl.AbstractBuildRule}

            ### Methods inherited from class com.facebook.buck.core.rules.impl.[AbstractBuildRule](../../core/rules/impl/AbstractBuildRule.html "class in com.facebook.buck.core.rules.impl")

            `equals, getBuildTarget, getDependencies, getProjectFilesystem, getSourcePathOutputs, getType, hasBuildSteps, hashCode, injectFields, isCacheable, toString`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, finalize, getClass, notify, notifyAll, wait, wait, wait`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.build.action.BuildEngineAction}

            ### Methods inherited from interface com.facebook.buck.core.build.action.[BuildEngineAction](../../core/build/action/BuildEngineAction.html "interface in com.facebook.buck.core.build.action")

            `getDependencies, getSourcePathOutputs`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.BuildRule}

            ### Methods inherited from interface com.facebook.buck.core.rules.[BuildRule](../../core/rules/BuildRule.html "interface in com.facebook.buck.core.rules")

            `getBuildTarget, getFullyQualifiedName, getProjectFilesystem, hasBuildSteps, isCacheable, outputFileCanBeCopied, shouldRespectInputSizeLimitForRemoteExecution, toString`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.HasNameAndType}

            ### Methods inherited from interface com.facebook.buck.core.rules.[HasNameAndType](../../core/rules/HasNameAndType.html "interface in com.facebook.buck.core.rules")

            `getType`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.rules.SourcePathRuleFinder,java.lang.Class)}

        -   #### ModernBuildRule

                protected ModernBuildRule​(BuildTarget buildTarget,
                                          ProjectFilesystem filesystem,
                                          SourcePathRuleFinder finder,
                                          Class<T> clazz)

        []{#<init>(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.rules.SourcePathRuleFinder,com.facebook.buck.rules.modern.Buildable)}
        []{#<init>(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.rules.SourcePathRuleFinder,T)}

        -   #### ModernBuildRule

                protected ModernBuildRule​(BuildTarget buildTarget,
                                          ProjectFilesystem filesystem,
                                          SourcePathRuleFinder ruleFinder,
                                          T buildable)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#injectFieldsIfNecessary(com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.model.BuildTarget,com.facebook.buck.rules.modern.Buildable,com.facebook.buck.core.rules.SourcePathRuleFinder)}

        -   #### injectFieldsIfNecessary

            ``` methodSignature
            public static void injectFieldsIfNecessary​(ProjectFilesystem filesystem,
                                                       BuildTarget target,
                                                       Buildable buildable,
                                                       SourcePathRuleFinder ruleFinder)
            ```

            ::: block
            Allows injecting the AbstractBuildRule fields into a
            Buildable after construction.
            :::

        []{#getBuildable()}

        -   #### getBuildable

            ``` methodSignature
            public final T getBuildable()
            ```

        []{#getSourcePathToOutput()}

        -   #### getSourcePathToOutput

            ``` methodSignature
            @Nullable
            public SourcePath getSourcePathToOutput()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getSourcePathToOutput` in interface `BuildRule`

        []{#getOutputPathResolver()}

        -   #### getOutputPathResolver

            ``` methodSignature
            public OutputPathResolver getOutputPathResolver()
            ```

            ::: block
            This field could be used unsafely, most ModernBuildRule
            should never need this directly and it should only be used
            within the getBuildSteps() call.
            :::

        []{#updateBuildRuleResolver(com.facebook.buck.core.rules.BuildRuleResolver)}

        -   #### updateBuildRuleResolver

            ``` methodSignature
            public void updateBuildRuleResolver​(BuildRuleResolver ruleResolver)
            ```

            ::: block
            [Description copied from
            interface: `BuildRule`]{.descfrmTypeLabel}
            :::

            ::: block
            Updates the BuildRuleResolver and associated objects for
            this build rule.
            Build rules sometimes hold field references to build rule
            resolvers. If this build rule is to be cached, it must
            update its BuildRuleResolver when a new action graph is
            constructed to avoid leaking the entire action graph it was
            originally associated with.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `updateBuildRuleResolver` in interface `BuildRule`

            [Overrides:]{.overrideSpecifyLabel}
            :   `updateBuildRuleResolver` in class `AbstractBuildRule`

        []{#inputBasedRuleKeyIsEnabled()}

        -   #### inputBasedRuleKeyIsEnabled

            ``` methodSignature
            public final boolean inputBasedRuleKeyIsEnabled()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `inputBasedRuleKeyIsEnabled` in
                interface `SupportsInputBasedRuleKey`

        []{#getSourcePath(com.facebook.buck.rules.modern.OutputPath)}

        -   #### getSourcePath

            ``` methodSignature
            protected final BuildTargetSourcePath getSourcePath​(OutputPath outputPath)
            ```

            ::: block
            This should only be exposed to implementations of the
            ModernBuildRule, not of the Buildable.
            :::

        []{#getSourcePaths(java.util.Collection)}

        -   #### getSourcePaths

            ``` methodSignature
            protected final com.google.common.collect.ImmutableSortedSet<SourcePath> getSourcePaths​(Collection<OutputPath> outputPaths)
            ```

            ::: block
            Same as
            [`getSourcePath(com.facebook.buck.rules.modern.OutputPath)`](#getSourcePath(com.facebook.buck.rules.modern.OutputPath)),
            but takes multiple
            [`OutputPath`](OutputPath.html "class in com.facebook.buck.rules.modern")
            instances and returns multiple
            [`SourcePath`](../../core/sourcepath/SourcePath.html "interface in com.facebook.buck.core.sourcepath")
            instances.
            :::

        []{#getBuildDeps()}

        -   #### getBuildDeps

            ``` methodSignature
            public final com.google.common.collect.ImmutableSortedSet<BuildRule> getBuildDeps()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getBuildDeps` in interface `BuildRule`

            [Returns:]{.returnLabel}

            :   the set of rules that must be built before this rule.
                Normally, this matches the value of the `deps` argument
                for this build rule in the build file in which it was
                defined.

                However, there are special cases where other arguments
                pull in implicit dependencies (e.g., the `keystore`
                argument in `android_binary`). In these cases, the
                implicit dependencies are also included in the set
                returned by this method. The value of the original
                `deps` argument, as defined in the build file, must be
                accessed via a custom getter provided by the build rule.

        []{#getBuildSteps(com.facebook.buck.core.build.context.BuildContext,com.facebook.buck.core.build.buildable.context.BuildableContext)}

        -   #### getBuildSteps

            ``` methodSignature
            public final com.google.common.collect.ImmutableList<Step> getBuildSteps​(BuildContext context,
                                                                                     BuildableContext buildableContext)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getBuildSteps` in interface `BuildRule`

        []{#stepsForBuildable(com.facebook.buck.core.build.context.BuildContext,com.facebook.buck.rules.modern.Buildable,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.model.BuildTarget,java.lang.Iterable)}
        []{#stepsForBuildable(com.facebook.buck.core.build.context.BuildContext,T,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.model.BuildTarget,java.lang.Iterable)}

        -   #### stepsForBuildable

            ``` methodSignature
            public static <T extends Buildable> com.google.common.collect.ImmutableList<Step> stepsForBuildable​(BuildContext context,
                                                                                                                T buildable,
                                                                                                                ProjectFilesystem filesystem,
                                                                                                                BuildTarget buildTarget,
                                                                                                                Iterable<Path> outputs)
            ```

            ::: block
            Returns the build steps for the Buildable. Unlike
            getBuildSteps(), this does not record outputs (callers
            should call recordOutputs() themselves).
            :::

        []{#getBuildCellPathFactory(com.facebook.buck.core.build.context.BuildContext,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.rules.modern.OutputPathResolver)}

        -   #### getBuildCellPathFactory

            ``` methodSignature
            protected static DefaultBuildCellRelativePathFactory getBuildCellPathFactory​(BuildContext context,
                                                                                         ProjectFilesystem filesystem,
                                                                                         OutputPathResolver outputPathResolver)
            ```

        []{#getSetupStepsForBuildable(com.facebook.buck.core.build.context.BuildContext,com.facebook.buck.io.filesystem.ProjectFilesystem,java.lang.Iterable,com.google.common.collect.ImmutableList.Builder,com.facebook.buck.rules.modern.OutputPathResolver)}

        -   #### getSetupStepsForBuildable

            ``` methodSignature
            public static void getSetupStepsForBuildable​(BuildContext context,
                                                         ProjectFilesystem filesystem,
                                                         Iterable<Path> outputs,
                                                         com.google.common.collect.ImmutableList.Builder<Step> stepBuilder,
                                                         OutputPathResolver outputPathResolver)
            ```

            ::: block
            Gets the steps for preparing the output directories of the
            build rule.
            :::

        []{#stepsForBuildable(com.facebook.buck.core.build.context.BuildContext,com.facebook.buck.rules.modern.Buildable,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.model.BuildTarget)}
        []{#stepsForBuildable(com.facebook.buck.core.build.context.BuildContext,T,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.model.BuildTarget)}

        -   #### stepsForBuildable

            ``` methodSignature
            public static <T extends Buildable> com.google.common.collect.ImmutableList<Step> stepsForBuildable​(BuildContext context,
                                                                                                                T buildable,
                                                                                                                ProjectFilesystem filesystem,
                                                                                                                BuildTarget buildTarget)
            ```

            ::: block
            Return the steps for a buildable.
            :::

        []{#recordOutputs(com.facebook.buck.core.build.buildable.context.BuildableContext)}

        -   #### recordOutputs

            ``` methodSignature
            public void recordOutputs​(BuildableContext buildableContext)
            ```

            ::: block
            Records the outputs of this buildrule. An output will only
            be recorded once (i.e. no duplicates and if a directory is
            recorded, none of its contents will be).
            :::

        []{#recordOutputs(com.facebook.buck.core.build.buildable.context.BuildableContext,com.facebook.buck.rules.modern.OutputPathResolver,com.facebook.buck.rules.modern.ClassInfo,com.facebook.buck.core.rulekey.AddsToRuleKey)}
        []{#recordOutputs(com.facebook.buck.core.build.buildable.context.BuildableContext,com.facebook.buck.rules.modern.OutputPathResolver,com.facebook.buck.rules.modern.ClassInfo,T)}

        -   #### recordOutputs

            ``` methodSignature
            public static <T extends AddsToRuleKey> void recordOutputs​(BuildableContext buildableContext,
                                                                       OutputPathResolver outputPathResolver,
                                                                       ClassInfo<T> classInfo,
                                                                       T buildable)
            ```

            ::: block
            Records the outputs of this buildrule. An output will only
            be recorded once (i.e. no duplicates and if a directory is
            recorded, none of its contents will be).
            :::

        []{#recordOutputs(com.facebook.buck.core.build.buildable.context.BuildableContext,com.facebook.buck.rules.modern.OutputPathResolver,com.facebook.buck.core.rulekey.AddsToRuleKey)}
        []{#recordOutputs(com.facebook.buck.core.build.buildable.context.BuildableContext,com.facebook.buck.rules.modern.OutputPathResolver,T)}

        -   #### recordOutputs

            ``` methodSignature
            public static <T extends AddsToRuleKey> void recordOutputs​(BuildableContext buildableContext,
                                                                       OutputPathResolver outputPathResolver,
                                                                       T buildable)
            ```

            ::: block
            Records the outputs of this buildrule. An output will only
            be recorded once (i.e. no duplicates and if a directory is
            recorded, none of its contents will be).
            :::

        []{#compareTo(com.facebook.buck.core.rules.BuildRule)}

        -   #### compareTo

            ``` methodSignature
            public final int compareTo​(BuildRule that)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `compareTo` in interface `BuildRule`

            [Specified by:]{.overrideSpecifyLabel}
            :   `compareTo` in
                interface `Comparable<T extends Buildable>`
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
