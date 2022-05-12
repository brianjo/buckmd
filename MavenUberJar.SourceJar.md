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
[Package]{.packageLabelInType} [com.facebook.buck.jvm.java](package-summary.html)
:::

## Class MavenUberJar.SourceJar {#class-mavenuberjar.sourcejar .title title="Class MavenUberJar.SourceJar"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.core.rules.impl.AbstractBuildRule](../../core/rules/impl/AbstractBuildRule.html "class in com.facebook.buck.core.rules.impl")

    -   -   [com.facebook.buck.core.rules.impl.AbstractBuildRuleWithDeclaredAndExtraDeps](../../core/rules/impl/AbstractBuildRuleWithDeclaredAndExtraDeps.html "class in com.facebook.buck.core.rules.impl")

        -   -   [com.facebook.buck.jvm.java.JavaSourceJar](JavaSourceJar.html "class in com.facebook.buck.jvm.java")

            -   -   com.facebook.buck.jvm.java.MavenUberJar.SourceJar

::: description
-   

    All Implemented Interfaces:
    :   `BuildEngineAction`, `AllowsNonAnnotatedFields`,
        `HasDeclaredAndExtraDeps`, `BuildRule`, `HasNameAndType`,
        `HasMavenCoordinates`, `HasSources`, `MavenPublishable`,
        `Comparable<BuildRule>`

    ```{=html}
    <!-- -->
    ```

    Enclosing class:
    :   [MavenUberJar](MavenUberJar.html "class in com.facebook.buck.jvm.java")

    ------------------------------------------------------------------------

        public static class MavenUberJar.SourceJar
        extends JavaSourceJar
        implements MavenPublishable
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                                                                                                        Description
          ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ -------------
          `SourceJar​(BuildTarget buildTarget,          ProjectFilesystem projectFilesystem,          BuildRuleParams params,          com.google.common.collect.ImmutableSortedSet<SourcePath> srcs,          Optional<String> mavenCoords,          Optional<SourcePath> mavenPomTemplate,          com.facebook.buck.jvm.java.MavenUberJar.TraversedDeps traversedDeps)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static Ma            | `create​(Buil          |                       |
        | venUberJar.SourceJar` | dTarget buildTarget,  |                       |
        |                       |       ProjectFilesyst |                       |
        |                       | em projectFilesystem, |                       |
        |                       |        BuildRuleParam |                       |
        |                       | s params,       com.g |                       |
        |                       | oogle.common.collect. |                       |
        |                       | ImmutableSortedSet<So |                       |
        |                       | urcePath> topLevelSrc |                       |
        |                       | s,       Optional<Str |                       |
        |                       | ing> mavenCoords,     |                       |
        |                       |    Optional<SourcePat |                       |
        |                       | h> mavenPomTemplate)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Iterable<            | `getMavenDeps()`      | ::: block             |
        | HasMavenCoordinates>` |                       | When published, these |
        |                       |                       | will be listed in     |
        |                       |                       | pom.xml as            |
        |                       |                       | dependencies          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Iterable<BuildRule>` | `getPa                | ::: block             |
        |                       | ckagedDependencies()` | When published, these |
        |                       |                       | will be included in   |
        |                       |                       | the artifact.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getPomTemplate()`    |                       |
        | Optional<SourcePath>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.jvm.java.JavaSourceJar}

            ### Methods inherited from class com.facebook.buck.jvm.java.[JavaSourceJar](JavaSourceJar.html "class in com.facebook.buck.jvm.java")

            `getBuildSteps, getMavenCoords, getSourcePathToOutput, getSources`

        ```{=html}
        <!-- -->
        ```
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

            `compareTo, getBuildDeps, getBuildSteps, getBuildTarget, getFullyQualifiedName, getProjectFilesystem, getSourcePathToOutput, hasBuildSteps, isCacheable, outputFileCanBeCopied, shouldRespectInputSizeLimitForRemoteExecution, toString, updateBuildRuleResolver`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.jvm.core.HasMavenCoordinates}

            ### Methods inherited from interface com.facebook.buck.jvm.core.[HasMavenCoordinates](../core/HasMavenCoordinates.html "interface in com.facebook.buck.jvm.core")

            `getMavenCoords`

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

        []{#<init>(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.rules.BuildRuleParams,com.google.common.collect.ImmutableSortedSet,java.util.Optional,java.util.Optional,com.facebook.buck.jvm.java.MavenUberJar.TraversedDeps)}

        -   #### SourceJar

                public SourceJar​(BuildTarget buildTarget,
                                 ProjectFilesystem projectFilesystem,
                                 BuildRuleParams params,
                                 com.google.common.collect.ImmutableSortedSet<SourcePath> srcs,
                                 Optional<String> mavenCoords,
                                 Optional<SourcePath> mavenPomTemplate,
                                 com.facebook.buck.jvm.java.MavenUberJar.TraversedDeps traversedDeps)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#create(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.rules.BuildRuleParams,com.google.common.collect.ImmutableSortedSet,java.util.Optional,java.util.Optional)}

        -   #### create

            ``` methodSignature
            public static MavenUberJar.SourceJar create​(BuildTarget buildTarget,
                                                        ProjectFilesystem projectFilesystem,
                                                        BuildRuleParams params,
                                                        com.google.common.collect.ImmutableSortedSet<SourcePath> topLevelSrcs,
                                                        Optional<String> mavenCoords,
                                                        Optional<SourcePath> mavenPomTemplate)
            ```

        []{#getPomTemplate()}

        -   #### getPomTemplate

            ``` methodSignature
            public Optional<SourcePath> getPomTemplate()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getPomTemplate` in interface `MavenPublishable`

            [Returns:]{.returnLabel}
            :   A template for the pom.xml to be generated when
                publishing this artifact.

        []{#getMavenDeps()}

        -   #### getMavenDeps

            ``` methodSignature
            public Iterable<HasMavenCoordinates> getMavenDeps()
            ```

            ::: block
            [Description copied from
            interface: `MavenPublishable`]{.descfrmTypeLabel}
            :::

            ::: block
            When published, these will be listed in pom.xml as
            dependencies
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getMavenDeps` in interface `MavenPublishable`

        []{#getPackagedDependencies()}

        -   #### getPackagedDependencies

            ``` methodSignature
            public Iterable<BuildRule> getPackagedDependencies()
            ```

            ::: block
            [Description copied from
            interface: `MavenPublishable`]{.descfrmTypeLabel}
            :::

            ::: block
            When published, these will be included in the artifact.
            This,
            [`MavenPublishable.getMavenDeps()`](MavenPublishable.html#getMavenDeps()),
            and the transitive dependencies of those maven deps would
            form the complete set of transitive dependencies for the
            artifact.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getPackagedDependencies` in
                interface `MavenPublishable`
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
