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
-   [Field](#field.summary) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.cxx.toolchain](package-summary.html)
:::

## Interface HasSystemFrameworkAndLibraries {#interface-hassystemframeworkandlibraries .title title="Interface HasSystemFrameworkAndLibraries"}
:::

::: contentContainer
::: description
-   

    All Superinterfaces:
    :   `BuildRuleArg`, `ConstructorArg`, `DataTransferObject`

    ```{=html}
    <!-- -->
    ```

    All Known Subinterfaces:
    :   `AppleNativeTargetDescriptionArg`,
        `CxxBinaryDescription.CommonArg`, `CxxConstructorArg`,
        `CxxLibraryDescription.CommonArg`, `LinkableCxxConstructorArg`

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `AppleBinaryDescriptionArg`, `AppleLibraryDescriptionArg`,
        `AppleTestDescriptionArg`, `CgoLibraryDescriptionArg`,
        `CxxBinaryDescriptionArg`, `CxxLibraryDescriptionArg`,
        `CxxLuaExtensionDescriptionArg`,
        `CxxPythonExtensionDescriptionArg`, `CxxTestDescriptionArg`,
        `HalideLibraryDescriptionArg`,
        `PrebuiltAppleFrameworkDescriptionArg`

    ------------------------------------------------------------------------

        public interface HasSystemFrameworkAndLibraries
        extends BuildRuleArg

    ::: block
    Constructor args which specify system framework and library fields.
    E.g. fields with members in the form of
    `$SDKROOT/user/lib/libz.dylib` or
    `  $SDKROOT/System/Library/Frameworks/Foundation.framework`.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        -   []{#fields.inherited.from.class.com.facebook.buck.core.description.arg.BuildRuleArg}

            ### Fields inherited from interface com.facebook.buck.core.description.arg.[BuildRuleArg](../../core/description/arg/BuildRuleArg.html "interface in com.facebook.buck.core.description.arg")

            `DEFAULT_TARGET_PLATFORM_PARAM_NAME`
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                               Method              Description
          --------------------------------------------------------------- ------------------- -------------
          `com.google.common.collect.ImmutableSortedSet<FrameworkPath>`   `getFrameworks()`    
          `com.google.common.collect.ImmutableSortedSet<FrameworkPath>`   `getLibraries()`     

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Abstract
          Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.core.description.arg.BuildRuleArg}

            ### Methods inherited from interface com.facebook.buck.core.description.arg.[BuildRuleArg](../../core/description/arg/BuildRuleArg.html "interface in com.facebook.buck.core.description.arg")

            `getCompatibleWith, getDefaultTargetPlatform, getLabels, getLicenses, labelsContainsAnyOf`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.description.arg.ConstructorArg}

            ### Methods inherited from interface com.facebook.buck.core.description.arg.[ConstructorArg](../../core/description/arg/ConstructorArg.html "interface in com.facebook.buck.core.description.arg")

            `getName`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getFrameworks()}

        -   #### getFrameworks

            ``` methodSignature
            @NaturalOrder
            com.google.common.collect.ImmutableSortedSet<FrameworkPath> getFrameworks()
            ```

        []{#getLibraries()}

        -   #### getLibraries

            ``` methodSignature
            @NaturalOrder
            com.google.common.collect.ImmutableSortedSet<FrameworkPath> getLibraries()
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
-   [Field](#field.summary) \| 
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
