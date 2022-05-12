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

## Class Javadoc {#class-javadoc .title title="Class Javadoc"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.core.rules.impl.AbstractBuildRule](../../core/rules/impl/AbstractBuildRule.html "class in com.facebook.buck.core.rules.impl")

    -   -   [com.facebook.buck.core.rules.impl.AbstractBuildRuleWithDeclaredAndExtraDeps](../../core/rules/impl/AbstractBuildRuleWithDeclaredAndExtraDeps.html "class in com.facebook.buck.core.rules.impl")

        -   -   com.facebook.buck.jvm.java.Javadoc

::: description
-   

    All Implemented Interfaces:
    :   `BuildEngineAction`, `AllowsNonAnnotatedFields`,
        `HasDeclaredAndExtraDeps`, `BuildRule`, `HasNameAndType`,
        `HasMavenCoordinates`, `MavenPublishable`,
        `Comparable<BuildRule>`

    ------------------------------------------------------------------------

        public class Javadoc
        extends AbstractBuildRuleWithDeclaredAndExtraDeps
        implements MavenPublishable
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type   Field       Description
          ------------------- ----------- -------------
          `static Flavor`     `DOC_JAR`    

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Modifier       Constructor                                                                                                                                                                                                                                                                                                                    Description
          -------------- ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ -------------
          `protected `   `Javadoc​(BuildTarget buildTarget,        ProjectFilesystem projectFilesystem,        BuildRuleParams buildRuleParams,        Optional<String> mavenCoords,        Optional<SourcePath> mavenPomTemplate,        Iterable<HasMavenCoordinates> mavenDeps,        com.google.common.collect.ImmutableSet<SourcePath> sources)`    

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
        | `Optional<String>`    | `getMavenCoords()`    | ::: block             |
        |                       |                       | Used to identify this |
        |                       |                       | library within a      |
        |                       |                       | maven repository      |
        |                       |                       | :::                   |
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
        | `SourcePath`          | `get                  |                       |
        |                       | SourcePathToOutput()` |                       |
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
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.HasNameAndType}

            ### Methods inherited from interface com.facebook.buck.core.rules.[HasNameAndType](../../core/rules/HasNameAndType.html "interface in com.facebook.buck.core.rules")

            `getType`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#field.detail}

        ### Field Detail

        []{#DOC_JAR}

        -   #### DOC_JAR

                public static final Flavor DOC_JAR
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.rules.BuildRuleParams,java.util.Optional,java.util.Optional,java.lang.Iterable,com.google.common.collect.ImmutableSet)}

        -   #### Javadoc

                protected Javadoc​(BuildTarget buildTarget,
                                  ProjectFilesystem projectFilesystem,
                                  BuildRuleParams buildRuleParams,
                                  Optional<String> mavenCoords,
                                  Optional<SourcePath> mavenPomTemplate,
                                  Iterable<HasMavenCoordinates> mavenDeps,
                                  com.google.common.collect.ImmutableSet<SourcePath> sources)
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
