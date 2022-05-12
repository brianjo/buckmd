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
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   [Constr](#constructor.detail) \| 
-   Method

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

## Class Genrule {#class-genrule .title title="Class Genrule"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.core.rules.impl.AbstractBuildRule](../core/rules/impl/AbstractBuildRule.html "class in com.facebook.buck.core.rules.impl")

    -   -   [com.facebook.buck.rules.modern.ModernBuildRule](../rules/modern/ModernBuildRule.html "class in com.facebook.buck.rules.modern")\<T\>

        -   -   [com.facebook.buck.shell.BaseGenrule](BaseGenrule.html "class in com.facebook.buck.shell")\<[GenruleBuildable](GenruleBuildable.html "class in com.facebook.buck.shell")\>

            -   -   com.facebook.buck.shell.Genrule

::: description
-   

    All Implemented Interfaces:
    :   `BuildEngineAction`, `HasOutputName`,
        `AllowsNonAnnotatedFields`, `HasMultipleOutputs`,
        `SupportsInputBasedRuleKey`, `BuildRule`, `HasNameAndType`,
        `Comparable<BuildRule>`

    ```{=html}
    <!-- -->
    ```

    Direct Known Subclasses:
    :   `GenruleBinary`

    ------------------------------------------------------------------------

        public class Genrule
        extends BaseGenrule<GenruleBuildable>
        implements HasOutputName, HasMultipleOutputs

    ::: block
    Build rule for generating a file via a shell command. For example,
    to generate the katana AndroidManifest.xml from the wakizashi
    AndroidManifest.xml, such a rule could be defined as:
         genrule(
           name = 'katana_manifest',
           srcs = [
             'wakizashi_to_katana_manifest.py',
             'AndroidManifest.xml',
           ],
           cmd = 'python wakizashi_to_katana_manifest.py ${SRCDIR}/AndroidManfiest.xml > $OUT',
           out = 'AndroidManifest.xml',
         )
         

    The output of this rule would likely be used as follows:

         android_binary(
           name = 'katana',
           manifest = ':katana_manifest',
           deps = [
             # Additional dependent android_library rules would be listed here, as well.
           ],
         )
         

    Named outputs are availabe in genrules by using \`outs\` instead of
    \`out\`. Only one of \'out\' or \'outs\' may be present in a
    genrule. For example, the aforementioned rule can be defined as:

         genrule(
           name = 'katana_manifest',
           srcs = [
             'wakizashi_to_katana_manifest.py',
             'AndroidManifest.xml',
           ],
           cmd = 'python wakizashi_to_katana_manifest.py ${SRCDIR}/AndroidManfiest.xml > $OUT',
           outs = {
            'manifest': [ 'AndroidManifest.xml'] ,
           },
         )
         

    The key-value pairs in \'outs\' define the named output groups
    provided by this genrule. The keys are
    [`OutputLabel`](../core/model/OutputLabel.html "class in com.facebook.buck.core.model")
    instances, while the values are outputs relative to this genrule\'s
    output directory. Genrule outputs with \'outs\' can be consumed
    using the
    [`BuildTargetWithOutputs`](../core/model/BuildTargetWithOutputs.html "class in com.facebook.buck.core.model")
    syntax. For example:

         android_binary(
           name = 'katana',
           manifest = ':katana_manifest[manifest]',
           deps = [
             # Additional dependent android_library rules would be listed here, as well.
           ],
         )
         

    If a rule with \'outs\' is consumed without an output label, the
    default output group is returned. Currently, the default output
    group is an empty set. In the future, it would be the set of all
    named outputs.

    A `genrule` is evaluated by running the shell command specified by
    `cmd` with the following environment variable substitutions:

    -   `SRCS` will be a space-delimited string expansion of the `srcs`
        attribute where each element of `srcs` will be translated into
        an absolute path.
    -   `SRCDIR` will be a directory containing all files mentioned in
        the srcs.
    -   `TMP` will be a temporary directory which can be used for
        intermediate results
    -   `OUT` is the output file for the `genrule()` if \'out\' is used.
        If using \`outs\`, it is the output directory. The file
        specified by this variable must always be written by this
        command. If not, the execution of this rule will be considered a
        failure, halting the build process.

    In the above example, if the `katana_manifest` rule were defined in
    the `  src/com/facebook/wakizashi` directory, then the command that
    would be executed would be:
         python convert_to_katana.py src/com/facebook/wakizashi/AndroidManifest.xml > \
             buck-out/gen/src/com/facebook/wakizashi/AndroidManifest.xml
         

    Note that `cmd` could be run on either Mac or Linux, so it should
    contain logic that works on either platform. If this becomes an
    issue in the future (or we want to support building on different
    platforms), then we could introduce a new attribute that is a map of
    target platforms to the appropriate build command for that platform.
    Note that the `SRCDIR` is populated by symlinking the sources.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Modifier       Constructor                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              Description
          -------------- ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `protected `   `Genrule​(BuildTarget buildTarget,        ProjectFilesystem projectFilesystem,        BuildRuleResolver buildRuleResolver,        SandboxExecutionStrategy sandboxExecutionStrategy,        SourceSet srcs,        Optional<Arg> cmd,        Optional<Arg> bash,        Optional<Arg> cmdExe,        Optional<String> type,        Optional<String> out,        Optional<com.google.common.collect.ImmutableMap<String,​com.google.common.collect.ImmutableSet<String>>> outs,        boolean enableSandboxingInGenrule,        boolean isCacheable,        Optional<String> environmentExpansionSeparator,        Optional<AndroidTools> androidTools,        boolean executeRemotely)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        -   []{#methods.inherited.from.class.com.facebook.buck.shell.BaseGenrule}

            ### Methods inherited from class com.facebook.buck.shell.[BaseGenrule](BaseGenrule.html "class in com.facebook.buck.shell")

            `getOutputLabels, getOutputName, getSourcePathToOutput, getSourcePathToOutput, getType, isCacheable`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.rules.modern.ModernBuildRule}

            ### Methods inherited from class com.facebook.buck.rules.modern.[ModernBuildRule](../rules/modern/ModernBuildRule.html "class in com.facebook.buck.rules.modern")

            `compareTo, getBuildable, getBuildCellPathFactory, getBuildDeps, getBuildSteps, getOutputPathResolver, getSetupStepsForBuildable, getSourcePath, getSourcePaths, injectFieldsIfNecessary, inputBasedRuleKeyIsEnabled, recordOutputs, recordOutputs, recordOutputs, stepsForBuildable, stepsForBuildable, updateBuildRuleResolver`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.impl.AbstractBuildRule}

            ### Methods inherited from class com.facebook.buck.core.rules.impl.[AbstractBuildRule](../core/rules/impl/AbstractBuildRule.html "class in com.facebook.buck.core.rules.impl")

            `equals, getBuildTarget, getDependencies, getProjectFilesystem, getSourcePathOutputs, hasBuildSteps, hashCode, injectFields, toString`

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

            ### Methods inherited from interface com.facebook.buck.core.build.action.[BuildEngineAction](../core/build/action/BuildEngineAction.html "interface in com.facebook.buck.core.build.action")

            `getDependencies, getSourcePathOutputs`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.BuildRule}

            ### Methods inherited from interface com.facebook.buck.core.rules.[BuildRule](../core/rules/BuildRule.html "interface in com.facebook.buck.core.rules")

            `compareTo, getBuildDeps, getBuildSteps, getBuildTarget, getFullyQualifiedName, getProjectFilesystem, hasBuildSteps, isCacheable, outputFileCanBeCopied, shouldRespectInputSizeLimitForRemoteExecution, toString, updateBuildRuleResolver`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.attr.HasMultipleOutputs}

            ### Methods inherited from interface com.facebook.buck.core.rules.attr.[HasMultipleOutputs](../core/rules/attr/HasMultipleOutputs.html "interface in com.facebook.buck.core.rules.attr")

            `getOutputLabels, getSourcePathToOutput, getSourcePathToOutput`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.HasNameAndType}

            ### Methods inherited from interface com.facebook.buck.core.rules.[HasNameAndType](../core/rules/HasNameAndType.html "interface in com.facebook.buck.core.rules")

            `getType`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.model.HasOutputName}

            ### Methods inherited from interface com.facebook.buck.core.model.[HasOutputName](../core/model/HasOutputName.html "interface in com.facebook.buck.core.model")

            `getOutputName`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.rules.BuildRuleResolver,com.facebook.buck.sandbox.SandboxExecutionStrategy,com.facebook.buck.rules.coercer.SourceSet,java.util.Optional,java.util.Optional,java.util.Optional,java.util.Optional,java.util.Optional,java.util.Optional,boolean,boolean,java.util.Optional,java.util.Optional,boolean)}

        -   #### Genrule

                protected Genrule​(BuildTarget buildTarget,
                                  ProjectFilesystem projectFilesystem,
                                  BuildRuleResolver buildRuleResolver,
                                  SandboxExecutionStrategy sandboxExecutionStrategy,
                                  SourceSet srcs,
                                  Optional<Arg> cmd,
                                  Optional<Arg> bash,
                                  Optional<Arg> cmdExe,
                                  Optional<String> type,
                                  Optional<String> out,
                                  Optional<com.google.common.collect.ImmutableMap<String,​com.google.common.collect.ImmutableSet<String>>> outs,
                                  boolean enableSandboxingInGenrule,
                                  boolean isCacheable,
                                  Optional<String> environmentExpansionSeparator,
                                  Optional<AndroidTools> androidTools,
                                  boolean executeRemotely)
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
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   [Constr](#constructor.detail) \| 
-   Method

</div>

[]{#skip.navbar.bottom}
:::
