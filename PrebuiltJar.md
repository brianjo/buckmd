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

## Class PrebuiltJar {#class-prebuiltjar .title title="Class PrebuiltJar"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.core.rules.impl.AbstractBuildRule](../../core/rules/impl/AbstractBuildRule.html "class in com.facebook.buck.core.rules.impl")

    -   -   [com.facebook.buck.core.rules.impl.AbstractBuildRuleWithDeclaredAndExtraDeps](../../core/rules/impl/AbstractBuildRuleWithDeclaredAndExtraDeps.html "class in com.facebook.buck.core.rules.impl")

        -   -   com.facebook.buck.jvm.java.PrebuiltJar

::: description
-   

    All Implemented Interfaces:
    :   `AndroidPackageable`, `BuildEngineAction`,
        `AllowsNonAnnotatedFields`, `ExportDependencies`,
        `HasDeclaredAndExtraDeps`, `HasRuntimeDeps`,
        `InitializableFromDisk<JavaLibrary.Data>`,
        `SupportsInputBasedRuleKey`, `BuildRule`, `HasNameAndType`,
        `HasClasspathDeps`, `HasClasspathEntries`, `HasDesugarSupport`,
        `HasJavaAbi`, `HasJavaClassHashes`, `HasMavenCoordinates`,
        `HasSources`, `JavaLibrary`, `MaybeRequiredForSourceOnlyAbi`,
        `Comparable<BuildRule>`

    ------------------------------------------------------------------------

        public class PrebuiltJar
        extends AbstractBuildRuleWithDeclaredAndExtraDeps
        implements AndroidPackageable, ExportDependencies, InitializableFromDisk<JavaLibrary.Data>, JavaLibrary, MaybeRequiredForSourceOnlyAbi, SupportsInputBasedRuleKey
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        -   []{#nested.classes.inherited.from.class.com.facebook.buck.jvm.core.JavaLibrary}

            ### Nested classes/interfaces inherited from interface com.facebook.buck.jvm.core.[JavaLibrary](../core/JavaLibrary.html "interface in com.facebook.buck.jvm.core")

            `JavaLibrary.Data`
    :::

    ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        -   []{#fields.inherited.from.class.com.facebook.buck.jvm.core.JavaLibrary}

            ### Fields inherited from interface com.facebook.buck.jvm.core.[JavaLibrary](../core/JavaLibrary.html "interface in com.facebook.buck.jvm.core")

            `GWT_MODULE_FLAVOR, MAVEN_JAR, SRC_JAR`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               Description
          ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `PrebuiltJar​(BuildTarget buildTarget,            ProjectFilesystem projectFilesystem,            BuildRuleParams params,            SourcePathResolverAdapter resolver,            SourcePath binaryJar,            Optional<SourcePath> sourceJar,            Optional<SourcePath> gwtJar,            Optional<String> javadocUrl,            Optional<String> mavenCoords,            boolean provided,            boolean requiredForSourceOnlyAbi,            boolean generateAbi,            boolean neverMarkAsUnusedDependency)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `void`                | `addToCollect         | ::: block             |
        |                       | or​(AndroidPackageable | Add concrete          |
        |                       | Collector collector)` | resources to the      |
        |                       |                       | given collector.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavaAbiInfo`         | `getAbiInfo()`        |                       |
        +-----------------------+-----------------------+-----------------------+
        | `O                    | `getAbiJar()`         |                       |
        | ptional<BuildTarget>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `BuildOutputInitializ | `getBuil              |                       |
        | er<JavaLibrary.Data>` | dOutputInitializer()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.                 | `                     |                       |
        | google.common.collect | getBuildSteps​(BuildCo |                       |
        | .ImmutableList<Step>` | ntext context,        |                       |
        |                       |        BuildableConte |                       |
        |                       | xt buildableContext)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Jav                  | `getC                 |                       |
        | aClassHashesProvider` | lassHashesProvider()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `c                    | `get                  |                       |
        | om.google.common.coll | ClassNamesToHashes()` |                       |
        | ect.ImmutableSortedMa |                       |                       |
        | p<String,​com.google.c |                       |                       |
        | ommon.hash.HashCode>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Set<BuildRule>`      | `getDepsForTransiti   |                       |
        |                       | veClasspathEntries()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getExportedDeps()`   |                       |
        | SortedSet<BuildRule>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getEx                |                       |
        | SortedSet<BuildRule>` | portedProvidedDeps()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getGeneratedAn       |                       |
        | Optional<SourcePath>` | notationSourcePath()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.googl            | `getI                 | ::: block             |
        | e.common.collect.Immu | mmediateClasspaths()` | Returns the           |
        | tableSet<SourcePath>` |                       | classpaths for only   |
        |                       |                       | this rule, not its    |
        |                       |                       | deps.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `getJavadocUrl()`     |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.comm      | `getJavaSrcs()`       |                       |
        | on.collect.ImmutableS |                       |                       |
        | ortedSet<SourcePath>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `getMavenCoords()`    | ::: block             |
        |                       |                       | Used to identify this |
        |                       |                       | library within a      |
        |                       |                       | maven repository      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.googl            | `g                    |                       |
        | e.common.collect.Immu | etOutputClasspaths()` |                       |
        | tableSet<SourcePath>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `getRequir            |                       |
        |                       | edForSourceOnlyAbi()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Iterable             | `getRequiredPac       | ::: block             |
        | <AndroidPackageable>` | kageables​(BuildRuleRe | Get the set of        |
        |                       | solver ruleResolver)` | packagables that need |
        |                       |                       | to be included in any |
        |                       |                       | package that includes |
        |                       |                       | this object.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.comm      | `getResources()`      |                       |
        | on.collect.ImmutableS |                       |                       |
        | ortedSet<SourcePath>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `getResourcesRoot()`  |                       |
        +-----------------------+-----------------------+-----------------------+
        | `java.util.stream     | `getRuntime           |                       |
        | .Stream<BuildTarget>` | Deps​(BuildRuleResolve |                       |
        |                       | r buildRuleResolver)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getSourceJar()`      |                       |
        | Optional<SourcePath>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `SourcePath`          | `get                  |                       |
        |                       | SourcePathToOutput()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.comm      | `getSources()`        |                       |
        | on.collect.ImmutableS |                       |                       |
        | ortedSet<SourcePath>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google           | `getTrans             |                       |
        | .common.collect.Immut | itiveClasspathDeps()` |                       |
        | ableSet<JavaLibrary>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.googl            | `getTr                |                       |
        | e.common.collect.Immu | ansitiveClasspaths()` |                       |
        | tableSet<SourcePath>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `hasAn                |                       |
        |                       | notationProcessing()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `JavaLibrary.Data`    | `initializeFromDis    |                       |
        |                       | k​(SourcePathResolverA |                       |
        |                       | dapter pathResolver)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `invalidateIniti      |                       |
        |                       | alizeFromDiskState()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isDesugarEnabled()`  | ::: block             |
        |                       |                       | Desugar support for   |
        |                       |                       | java 8 features       |
        |                       |                       | withing single class  |
        |                       |                       | file.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isInterfaceMet       | ::: block             |
        |                       | hodsDesugarEnabled()` | Desugar support for   |
        |                       |                       | interface default and |
        |                       |                       | static methods.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `neverMark            |                       |
        |                       | AsUnusedDependency()` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.impl.AbstractBuildRuleWithDeclaredAndExtraDeps}

            ### Methods inherited from class com.facebook.buck.core.rules.impl.[AbstractBuildRuleWithDeclaredAndExtraDeps](../../core/rules/impl/AbstractBuildRuleWithDeclaredAndExtraDeps.html "class in com.facebook.buck.core.rules.impl")

            `deprecatedGetExtraDeps, getBuildDeps, getDeclaredDeps, getTargetGraphOnlyDeps`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.impl.AbstractBuildRule}

            ### Methods inherited from class com.facebook.buck.core.rules.impl.[AbstractBuildRule](../../core/rules/impl/AbstractBuildRule.html "class in com.facebook.buck.core.rules.impl")

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

            ### Methods inherited from interface com.facebook.buck.core.build.action.[BuildEngineAction](../../core/build/action/BuildEngineAction.html "interface in com.facebook.buck.core.build.action")

            `getDependencies, getSourcePathOutputs`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.BuildRule}

            ### Methods inherited from interface com.facebook.buck.core.rules.[BuildRule](../../core/rules/BuildRule.html "interface in com.facebook.buck.core.rules")

            `compareTo, getBuildDeps, getBuildTarget, getFullyQualifiedName, getProjectFilesystem, hasBuildSteps, isCacheable, outputFileCanBeCopied, shouldRespectInputSizeLimitForRemoteExecution, toString, updateBuildRuleResolver`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.jvm.core.HasJavaAbi}

            ### Methods inherited from interface com.facebook.buck.jvm.core.[HasJavaAbi](../core/HasJavaAbi.html "interface in com.facebook.buck.jvm.core")

            `getSourceOnlyAbiJar`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.HasNameAndType}

            ### Methods inherited from interface com.facebook.buck.core.rules.[HasNameAndType](../../core/rules/HasNameAndType.html "interface in com.facebook.buck.core.rules")

            `getType`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.attr.SupportsInputBasedRuleKey}

            ### Methods inherited from interface com.facebook.buck.core.rules.attr.[SupportsInputBasedRuleKey](../../core/rules/attr/SupportsInputBasedRuleKey.html "interface in com.facebook.buck.core.rules.attr")

            `inputBasedRuleKeyIsEnabled`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.rules.BuildRuleParams,com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter,com.facebook.buck.core.sourcepath.SourcePath,java.util.Optional,java.util.Optional,java.util.Optional,java.util.Optional,boolean,boolean,boolean,boolean)}

        -   #### PrebuiltJar

                public PrebuiltJar​(BuildTarget buildTarget,
                                   ProjectFilesystem projectFilesystem,
                                   BuildRuleParams params,
                                   SourcePathResolverAdapter resolver,
                                   SourcePath binaryJar,
                                   Optional<SourcePath> sourceJar,
                                   Optional<SourcePath> gwtJar,
                                   Optional<String> javadocUrl,
                                   Optional<String> mavenCoords,
                                   boolean provided,
                                   boolean requiredForSourceOnlyAbi,
                                   boolean generateAbi,
                                   boolean neverMarkAsUnusedDependency)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getRequiredForSourceOnlyAbi()}

        -   #### getRequiredForSourceOnlyAbi

            ``` methodSignature
            public boolean getRequiredForSourceOnlyAbi()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getRequiredForSourceOnlyAbi` in
                interface `MaybeRequiredForSourceOnlyAbi`

        []{#getSourceJar()}

        -   #### getSourceJar

            ``` methodSignature
            public Optional<SourcePath> getSourceJar()
            ```

        []{#getJavadocUrl()}

        -   #### getJavadocUrl

            ``` methodSignature
            public Optional<String> getJavadocUrl()
            ```

        []{#isDesugarEnabled()}

        -   #### isDesugarEnabled

            ``` methodSignature
            public boolean isDesugarEnabled()
            ```

            ::: block
            [Description copied from
            interface: `HasDesugarSupport`]{.descfrmTypeLabel}
            :::

            ::: block
            Desugar support for java 8 features withing single class
            file.
            Such as Lambda expressions, Method references, Repeating
            annotations
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `isDesugarEnabled` in interface `HasDesugarSupport`

        []{#isInterfaceMethodsDesugarEnabled()}

        -   #### isInterfaceMethodsDesugarEnabled

            ``` methodSignature
            public boolean isInterfaceMethodsDesugarEnabled()
            ```

            ::: block
            [Description copied from
            interface: `HasDesugarSupport`]{.descfrmTypeLabel}
            :::

            ::: block
            Desugar support for interface default and static methods.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `isInterfaceMethodsDesugarEnabled` in
                interface `HasDesugarSupport`

        []{#getClassNamesToHashes()}

        -   #### getClassNamesToHashes

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedMap<String,​com.google.common.hash.HashCode> getClassNamesToHashes()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getClassNamesToHashes` in
                interface `HasJavaClassHashes`

            [Returns:]{.returnLabel}
            :   a (possibly empty) map of names of `.class` files in the
                output of this rule to SHA-1 hashes of their contents.

        []{#invalidateInitializeFromDiskState()}

        -   #### invalidateInitializeFromDiskState

            ``` methodSignature
            public void invalidateInitializeFromDiskState()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `invalidateInitializeFromDiskState` in
                interface `InitializableFromDisk<JavaLibrary.Data>`

        []{#initializeFromDisk(com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter)}

        -   #### initializeFromDisk

            ``` methodSignature
            public JavaLibrary.Data initializeFromDisk​(SourcePathResolverAdapter pathResolver)
                                                throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `initializeFromDisk` in
                interface `InitializableFromDisk<JavaLibrary.Data>`

            [Returns:]{.returnLabel}
            :   an object that has the in-memory data structures that
                need to be populated as a result of executing this
                object\'s steps.

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#getBuildOutputInitializer()}

        -   #### getBuildOutputInitializer

            ``` methodSignature
            public BuildOutputInitializer<JavaLibrary.Data> getBuildOutputInitializer()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getBuildOutputInitializer` in
                interface `InitializableFromDisk<JavaLibrary.Data>`

        []{#getDepsForTransitiveClasspathEntries()}

        -   #### getDepsForTransitiveClasspathEntries

            ``` methodSignature
            public Set<BuildRule> getDepsForTransitiveClasspathEntries()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getDepsForTransitiveClasspathEntries` in
                interface `HasClasspathDeps`

            [Returns:]{.returnLabel}
            :   all direct dependencies which may contribute to the
                classpath of this rule

        []{#getTransitiveClasspaths()}

        -   #### getTransitiveClasspaths

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<SourcePath> getTransitiveClasspaths()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getTransitiveClasspaths` in
                interface `HasClasspathEntries`

            [Returns:]{.returnLabel}
            :   Classpath entries for this rule and its dependencies.
                e.g. If the rule represents a java library, then these
                entries will be passed to `javac`\'s `-classpath` flag
                in order to build a jar associated with this rule.

        []{#getTransitiveClasspathDeps()}

        -   #### getTransitiveClasspathDeps

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<JavaLibrary> getTransitiveClasspathDeps()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getTransitiveClasspathDeps` in
                interface `HasClasspathEntries`

            [Returns:]{.returnLabel}
            :   A set of rules contributing classpath entries for this
                rule and its dependencies.

        []{#getImmediateClasspaths()}

        -   #### getImmediateClasspaths

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<SourcePath> getImmediateClasspaths()
            ```

            ::: block
            [Description copied from
            interface: `HasClasspathEntries`]{.descfrmTypeLabel}
            :::

            ::: block
            Returns the classpaths for only this rule, not its deps.
            Used to generate the value of
            [`HasClasspathEntries.getTransitiveClasspaths()`](../core/HasClasspathEntries.html#getTransitiveClasspaths()).
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getImmediateClasspaths` in
                interface `HasClasspathEntries`

        []{#getOutputClasspaths()}

        -   #### getOutputClasspaths

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<SourcePath> getOutputClasspaths()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getOutputClasspaths` in interface `HasClasspathEntries`

            [Returns:]{.returnLabel}
            :   Classpath entries that this rule will contribute when it
                is used as a dependency. e.g. If the rule represents a
                java library, then these entries must be passed to
                `javac`\'s `-classpath` flag in order to compile rules
                that depend on this rule. This is a superset of
                `getImmediateClasspaths` which also contains the
                classpath entries of any exported deps.

        []{#getJavaSrcs()}

        -   #### getJavaSrcs

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedSet<SourcePath> getJavaSrcs()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getJavaSrcs` in interface `JavaLibrary`

        []{#getSources()}

        -   #### getSources

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedSet<SourcePath> getSources()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getSources` in interface `HasSources`

        []{#getResources()}

        -   #### getResources

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedSet<SourcePath> getResources()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getResources` in interface `JavaLibrary`

        []{#getResourcesRoot()}

        -   #### getResourcesRoot

            ``` methodSignature
            public Optional<String> getResourcesRoot()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getResourcesRoot` in interface `JavaLibrary`

        []{#getExportedDeps()}

        -   #### getExportedDeps

            ``` methodSignature
            public SortedSet<BuildRule> getExportedDeps()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getExportedDeps` in interface `ExportDependencies`

        []{#getExportedProvidedDeps()}

        -   #### getExportedProvidedDeps

            ``` methodSignature
            public SortedSet<BuildRule> getExportedProvidedDeps()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getExportedProvidedDeps` in
                interface `ExportDependencies`

        []{#getGeneratedAnnotationSourcePath()}

        -   #### getGeneratedAnnotationSourcePath

            ``` methodSignature
            public Optional<SourcePath> getGeneratedAnnotationSourcePath()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getGeneratedAnnotationSourcePath` in
                interface `JavaLibrary`

        []{#hasAnnotationProcessing()}

        -   #### hasAnnotationProcessing

            ``` methodSignature
            public boolean hasAnnotationProcessing()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `hasAnnotationProcessing` in interface `JavaLibrary`

        []{#neverMarkAsUnusedDependency()}

        -   #### neverMarkAsUnusedDependency

            ``` methodSignature
            public boolean neverMarkAsUnusedDependency()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `neverMarkAsUnusedDependency` in interface `JavaLibrary`

        []{#getRuntimeDeps(com.facebook.buck.core.rules.BuildRuleResolver)}

        -   #### getRuntimeDeps

            ``` methodSignature
            public java.util.stream.Stream<BuildTarget> getRuntimeDeps​(BuildRuleResolver buildRuleResolver)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getRuntimeDeps` in interface `HasRuntimeDeps`

        []{#getBuildSteps(com.facebook.buck.core.build.context.BuildContext,com.facebook.buck.core.build.buildable.context.BuildableContext)}

        -   #### getBuildSteps

            ``` methodSignature
            public com.google.common.collect.ImmutableList<Step> getBuildSteps​(BuildContext context,
                                                                               BuildableContext buildableContext)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getBuildSteps` in interface `BuildRule`

        []{#getRequiredPackageables(com.facebook.buck.core.rules.BuildRuleResolver)}

        -   #### getRequiredPackageables

            ``` methodSignature
            public Iterable<AndroidPackageable> getRequiredPackageables​(BuildRuleResolver ruleResolver)
            ```

            ::: block
            [Description copied from
            interface: `AndroidPackageable`]{.descfrmTypeLabel}
            :::

            ::: block
            Get the set of packagables that need to be included in any
            package that includes this object.
            For example, an android_library will need all of its Java
            deps (except provided_deps), its resource deps, and its
            native library deps (even though it doesn\'t need the native
            library as a build-time dependency). An android_resource
            might need an android_library that declares a custom view
            that it references, as well as other android_resource rules
            that it references directly.

            TODO(natthu): Once build rules and buildables are merged,
            replace this method with another interface that lets an
            [`AndroidPackageable`](../../android/packageable/AndroidPackageable.html "interface in com.facebook.buck.android.packageable")
            override the default set which is all deps of the type
            [`AndroidPackageable`](../../android/packageable/AndroidPackageable.html "interface in com.facebook.buck.android.packageable").
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getRequiredPackageables` in
                interface `AndroidPackageable`

            [Returns:]{.returnLabel}
            :   All
                [`AndroidPackageable`](../../android/packageable/AndroidPackageable.html "interface in com.facebook.buck.android.packageable")s
                that must be included along with this one.

        []{#addToCollector(com.facebook.buck.android.packageable.AndroidPackageableCollector)}

        -   #### addToCollector

            ``` methodSignature
            public void addToCollector​(AndroidPackageableCollector collector)
            ```

            ::: block
            [Description copied from
            interface: `AndroidPackageable`]{.descfrmTypeLabel}
            :::

            ::: block
            Add concrete resources to the given collector.
            Implementations should call methods on the collector specify
            what concrete content must be included in an Android package
            that includes this object. For example, an android_library
            will add Java classes, an ndk_library will add native
            libraries, and android_resource will add resource
            directories.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `addToCollector` in interface `AndroidPackageable`

            [Parameters:]{.paramLabel}
            :   `collector` - The
                [`AndroidPackageableCollector`](../../android/packageable/AndroidPackageableCollector.html "class in com.facebook.buck.android.packageable")
                that will receive the content.

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
                [`SourcePath`](../../core/sourcepath/SourcePath.html "interface in com.facebook.buck.core.sourcepath")
                representing the ABI Jar for this rule.

        []{#getMavenCoords()}

        -   #### getMavenCoords

            ``` methodSignature
            public Optional<String> getMavenCoords()
            ```

            ::: block
            [Description copied from
            interface: `HasMavenCoordinates`]{.descfrmTypeLabel}
            :::

            ::: block
            Used to identify this library within a maven repository
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getMavenCoords` in interface `HasMavenCoordinates`

        []{#getClassHashesProvider()}

        -   #### getClassHashesProvider

            ``` methodSignature
            public JavaClassHashesProvider getClassHashesProvider()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getClassHashesProvider` in
                interface `HasJavaClassHashes`
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
