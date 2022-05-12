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

-   [Overview](../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../deprecated-list.html)
-   [Index](../../../../index-all.html)
-   [Help](../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.shell](package-summary.html)
:::

## Interface AbstractGenruleDescription.CommonArg {#interface-abstractgenruledescription.commonarg .title title="Interface AbstractGenruleDescription.CommonArg"}
:::

::: contentContainer
::: description
-   

    All Superinterfaces:
    :   `BuildRuleArg`, `ConstructorArg`, `DataTransferObject`,
        `HasTests`

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `ApkGenruleDescriptionArg`, `CxxGenruleDescriptionArg`,
        `GenruleDescriptionArg`, `JarGenruleDescriptionArg`,
        `JsBundleGenruleDescriptionArg`

    ```{=html}
    <!-- -->
    ```

    Enclosing class:
    :   [AbstractGenruleDescription](AbstractGenruleDescription.html "class in com.facebook.buck.shell")\<[T](AbstractGenruleDescription.html "type parameter in AbstractGenruleDescription")
        extends
        [AbstractGenruleDescription.CommonArg](AbstractGenruleDescription.CommonArg.html "interface in com.facebook.buck.shell")\>

    ------------------------------------------------------------------------

        public static interface AbstractGenruleDescription.CommonArg
        extends BuildRuleArg, HasTests
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        -   []{#fields.inherited.from.class.com.facebook.buck.core.description.arg.BuildRuleArg}

            ### Fields inherited from interface com.facebook.buck.core.description.arg.[BuildRuleArg](../core/description/arg/BuildRuleArg.html "interface in com.facebook.buck.core.description.arg")

            `DEFAULT_TARGET_PLATFORM_PARAM_NAME`
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `Option               | `getBash()`           |                       |
        | al<StringWithMacros>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Boolean>`   | `getCacheable()`      | ::: block             |
        |                       |                       | This functionality    |
        |                       |                       | only exists to get    |
        |                       |                       | around the lack of    |
        |                       |                       | extensibility in our  |
        |                       |                       | current build rule /  |
        |                       |                       | build file apis.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Option               | `getCmd()`            |                       |
        | al<StringWithMacros>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Option               | `getCmdExe()`         |                       |
        | al<StringWithMacros>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Boolean>`   | `getEnableSandbox()`  |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `getEnvironment       |                       |
        |                       | ExpansionSeparator()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Boolean>`   | `getRemote()`         | ::: block             |
        |                       |                       | If present and true,  |
        |                       |                       | requests that Buck    |
        |                       |                       | run this genrule      |
        |                       |                       | remotely if possible. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `default SourceSet`   | `getSrcs()`           |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `getType()`           |                       |
        +-----------------------+-----------------------+-----------------------+
        | `default boolean`     | `                     | ::: block             |
        |                       | isNeedAndroidTools()` | This argument allows  |
        |                       |                       | genrule to specify if |
        |                       |                       | it needs android      |
        |                       |                       | tools (like dex,      |
        |                       |                       | aapt, ndk, sdk).      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
        .tableTab}[[Default
        Methods](javascript:show(16);)[ ]{.tabEnd}]{#t5 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.core.description.arg.BuildRuleArg}

            ### Methods inherited from interface com.facebook.buck.core.description.arg.[BuildRuleArg](../core/description/arg/BuildRuleArg.html "interface in com.facebook.buck.core.description.arg")

            `getCompatibleWith, getDefaultTargetPlatform, getLabels, getLicenses, labelsContainsAnyOf`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.description.arg.ConstructorArg}

            ### Methods inherited from interface com.facebook.buck.core.description.arg.[ConstructorArg](../core/description/arg/ConstructorArg.html "interface in com.facebook.buck.core.description.arg")

            `getName`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.description.arg.HasTests}

            ### Methods inherited from interface com.facebook.buck.core.description.arg.[HasTests](../core/description/arg/HasTests.html "interface in com.facebook.buck.core.description.arg")

            `getTests`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getBash()}

        -   #### getBash

            ``` methodSignature
            Optional<StringWithMacros> getBash()
            ```

        []{#getCmd()}

        -   #### getCmd

            ``` methodSignature
            Optional<StringWithMacros> getCmd()
            ```

        []{#getCmdExe()}

        -   #### getCmdExe

            ``` methodSignature
            Optional<StringWithMacros> getCmdExe()
            ```

        []{#getType()}

        -   #### getType

            ``` methodSignature
            Optional<String> getType()
            ```

        []{#getSrcs()}

        -   #### getSrcs

            ``` methodSignature
            @Default
            default SourceSet getSrcs()
            ```

        []{#getEnableSandbox()}

        -   #### getEnableSandbox

            ``` methodSignature
            Optional<Boolean> getEnableSandbox()
            ```

        []{#getEnvironmentExpansionSeparator()}

        -   #### getEnvironmentExpansionSeparator

            ``` methodSignature
            Optional<String> getEnvironmentExpansionSeparator()
            ```

        []{#getRemote()}

        -   #### getRemote

            ``` methodSignature
            Optional<Boolean> getRemote()
            ```

            ::: block
            If present and true, requests that Buck run this genrule
            remotely if possible. Defaults to false for now.
            :::

        []{#getCacheable()}

        -   #### getCacheable

            ``` methodSignature
            Optional<Boolean> getCacheable()
            ```

            ::: block
            This functionality only exists to get around the lack of
            extensibility in our current build rule / build file apis.
            It may go away at some point. Also, make sure that you
            understand what
            [`BuildRule.isCacheable()`](../core/rules/BuildRule.html#isCacheable())
            does with respect to caching if you decide to use this
            attribute
            :::

        []{#isNeedAndroidTools()}

        -   #### isNeedAndroidTools

            ``` methodSignature
            @Default
            default boolean isNeedAndroidTools()
            ```

            ::: block
            This argument allows genrule to specify if it needs android
            tools (like dex, aapt, ndk, sdk).
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

-   [Overview](../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../deprecated-list.html)
-   [Index](../../../../index-all.html)
-   [Help](../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../allclasses.html)

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
