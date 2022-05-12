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
[Package]{.packageLabelInType} [com.facebook.buck.jvm.java](package-summary.html)
:::

## Interface JavacPluginArgs {#interface-javacpluginargs .title title="Interface JavacPluginArgs"}
:::

::: contentContainer
::: description
-   

    All Superinterfaces:
    :   `BuildRuleArg`, `ConstructorArg`, `DataTransferObject`,
        `HasDeclaredDeps`

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `JavaAnnotationProcessorDescriptionArg`,
        `JavaPluginDescriptionArg`

    ------------------------------------------------------------------------

        public interface JavacPluginArgs
        extends BuildRuleArg, HasDeclaredDeps

    ::: block
    Constructor arg of javac plugin rule
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

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `default boolean`     | `                     | ::: block             |
        |                       | isDoesNotAffectAbi()` | A value of false      |
        |                       |                       | indicates that the    |
        |                       |                       | plugin either         |
        |                       |                       | generates classes     |
        |                       |                       | that are intended for |
        |                       |                       | use outside of the    |
        |                       |                       | code being processed  |
        |                       |                       | or modifies bytecode  |
        |                       |                       | in a way that         |
        |                       |                       | modifies ABI.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `default boolean`     | `is                   | ::: block             |
        |                       | IsolateClassLoader()` | A value of false      |
        |                       |                       | indicates that the    |
        |                       |                       | plugin will not use a |
        |                       |                       | shared class loader   |
        |                       |                       | to be loaded.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `default boolean`     | `isSupportsAbiGe      | ::: block             |
        |                       | nerationFromSource()` | If true, allows       |
        |                       |                       | ABI-affecting plugins |
        |                       |                       | to run during ABI     |
        |                       |                       | generation from       |
        |                       |                       | source.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
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
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#isIsolateClassLoader()}

        -   #### isIsolateClassLoader

            ``` methodSignature
            @Default
            default boolean isIsolateClassLoader()
            ```

            ::: block
            A value of false indicates that the plugin will not use a
            shared class loader to be loaded. This should be true if the
            same instance of the plugin has not support to run
            concurrently multiple times for different javac calls.
            Defaults to false because that\'s the \"safe\" value and
            optimizes build time.
            :::

        []{#isDoesNotAffectAbi()}

        -   #### isDoesNotAffectAbi

            ``` methodSignature
            @Default
            default boolean isDoesNotAffectAbi()
            ```

            ::: block
            A value of false indicates that the plugin either generates
            classes that are intended for use outside of the code being
            processed or modifies bytecode in a way that modifies ABI.
            Plugins that affect the ABI of the rule in which they run
            must be run during ABI generation from source.
            Defaults to false because that\'s the \"safe\" value. When
            migrating to ABI generation from source, having as few
            ABI-affecting plugins as possible will yield the fastest ABI
            generation.
            :::

        []{#isSupportsAbiGenerationFromSource()}

        -   #### isSupportsAbiGenerationFromSource

            ``` methodSignature
            @Default
            default boolean isSupportsAbiGenerationFromSource()
            ```

            ::: block
            If true, allows ABI-affecting plugins to run during ABI
            generation from source. To run during ABI generation from
            source, a plugin must meet all of the following criteria:

            ```{=html}
            <!-- -->
            ```

            Defaults to false because that\'s the \"safe\" value. When
            migrating to ABI generation from source, having as many
            ABI-affecting plugins as possible running during ABI
            generation will result in the flattest build graph.
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
