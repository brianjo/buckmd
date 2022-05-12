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

## Class NativeLinkableInfo {#class-nativelinkableinfo .title title="Class NativeLinkableInfo"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.cxx.toolchain.nativelink.NativeLinkableInfo

::: description
-   

    All Implemented Interfaces:
    :   `NativeLinkable`

    ------------------------------------------------------------------------

        public class NativeLinkableInfo
        extends Object
        implements NativeLinkable

    ::: block
    An implementation of
    [`NativeLinkable`](NativeLinkable.html "interface in com.facebook.buck.cxx.toolchain.nativelink")
    where (most of) the behavior is fixed when created.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static class `       | `NativeLinkab         | ::: block             |
        |                       | leInfo.Configuration` | Configuration is used |
        |                       |                       | for configuring the   |
        |                       |                       | less-commonly changed |
        |                       |                       | parts of the \@{link  |
        |                       |                       | NativeLinkableInfo}.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static interface `   | `NativeL              | ::: block             |
        |                       | inkableInfo.Delegate` | The Delegate allows   |
        |                       |                       | instances to create   |
        |                       |                       | [`NativeLinkableInp   |
        |                       |                       | ut`](NativeLinkableIn |
        |                       |                       | put.html "class in co |
        |                       |                       | m.facebook.buck.cxx.t |
        |                       |                       | oolchain.nativelink") |
        |                       |                       | when requested.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                                                                                                                                                                                   Description
          --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `NativeLinkableInfo​(BuildTarget buildTarget,                   String ruleType,                   com.google.common.collect.ImmutableList<NativeLinkable> deps,                   com.google.common.collect.ImmutableList<NativeLinkable> exportedDeps,                   NativeLinkableGroup.Linkage preferredLinkage,                   NativeLinkableInfo.Delegate delegate,                   NativeLinkableInfo.Configuration config)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static NativeLinkab  | `defaults()`          | ::: block             |
        | leInfo.Configuration` |                       | Returns a             |
        |                       |                       | Configuration with    |
        |                       |                       | all the default       |
        |                       |                       | values.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static NativeL       | `fixedD               | ::: block             |
        | inkableInfo.Delegate` | elegate​(NativeLinkabl | Creates a delegate    |
        |                       | eInput instance,      | that always returns a |
        |                       |          com.google.c | fixed instance.       |
        |                       | ommon.collect.Immutab | :::                   |
        |                       | leMap<String,​SourcePa |                       |
        |                       | th> sharedLibraries)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `forceLinkWhol        |                       |
        |                       | eForHaskellOmnibus()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `BuildTarget`         | `getBuildTarget()`    |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Ite                  | `getExportedLin       |                       |
        | rable<? extends Arg>` | kerFlags​(ActionGraphB |                       |
        |                       | uilder graphBuilder)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Ite                  | `getExportedPostLin   |                       |
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
        | `String`              | `getRuleType()`       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.commo     | `getSharedL           |                       |
        | n.collect.ImmutableMa | ibraries​(ActionGraphB |                       |
        | p<String,​SourcePath>` | uilder graphBuilder)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `                     |                       |
        |                       | isPrebuiltSOForHaskel |                       |
        |                       | lOmnibus​(ActionGraphB |                       |
        |                       | uilder graphBuilder)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `shouldBeLinked       |                       |
        |                       | InAppleTestAndHost()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `supp                 |                       |
        |                       | ortsOmnibusLinking()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `supportsOmnibu       |                       |
        |                       | sLinkingForHaskell()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `toString()`          |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, wait, wait, wait`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.cxx.toolchain.nativelink.NativeLinkable}

            ### Methods inherited from interface com.facebook.buck.cxx.toolchain.nativelink.[NativeLinkable](NativeLinkable.html "interface in com.facebook.buck.cxx.toolchain.nativelink")

            `getNativeLinkableInput`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.core.model.BuildTarget,java.lang.String,com.google.common.collect.ImmutableList,com.google.common.collect.ImmutableList,com.facebook.buck.cxx.toolchain.nativelink.NativeLinkableGroup.Linkage,com.facebook.buck.cxx.toolchain.nativelink.NativeLinkableInfo.Delegate,com.facebook.buck.cxx.toolchain.nativelink.NativeLinkableInfo.Configuration)}

        -   #### NativeLinkableInfo

                public NativeLinkableInfo​(BuildTarget buildTarget,
                                          String ruleType,
                                          com.google.common.collect.ImmutableList<NativeLinkable> deps,
                                          com.google.common.collect.ImmutableList<NativeLinkable> exportedDeps,
                                          NativeLinkableGroup.Linkage preferredLinkage,
                                          NativeLinkableInfo.Delegate delegate,
                                          NativeLinkableInfo.Configuration config)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#fixedDelegate(com.facebook.buck.cxx.toolchain.nativelink.NativeLinkableInput,com.google.common.collect.ImmutableMap)}

        -   #### fixedDelegate

            ``` methodSignature
            public static NativeLinkableInfo.Delegate fixedDelegate​(NativeLinkableInput instance,
                                                                    com.google.common.collect.ImmutableMap<String,​SourcePath> sharedLibraries)
            ```

            ::: block
            Creates a delegate that always returns a fixed instance.
            :::

        []{#defaults()}

        -   #### defaults

            ``` methodSignature
            public static NativeLinkableInfo.Configuration defaults()
            ```

            ::: block
            Returns a Configuration with all the default values. These
            can be overriden with the various set methods.
            :::

        []{#toString()}

        -   #### toString

            ``` methodSignature
            public String toString()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `toString` in class `Object`

        []{#getRuleType()}

        -   #### getRuleType

            ``` methodSignature
            public String getRuleType()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getRuleType` in interface `NativeLinkable`

        []{#supportsOmnibusLinking()}

        -   #### supportsOmnibusLinking

            ``` methodSignature
            public boolean supportsOmnibusLinking()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `supportsOmnibusLinking` in interface `NativeLinkable`

            [Returns:]{.returnLabel}
            :   whether this
                [`NativeLinkable`](NativeLinkable.html "interface in com.facebook.buck.cxx.toolchain.nativelink")
                supports omnibus linking.

        []{#isPrebuiltSOForHaskellOmnibus(com.facebook.buck.core.rules.ActionGraphBuilder)}

        -   #### isPrebuiltSOForHaskellOmnibus

            ``` methodSignature
            public boolean isPrebuiltSOForHaskellOmnibus​(ActionGraphBuilder graphBuilder)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `isPrebuiltSOForHaskellOmnibus` in
                interface `NativeLinkable`

        []{#supportsOmnibusLinkingForHaskell()}

        -   #### supportsOmnibusLinkingForHaskell

            ``` methodSignature
            public boolean supportsOmnibusLinkingForHaskell()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `supportsOmnibusLinkingForHaskell` in
                interface `NativeLinkable`

        []{#forceLinkWholeForHaskellOmnibus()}

        -   #### forceLinkWholeForHaskellOmnibus

            ``` methodSignature
            public boolean forceLinkWholeForHaskellOmnibus()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `forceLinkWholeForHaskellOmnibus` in
                interface `NativeLinkable`

        []{#getBuildTarget()}

        -   #### getBuildTarget

            ``` methodSignature
            public BuildTarget getBuildTarget()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getBuildTarget` in interface `NativeLinkable`

            [Returns:]{.returnLabel}
            :   The
                [`BuildTarget`](../../../core/model/BuildTarget.html "class in com.facebook.buck.core.model")
                for this linkable.

        []{#getNativeLinkableDeps(com.facebook.buck.core.rules.ActionGraphBuilder)}

        -   #### getNativeLinkableDeps

            ``` methodSignature
            public Iterable<? extends NativeLinkable> getNativeLinkableDeps​(ActionGraphBuilder graphBuilder)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getNativeLinkableDeps` in interface `NativeLinkable`

            [Returns:]{.returnLabel}
            :   All native linkable dependencies that might be required
                by this linkable.

        []{#getNativeLinkableExportedDeps(com.facebook.buck.core.rules.ActionGraphBuilder)}

        -   #### getNativeLinkableExportedDeps

            ``` methodSignature
            public Iterable<? extends NativeLinkable> getNativeLinkableExportedDeps​(ActionGraphBuilder graphBuilder)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getNativeLinkableExportedDeps` in
                interface `NativeLinkable`

            [Returns:]{.returnLabel}
            :   All native linkable exported dependencies that might be
                required by this linkable.

        []{#getNativeLinkableInput(com.facebook.buck.cxx.toolchain.linker.Linker.LinkableDepType,boolean,com.facebook.buck.core.rules.ActionGraphBuilder,com.facebook.buck.core.model.TargetConfiguration)}

        -   #### getNativeLinkableInput

            ``` methodSignature
            public NativeLinkableInput getNativeLinkableInput​(Linker.LinkableDepType type,
                                                              boolean forceLinkWhole,
                                                              ActionGraphBuilder graphBuilder,
                                                              TargetConfiguration targetConfiguration)
            ```

            ::: block
            [Description copied from
            interface: `NativeLinkable`]{.descfrmTypeLabel}
            :::

            ::: block
            Return input that \*dependents\* should put on their link
            line when linking against this linkable.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getNativeLinkableInput` in interface `NativeLinkable`

        []{#getNativeLinkTarget(com.facebook.buck.core.rules.ActionGraphBuilder,boolean)}

        -   #### getNativeLinkTarget

            ``` methodSignature
            public Optional<NativeLinkTarget> getNativeLinkTarget​(ActionGraphBuilder graphBuilder,
                                                                  boolean includePrivateLinkerFlags)
            ```

            ::: block
            [Description copied from
            interface: `NativeLinkable`]{.descfrmTypeLabel}
            :::

            ::: block
            Optionally returns a
            [`NativeLinkTarget`](NativeLinkTarget.html "interface in com.facebook.buck.cxx.toolchain.nativelink").
            Most implementations of NativeLinkable are themselves
            instances of NativeLinkTarget.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getNativeLinkTarget` in interface `NativeLinkable`
            :   `includePrivateLinkerFlags` - whether to include
                rule-specific non-exported linker flags.

        []{#getPreferredLinkage()}

        -   #### getPreferredLinkage

            ``` methodSignature
            public NativeLinkableGroup.Linkage getPreferredLinkage()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getPreferredLinkage` in interface `NativeLinkable`

            [Returns:]{.returnLabel}
            :   The preferred
                [`NativeLinkableGroup.Linkage`](NativeLinkableGroup.Linkage.html "enum in com.facebook.buck.cxx.toolchain.nativelink")
                for this linkable.

        []{#getSharedLibraries(com.facebook.buck.core.rules.ActionGraphBuilder)}

        -   #### getSharedLibraries

            ``` methodSignature
            public com.google.common.collect.ImmutableMap<String,​SourcePath> getSharedLibraries​(ActionGraphBuilder graphBuilder)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getSharedLibraries` in interface `NativeLinkable`

            [Returns:]{.returnLabel}
            :   a map of shared library SONAME to shared library path
                for the given
                [`CxxPlatform`](../CxxPlatform.html "interface in com.facebook.buck.cxx.toolchain").

        []{#getExportedLinkerFlags(com.facebook.buck.core.rules.ActionGraphBuilder)}

        -   #### getExportedLinkerFlags

            ``` methodSignature
            public Iterable<? extends Arg> getExportedLinkerFlags​(ActionGraphBuilder graphBuilder)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getExportedLinkerFlags` in interface `NativeLinkable`

            [Returns:]{.returnLabel}
            :   exported linker flags. These should be added to link
                lines of dependents.

        []{#getExportedPostLinkerFlags(com.facebook.buck.core.rules.ActionGraphBuilder)}

        -   #### getExportedPostLinkerFlags

            ``` methodSignature
            public Iterable<? extends Arg> getExportedPostLinkerFlags​(ActionGraphBuilder graphBuilder)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getExportedPostLinkerFlags` in
                interface `NativeLinkable`

            [Returns:]{.returnLabel}
            :   exported post-linker flags. This should be added to
                lines of dependents after other linker flags.

        []{#shouldBeLinkedInAppleTestAndHost()}

        -   #### shouldBeLinkedInAppleTestAndHost

            ``` methodSignature
            public boolean shouldBeLinkedInAppleTestAndHost()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `shouldBeLinkedInAppleTestAndHost` in
                interface `NativeLinkable`
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
