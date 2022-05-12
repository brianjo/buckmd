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
[Package]{.packageLabelInType} [com.facebook.buck.jvm.java](package-summary.html)
:::

## Class JarFattener {#class-jarfattener .title title="Class JarFattener"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.core.rules.impl.AbstractBuildRule](../../core/rules/impl/AbstractBuildRule.html "class in com.facebook.buck.core.rules.impl")

    -   -   [com.facebook.buck.core.rules.impl.AbstractBuildRuleWithDeclaredAndExtraDeps](../../core/rules/impl/AbstractBuildRuleWithDeclaredAndExtraDeps.html "class in com.facebook.buck.core.rules.impl")

        -   -   com.facebook.buck.jvm.java.JarFattener

::: description
-   

    All Implemented Interfaces:
    :   `BuildEngineAction`, `AllowsNonAnnotatedFields`,
        `HasDeclaredAndExtraDeps`, `BuildRule`, `HasNameAndType`,
        `BinaryBuildRule`, `HasClasspathEntries`,
        `Comparable<BuildRule>`

    ------------------------------------------------------------------------

        public class JarFattener
        extends AbstractBuildRuleWithDeclaredAndExtraDeps
        implements BinaryBuildRule, HasClasspathEntries

    ::: block
    Build a fat JAR that packages an inner JAR along with any required
    native libraries.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type                                          Field                         Description
          ---------------------------------------------------------- ----------------------------- -------------
          `static String`                                            `FAT_JAR_MAIN_SRC_RESOURCE`    
          `static com.google.common.collect.ImmutableList<String>`   `FAT_JAR_SRC_RESOURCES`        

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                                                                                                                              Description
          ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `JarFattener​(BuildTarget buildTarget,            ProjectFilesystem projectFilesystem,            BuildRuleParams params,            Javac javac,            JavacOptions javacOptions,            SourcePath innerJar,            JavaBinary innerJarRule,            com.google.common.collect.ImmutableMap<String,​SourcePath> nativeLibraries,            Tool javaRuntimeLauncher)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `com.                 | `                     |                       |
        | google.common.collect | getBuildSteps​(BuildCo |                       |
        | .ImmutableList<Step>` | ntext context,        |                       |
        |                       |        BuildableConte |                       |
        |                       | xt buildableContext)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Tool`                | `getE                 | ::: block             |
        |                       | xecutableCommand​(Outp | Command to execute    |
        |                       | utLabel outputLabel)` | the output of this    |
        |                       |                       | rule.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.googl            | `getI                 | ::: block             |
        | e.common.collect.Immu | mmediateClasspaths()` | Returns the           |
        | tableSet<SourcePath>` |                       | classpaths for only   |
        |                       |                       | this rule, not its    |
        |                       |                       | deps.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.commo     | `                     |                       |
        | n.collect.ImmutableMa | getNativeLibraries()` |                       |
        | p<String,​SourcePath>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.googl            | `g                    |                       |
        | e.common.collect.Immu | etOutputClasspaths()` |                       |
        | tableSet<SourcePath>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `SourcePath`          | `get                  |                       |
        |                       | SourcePathToOutput()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google           | `getTrans             |                       |
        | .common.collect.Immut | itiveClasspathDeps()` |                       |
        | ableSet<JavaLibrary>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.googl            | `getTr                |                       |
        | e.common.collect.Immu | ansitiveClasspaths()` |                       |
        | tableSet<SourcePath>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `updateBuildRul       | ::: block             |
        |                       | eResolver​(BuildRuleRe | Updates the           |
        |                       | solver ruleResolver)` | BuildRuleResolver and |
        |                       |                       | associated objects    |
        |                       |                       | for this build rule.  |
        |                       |                       | :::                   |
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

            `compareTo, getBuildDeps, getBuildTarget, getFullyQualifiedName, getProjectFilesystem, hasBuildSteps, isCacheable, outputFileCanBeCopied, shouldRespectInputSizeLimitForRemoteExecution, toString`

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
    -   []{#field.detail}

        ### Field Detail

        []{#FAT_JAR_SRC_RESOURCES}

        -   #### FAT_JAR_SRC_RESOURCES

                public static final com.google.common.collect.ImmutableList<String> FAT_JAR_SRC_RESOURCES

        []{#FAT_JAR_MAIN_SRC_RESOURCE}

        -   #### FAT_JAR_MAIN_SRC_RESOURCE

                public static final String FAT_JAR_MAIN_SRC_RESOURCE

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.jvm.java.JarFattener.FAT_JAR_MAIN_SRC_RESOURCE)
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.rules.BuildRuleParams,com.facebook.buck.jvm.java.Javac,com.facebook.buck.jvm.java.JavacOptions,com.facebook.buck.core.sourcepath.SourcePath,com.facebook.buck.jvm.java.JavaBinary,com.google.common.collect.ImmutableMap,com.facebook.buck.core.toolchain.tool.Tool)}

        -   #### JarFattener

                public JarFattener​(BuildTarget buildTarget,
                                   ProjectFilesystem projectFilesystem,
                                   BuildRuleParams params,
                                   Javac javac,
                                   JavacOptions javacOptions,
                                   SourcePath innerJar,
                                   JavaBinary innerJarRule,
                                   com.google.common.collect.ImmutableMap<String,​SourcePath> nativeLibraries,
                                   Tool javaRuntimeLauncher)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getBuildSteps(com.facebook.buck.core.build.context.BuildContext,com.facebook.buck.core.build.buildable.context.BuildableContext)}

        -   #### getBuildSteps

            ``` methodSignature
            public com.google.common.collect.ImmutableList<Step> getBuildSteps​(BuildContext context,
                                                                               BuildableContext buildableContext)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getBuildSteps` in interface `BuildRule`

        []{#getSourcePathToOutput()}

        -   #### getSourcePathToOutput

            ``` methodSignature
            public SourcePath getSourcePathToOutput()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getSourcePathToOutput` in interface `BuildRule`

        []{#getExecutableCommand(com.facebook.buck.core.model.OutputLabel)}

        -   #### getExecutableCommand

            ``` methodSignature
            public Tool getExecutableCommand​(OutputLabel outputLabel)
            ```

            ::: block
            [Description copied from
            interface: `BinaryBuildRule`]{.descfrmTypeLabel}
            :::

            ::: block
            Command to execute the output of this rule.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getExecutableCommand` in interface `BinaryBuildRule`

            [Parameters:]{.paramLabel}
            :   `outputLabel` - associated with the executable

        []{#getNativeLibraries()}

        -   #### getNativeLibraries

            ``` methodSignature
            public com.google.common.collect.ImmutableMap<String,​SourcePath> getNativeLibraries()
            ```

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
