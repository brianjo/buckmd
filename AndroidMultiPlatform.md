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
[Package]{.packageLabelInType} [com.facebook.buck.android.toolchain.platform](package-summary.html)
:::

## Class AndroidMultiPlatform {#class-androidmultiplatform .title title="Class AndroidMultiPlatform"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.android.toolchain.platform.AndroidMultiPlatform

::: description
-   

    All Implemented Interfaces:
    :   `MultiPlatform`, `NamedPlatform`, `Platform`

    ------------------------------------------------------------------------

        public class AndroidMultiPlatform
        extends Object
        implements MultiPlatform

    ::: block
    Android-specific implementation of multi-platform.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

        +-----------------------------------+-----------------------------------+
        | Constructor                       | Description                       |
        +===================================+===================================+
        | `An                               | ::: block                         |
        | droidMultiPlatform​(BuildTarget bu | Creates an instance of            |
        | ildTarget,                     Pl | [`Android                         |
        | atform basePlatform,              | MultiPlatform`](AndroidMultiPlatf |
        |         com.google.common.collect | orm.html "class in com.facebook.b |
        | .ImmutableSortedMap<TargetCpuType | uck.android.toolchain.platform"). |
        | ,​NamedPlatform> nestedPlatforms)` | :::                               |
        +-----------------------------------+-----------------------------------+

        : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `Platform`            | `getBasePlatform()`   | ::: block             |
        |                       |                       | Access base platform  |
        |                       |                       | of this platform, for |
        |                       |                       | example, CPU-neutral  |
        |                       |                       | Android platform      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `BuildTarget`         | `getBuildTarget()`    | ::: block             |
        |                       |                       | Build target used to  |
        |                       |                       | define this platform  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.common.c  | `                     | ::: block             |
        | ollect.ImmutableColle | getNestedPlatforms()` | Access nested         |
        | ction<NamedPlatform>` |                       | platforms, for        |
        |                       |                       | example, per-CPU      |
        |                       |                       | platforms for Android |
        |                       |                       | platform              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.          | `getNested            | ::: block             |
        | common.collect.Immuta | PlatformsByCpuType()` | Android platform is a |
        | bleSortedMap<TargetCp |                       | multiplatform which   |
        | uType,​NamedPlatform>` |                       | maps knows CPUs to    |
        |                       |                       | nested platforms.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.model.platform.MultiPlatform}

            ### Methods inherited from interface com.facebook.buck.core.model.platform.[MultiPlatform](../../../core/model/platform/MultiPlatform.html "interface in com.facebook.buck.core.model.platform")

            `matchesAll`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.model.platform.Platform,com.google.common.collect.ImmutableSortedMap)}

        -   #### AndroidMultiPlatform

                public AndroidMultiPlatform​(BuildTarget buildTarget,
                                            Platform basePlatform,
                                            com.google.common.collect.ImmutableSortedMap<TargetCpuType,​NamedPlatform> nestedPlatforms)

            ::: block
            Creates an instance of
            [`AndroidMultiPlatform`](AndroidMultiPlatform.html "class in com.facebook.buck.android.toolchain.platform").
            A multiplatform is a platform the has a base platform and
            multiple nested platforms. Base platform is the platform
            that is used in the context that expects a single platform.
            Nested platforms a handled by special logic in particular
            places. For example, when the same target needs to be built
            for every platform specified in nested platform the
            multiplatform is processed by duplicating targets with
            nested platforms in configurations.
            :::
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
            interface: `NamedPlatform`]{.descfrmTypeLabel}
            :::

            ::: block
            Build target used to define this platform
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getBuildTarget` in interface `NamedPlatform`

        []{#getBasePlatform()}

        -   #### getBasePlatform

            ``` methodSignature
            public Platform getBasePlatform()
            ```

            ::: block
            [Description copied from
            interface: `MultiPlatform`]{.descfrmTypeLabel}
            :::

            ::: block
            Access base platform of this platform, for example,
            CPU-neutral Android platform
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getBasePlatform` in interface `MultiPlatform`

        []{#getNestedPlatforms()}

        -   #### getNestedPlatforms

            ``` methodSignature
            public com.google.common.collect.ImmutableCollection<NamedPlatform> getNestedPlatforms()
            ```

            ::: block
            [Description copied from
            interface: `MultiPlatform`]{.descfrmTypeLabel}
            :::

            ::: block
            Access nested platforms, for example, per-CPU platforms for
            Android platform
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getNestedPlatforms` in interface `MultiPlatform`

        []{#getNestedPlatformsByCpuType()}

        -   #### getNestedPlatformsByCpuType

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedMap<TargetCpuType,​NamedPlatform> getNestedPlatformsByCpuType()
            ```

            ::: block
            Android platform is a multiplatform which maps knows CPUs to
            nested platforms. This functions returns that mapping.
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
