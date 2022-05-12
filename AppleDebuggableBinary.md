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
-   [Field](#field.summary) \| 
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.apple](package-summary.html)
:::

## Class AppleDebuggableBinary {#class-appledebuggablebinary .title title="Class AppleDebuggableBinary"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.core.rules.impl.AbstractBuildRule](../core/rules/impl/AbstractBuildRule.html "class in com.facebook.buck.core.rules.impl")

    -   -   com.facebook.buck.apple.AppleDebuggableBinary

::: description
-   

    All Implemented Interfaces:
    :   `BuildRuleWithBinary`, `BuildEngineAction`,
        `AllowsNonAnnotatedFields`, `HasDeclaredAndExtraDeps`,
        `HasRuntimeDeps`, `BuildRule`, `HasNameAndType`,
        `Comparable<BuildRule>`

    ------------------------------------------------------------------------

        public class AppleDebuggableBinary
        extends AbstractBuildRule
        implements BuildRuleWithBinary, HasRuntimeDeps, HasDeclaredAndExtraDeps

    ::: block
    This build rule wraps the usual build rule and should be treated as
    top-level binary rule for apple platform. Depending on the debug
    format, it should depend on dsym and stripped cxx binary, or just on
    stripped binary.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type   Field           Description
          ------------------- --------------- -------------
          `static Flavor`     `RULE_FLAVOR`    

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static boolean`      | `canWrapB             | ::: block             |
        |                       | inaryBuildRule​(BuildR | Indicates whether its |
        |                       | ule binaryBuildRule)` | possible to wrap      |
        |                       |                       | given \_binary\_      |
        |                       |                       | rule.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `depr                 |                       |
        | SortedSet<BuildRule>` | ecatedGetExtraDeps()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<AppleDsym>` | `getAppleDsym()`      |                       |
        +-----------------------+-----------------------+-----------------------+
        | `BuildRule`           | `                     |                       |
        |                       | getBinaryBuildRule()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getBuildDeps()`      |                       |
        | SortedSet<BuildRule>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.                 | `                     |                       |
        | google.common.collect | getBuildSteps​(BuildCo |                       |
        | .ImmutableList<Step>` | ntext context,        |                       |
        |                       |        BuildableConte |                       |
        |                       | xt buildableContext)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getDeclaredDeps()`   |                       |
        | SortedSet<BuildRule>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `java.util.stream     | `getRuntime           |                       |
        | .Stream<BuildTarget>` | Deps​(BuildRuleResolve |                       |
        |                       | r buildRuleResolver)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `SourcePath`          | `get                  |                       |
        |                       | SourcePathToOutput()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.com       | `getT                 |                       |
        | mon.collect.Immutable | argetGraphOnlyDeps()` |                       |
        | SortedSet<BuildRule>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static boolean`      | `i                    |                       |
        |                       | sBuildRuleDebuggable​( |                       |
        |                       | BuildRule buildRule)` |                       |
        +-----------------------+-----------------------+-----------------------+

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
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.HasNameAndType}

            ### Methods inherited from interface com.facebook.buck.core.rules.[HasNameAndType](../core/rules/HasNameAndType.html "interface in com.facebook.buck.core.rules")

            `getType`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#field.detail}

        ### Field Detail

        []{#RULE_FLAVOR}

        -   #### RULE_FLAVOR

                public static final Flavor RULE_FLAVOR
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#canWrapBinaryBuildRule(com.facebook.buck.core.rules.BuildRule)}

        -   #### canWrapBinaryBuildRule

            ``` methodSignature
            public static boolean canWrapBinaryBuildRule​(BuildRule binaryBuildRule)
            ```

            ::: block
            Indicates whether its possible to wrap given \_binary\_
            rule.
            :::

        []{#isBuildRuleDebuggable(com.facebook.buck.core.rules.BuildRule)}

        -   #### isBuildRuleDebuggable

            ``` methodSignature
            public static boolean isBuildRuleDebuggable​(BuildRule buildRule)
            ```

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

        []{#getBinaryBuildRule()}

        -   #### getBinaryBuildRule

            ``` methodSignature
            public BuildRule getBinaryBuildRule()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getBinaryBuildRule` in interface `BuildRuleWithBinary`

        []{#getAppleDsym()}

        -   #### getAppleDsym

            ``` methodSignature
            public Optional<AppleDsym> getAppleDsym()
            ```

        []{#getRuntimeDeps(com.facebook.buck.core.rules.BuildRuleResolver)}

        -   #### getRuntimeDeps

            ``` methodSignature
            public java.util.stream.Stream<BuildTarget> getRuntimeDeps​(BuildRuleResolver buildRuleResolver)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getRuntimeDeps` in interface `HasRuntimeDeps`

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

        []{#getDeclaredDeps()}

        -   #### getDeclaredDeps

            ``` methodSignature
            public SortedSet<BuildRule> getDeclaredDeps()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getDeclaredDeps` in interface `HasDeclaredAndExtraDeps`

        []{#deprecatedGetExtraDeps()}

        -   #### deprecatedGetExtraDeps

            ``` methodSignature
            public SortedSet<BuildRule> deprecatedGetExtraDeps()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `deprecatedGetExtraDeps` in
                interface `HasDeclaredAndExtraDeps`

        []{#getTargetGraphOnlyDeps()}

        -   #### getTargetGraphOnlyDeps

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedSet<BuildRule> getTargetGraphOnlyDeps()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getTargetGraphOnlyDeps` in
                interface `HasDeclaredAndExtraDeps`
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
-   [Field](#field.summary) \| 
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
-   Constr \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
