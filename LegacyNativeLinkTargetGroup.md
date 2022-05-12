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

## Interface LegacyNativeLinkTargetGroup {#interface-legacynativelinktargetgroup .title title="Interface LegacyNativeLinkTargetGroup"}
:::

::: contentContainer
::: description
-   

    All Superinterfaces:
    :   `NativeLinkTargetGroup`

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `CxxLibraryGroup`

    ------------------------------------------------------------------------

        public interface LegacyNativeLinkTargetGroup
        extends NativeLinkTargetGroup

    ::: block
    An implementation of
    [`NativeLinkTargetGroup`](NativeLinkTargetGroup.html "interface in com.facebook.buck.cxx.toolchain.nativelink")
    where the corresponding
    [`NativeLinkTarget`](NativeLinkTarget.html "interface in com.facebook.buck.cxx.toolchain.nativelink")
    just refer back to this.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `Iterable<? extends   | `                     | ::: block             |
        | NativeLinkableGroup>` | getNativeLinkTargetDe | [Deprecate            |
        |                       | ps​(CxxPlatform cxxPla | d.]{.deprecatedLabel} |
        |                       | tform,                |                       |
        |                       |          ActionGraphB | :                     |
        |                       | uilder graphBuilder)` | :: deprecationComment |
        |                       |                       | Convert to a          |
        |                       |                       | [`NativeLinkTarge     |
        |                       |                       | t`](NativeLinkTarget. |
        |                       |                       | html "interface in co |
        |                       |                       | m.facebook.buck.cxx.t |
        |                       |                       | oolchain.nativelink") |
        |                       |                       | and use               |
        |                       |                       | [`NativeLinkT         |
        |                       |                       | arget.getNativeLinkTa |
        |                       |                       | rgetDeps(ActionGraphB |
        |                       |                       | uilder)`](NativeLinkT |
        |                       |                       | arget.html#getNativeL |
        |                       |                       | inkTargetDeps(com.fac |
        |                       |                       | ebook.buck.core.rules |
        |                       |                       | .ActionGraphBuilder)) |
        |                       |                       | instead.              |
        |                       |                       | :::                   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `NativeLinkableInput` | `getNativeLinkTargetI |                       |
        |                       | nput​(CxxPlatform cxxP |                       |
        |                       | latform,              |                       |
        |                       |             ActionGra |                       |
        |                       | phBuilder graphBuilde |                       |
        |                       | r,                    |                       |
        |                       |       SourcePathResol |                       |
        |                       | verAdapter pathResolv |                       |
        |                       | er,                   |                       |
        |                       |        boolean includ |                       |
        |                       | ePrivateLinkerFlags)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getNati              | ::: block             |
        | NativeLinkTargetMode` | veLinkTargetMode​(CxxP | [Deprecate            |
        |                       | latform cxxPlatform)` | d.]{.deprecatedLabel} |
        |                       |                       |                       |
        |                       |                       | :                     |
        |                       |                       | :: deprecationComment |
        |                       |                       | Convert to a          |
        |                       |                       | [`NativeLinkTarge     |
        |                       |                       | t`](NativeLinkTarget. |
        |                       |                       | html "interface in co |
        |                       |                       | m.facebook.buck.cxx.t |
        |                       |                       | oolchain.nativelink") |
        |                       |                       | and use               |
        |                       |                       | [`NativeLin           |
        |                       |                       | kTarget.getNativeLink |
        |                       |                       | TargetMode()`](Native |
        |                       |                       | LinkTarget.html#getNa |
        |                       |                       | tiveLinkTargetMode()) |
        |                       |                       | instead.              |
        |                       |                       | :::                   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Path>`      | `getNativeLi          | ::: block             |
        |                       | nkTargetOutputPath()` | [Deprecate            |
        |                       |                       | d.]{.deprecatedLabel} |
        |                       |                       |                       |
        |                       |                       | :                     |
        |                       |                       | :: deprecationComment |
        |                       |                       | Convert to a          |
        |                       |                       | [`NativeLinkTarge     |
        |                       |                       | t`](NativeLinkTarget. |
        |                       |                       | html "interface in co |
        |                       |                       | m.facebook.buck.cxx.t |
        |                       |                       | oolchain.nativelink") |
        |                       |                       | and use               |
        |                       |                       | [`NativeLin           |
        |                       |                       | kTarget.getNativeLink |
        |                       |                       | TargetMode()`](Native |
        |                       |                       | LinkTarget.html#getNa |
        |                       |                       | tiveLinkTargetMode()) |
        |                       |                       | instead.              |
        |                       |                       | :::                   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `defa                 | `getTargetForPlatf    |                       |
        | ult NativeLinkTarget` | orm​(CxxPlatform cxxPl |                       |
        |                       | atform,               |                       |
        |                       |        boolean includ |                       |
        |                       | ePrivateLinkerFlags)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
        .tableTab}[[Default
        Methods](javascript:show(16);)[ ]{.tabEnd}]{#t5
        .tableTab}[[Deprecated
        Methods](javascript:show(32);)[ ]{.tabEnd}]{#t6 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.cxx.toolchain.nativelink.NativeLinkTargetGroup}

            ### Methods inherited from interface com.facebook.buck.cxx.toolchain.nativelink.[NativeLinkTargetGroup](NativeLinkTargetGroup.html "interface in com.facebook.buck.cxx.toolchain.nativelink")

            `getBuildTarget`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getNativeLinkTargetMode(com.facebook.buck.cxx.toolchain.CxxPlatform)}

        -   #### getNativeLinkTargetMode

            ``` methodSignature
            @Deprecated
            NativeLinkTargetMode getNativeLinkTargetMode​(CxxPlatform cxxPlatform)
            ```

            ::: deprecationBlock
            [Deprecated.]{.deprecatedLabel}

            ::: deprecationComment
            Convert to a
            [`NativeLinkTarget`](NativeLinkTarget.html "interface in com.facebook.buck.cxx.toolchain.nativelink")
            and use
            [`NativeLinkTarget.getNativeLinkTargetMode()`](NativeLinkTarget.html#getNativeLinkTargetMode())
            instead.
            :::
            :::

        []{#getNativeLinkTargetDeps(com.facebook.buck.cxx.toolchain.CxxPlatform,com.facebook.buck.core.rules.ActionGraphBuilder)}

        -   #### getNativeLinkTargetDeps

            ``` methodSignature
            @Deprecated
            Iterable<? extends NativeLinkableGroup> getNativeLinkTargetDeps​(CxxPlatform cxxPlatform,
                                                                            ActionGraphBuilder graphBuilder)
            ```

            ::: deprecationBlock
            [Deprecated.]{.deprecatedLabel}

            ::: deprecationComment
            Convert to a
            [`NativeLinkTarget`](NativeLinkTarget.html "interface in com.facebook.buck.cxx.toolchain.nativelink")
            and use
            [`NativeLinkTarget.getNativeLinkTargetDeps(ActionGraphBuilder)`](NativeLinkTarget.html#getNativeLinkTargetDeps(com.facebook.buck.core.rules.ActionGraphBuilder))
            instead.
            :::
            :::

            [Returns:]{.returnLabel}
            :   the
                [`NativeLinkableGroup`](NativeLinkableGroup.html "interface in com.facebook.buck.cxx.toolchain.nativelink")
                dependencies used to link this target.

        []{#getNativeLinkTargetOutputPath()}

        -   #### getNativeLinkTargetOutputPath

            ``` methodSignature
            @Deprecated
            Optional<Path> getNativeLinkTargetOutputPath()
            ```

            ::: deprecationBlock
            [Deprecated.]{.deprecatedLabel}

            ::: deprecationComment
            Convert to a
            [`NativeLinkTarget`](NativeLinkTarget.html "interface in com.facebook.buck.cxx.toolchain.nativelink")
            and use
            [`NativeLinkTarget.getNativeLinkTargetMode()`](NativeLinkTarget.html#getNativeLinkTargetMode())
            instead.
            :::
            :::

            [Returns:]{.returnLabel}
            :   an explicit
                [`Path`](http://docs.oracle.com/javase/7/docs/api/java/nio/file/Path.html?is-external=true "class or interface in java.nio.file"){.externalLink}
                to use for the output location.

        []{#getTargetForPlatform(com.facebook.buck.cxx.toolchain.CxxPlatform,boolean)}

        -   #### getTargetForPlatform

            ``` methodSignature
            default NativeLinkTarget getTargetForPlatform​(CxxPlatform cxxPlatform,
                                                          boolean includePrivateLinkerFlags)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getTargetForPlatform` in
                interface `NativeLinkTargetGroup`
            :   `includePrivateLinkerFlags` - whether to include
                rule-specific non-exported linker flags.

        []{#getNativeLinkTargetInput(com.facebook.buck.cxx.toolchain.CxxPlatform,com.facebook.buck.core.rules.ActionGraphBuilder,com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter,boolean)}

        -   #### getNativeLinkTargetInput

            ``` methodSignature
            NativeLinkableInput getNativeLinkTargetInput​(CxxPlatform cxxPlatform,
                                                         ActionGraphBuilder graphBuilder,
                                                         SourcePathResolverAdapter pathResolver,
                                                         boolean includePrivateLinkerFlags)
            ```

            [Returns:]{.returnLabel}
            :   the
                [`NativeLinkableInput`](NativeLinkableInput.html "class in com.facebook.buck.cxx.toolchain.nativelink")
                used to link this target.
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
