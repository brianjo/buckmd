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
[Package]{.packageLabelInType} [com.facebook.buck.cxx.toolchain.nativelink](package-summary.html)
:::

## Interface NativeLinkable {#interface-nativelinkable .title title="Interface NativeLinkable"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `NativeLinkableInfo`, `PlatformLockedNativeLinkableGroup`

    ------------------------------------------------------------------------

        public interface NativeLinkable

    ::: block
    Interface for objects (e.g. C++ libraries) which can contribute to
    the top-level link of a native binary (e.g. C++ binary). This
    represents the linkable object for a specific platform.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `default boolean`     | `forceLinkWhol        |                       |
        |                       | eForHaskellOmnibus()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `BuildTarget`         | `getBuildTarget()`    |                       |
        +-----------------------+-----------------------+-----------------------+
        | `default Ite          | `getExportedLin       |                       |
        | rable<? extends Arg>` | kerFlags​(ActionGraphB |                       |
        |                       | uilder graphBuilder)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `default Ite          | `getExportedPostLin   |                       |
        | rable<? extends Arg>` | kerFlags​(ActionGraphB |                       |
        |                       | uilder graphBuilder)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Iterable<? ext       | `getNativeLink        |                       |
        | ends NativeLinkable>` | ableDeps​(ActionGraphB |                       |
        |                       | uilder graphBuilder)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Iterable<? ext       | `                     |                       |
        | ends NativeLinkable>` | getNativeLinkableExpo |                       |
        |                       | rtedDeps​(ActionGraphB |                       |
        |                       | uilder graphBuilder)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `NativeLinkableInput` | `getNat               | ::: block             |
        |                       | iveLinkableInput​(Link | Return input that     |
        |                       | er.LinkableDepType ty | \*dependents\* should |
        |                       | pe,                   | put on their link     |
        |                       |      boolean forceLin | line when linking     |
        |                       | kWhole,               | against this          |
        |                       |          ActionGraphB | linkable.             |
        |                       | uilder graphBuilder,  | :::                   |
        |                       |                       |                       |
        |                       |  TargetConfiguration  |                       |
        |                       | targetConfiguration)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `default              | `ge                   | ::: block             |
        |  NativeLinkableInput` | tNativeLinkableInput​( | Return input that     |
        |                       | Linker.LinkableDepTyp | \*dependents\* should |
        |                       | e type,               | put on their link     |
        |                       |          ActionGraphB | line when linking     |
        |                       | uilder graphBuilder,  | against this          |
        |                       |                       | linkable.             |
        |                       |  TargetConfiguration  | :::                   |
        |                       | targetConfiguration)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Option               | `ge                   | ::: block             |
        | al<NativeLinkTarget>` | tNativeLinkTarget​(Act | Optionally returns a  |
        |                       | ionGraphBuilder graph | [`NativeLinkTarget    |
        |                       | Builder,              | `](NativeLinkTarget.h |
        |                       |        boolean includ | tml "interface in com |
        |                       | ePrivateLinkerFlags)` | .facebook.buck.cxx.to |
        |                       |                       | olchain.nativelink"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `NativeL              | `g                    |                       |
        | inkableGroup.Linkage` | etPreferredLinkage()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `default String`      | `getRuleType()`       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.commo     | `getSharedL           |                       |
        | n.collect.ImmutableMa | ibraries​(ActionGraphB |                       |
        | p<String,​SourcePath>` | uilder graphBuilder)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `default boolean`     | `                     |                       |
        |                       | isPrebuiltSOForHaskel |                       |
        |                       | lOmnibus​(ActionGraphB |                       |
        |                       | uilder graphBuilder)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `shouldBeLinked       |                       |
        |                       | InAppleTestAndHost()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `default boolean`     | `supp                 |                       |
        |                       | ortsOmnibusLinking()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `default boolean`     | `supportsOmnibu       |                       |
        |                       | sLinkingForHaskell()` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
        .tableTab}[[Default
        Methods](javascript:show(16);)[ ]{.tabEnd}]{#t5 .tableTab}
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getBuildTarget()}

        -   #### getBuildTarget

            ``` methodSignature
            BuildTarget getBuildTarget()
            ```

            [Returns:]{.returnLabel}
            :   The
                [`BuildTarget`](../../../core/model/BuildTarget.html "class in com.facebook.buck.core.model")
                for this linkable.

        []{#getNativeLinkableDeps(com.facebook.buck.core.rules.ActionGraphBuilder)}

        -   #### getNativeLinkableDeps

            ``` methodSignature
            Iterable<? extends NativeLinkable> getNativeLinkableDeps​(ActionGraphBuilder graphBuilder)
            ```

            [Returns:]{.returnLabel}
            :   All native linkable dependencies that might be required
                by this linkable.

        []{#getNativeLinkableExportedDeps(com.facebook.buck.core.rules.ActionGraphBuilder)}

        -   #### getNativeLinkableExportedDeps

            ``` methodSignature
            Iterable<? extends NativeLinkable> getNativeLinkableExportedDeps​(ActionGraphBuilder graphBuilder)
            ```

            [Returns:]{.returnLabel}
            :   All native linkable exported dependencies that might be
                required by this linkable.

        []{#getNativeLinkableInput(com.facebook.buck.cxx.toolchain.linker.Linker.LinkableDepType,boolean,com.facebook.buck.core.rules.ActionGraphBuilder,com.facebook.buck.core.model.TargetConfiguration)}

        -   #### getNativeLinkableInput

            ``` methodSignature
            NativeLinkableInput getNativeLinkableInput​(Linker.LinkableDepType type,
                                                       boolean forceLinkWhole,
                                                       ActionGraphBuilder graphBuilder,
                                                       TargetConfiguration targetConfiguration)
            ```

            ::: block
            Return input that \*dependents\* should put on their link
            line when linking against this linkable.
            :::

        []{#getNativeLinkableInput(com.facebook.buck.cxx.toolchain.linker.Linker.LinkableDepType,com.facebook.buck.core.rules.ActionGraphBuilder,com.facebook.buck.core.model.TargetConfiguration)}

        -   #### getNativeLinkableInput

            ``` methodSignature
            default NativeLinkableInput getNativeLinkableInput​(Linker.LinkableDepType type,
                                                               ActionGraphBuilder graphBuilder,
                                                               TargetConfiguration targetConfiguration)
            ```

            ::: block
            Return input that \*dependents\* should put on their link
            line when linking against this linkable.
            :::

        []{#getNativeLinkTarget(com.facebook.buck.core.rules.ActionGraphBuilder,boolean)}

        -   #### getNativeLinkTarget

            ``` methodSignature
            Optional<NativeLinkTarget> getNativeLinkTarget​(ActionGraphBuilder graphBuilder,
                                                           boolean includePrivateLinkerFlags)
            ```

            ::: block
            Optionally returns a
            [`NativeLinkTarget`](NativeLinkTarget.html "interface in com.facebook.buck.cxx.toolchain.nativelink").
            Most implementations of NativeLinkable are themselves
            instances of NativeLinkTarget.
            :::

            [Parameters:]{.paramLabel}
            :   `includePrivateLinkerFlags` - whether to include
                rule-specific non-exported linker flags.

        []{#getPreferredLinkage()}

        -   #### getPreferredLinkage

            ``` methodSignature
            NativeLinkableGroup.Linkage getPreferredLinkage()
            ```

            [Returns:]{.returnLabel}
            :   The preferred
                [`NativeLinkableGroup.Linkage`](NativeLinkableGroup.Linkage.html "enum in com.facebook.buck.cxx.toolchain.nativelink")
                for this linkable.

        []{#getSharedLibraries(com.facebook.buck.core.rules.ActionGraphBuilder)}

        -   #### getSharedLibraries

            ``` methodSignature
            com.google.common.collect.ImmutableMap<String,​SourcePath> getSharedLibraries​(ActionGraphBuilder graphBuilder)
            ```

            [Returns:]{.returnLabel}
            :   a map of shared library SONAME to shared library path
                for the given
                [`CxxPlatform`](../CxxPlatform.html "interface in com.facebook.buck.cxx.toolchain").

        []{#supportsOmnibusLinking()}

        -   #### supportsOmnibusLinking

            ``` methodSignature
            default boolean supportsOmnibusLinking()
            ```

            [Returns:]{.returnLabel}
            :   whether this
                [`NativeLinkable`](NativeLinkable.html "interface in com.facebook.buck.cxx.toolchain.nativelink")
                supports omnibus linking.

        []{#getExportedLinkerFlags(com.facebook.buck.core.rules.ActionGraphBuilder)}

        -   #### getExportedLinkerFlags

            ``` methodSignature
            default Iterable<? extends Arg> getExportedLinkerFlags​(ActionGraphBuilder graphBuilder)
            ```

            [Returns:]{.returnLabel}
            :   exported linker flags. These should be added to link
                lines of dependents.

        []{#getExportedPostLinkerFlags(com.facebook.buck.core.rules.ActionGraphBuilder)}

        -   #### getExportedPostLinkerFlags

            ``` methodSignature
            default Iterable<? extends Arg> getExportedPostLinkerFlags​(ActionGraphBuilder graphBuilder)
            ```

            [Returns:]{.returnLabel}
            :   exported post-linker flags. This should be added to
                lines of dependents after other linker flags.

        []{#getRuleType()}

        -   #### getRuleType

            ``` methodSignature
            default String getRuleType()
            ```

        []{#shouldBeLinkedInAppleTestAndHost()}

        -   #### shouldBeLinkedInAppleTestAndHost

            ``` methodSignature
            boolean shouldBeLinkedInAppleTestAndHost()
            ```

        []{#isPrebuiltSOForHaskellOmnibus(com.facebook.buck.core.rules.ActionGraphBuilder)}

        -   #### isPrebuiltSOForHaskellOmnibus

            ``` methodSignature
            default boolean isPrebuiltSOForHaskellOmnibus​(ActionGraphBuilder graphBuilder)
            ```

        []{#supportsOmnibusLinkingForHaskell()}

        -   #### supportsOmnibusLinkingForHaskell

            ``` methodSignature
            default boolean supportsOmnibusLinkingForHaskell()
            ```

        []{#forceLinkWholeForHaskellOmnibus()}

        -   #### forceLinkWholeForHaskellOmnibus

            ``` methodSignature
            default boolean forceLinkWholeForHaskellOmnibus()
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
