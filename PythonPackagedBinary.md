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
[Package]{.packageLabelInType} [com.facebook.buck.features.python](package-summary.html)
:::

## Class PythonPackagedBinary {#class-pythonpackagedbinary .title title="Class PythonPackagedBinary"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.core.rules.impl.AbstractBuildRule](../../core/rules/impl/AbstractBuildRule.html "class in com.facebook.buck.core.rules.impl")

    -   -   [com.facebook.buck.features.python.PythonBinary](PythonBinary.html "class in com.facebook.buck.features.python")

        -   -   com.facebook.buck.features.python.PythonPackagedBinary

::: description
-   

    All Implemented Interfaces:
    :   `BuildEngineAction`, `AllowsNonAnnotatedFields`,
        `HasRuntimeDeps`, `BuildRule`, `HasNameAndType`,
        `BinaryBuildRule`, `Comparable<BuildRule>`

    ------------------------------------------------------------------------

        public class PythonPackagedBinary
        extends PythonBinary
        implements HasRuntimeDeps
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `                     | `getBuildDeps()`      |                       |
        | SortedSet<BuildRule>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
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
        | `java.util.stream     | `getRuntime           |                       |
        | .Stream<BuildTarget>` | Deps​(BuildRuleResolve |                       |
        |                       | r buildRuleResolver)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isCacheable()`       | ::: block             |
        |                       |                       | Whether this          |
        |                       |                       | [`Buil                |
        |                       |                       | dRule`](../../core/ru |
        |                       |                       | les/BuildRule.html "i |
        |                       |                       | nterface in com.faceb |
        |                       |                       | ook.buck.core.rules") |
        |                       |                       | can be cached.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.features.python.PythonBinary}

            ### Methods inherited from class com.facebook.buck.features.python.[PythonBinary](PythonBinary.html "class in com.facebook.buck.features.python")

            `getComponents, getMainModule, getPreloadLibraries, getPythonPlatform, getSourcePathToOutput`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.impl.AbstractBuildRule}

            ### Methods inherited from class com.facebook.buck.core.rules.impl.[AbstractBuildRule](../../core/rules/impl/AbstractBuildRule.html "class in com.facebook.buck.core.rules.impl")

            `equals, getBuildTarget, getDependencies, getProjectFilesystem, getSourcePathOutputs, getType, hasBuildSteps, hashCode, injectFields, toString, updateBuildRuleResolver`

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

            `compareTo, getBuildTarget, getFullyQualifiedName, getProjectFilesystem, getSourcePathToOutput, hasBuildSteps, outputFileCanBeCopied, shouldRespectInputSizeLimitForRemoteExecution, toString, updateBuildRuleResolver`

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

        []{#getBuildSteps(com.facebook.buck.core.build.context.BuildContext,com.facebook.buck.core.build.buildable.context.BuildableContext)}

        -   #### getBuildSteps

            ``` methodSignature
            public com.google.common.collect.ImmutableList<Step> getBuildSteps​(BuildContext context,
                                                                               BuildableContext buildableContext)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getBuildSteps` in interface `BuildRule`

        []{#getRuntimeDeps(com.facebook.buck.core.rules.BuildRuleResolver)}

        -   #### getRuntimeDeps

            ``` methodSignature
            public java.util.stream.Stream<BuildTarget> getRuntimeDeps​(BuildRuleResolver buildRuleResolver)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getRuntimeDeps` in interface `HasRuntimeDeps`

            [Overrides:]{.overrideSpecifyLabel}
            :   `getRuntimeDeps` in class `PythonBinary`

        []{#isCacheable()}

        -   #### isCacheable

            ``` methodSignature
            public boolean isCacheable()
            ```

            ::: block
            [Description copied from
            interface: `BuildRule`]{.descfrmTypeLabel}
            :::

            ::: block
            Whether this
            [`BuildRule`](../../core/rules/BuildRule.html "interface in com.facebook.buck.core.rules")
            can be cached.
            Uncached build rules are never written out to cache, never
            read from cache, and does not count in cache statistics.
            This rule is useful for artifacts which cannot be easily
            normalized.

            Uncached rules are not always rebuilt, however, as long as
            the existing on-disk representation is up to date. This
            means that these rules can take advantage of
            [`SupportsInputBasedRuleKey`](../../core/rules/attr/SupportsInputBasedRuleKey.html "interface in com.facebook.buck.core.rules.attr")
            to prevent rebuilding.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `isCacheable` in interface `BuildEngineAction`

            [Specified by:]{.overrideSpecifyLabel}
            :   `isCacheable` in interface `BuildRule`

            [Overrides:]{.overrideSpecifyLabel}
            :   `isCacheable` in class `AbstractBuildRule`

        []{#getBuildDeps()}

        -   #### getBuildDeps

            ``` methodSignature
            public SortedSet<BuildRule> getBuildDeps()
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