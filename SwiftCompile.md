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
[Package]{.packageLabelInType} [com.facebook.buck.swift](package-summary.html)
:::

## Class SwiftCompile {#class-swiftcompile .title title="Class SwiftCompile"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.core.rules.impl.AbstractBuildRule](../core/rules/impl/AbstractBuildRule.html "class in com.facebook.buck.core.rules.impl")

    -   -   com.facebook.buck.swift.SwiftCompile

::: description
-   

    All Implemented Interfaces:
    :   `BuildEngineAction`, `AllowsNonAnnotatedFields`,
        `SupportsInputBasedRuleKey`, `BuildRule`, `HasNameAndType`,
        `Comparable<BuildRule>`

    ------------------------------------------------------------------------

        public class SwiftCompile
        extends AbstractBuildRule
        implements SupportsInputBasedRuleKey

    ::: block
    A build rule which compiles one or more Swift sources into a Swift
    module.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `com                  | `getAstLinkArgs()`    |                       |
        | .google.common.collec |                       |                       |
        | t.ImmutableList<Arg>` |                       |                       |
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
        | `String`              | `getModuleName()`     |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getObjCGener         |                       |
        |                       | atedHeaderFileName()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `SourcePath`          | `getObjCG             |                       |
        |                       | eneratedHeaderPath()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google           | `getObjectPaths()`    |                       |
        | .common.collect.Immut |                       |                       |
        | ableList<SourcePath>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `SourcePath`          | `getOutputPath()`     |                       |
        +-----------------------+-----------------------+-----------------------+
        | `SourcePath`          | `get                  |                       |
        |                       | SourcePathToOutput()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `SourcePath`          | `getSwi               |                       |
        |                       | ftModuleOutputPath()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isCacheable()`       | ::: block             |
        |                       |                       | Whether this          |
        |                       |                       | [`B                   |
        |                       |                       | uildRule`](../core/ru |
        |                       |                       | les/BuildRule.html "i |
        |                       |                       | nterface in com.faceb |
        |                       |                       | ook.buck.core.rules") |
        |                       |                       | can be cached.        |
        |                       |                       | :::                   |
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

        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.impl.AbstractBuildRule}

            ### Methods inherited from class com.facebook.buck.core.rules.impl.[AbstractBuildRule](../core/rules/impl/AbstractBuildRule.html "class in com.facebook.buck.core.rules.impl")

            `equals, getBuildTarget, getDependencies, getProjectFilesystem, getSourcePathOutputs, getType, hasBuildSteps, hashCode, injectFields, toString`

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

            `compareTo, getBuildTarget, getFullyQualifiedName, getProjectFilesystem, hasBuildSteps, outputFileCanBeCopied, shouldRespectInputSizeLimitForRemoteExecution, toString`

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
    -   []{#method.detail}

        ### Method Detail

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
            [`BuildRule`](../core/rules/BuildRule.html "interface in com.facebook.buck.core.rules")
            can be cached.
            Uncached build rules are never written out to cache, never
            read from cache, and does not count in cache statistics.
            This rule is useful for artifacts which cannot be easily
            normalized.

            Uncached rules are not always rebuilt, however, as long as
            the existing on-disk representation is up to date. This
            means that these rules can take advantage of
            [`SupportsInputBasedRuleKey`](../core/rules/attr/SupportsInputBasedRuleKey.html "interface in com.facebook.buck.core.rules.attr")
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

        []{#getAstLinkArgs()}

        -   #### getAstLinkArgs

            ``` methodSignature
            public com.google.common.collect.ImmutableList<Arg> getAstLinkArgs()
            ```

        []{#getModuleName()}

        -   #### getModuleName

            ``` methodSignature
            public String getModuleName()
            ```

            [Returns:]{.returnLabel}
            :   The name of the Swift module.

        []{#getObjectPaths()}

        -   #### getObjectPaths

            ``` methodSignature
            public com.google.common.collect.ImmutableList<SourcePath> getObjectPaths()
            ```

            [Returns:]{.returnLabel}
            :   List of
                [`SourcePath`](../core/sourcepath/SourcePath.html "interface in com.facebook.buck.core.sourcepath")
                to the output object file(s) (i.e., .o file)

        []{#getObjCGeneratedHeaderFileName()}

        -   #### getObjCGeneratedHeaderFileName

            ``` methodSignature
            public String getObjCGeneratedHeaderFileName()
            ```

            [Returns:]{.returnLabel}
            :   File name of the Objective-C Generated Interface Header.

        []{#getObjCGeneratedHeaderPath()}

        -   #### getObjCGeneratedHeaderPath

            ``` methodSignature
            public SourcePath getObjCGeneratedHeaderPath()
            ```

            [Returns:]{.returnLabel}
            :   [`SourcePath`](../core/sourcepath/SourcePath.html "interface in com.facebook.buck.core.sourcepath")
                of the Objective-C Generated Interface Header.

        []{#getOutputPath()}

        -   #### getOutputPath

            ``` methodSignature
            public SourcePath getOutputPath()
            ```

            [Returns:]{.returnLabel}
            :   [`SourcePath`](../core/sourcepath/SourcePath.html "interface in com.facebook.buck.core.sourcepath")
                to the directory containing outputs from the compilation
                process (object files, Swift module metadata, etc).

        []{#getSwiftModuleOutputPath()}

        -   #### getSwiftModuleOutputPath

            ``` methodSignature
            public SourcePath getSwiftModuleOutputPath()
            ```

            [Returns:]{.returnLabel}
            :   [`SourcePath`](../core/sourcepath/SourcePath.html "interface in com.facebook.buck.core.sourcepath")
                to the .swiftmodule output from the compilation process.
                A swiftmodule file contains the public interface for a
                module, and is basically a binary file format equivalent
                to header files for a C framework or library. A
                swiftmodule file contains serialized ASTs (and possibly
                SIL), it conforms to Swift Binary Serialization Format,
                more details about this binary format can be found here:
                https://github.com/apple/swift/blob/7e6d62dae4bae4eb3737a6f76c0e51534c1bcca3/docs/Serialization.rst.
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
