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
[Package]{.packageLabelInType} [com.facebook.buck.features.rust](package-summary.html)
:::

## Interface RustCommonArgs {#interface-rustcommonargs .title title="Interface RustCommonArgs"}
:::

::: contentContainer
::: description
-   

    All Superinterfaces:
    :   `BuildRuleArg`, `ConstructorArg`, `DataTransferObject`,
        `HasDeclaredDeps`, `HasDefaultPlatform`, `HasNamedDeclaredDeps`,
        `HasSrcs`

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `RustBinaryDescriptionArg`, `RustLibraryDescriptionArg`,
        `RustTestDescriptionArg`

    ------------------------------------------------------------------------

        public interface RustCommonArgs
        extends BuildRuleArg, HasNamedDeclaredDeps, HasSrcs, HasDefaultPlatform
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

          Modifier and Type                                                                               Method                Description
          ----------------------------------------------------------------------------------------------- --------------------- -------------
          `Optional<String>`                                                                              `getCrate()`           
          `Optional<String>`                                                                              `getCrateRoot()`       
          `Optional<String>`                                                                              `getEdition()`         
          `com.google.common.collect.ImmutableSortedMap<String,​StringWithMacros>`                         `getEnv()`             
          `com.google.common.collect.ImmutableSortedSet<String>`                                          `getFeatures()`        
          `com.google.common.collect.ImmutableSortedMap<SourcePath,​String>`                               `getMappedSrcs()`      
          `default PatternMatchedCollection<com.google.common.collect.ImmutableSortedSet<BuildTarget>>`   `getPlatformDeps()`    
          `com.google.common.collect.ImmutableList<StringWithMacros>`                                     `getRustcFlags()`      

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Abstract
          Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
          .tableTab}[[Default
          Methods](javascript:show(16);)[ ]{.tabEnd}]{#t5 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.core.description.arg.BuildRuleArg}

            ### Methods inherited from interface com.facebook.buck.core.description.arg.[BuildRuleArg](../../core/description/arg/BuildRuleArg.html "interface in com.facebook.buck.core.description.arg")

            `getCompatibleWith, getDefaultTargetPlatform, getLabels, getLicenses, labelsContainsAnyOf`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.description.arg.ConstructorArg}

            ### Methods inherited from interface com.facebook.buck.core.description.arg.[ConstructorArg](../../core/description/arg/ConstructorArg.html "interface in com.facebook.buck.core.description.arg")

            `getName`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.description.arg.HasDeclaredDeps}

            ### Methods inherited from interface com.facebook.buck.core.description.arg.[HasDeclaredDeps](../../core/description/arg/HasDeclaredDeps.html "interface in com.facebook.buck.core.description.arg")

            `getDeps`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.description.arg.HasDefaultPlatform}

            ### Methods inherited from interface com.facebook.buck.core.description.arg.[HasDefaultPlatform](../../core/description/arg/HasDefaultPlatform.html "interface in com.facebook.buck.core.description.arg")

            `getDefaultPlatform`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.features.rust.HasNamedDeclaredDeps}

            ### Methods inherited from interface com.facebook.buck.features.rust.[HasNamedDeclaredDeps](HasNamedDeclaredDeps.html "interface in com.facebook.buck.features.rust")

            `getNamedDeps`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.description.arg.HasSrcs}

            ### Methods inherited from interface com.facebook.buck.core.description.arg.[HasSrcs](../../core/description/arg/HasSrcs.html "interface in com.facebook.buck.core.description.arg")

            `getSrcs`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getMappedSrcs()}

        -   #### getMappedSrcs

            ``` methodSignature
            @NaturalOrder
            com.google.common.collect.ImmutableSortedMap<SourcePath,​String> getMappedSrcs()
            ```

        []{#getEnv()}

        -   #### getEnv

            ``` methodSignature
            @NaturalOrder
            com.google.common.collect.ImmutableSortedMap<String,​StringWithMacros> getEnv()
            ```

        []{#getEdition()}

        -   #### getEdition

            ``` methodSignature
            Optional<String> getEdition()
            ```

        []{#getFeatures()}

        -   #### getFeatures

            ``` methodSignature
            @NaturalOrder
            com.google.common.collect.ImmutableSortedSet<String> getFeatures()
            ```

        []{#getRustcFlags()}

        -   #### getRustcFlags

            ``` methodSignature
            com.google.common.collect.ImmutableList<StringWithMacros> getRustcFlags()
            ```

        []{#getCrate()}

        -   #### getCrate

            ``` methodSignature
            Optional<String> getCrate()
            ```

        []{#getCrateRoot()}

        -   #### getCrateRoot

            ``` methodSignature
            Optional<String> getCrateRoot()
            ```

        []{#getPlatformDeps()}

        -   #### getPlatformDeps

            ``` methodSignature
            @Default
            default PatternMatchedCollection<com.google.common.collect.ImmutableSortedSet<BuildTarget>> getPlatformDeps()
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
