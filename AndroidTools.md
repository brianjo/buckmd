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
[Package]{.packageLabelInType} [com.facebook.buck.android.toolchain](package-summary.html)
:::

## Interface AndroidTools {#interface-androidtools .title title="Interface AndroidTools"}
:::

::: contentContainer
::: description
-   

    ------------------------------------------------------------------------

        public interface AndroidTools

    ::: block
    Represents different android tools
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static void`         | `addParseTimeDepsT    | ::: block             |
        |                       | oAndroidTools​(Toolcha | Adds parse time deps  |
        |                       | inProvider toolchainP | to android tools      |
        |                       | rovider,              | :::                   |
        |                       |                   Bui |                       |
        |                       | ldTarget buildTarget, |                       |
        |                       |                       |                       |
        |                       |           com.google. |                       |
        |                       | common.collect.Immuta |                       |
        |                       | bleCollection.Builder |                       |
        |                       | <BuildTarget> targetG |                       |
        |                       | raphOnlyDepsBuilder)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getAndroidNdk()`     |                       |
        | Optional<AndroidNdk>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `A                    | `getAnd               |                       |
        | ndroidPlatformTarget` | roidPlatformTarget()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidSdkLocation`  | `get                  |                       |
        |                       | AndroidSdkLocation()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static AndroidTools` | `getAndroidToo        | ::: block             |
        |                       | ls​(ToolchainProvider  | Returns               |
        |                       | toolchainProvider,    | `AndroidTools`        |
        |                       |              TargetCo | derived from a given  |
        |                       | nfiguration toolchain | `toolProvider`        |
        |                       | TargetConfiguration)` | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getAndroidPlatformTarget()}

        -   #### getAndroidPlatformTarget

            ``` methodSignature
            AndroidPlatformTarget getAndroidPlatformTarget()
            ```

        []{#getAndroidSdkLocation()}

        -   #### getAndroidSdkLocation

            ``` methodSignature
            AndroidSdkLocation getAndroidSdkLocation()
            ```

        []{#getAndroidNdk()}

        -   #### getAndroidNdk

            ``` methodSignature
            Optional<AndroidNdk> getAndroidNdk()
            ```

        []{#getAndroidTools(com.facebook.buck.core.toolchain.ToolchainProvider,com.facebook.buck.core.model.TargetConfiguration)}

        -   #### getAndroidTools

            ``` methodSignature
            static AndroidTools getAndroidTools​(ToolchainProvider toolchainProvider,
                                                TargetConfiguration toolchainTargetConfiguration)
            ```

            ::: block
            Returns `AndroidTools` derived from a given `toolProvider`
            :::

        []{#addParseTimeDepsToAndroidTools(com.facebook.buck.core.toolchain.ToolchainProvider,com.facebook.buck.core.model.BuildTarget,com.google.common.collect.ImmutableCollection.Builder)}

        -   #### addParseTimeDepsToAndroidTools

            ``` methodSignature
            static void addParseTimeDepsToAndroidTools​(ToolchainProvider toolchainProvider,
                                                       BuildTarget buildTarget,
                                                       com.google.common.collect.ImmutableCollection.Builder<BuildTarget> targetGraphOnlyDepsBuilder)
            ```

            ::: block
            Adds parse time deps to android tools
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
