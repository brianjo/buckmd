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
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   Constr \| 
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

## Interface MavenPublishable {#interface-mavenpublishable .title title="Interface MavenPublishable"}
:::

::: contentContainer
::: description
-   

    All Superinterfaces:
    :   `AllowsNonAnnotatedFields`, `BuildEngineAction`, `BuildRule`,
        `Comparable<BuildRule>`, `HasMavenCoordinates`, `HasNameAndType`

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `Javadoc`, `MavenUberJar`, `MavenUberJar.SourceJar`

    ------------------------------------------------------------------------

        public interface MavenPublishable
        extends HasMavenCoordinates

    ::: block
    A
    [`BuildRule`](../../core/rules/BuildRule.html "interface in com.facebook.buck.core.rules")
    that can have its
    output([`BuildRule.getSourcePathToOutput()`](../../core/rules/BuildRule.html#getSourcePathToOutput()))
    published to a maven repository under the maven coordinates provided
    by
    [`HasMavenCoordinates.getMavenCoords()`](../core/HasMavenCoordinates.html#getMavenCoords())
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
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

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}

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
    -   []{#method.detail}

        ### Method Detail

        []{#getMavenDeps()}

        -   #### getMavenDeps

            ``` methodSignature
            Iterable<HasMavenCoordinates> getMavenDeps()
            ```

            ::: block
            When published, these will be listed in pom.xml as
            dependencies
            :::

        []{#getPackagedDependencies()}

        -   #### getPackagedDependencies

            ``` methodSignature
            Iterable<BuildRule> getPackagedDependencies()
            ```

            ::: block
            When published, these will be included in the artifact.
            This, [`getMavenDeps()`](#getMavenDeps()), and the
            transitive dependencies of those maven deps would form the
            complete set of transitive dependencies for the artifact.
            :::

        []{#getPomTemplate()}

        -   #### getPomTemplate

            ``` methodSignature
            Optional<SourcePath> getPomTemplate()
            ```

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
-   Field \| 
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   Constr \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
