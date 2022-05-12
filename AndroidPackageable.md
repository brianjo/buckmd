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
[Package]{.packageLabelInType} [com.facebook.buck.android.packageable](package-summary.html)
:::

## Interface AndroidPackageable {#interface-androidpackageable .title title="Interface AndroidPackageable"}
:::

::: contentContainer
::: description
-   

    All Known Subinterfaces:
    :   `AbstractCxxLibraryGroup`

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `AndroidLibrary`, `AndroidPrebuiltAar`, `AndroidResource`,
        `CxxLibraryGroup`, `CxxPrecompiledHeaderTemplate`,
        `DefaultJavaLibrary`, `JsBundleAndroid`, `JsBundleGenrule`,
        `NdkLibrary`, `PrebuiltCxxLibrary`,
        `PrebuiltCxxLibraryGroupDescription.CustomPrebuiltCxxLibrary`,
        `PrebuiltJar`, `PrebuiltNativeLibrary`, `SystemLuaCxxLibrary`

    ------------------------------------------------------------------------

        public interface AndroidPackageable

    ::: block
    Something (usually a
    [`BuildRule`](../../core/rules/BuildRule.html "interface in com.facebook.buck.core.rules"))
    that can be included in an Android package (android_binary,
    cxx_library or android_prebuilt_aar).
    :::
:::

::: summary
-   ::: {.section role="region"}
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
        | `Iterable             | `getRequiredPac       | ::: block             |
        | <AndroidPackageable>` | kageables​(BuildRuleRe | Get the set of        |
        |                       | solver ruleResolver)` | packagables that need |
        |                       |                       | to be included in any |
        |                       |                       | package that includes |
        |                       |                       | this object.          |
        |                       |                       | :::                   |
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

        []{#getRequiredPackageables(com.facebook.buck.core.rules.BuildRuleResolver)}

        -   #### getRequiredPackageables

            ``` methodSignature
            Iterable<AndroidPackageable> getRequiredPackageables​(BuildRuleResolver ruleResolver)
            ```

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
            [`AndroidPackageable`](AndroidPackageable.html "interface in com.facebook.buck.android.packageable")
            override the default set which is all deps of the type
            [`AndroidPackageable`](AndroidPackageable.html "interface in com.facebook.buck.android.packageable").
            :::

            [Returns:]{.returnLabel}
            :   All
                [`AndroidPackageable`](AndroidPackageable.html "interface in com.facebook.buck.android.packageable")s
                that must be included along with this one.

        []{#addToCollector(com.facebook.buck.android.packageable.AndroidPackageableCollector)}

        -   #### addToCollector

            ``` methodSignature
            void addToCollector​(AndroidPackageableCollector collector)
            ```

            ::: block
            Add concrete resources to the given collector.
            Implementations should call methods on the collector specify
            what concrete content must be included in an Android package
            that includes this object. For example, an android_library
            will add Java classes, an ndk_library will add native
            libraries, and android_resource will add resource
            directories.
            :::

            [Parameters:]{.paramLabel}
            :   `collector` - The
                [`AndroidPackageableCollector`](AndroidPackageableCollector.html "class in com.facebook.buck.android.packageable")
                that will receive the content.
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
