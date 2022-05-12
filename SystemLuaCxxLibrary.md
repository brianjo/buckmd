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
[Package]{.packageLabelInType} [com.facebook.buck.features.lua](package-summary.html)
:::

## Class SystemLuaCxxLibrary {#class-systemluacxxlibrary .title title="Class SystemLuaCxxLibrary"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.features.lua.SystemLuaCxxLibrary

::: description
-   

    All Implemented Interfaces:
    :   `AndroidPackageable`, `AbstractCxxLibraryGroup`,
        `CxxPreprocessorDep`, `NativeLinkableGroup`

    ------------------------------------------------------------------------

        public class SystemLuaCxxLibrary
        extends Object
        implements AbstractCxxLibraryGroup, NativeLinkableGroup

    ::: block
    Represents the system lua c++ library.
    :::
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

          Constructor                                 Description
          ------------------------------------------- -------------
          `SystemLuaCxxLibrary​(BuildTarget target)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `void`                | `addToCollect         | ::: block             |
        |                       | or​(AndroidPackageable | Add concrete          |
        |                       | Collector collector)` | resources to the      |
        |                       |                       | given collector.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `BuildTarget`         | `getBuildTarget()`    |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Iterable             | `getCxxPreprocessor   |                       |
        | <CxxPreprocessorDep>` | Deps​(CxxPlatform cxxP |                       |
        |                       | latform,              |                       |
        |                       |           BuildRuleRe |                       |
        |                       | solver ruleResolver)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `                     | ::: block             |
        | CxxPreprocessorInput` | getCxxPreprocessorInp | Returns the           |
        |                       | ut​(CxxPlatform cxxPla | preprocessor input    |
        |                       | tform,                | that represents this  |
        |                       |          ActionGraphB | rule\'s public        |
        |                       | uilder graphBuilder)` | (exported)            |
        |                       |                       | declarations.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `NativeLinkable`      | `getNative            |                       |
        |                       | Linkable​(CxxPlatform  |                       |
        |                       | cxxPlatform,          |                       |
        |                       |          ActionGraphB |                       |
        |                       | uilder graphBuilder)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Iterable             | `getRequiredPac       | ::: block             |
        | <AndroidPackageable>` | kageables​(BuildRuleRe | Get the set of        |
        |                       | solver ruleResolver)` | packagables that need |
        |                       |                       | to be included in any |
        |                       |                       | package that includes |
        |                       |                       | this object.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.google           | `getTransitiveCxxPrep | ::: block             |
        | .common.collect.Immut | rocessorInput​(CxxPlat | Returns all           |
        | ableMap<BuildTarget,​C | form cxxPlatform,     | transitive            |
        | xxPreprocessorInput>` |                       | preprocessor inputs   |
        |                       |          ActionGraphB | for this library.     |
        |                       | uilder graphBuilder)` | :::                   |
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

        []{#<init>(com.facebook.buck.core.model.BuildTarget)}

        -   #### SystemLuaCxxLibrary

                public SystemLuaCxxLibrary​(BuildTarget target)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getBuildTarget()}

        -   #### getBuildTarget

            ``` methodSignature
            public BuildTarget getBuildTarget()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getBuildTarget` in interface `CxxPreprocessorDep`

            [Specified by:]{.overrideSpecifyLabel}
            :   `getBuildTarget` in interface `NativeLinkableGroup`

        []{#getRequiredPackageables(com.facebook.buck.core.rules.BuildRuleResolver)}

        -   #### getRequiredPackageables

            ``` methodSignature
            public Iterable<AndroidPackageable> getRequiredPackageables​(BuildRuleResolver ruleResolver)
            ```

            ::: block
            [Description copied from
            interface: `AndroidPackageable`]{.descfrmTypeLabel}
            :::

            ::: block
            Get the set of packagables that need to be included in any
            package that includes this object.
            For example, an android_library will need all of its Java
            deps (except provided_deps), its resource deps, and its
            native library deps (even though it doesn\'t need the native
            library as a build-time dependency). An android_resource
            might need an android_library that declares a custom view
            that it references, as well as other android_resource rules
            that it references directly.

            TODO(natthu): Once build rules and buildables are merged,
            replace this method with another interface that lets an
            [`AndroidPackageable`](../../android/packageable/AndroidPackageable.html "interface in com.facebook.buck.android.packageable")
            override the default set which is all deps of the type
            [`AndroidPackageable`](../../android/packageable/AndroidPackageable.html "interface in com.facebook.buck.android.packageable").
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getRequiredPackageables` in
                interface `AndroidPackageable`

            [Returns:]{.returnLabel}
            :   All
                [`AndroidPackageable`](../../android/packageable/AndroidPackageable.html "interface in com.facebook.buck.android.packageable")s
                that must be included along with this one.

        []{#addToCollector(com.facebook.buck.android.packageable.AndroidPackageableCollector)}

        -   #### addToCollector

            ``` methodSignature
            public void addToCollector​(AndroidPackageableCollector collector)
            ```

            ::: block
            [Description copied from
            interface: `AndroidPackageable`]{.descfrmTypeLabel}
            :::

            ::: block
            Add concrete resources to the given collector.
            Implementations should call methods on the collector specify
            what concrete content must be included in an Android package
            that includes this object. For example, an android_library
            will add Java classes, an ndk_library will add native
            libraries, and android_resource will add resource
            directories.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `addToCollector` in interface `AndroidPackageable`

            [Parameters:]{.paramLabel}
            :   `collector` - The
                [`AndroidPackageableCollector`](../../android/packageable/AndroidPackageableCollector.html "class in com.facebook.buck.android.packageable")
                that will receive the content.

        []{#getCxxPreprocessorDeps(com.facebook.buck.cxx.toolchain.CxxPlatform,com.facebook.buck.core.rules.BuildRuleResolver)}

        -   #### getCxxPreprocessorDeps

            ``` methodSignature
            public Iterable<CxxPreprocessorDep> getCxxPreprocessorDeps​(CxxPlatform cxxPlatform,
                                                                       BuildRuleResolver ruleResolver)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getCxxPreprocessorDeps` in
                interface `CxxPreprocessorDep`

        []{#getCxxPreprocessorInput(com.facebook.buck.cxx.toolchain.CxxPlatform,com.facebook.buck.core.rules.ActionGraphBuilder)}

        -   #### getCxxPreprocessorInput

            ``` methodSignature
            public CxxPreprocessorInput getCxxPreprocessorInput​(CxxPlatform cxxPlatform,
                                                                ActionGraphBuilder graphBuilder)
            ```

            ::: block
            [Description copied from
            interface: `CxxPreprocessorDep`]{.descfrmTypeLabel}
            :::

            ::: block
            Returns the preprocessor input that represents this rule\'s
            public (exported) declarations. This includes any exported
            preprocessor flags, headers, etc.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getCxxPreprocessorInput` in
                interface `CxxPreprocessorDep`

        []{#getTransitiveCxxPreprocessorInput(com.facebook.buck.cxx.toolchain.CxxPlatform,com.facebook.buck.core.rules.ActionGraphBuilder)}

        -   #### getTransitiveCxxPreprocessorInput

            ``` methodSignature
            public com.google.common.collect.ImmutableMap<BuildTarget,​CxxPreprocessorInput> getTransitiveCxxPreprocessorInput​(CxxPlatform cxxPlatform,
                                                                                                                                    ActionGraphBuilder graphBuilder)
            ```

            ::: block
            [Description copied from
            interface: `CxxPreprocessorDep`]{.descfrmTypeLabel}
            :::

            ::: block
            Returns all transitive preprocessor inputs for this library.
            This includes public headers (and exported preprocessor
            flags) of all exported dependencies.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getTransitiveCxxPreprocessorInput` in
                interface `CxxPreprocessorDep`

        []{#getNativeLinkable(com.facebook.buck.cxx.toolchain.CxxPlatform,com.facebook.buck.core.rules.ActionGraphBuilder)}

        -   #### getNativeLinkable

            ``` methodSignature
            public NativeLinkable getNativeLinkable​(CxxPlatform cxxPlatform,
                                                    ActionGraphBuilder graphBuilder)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getNativeLinkable` in interface `NativeLinkableGroup`
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
