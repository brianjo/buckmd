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

## Class DummyRDotJava {#class-dummyrdotjava .title title="Class DummyRDotJava"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.core.rules.impl.AbstractBuildRule](../core/rules/impl/AbstractBuildRule.html "class in com.facebook.buck.core.rules.impl")

    -   -   com.facebook.buck.android.DummyRDotJava

::: description
-   

    All Implemented Interfaces:
    :   `BuildEngineAction`, `AllowsNonAnnotatedFields`,
        `InitializableFromDisk<Object>`, `SupportsInputBasedRuleKey`,
        `BuildRule`, `HasNameAndType`, `HasJavaAbi`,
        `Comparable<BuildRule>`

    ------------------------------------------------------------------------

        public class DummyRDotJava
        extends AbstractBuildRule
        implements SupportsInputBasedRuleKey, InitializableFromDisk<Object>, HasJavaAbi

    ::: block
    Buildable that takes in a list of
    [`HasAndroidResourceDeps`](HasAndroidResourceDeps.html "interface in com.facebook.buck.android")
    and for each of these rules, first creates an `R.java` file using
    [`MergeAndroidResourcesStep`](MergeAndroidResourcesStep.html "class in com.facebook.buck.android")
    and compiles it to generate a corresponding `R.class` file. These
    are called \"dummy\" `R.java` files since these are later merged
    together into a single `R.java` file by
    [`AaptStep`](AaptStep.html "class in com.facebook.buck.android").
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                                                                                                                                                                                                                              Description
          ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `DummyRDotJava​(BuildTarget buildTarget,              ProjectFilesystem projectFilesystem,              SourcePathRuleFinder ruleFinder,              Set<HasAndroidResourceDeps> androidResourceDeps,              JavacToJarStepFactory compileStepFactory,              boolean forceFinalResourceIds,              Optional<String> unionPackage,              Optional<String> finalRName,              boolean useOldStyleableFormat,              boolean skipNonUnionRDotJava)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                   Method                                                                                              Description
          ------------------------------------------------------------------- --------------------------------------------------------------------------------------------------- -------------
          `JavaAbiInfo`                                                       `getAbiInfo()`                                                                                       
          `Optional<BuildTarget>`                                             `getAbiJar()`                                                                                        
          `com.google.common.collect.ImmutableList<HasAndroidResourceDeps>`   `getAndroidResourceDeps()`                                                                           
          `com.google.common.collect.ImmutableSortedSet<BuildRule>`           `getBuildDeps()`                                                                                     
          `BuildOutputInitializer<Object>`                                    `getBuildOutputInitializer()`                                                                        
          `com.google.common.collect.ImmutableList<Step>`                     `getBuildSteps​(BuildContext context,              BuildableContext buildableContext)`                
          `static Path`                                                       `getOutputJarPath​(BuildTarget buildTarget,                 ProjectFilesystem filesystem)`            
          `static Path`                                                       `getPathToOutputDir​(BuildTarget buildTarget,                   ProjectFilesystem filesystem)`        
          `Path`                                                              `getRDotJavaBinFolder()`                                                                             
          `static Path`                                                       `getRDotJavaBinFolder​(BuildTarget buildTarget,                     ProjectFilesystem filesystem)`    
          `static Path`                                                       `getRDotJavaSrcFolder​(BuildTarget buildTarget,                     ProjectFilesystem filesystem)`    
          `SourcePath`                                                        `getSourcePathToOutput()`                                                                            
          `Object`                                                            `initializeFromDisk​(SourcePathResolverAdapter pathResolver)`                                         
          `void`                                                              `invalidateInitializeFromDiskState()`                                                                

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
          Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
          .tableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.impl.AbstractBuildRule}

            ### Methods inherited from class com.facebook.buck.core.rules.impl.[AbstractBuildRule](../core/rules/impl/AbstractBuildRule.html "class in com.facebook.buck.core.rules.impl")

            `equals, getBuildTarget, getDependencies, getProjectFilesystem, getSourcePathOutputs, getType, hasBuildSteps, hashCode, injectFields, isCacheable, toString, updateBuildRuleResolver`

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

            `compareTo, getBuildTarget, getFullyQualifiedName, getProjectFilesystem, hasBuildSteps, isCacheable, outputFileCanBeCopied, shouldRespectInputSizeLimitForRemoteExecution, toString, updateBuildRuleResolver`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.jvm.core.HasJavaAbi}

            ### Methods inherited from interface com.facebook.buck.jvm.core.[HasJavaAbi](../jvm/core/HasJavaAbi.html "interface in com.facebook.buck.jvm.core")

            `getSourceOnlyAbiJar`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.HasNameAndType}

            ### Methods inherited from interface com.facebook.buck.core.rules.[HasNameAndType](../core/rules/HasNameAndType.html "interface in com.facebook.buck.core.rules")

            `getType`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.attr.SupportsInputBasedRuleKey}

            ### Methods inherited from interface com.facebook.buck.core.rules.attr.[SupportsInputBasedRuleKey](../core/rules/attr/SupportsInputBasedRuleKey.html "interface in com.facebook.buck.core.rules.attr")

            `inputBasedRuleKeyIsEnabled`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.rules.SourcePathRuleFinder,java.util.Set,com.facebook.buck.jvm.java.JavacToJarStepFactory,boolean,java.util.Optional,java.util.Optional,boolean,boolean)}

        -   #### DummyRDotJava

                public DummyRDotJava​(BuildTarget buildTarget,
                                     ProjectFilesystem projectFilesystem,
                                     SourcePathRuleFinder ruleFinder,
                                     Set<HasAndroidResourceDeps> androidResourceDeps,
                                     JavacToJarStepFactory compileStepFactory,
                                     boolean forceFinalResourceIds,
                                     Optional<String> unionPackage,
                                     Optional<String> finalRName,
                                     boolean useOldStyleableFormat,
                                     boolean skipNonUnionRDotJava)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getBuildDeps()}

        -   #### getBuildDeps

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedSet<BuildRule> getBuildDeps()
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
            public com.google.common.collect.ImmutableList<Step> getBuildSteps​(BuildContext context,
                                                                               BuildableContext buildableContext)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getBuildSteps` in interface `BuildRule`

        []{#invalidateInitializeFromDiskState()}

        -   #### invalidateInitializeFromDiskState

            ``` methodSignature
            public void invalidateInitializeFromDiskState()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `invalidateInitializeFromDiskState` in
                interface `InitializableFromDisk<Object>`

        []{#initializeFromDisk(com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter)}

        -   #### initializeFromDisk

            ``` methodSignature
            public Object initializeFromDisk​(SourcePathResolverAdapter pathResolver)
                                      throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `initializeFromDisk` in
                interface `InitializableFromDisk<Object>`

            [Returns:]{.returnLabel}
            :   an object that has the in-memory data structures that
                need to be populated as a result of executing this
                object\'s steps.

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#getBuildOutputInitializer()}

        -   #### getBuildOutputInitializer

            ``` methodSignature
            public BuildOutputInitializer<Object> getBuildOutputInitializer()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getBuildOutputInitializer` in
                interface `InitializableFromDisk<Object>`

        []{#getRDotJavaSrcFolder(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem)}

        -   #### getRDotJavaSrcFolder

            ``` methodSignature
            public static Path getRDotJavaSrcFolder​(BuildTarget buildTarget,
                                                    ProjectFilesystem filesystem)
            ```

        []{#getRDotJavaBinFolder(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem)}

        -   #### getRDotJavaBinFolder

            ``` methodSignature
            public static Path getRDotJavaBinFolder​(BuildTarget buildTarget,
                                                    ProjectFilesystem filesystem)
            ```

        []{#getPathToOutputDir(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem)}

        -   #### getPathToOutputDir

            ``` methodSignature
            public static Path getPathToOutputDir​(BuildTarget buildTarget,
                                                  ProjectFilesystem filesystem)
            ```

        []{#getOutputJarPath(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem)}

        -   #### getOutputJarPath

            ``` methodSignature
            public static Path getOutputJarPath​(BuildTarget buildTarget,
                                                ProjectFilesystem filesystem)
            ```

        []{#getSourcePathToOutput()}

        -   #### getSourcePathToOutput

            ``` methodSignature
            public SourcePath getSourcePathToOutput()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getSourcePathToOutput` in interface `BuildRule`

        []{#getAbiInfo()}

        -   #### getAbiInfo

            ``` methodSignature
            public JavaAbiInfo getAbiInfo()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getAbiInfo` in interface `HasJavaAbi`

        []{#getAbiJar()}

        -   #### getAbiJar

            ``` methodSignature
            public Optional<BuildTarget> getAbiJar()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getAbiJar` in interface `HasJavaAbi`

            [Returns:]{.returnLabel}
            :   the
                [`SourcePath`](../core/sourcepath/SourcePath.html "interface in com.facebook.buck.core.sourcepath")
                representing the ABI Jar for this rule.

        []{#getRDotJavaBinFolder()}

        -   #### getRDotJavaBinFolder

            ``` methodSignature
            public Path getRDotJavaBinFolder()
            ```

        []{#getAndroidResourceDeps()}

        -   #### getAndroidResourceDeps

            ``` methodSignature
            public com.google.common.collect.ImmutableList<HasAndroidResourceDeps> getAndroidResourceDeps()
            ```
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
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
