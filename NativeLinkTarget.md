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

## Interface NativeLinkTarget {#interface-nativelinktarget .title title="Interface NativeLinkTarget"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `NativeLinkTargetInfo`, `PlatformLockedNativeLinkTargetGroup`

    ------------------------------------------------------------------------

        public interface NativeLinkTarget

    ::: block
    Interface for an object that can be the target of a native link.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `BuildTarget`         | `getBuildTarget()`    | ::: block             |
        |                       |                       | A representative      |
        |                       |                       | [`BuildTa             |
        |                       |                       | rget`](../../../core/ |
        |                       |                       | model/BuildTarget.htm |
        |                       |                       | l "class in com.faceb |
        |                       |                       | ook.buck.core.model") |
        |                       |                       | for this object.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Iterable<? ext       | `getNativeLinkTa      |                       |
        | ends NativeLinkable>` | rgetDeps​(ActionGraphB |                       |
        |                       | uilder graphBuilder)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `NativeLinkableInput` | `getNativeLinkTarg    |                       |
        |                       | etInput​(ActionGraphBu |                       |
        |                       | ilder graphBuilder,   |                       |
        |                       |                       |                       |
        |                       |   SourcePathResolverA |                       |
        |                       | dapter pathResolver)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getNa                | ::: block             |
        | NativeLinkTargetMode` | tiveLinkTargetMode()` | The                   |
        |                       |                       | [`NativeLinkTargetMod |
        |                       |                       | e`](NativeLinkTargetM |
        |                       |                       | ode.html "class in co |
        |                       |                       | m.facebook.buck.cxx.t |
        |                       |                       | oolchain.nativelink") |
        |                       |                       | for this target.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Path>`      | `getNativeLi          |                       |
        |                       | nkTargetOutputPath()` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}
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

            ::: block
            A representative
            [`BuildTarget`](../../../core/model/BuildTarget.html "class in com.facebook.buck.core.model")
            for this object.
            :::

        []{#getNativeLinkTargetMode()}

        -   #### getNativeLinkTargetMode

            ``` methodSignature
            NativeLinkTargetMode getNativeLinkTargetMode()
            ```

            ::: block
            The
            [`NativeLinkTargetMode`](NativeLinkTargetMode.html "class in com.facebook.buck.cxx.toolchain.nativelink")
            for this target.
            :::

        []{#getNativeLinkTargetDeps(com.facebook.buck.core.rules.ActionGraphBuilder)}

        -   #### getNativeLinkTargetDeps

            ``` methodSignature
            Iterable<? extends NativeLinkable> getNativeLinkTargetDeps​(ActionGraphBuilder graphBuilder)
            ```

            [Returns:]{.returnLabel}
            :   the
                [`NativeLinkable`](NativeLinkable.html "interface in com.facebook.buck.cxx.toolchain.nativelink")
                dependencies used to link this target.

        []{#getNativeLinkTargetInput(com.facebook.buck.core.rules.ActionGraphBuilder,com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter)}

        -   #### getNativeLinkTargetInput

            ``` methodSignature
            NativeLinkableInput getNativeLinkTargetInput​(ActionGraphBuilder graphBuilder,
                                                         SourcePathResolverAdapter pathResolver)
            ```

            [Returns:]{.returnLabel}
            :   the
                [`NativeLinkableInput`](NativeLinkableInput.html "class in com.facebook.buck.cxx.toolchain.nativelink")
                used to link this target.

        []{#getNativeLinkTargetOutputPath()}

        -   #### getNativeLinkTargetOutputPath

            ``` methodSignature
            Optional<Path> getNativeLinkTargetOutputPath()
            ```

            [Returns:]{.returnLabel}
            :   an explicit
                [`Path`](http://docs.oracle.com/javase/7/docs/api/java/nio/file/Path.html?is-external=true "class or interface in java.nio.file"){.externalLink}
                to use for the output location.
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
