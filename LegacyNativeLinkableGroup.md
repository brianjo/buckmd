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

-   [Overview](../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../deprecated-list.html)
-   [Index](../../../../../../index-all.html)
-   [Help](../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.cxx.toolchain.nativelink](package-summary.html)
:::

## Interface LegacyNativeLinkableGroup {#interface-legacynativelinkablegroup .title title="Interface LegacyNativeLinkableGroup"}
:::

::: contentContainer
::: description
-   

    All Superinterfaces:
    :   `NativeLinkableGroup`

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `CxxLibraryGroup`, `HaskellLibrary`, `PrebuiltAppleFramework`,
        `PrebuiltCxxLibraryGroupDescription.CustomPrebuiltCxxLibrary`,
        `RustLibrary`

    ------------------------------------------------------------------------

        public interface LegacyNativeLinkableGroup
        extends NativeLinkableGroup

    ::: block
    An implementation of
    [`NativeLinkableGroup`](NativeLinkableGroup.html "interface in com.facebook.buck.cxx.toolchain.nativelink")
    where the corresponding
    [`NativeLinkable`](NativeLinkable.html "interface in com.facebook.buck.cxx.toolchain.nativelink")
    just refer back to this.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        -   []{#nested.classes.inherited.from.class.com.facebook.buck.cxx.toolchain.nativelink.NativeLinkableGroup}

            ### Nested classes/interfaces inherited from interface com.facebook.buck.cxx.toolchain.nativelink.[NativeLinkableGroup](NativeLinkableGroup.html "interface in com.facebook.buck.cxx.toolchain.nativelink")

            `NativeLinkableGroup.Linkage`
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `default boolean`     | `forceLinkWhol        | ::: block             |
        |                       | eForHaskellOmnibus()` | [Deprecate            |
        |                       |                       | d.]{.deprecatedLabel} |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `default Ite          | `getExportedLinkerFl  | ::: block             |
        | rable<? extends Arg>` | ags​(CxxPlatform cxxPl | [Deprecate            |
        |                       | atform,               | d.]{.deprecatedLabel} |
        |                       |          ActionGraphB | :::                   |
        |                       | uilder graphBuilder)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `default Ite          | `getExp               | ::: block             |
        | rable<? extends Arg>` | ortedPostLinkerFlags​( | [Deprecate            |
        |                       | CxxPlatform cxxPlatfo | d.]{.deprecatedLabel} |
        |                       | rm,                   | :::                   |
        |                       |          ActionGraphB |                       |
        |                       | uilder graphBuilder)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `de                   | `getNative            |                       |
        | fault NativeLinkable` | Linkable​(CxxPlatform  |                       |
        |                       | cxxPlatform,          |                       |
        |                       |          ActionGraphB |                       |
        |                       | uilder graphBuilder)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `stati                | `getNativeLinka       |                       |
        | c PlatformLockedNativ | bleCache​(LegacyNative |                       |
        | eLinkableGroup.Cache` | LinkableGroup group)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `PlatformLockedNativ  | `getNativeLinkable    |                       |
        | eLinkableGroup.Cache` | CompatibilityCache()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Iterable<? extends   | `getNativeLin         |                       |
        | NativeLinkableGroup>` | kableDeps​(BuildRuleRe |                       |
        |                       | solver ruleResolver)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `defaul               | `getNativeLinkable    | ::: block             |
        | t Iterable<? extends  | DepsForPlatform​(CxxPl | [Deprecate            |
        | NativeLinkableGroup>` | atform cxxPlatform,   | d.]{.deprecatedLabel} |
        |                       |                       | :::                   |
        |                       |           BuildRuleRe |                       |
        |                       | solver ruleResolver)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Iterable<? extends   | `getNativeLinkableExp |                       |
        | NativeLinkableGroup>` | ortedDeps​(BuildRuleRe |                       |
        |                       | solver ruleResolver)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `defaul               | `getNativeLink        | ::: block             |
        | t Iterable<? extends  | ableExportedDepsForPl | [Deprecate            |
        | NativeLinkableGroup>` | atform​(CxxPlatform cx | d.]{.deprecatedLabel} |
        |                       | xPlatform,            | :::                   |
        |                       |                       |                       |
        |                       |          ActionGraphB |                       |
        |                       | uilder graphBuilder)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `NativeLinkableInput` | `getNativeLi          | ::: block             |
        |                       | nkableInput​(CxxPlatfo | [Deprecate            |
        |                       | rm cxxPlatform,       | d.]{.deprecatedLabel} |
        |                       |                  Link | :::                   |
        |                       | er.LinkableDepType ty |                       |
        |                       | pe,                   |                       |
        |                       |      boolean forceLin |                       |
        |                       | kWhole,               |                       |
        |                       |          ActionGraphB |                       |
        |                       | uilder graphBuilder,  |                       |
        |                       |                       |                       |
        |                       |  TargetConfiguration  |                       |
        |                       | targetConfiguration)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `default              | `getNati              | ::: block             |
        |  NativeLinkableInput` | veLinkableInput​(CxxPl | [Deprecate            |
        |                       | atform cxxPlatform,   | d.]{.deprecatedLabel} |
        |                       |                       | :::                   |
        |                       | Linker.LinkableDepTyp |                       |
        |                       | e type,               |                       |
        |                       |          ActionGraphB |                       |
        |                       | uilder graphBuilder,  |                       |
        |                       |                       |                       |
        |                       |  TargetConfiguration  |                       |
        |                       | targetConfiguration)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `default Optional<Na  | `getNativeLink        | ::: block             |
        | tiveLinkTargetGroup>` | Target​(CxxPlatform cx | [Deprecate            |
        |                       | xPlatform,            | d.]{.deprecatedLabel} |
        |                       |          ActionGraphB | :::                   |
        |                       | uilder graphBuilder)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `NativeL              | `get                  | ::: block             |
        | inkableGroup.Linkage` | PreferredLinkage​(CxxP | [Deprecate            |
        |                       | latform cxxPlatform)` | d.]{.deprecatedLabel} |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `default String`      | `getRuleType()`       | ::: block             |
        |                       |                       | [Deprecate            |
        |                       |                       | d.]{.deprecatedLabel} |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.commo     | `getSharedLi          | ::: block             |
        | n.collect.ImmutableMa | braries​(CxxPlatform c | [Deprecate            |
        | p<String,​SourcePath>` | xxPlatform,           | d.]{.deprecatedLabel} |
        |                       |          ActionGraphB | :::                   |
        |                       | uilder graphBuilder)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `default boolean`     | `isPrebuiltSO         | ::: block             |
        |                       | ForHaskellOmnibus​(Cxx | [Deprecate            |
        |                       | Platform cxxPlatform, | d.]{.deprecatedLabel} |
        |                       |                       | :::                   |
        |                       |          ActionGraphB |                       |
        |                       | uilder graphBuilder)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `default boolean`     | `shouldBeLinked       | ::: block             |
        |                       | InAppleTestAndHost()` | [Deprecate            |
        |                       |                       | d.]{.deprecatedLabel} |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `default boolean`     | `suppor               | ::: block             |
        |                       | tsOmnibusLinking​(CxxP | [Deprecate            |
        |                       | latform cxxPlatform)` | d.]{.deprecatedLabel} |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `default boolean`     | `supportsOmnibusL     | ::: block             |
        |                       | inkingForHaskell​(CxxP | [Deprecate            |
        |                       | latform cxxPlatform)` | d.]{.deprecatedLabel} |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
        .tableTab}[[Default
        Methods](javascript:show(16);)[ ]{.tabEnd}]{#t5
        .tableTab}[[Deprecated
        Methods](javascript:show(32);)[ ]{.tabEnd}]{#t6 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.cxx.toolchain.nativelink.NativeLinkableGroup}

            ### Methods inherited from interface com.facebook.buck.cxx.toolchain.nativelink.[NativeLinkableGroup](NativeLinkableGroup.html "interface in com.facebook.buck.cxx.toolchain.nativelink")

            `getBuildTarget`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getNativeLinkableDeps(com.facebook.buck.core.rules.BuildRuleResolver)}

        -   #### getNativeLinkableDeps

            ``` methodSignature
            Iterable<? extends NativeLinkableGroup> getNativeLinkableDeps​(BuildRuleResolver ruleResolver)
            ```

            [Returns:]{.returnLabel}
            :   All native linkable dependencies that might be required
                by this linkable on any platform.

        []{#getNativeLinkableExportedDeps(com.facebook.buck.core.rules.BuildRuleResolver)}

        -   #### getNativeLinkableExportedDeps

            ``` methodSignature
            Iterable<? extends NativeLinkableGroup> getNativeLinkableExportedDeps​(BuildRuleResolver ruleResolver)
            ```

            [Returns:]{.returnLabel}
            :   All native linkable exported dependencies that might be
                required by this linkable on any platform.

        []{#getNativeLinkableDepsForPlatform(com.facebook.buck.cxx.toolchain.CxxPlatform,com.facebook.buck.core.rules.BuildRuleResolver)}

        -   #### getNativeLinkableDepsForPlatform

            ``` methodSignature
            @Deprecated
            default Iterable<? extends NativeLinkableGroup> getNativeLinkableDepsForPlatform​(CxxPlatform cxxPlatform,
                                                                                             BuildRuleResolver ruleResolver)
            ```

            ::: deprecationBlock
            [Deprecated.]{.deprecatedLabel}
            :::

            [Returns:]{.returnLabel}
            :   All native linkable dependencies that are required by
                this linkable on a specific platform.

        []{#getNativeLinkableExportedDepsForPlatform(com.facebook.buck.cxx.toolchain.CxxPlatform,com.facebook.buck.core.rules.ActionGraphBuilder)}

        -   #### getNativeLinkableExportedDepsForPlatform

            ``` methodSignature
            @Deprecated
            default Iterable<? extends NativeLinkableGroup> getNativeLinkableExportedDepsForPlatform​(CxxPlatform cxxPlatform,
                                                                                                     ActionGraphBuilder graphBuilder)
            ```

            ::: deprecationBlock
            [Deprecated.]{.deprecatedLabel}
            :::

            [Returns:]{.returnLabel}
            :   All native linkable exported dependencies that are
                required by this linkable on a specific platform.

        []{#getNativeLinkableInput(com.facebook.buck.cxx.toolchain.CxxPlatform,com.facebook.buck.cxx.toolchain.linker.Linker.LinkableDepType,boolean,com.facebook.buck.core.rules.ActionGraphBuilder,com.facebook.buck.core.model.TargetConfiguration)}

        -   #### getNativeLinkableInput

            ``` methodSignature
            @Deprecated
            NativeLinkableInput getNativeLinkableInput​(CxxPlatform cxxPlatform,
                                                       Linker.LinkableDepType type,
                                                       boolean forceLinkWhole,
                                                       ActionGraphBuilder graphBuilder,
                                                       TargetConfiguration targetConfiguration)
            ```

            ::: deprecationBlock
            [Deprecated.]{.deprecatedLabel}
            :::

            ::: block
            Return input that \*dependents\* should put on their link
            line when linking against this linkable.
            :::

        []{#getNativeLinkableInput(com.facebook.buck.cxx.toolchain.CxxPlatform,com.facebook.buck.cxx.toolchain.linker.Linker.LinkableDepType,com.facebook.buck.core.rules.ActionGraphBuilder,com.facebook.buck.core.model.TargetConfiguration)}

        -   #### getNativeLinkableInput

            ``` methodSignature
            @Deprecated
            default NativeLinkableInput getNativeLinkableInput​(CxxPlatform cxxPlatform,
                                                               Linker.LinkableDepType type,
                                                               ActionGraphBuilder graphBuilder,
                                                               TargetConfiguration targetConfiguration)
            ```

            ::: deprecationBlock
            [Deprecated.]{.deprecatedLabel}
            :::

            ::: block
            Return input that \*dependents\* should put on their link
            line when linking against this linkable.
            :::

        []{#getNativeLinkTarget(com.facebook.buck.cxx.toolchain.CxxPlatform,com.facebook.buck.core.rules.ActionGraphBuilder)}

        -   #### getNativeLinkTarget

            ``` methodSignature
            @Deprecated
            default Optional<NativeLinkTargetGroup> getNativeLinkTarget​(CxxPlatform cxxPlatform,
                                                                        ActionGraphBuilder graphBuilder)
            ```

            ::: deprecationBlock
            [Deprecated.]{.deprecatedLabel}
            :::

            ::: block
            Optionally returns a
            [`NativeLinkTargetGroup`](NativeLinkTargetGroup.html "interface in com.facebook.buck.cxx.toolchain.nativelink").
            Most implementations of NativeLinkableGroup are themselves
            instances of NativeLinkTargetGroup.
            :::

        []{#supportsOmnibusLinking(com.facebook.buck.cxx.toolchain.CxxPlatform)}

        -   #### supportsOmnibusLinking

            ``` methodSignature
            @Deprecated
            default boolean supportsOmnibusLinking​(CxxPlatform cxxPlatform)
            ```

            ::: deprecationBlock
            [Deprecated.]{.deprecatedLabel}
            :::

            [Returns:]{.returnLabel}
            :   whether this
                [`NativeLinkableGroup`](NativeLinkableGroup.html "interface in com.facebook.buck.cxx.toolchain.nativelink")
                supports omnibus linking.

        []{#isPrebuiltSOForHaskellOmnibus(com.facebook.buck.cxx.toolchain.CxxPlatform,com.facebook.buck.core.rules.ActionGraphBuilder)}

        -   #### isPrebuiltSOForHaskellOmnibus

            ``` methodSignature
            @Deprecated
            default boolean isPrebuiltSOForHaskellOmnibus​(CxxPlatform cxxPlatform,
                                                          ActionGraphBuilder graphBuilder)
            ```

            ::: deprecationBlock
            [Deprecated.]{.deprecatedLabel}
            :::

            ::: block
            Whether the nativeLinkable should be linked shared or
            otherwise for haskell omnibus.
            :::

        []{#supportsOmnibusLinkingForHaskell(com.facebook.buck.cxx.toolchain.CxxPlatform)}

        -   #### supportsOmnibusLinkingForHaskell

            ``` methodSignature
            @Deprecated
            default boolean supportsOmnibusLinkingForHaskell​(CxxPlatform cxxPlatform)
            ```

            ::: deprecationBlock
            [Deprecated.]{.deprecatedLabel}
            :::

            [Returns:]{.returnLabel}
            :   whether this
                [`NativeLinkableGroup`](NativeLinkableGroup.html "interface in com.facebook.buck.cxx.toolchain.nativelink")
                supports omnibus linking for haskell.

        []{#getExportedLinkerFlags(com.facebook.buck.cxx.toolchain.CxxPlatform,com.facebook.buck.core.rules.ActionGraphBuilder)}

        -   #### getExportedLinkerFlags

            ``` methodSignature
            @Deprecated
            default Iterable<? extends Arg> getExportedLinkerFlags​(CxxPlatform cxxPlatform,
                                                                   ActionGraphBuilder graphBuilder)
            ```

            ::: deprecationBlock
            [Deprecated.]{.deprecatedLabel}
            :::

            [Returns:]{.returnLabel}
            :   exported linker flags. These should be added to link
                lines of dependents.

        []{#getExportedPostLinkerFlags(com.facebook.buck.cxx.toolchain.CxxPlatform,com.facebook.buck.core.rules.ActionGraphBuilder)}

        -   #### getExportedPostLinkerFlags

            ``` methodSignature
            @Deprecated
            default Iterable<? extends Arg> getExportedPostLinkerFlags​(CxxPlatform cxxPlatform,
                                                                       ActionGraphBuilder graphBuilder)
            ```

            ::: deprecationBlock
            [Deprecated.]{.deprecatedLabel}
            :::

            [Returns:]{.returnLabel}
            :   exported post-linker flags. This should be added to
                lines of dependents after other linker flags.

        []{#forceLinkWholeForHaskellOmnibus()}

        -   #### forceLinkWholeForHaskellOmnibus

            ``` methodSignature
            @Deprecated
            default boolean forceLinkWholeForHaskellOmnibus()
            ```

            ::: deprecationBlock
            [Deprecated.]{.deprecatedLabel}
            :::

        []{#shouldBeLinkedInAppleTestAndHost()}

        -   #### shouldBeLinkedInAppleTestAndHost

            ``` methodSignature
            @Deprecated
            default boolean shouldBeLinkedInAppleTestAndHost()
            ```

            ::: deprecationBlock
            [Deprecated.]{.deprecatedLabel}
            :::

            ::: block
            Indicates whether this linkable should be included in both
            the test binary and the host binary for Apple tests.
            :::

        []{#getRuleType()}

        -   #### getRuleType

            ``` methodSignature
            @Deprecated
            default String getRuleType()
            ```

            ::: deprecationBlock
            [Deprecated.]{.deprecatedLabel}
            :::

            ::: block
            Return a string representing the type of this rule.
            :::

        []{#getPreferredLinkage(com.facebook.buck.cxx.toolchain.CxxPlatform)}

        -   #### getPreferredLinkage

            ``` methodSignature
            @Deprecated
            NativeLinkableGroup.Linkage getPreferredLinkage​(CxxPlatform cxxPlatform)
            ```

            ::: deprecationBlock
            [Deprecated.]{.deprecatedLabel}
            :::

        []{#getSharedLibraries(com.facebook.buck.cxx.toolchain.CxxPlatform,com.facebook.buck.core.rules.ActionGraphBuilder)}

        -   #### getSharedLibraries

            ``` methodSignature
            @Deprecated
            com.google.common.collect.ImmutableMap<String,​SourcePath> getSharedLibraries​(CxxPlatform cxxPlatform,
                                                                                               ActionGraphBuilder graphBuilder)
            ```

            ::: deprecationBlock
            [Deprecated.]{.deprecatedLabel}
            :::

            [Returns:]{.returnLabel}
            :   a map of shared library SONAME to shared library path
                for the given
                [`CxxPlatform`](../CxxPlatform.html "interface in com.facebook.buck.cxx.toolchain").

        []{#getNativeLinkable(com.facebook.buck.cxx.toolchain.CxxPlatform,com.facebook.buck.core.rules.ActionGraphBuilder)}

        -   #### getNativeLinkable

            ``` methodSignature
            default NativeLinkable getNativeLinkable​(CxxPlatform cxxPlatform,
                                                     ActionGraphBuilder graphBuilder)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getNativeLinkable` in interface `NativeLinkableGroup`

        []{#getNativeLinkableCompatibilityCache()}

        -   #### getNativeLinkableCompatibilityCache

            ``` methodSignature
            PlatformLockedNativeLinkableGroup.Cache getNativeLinkableCompatibilityCache()
            ```

        []{#getNativeLinkableCache(com.facebook.buck.cxx.toolchain.nativelink.LegacyNativeLinkableGroup)}

        -   #### getNativeLinkableCache

            ``` methodSignature
            static PlatformLockedNativeLinkableGroup.Cache getNativeLinkableCache​(LegacyNativeLinkableGroup group)
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

-   [Overview](../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../deprecated-list.html)
-   [Index](../../../../../../index-all.html)
-   [Help](../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../allclasses.html)

<div>

<div>

JavaScript is disabled on your browser.

</div>

</div>

<div>

-   Summary: 
-   [Nested](#nested.class.summary) \| 
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
