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
[Package]{.packageLabelInType} [com.facebook.buck.features.rust](package-summary.html)
:::

## Class RustLibrary {#class-rustlibrary .title title="Class RustLibrary"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.core.rules.impl.AbstractBuildRule](../../core/rules/impl/AbstractBuildRule.html "class in com.facebook.buck.core.rules.impl")

    -   -   [com.facebook.buck.core.rules.impl.AbstractBuildRuleWithDeclaredAndExtraDeps](../../core/rules/impl/AbstractBuildRuleWithDeclaredAndExtraDeps.html "class in com.facebook.buck.core.rules.impl")

        -   -   [com.facebook.buck.core.rules.impl.NoopBuildRuleWithDeclaredAndExtraDeps](../../core/rules/impl/NoopBuildRuleWithDeclaredAndExtraDeps.html "class in com.facebook.buck.core.rules.impl")

            -   -   com.facebook.buck.features.rust.RustLibrary

::: description
-   

    All Implemented Interfaces:
    :   `BuildEngineAction`, `AllowsNonAnnotatedFields`,
        `HasDeclaredAndExtraDeps`, `BuildRule`, `HasNameAndType`,
        `LegacyNativeLinkableGroup`, `NativeLinkableGroup`,
        `Comparable<BuildRule>`

    ------------------------------------------------------------------------

        public abstract class RustLibrary
        extends NoopBuildRuleWithDeclaredAndExtraDeps
        implements LegacyNativeLinkableGroup
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        -   []{#nested.classes.inherited.from.class.com.facebook.buck.cxx.toolchain.nativelink.NativeLinkableGroup}

            ### Nested classes/interfaces inherited from interface com.facebook.buck.cxx.toolchain.nativelink.[NativeLinkableGroup](../../cxx/toolchain/nativelink/NativeLinkableGroup.html "interface in com.facebook.buck.cxx.toolchain.nativelink")

            `NativeLinkableGroup.Linkage`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                 Description
          --------------------------------------------------------------------------------------------------------------------------- -------------
          `RustLibrary​(BuildTarget buildTarget,            ProjectFilesystem projectFilesystem,            BuildRuleParams params)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `BuildTarget`         | `getBuildTarget()`    | ::: block             |
        |                       |                       | Return                |
        |                       |                       | [`Buil                |
        |                       |                       | dTarget`](../../core/ |
        |                       |                       | model/BuildTarget.htm |
        |                       |                       | l "class in com.faceb |
        |                       |                       | ook.buck.core.model") |
        |                       |                       | for linkable          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Arg`                 | `getLinkerArg​(boolean | ::: block             |
        |                       |  direct,              | Return Arg for        |
        |                       | boolean isCheck,      | dependency.           |
        |                       |         com.facebook. | :::                   |
        |                       | buck.features.rust.Ru |                       |
        |                       | stPlatform rustPlatfo |                       |
        |                       | rm,             Linke |                       |
        |                       | r.LinkableDepType dep |                       |
        |                       | Type,             Opt |                       |
        |                       | ional<String> alias)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `NativeL              | `g                    | ::: block             |
        | inkableGroup.Linkage` | etPreferredLinkage()` | Return the linkage    |
        |                       |                       | style for this        |
        |                       |                       | linkable.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Iterable<BuildRule>` | `getRustLinakbleD     |                       |
        |                       | eps​(com.facebook.buck |                       |
        |                       | .features.rust.RustPl |                       |
        |                       | atform rustPlatform)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.commo     | `getRustSharedLibrar  | ::: block             |
        | n.collect.ImmutableMa | ies​(com.facebook.buck | Return a map of       |
        | p<String,​SourcePath>` | .features.rust.RustPl | shared libraries this |
        |                       | atform rustPlatform)` | linkable produces     |
        |                       |                       | (typically just one)  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isProcMacro()`       | ::: block             |
        |                       |                       | Return true if this   |
        |                       |                       | is a compiler plugin  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.impl.NoopBuildRuleWithDeclaredAndExtraDeps}

            ### Methods inherited from class com.facebook.buck.core.rules.impl.[NoopBuildRuleWithDeclaredAndExtraDeps](../../core/rules/impl/NoopBuildRuleWithDeclaredAndExtraDeps.html "class in com.facebook.buck.core.rules.impl")

            `getBuildSteps, getSourcePathToOutput, hasBuildSteps, isCacheable`

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

            `equals, getBuildTarget, getDependencies, getProjectFilesystem, getSourcePathOutputs, getType, hashCode, injectFields, toString, updateBuildRuleResolver`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, finalize, getClass, notify, notifyAll, wait, wait, wait`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.BuildRule}

            ### Methods inherited from interface com.facebook.buck.core.rules.[BuildRule](../../core/rules/BuildRule.html "interface in com.facebook.buck.core.rules")

            `compareTo, getFullyQualifiedName, outputFileCanBeCopied, shouldRespectInputSizeLimitForRemoteExecution`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.cxx.toolchain.nativelink.LegacyNativeLinkableGroup}

            ### Methods inherited from interface com.facebook.buck.cxx.toolchain.nativelink.[LegacyNativeLinkableGroup](../../cxx/toolchain/nativelink/LegacyNativeLinkableGroup.html "interface in com.facebook.buck.cxx.toolchain.nativelink")

            `forceLinkWholeForHaskellOmnibus, getExportedLinkerFlags, getExportedPostLinkerFlags, getNativeLinkable, getNativeLinkableCompatibilityCache, getNativeLinkableDeps, getNativeLinkableDepsForPlatform, getNativeLinkableExportedDeps, getNativeLinkableExportedDepsForPlatform, getNativeLinkableInput, getNativeLinkableInput, getNativeLinkTarget, getPreferredLinkage, getRuleType, getSharedLibraries, isPrebuiltSOForHaskellOmnibus, shouldBeLinkedInAppleTestAndHost, supportsOmnibusLinking, supportsOmnibusLinkingForHaskell`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.cxx.toolchain.nativelink.NativeLinkableGroup}

            ### Methods inherited from interface com.facebook.buck.cxx.toolchain.nativelink.[NativeLinkableGroup](../../cxx/toolchain/nativelink/NativeLinkableGroup.html "interface in com.facebook.buck.cxx.toolchain.nativelink")

            `getBuildTarget`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.rules.BuildRuleParams)}

        -   #### RustLibrary

                public RustLibrary​(BuildTarget buildTarget,
                                   ProjectFilesystem projectFilesystem,
                                   BuildRuleParams params)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getLinkerArg(boolean,boolean,com.facebook.buck.features.rust.RustPlatform,com.facebook.buck.cxx.toolchain.linker.Linker.LinkableDepType,java.util.Optional)}

        -   #### getLinkerArg

            ``` methodSignature
            public abstract Arg getLinkerArg​(boolean direct,
                                             boolean isCheck,
                                             com.facebook.buck.features.rust.RustPlatform rustPlatform,
                                             Linker.LinkableDepType depType,
                                             Optional<String> alias)
            ```

            ::: block
            Return Arg for dependency.
            :::

            [Parameters:]{.paramLabel}
            :   `direct` - true for direct dependency, false for
                transitive
            :   `isCheck` - true if we\'re generated check builds
            :   `rustPlatform` - Current platform we\'re building for.
            :   `depType` - What kind of linkage we want with the
                dependency.
            :   `alias` -

            [Returns:]{.returnLabel}
            :   Arg for linking dependency.

        []{#getBuildTarget()}

        -   #### getBuildTarget

            ``` methodSignature
            public abstract BuildTarget getBuildTarget()
            ```

            ::: block
            Return
            [`BuildTarget`](../../core/model/BuildTarget.html "class in com.facebook.buck.core.model")
            for linkable
            :::

            [Returns:]{.returnLabel}
            :   BuildTarget for linkable.

        []{#getRustSharedLibraries(com.facebook.buck.features.rust.RustPlatform)}

        -   #### getRustSharedLibraries

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableMap<String,​SourcePath> getRustSharedLibraries​(com.facebook.buck.features.rust.RustPlatform rustPlatform)
            ```

            ::: block
            Return a map of shared libraries this linkable produces
            (typically just one)
            :::

            [Parameters:]{.paramLabel}
            :   `rustPlatform` - the platform we\'re generating the
                shared library for

            [Returns:]{.returnLabel}
            :   Map of soname -\> source path

        []{#getRustLinakbleDeps(com.facebook.buck.features.rust.RustPlatform)}

        -   #### getRustLinakbleDeps

            ``` methodSignature
            public abstract Iterable<BuildRule> getRustLinakbleDeps​(com.facebook.buck.features.rust.RustPlatform rustPlatform)
            ```

            [Returns:]{.returnLabel}
            :   the dependencies of this `RustLinkable`.

        []{#getPreferredLinkage()}

        -   #### getPreferredLinkage

            ``` methodSignature
            public abstract NativeLinkableGroup.Linkage getPreferredLinkage()
            ```

            ::: block
            Return the linkage style for this linkable.
            :::

            [Returns:]{.returnLabel}
            :   Linkage mode.

        []{#isProcMacro()}

        -   #### isProcMacro

            ``` methodSignature
            public abstract boolean isProcMacro()
            ```

            ::: block
            Return true if this is a compiler plugin
            :::
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
