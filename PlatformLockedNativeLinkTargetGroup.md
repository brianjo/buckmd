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
[Package]{.packageLabelInType} [com.facebook.buck.cxx.toolchain.nativelink](package-summary.html)
:::

## Class PlatformLockedNativeLinkTargetGroup {#class-platformlockednativelinktargetgroup .title title="Class PlatformLockedNativeLinkTargetGroup"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.cxx.toolchain.nativelink.PlatformLockedNativeLinkTargetGroup

::: description
-   

    All Implemented Interfaces:
    :   `NativeLinkTarget`

    ------------------------------------------------------------------------

        public class PlatformLockedNativeLinkTargetGroup
        extends Object
        implements NativeLinkTarget

    ::: block
    Implementation of
    [`NativeLinkTarget`](NativeLinkTarget.html "interface in com.facebook.buck.cxx.toolchain.nativelink")
    in terms of just a fixed
    [`CxxPlatform`](../CxxPlatform.html "interface in com.facebook.buck.cxx.toolchain")
    and
    [`NativeLinkTargetGroup`](NativeLinkTargetGroup.html "interface in com.facebook.buck.cxx.toolchain.nativelink").
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                            Description
          ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `PlatformLockedNativeLinkTargetGroup​(LegacyNativeLinkTargetGroup underlyingGroup,                                    CxxPlatform cxxPlatform,                                    boolean includePrivateLinkerFlags)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
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
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.cxx.toolchain.nativelink.LegacyNativeLinkTargetGroup,com.facebook.buck.cxx.toolchain.CxxPlatform,boolean)}

        -   #### PlatformLockedNativeLinkTargetGroup

                public PlatformLockedNativeLinkTargetGroup​(LegacyNativeLinkTargetGroup underlyingGroup,
                                                           CxxPlatform cxxPlatform,
                                                           boolean includePrivateLinkerFlags)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getBuildTarget()}

        -   #### getBuildTarget

            ``` methodSignature
            public BuildTarget getBuildTarget()
            ```

            ::: block
            [Description copied from
            interface: `NativeLinkTarget`]{.descfrmTypeLabel}
            :::

            ::: block
            A representative
            [`BuildTarget`](../../../core/model/BuildTarget.html "class in com.facebook.buck.core.model")
            for this object.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getBuildTarget` in interface `NativeLinkTarget`

        []{#getNativeLinkTargetMode()}

        -   #### getNativeLinkTargetMode

            ``` methodSignature
            public NativeLinkTargetMode getNativeLinkTargetMode()
            ```

            ::: block
            [Description copied from
            interface: `NativeLinkTarget`]{.descfrmTypeLabel}
            :::

            ::: block
            The
            [`NativeLinkTargetMode`](NativeLinkTargetMode.html "class in com.facebook.buck.cxx.toolchain.nativelink")
            for this target.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getNativeLinkTargetMode` in
                interface `NativeLinkTarget`

        []{#getNativeLinkTargetDeps(com.facebook.buck.core.rules.ActionGraphBuilder)}

        -   #### getNativeLinkTargetDeps

            ``` methodSignature
            public Iterable<? extends NativeLinkable> getNativeLinkTargetDeps​(ActionGraphBuilder graphBuilder)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getNativeLinkTargetDeps` in
                interface `NativeLinkTarget`

            [Returns:]{.returnLabel}
            :   the
                [`NativeLinkable`](NativeLinkable.html "interface in com.facebook.buck.cxx.toolchain.nativelink")
                dependencies used to link this target.

        []{#getNativeLinkTargetInput(com.facebook.buck.core.rules.ActionGraphBuilder,com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter)}

        -   #### getNativeLinkTargetInput

            ``` methodSignature
            public NativeLinkableInput getNativeLinkTargetInput​(ActionGraphBuilder graphBuilder,
                                                                SourcePathResolverAdapter pathResolver)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getNativeLinkTargetInput` in
                interface `NativeLinkTarget`

            [Returns:]{.returnLabel}
            :   the
                [`NativeLinkableInput`](NativeLinkableInput.html "class in com.facebook.buck.cxx.toolchain.nativelink")
                used to link this target.

        []{#getNativeLinkTargetOutputPath()}

        -   #### getNativeLinkTargetOutputPath

            ``` methodSignature
            public Optional<Path> getNativeLinkTargetOutputPath()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getNativeLinkTargetOutputPath` in
                interface `NativeLinkTarget`

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
