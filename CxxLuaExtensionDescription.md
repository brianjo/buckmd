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

## Class CxxLuaExtensionDescription {#class-cxxluaextensiondescription .title title="Class CxxLuaExtensionDescription"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.features.lua.CxxLuaExtensionDescription

::: description
-   

    All Implemented Interfaces:
    :   `ImplicitDepsInferringDescription<com.facebook.buck.features.lua.CxxLuaExtensionDescription.AbstractCxxLuaExtensionDescriptionArg>`,
        `BaseDescription<CxxLuaExtensionDescriptionArg>`,
        `Description<CxxLuaExtensionDescriptionArg>`, `Flavored`,
        `DescriptionWithTargetGraph<CxxLuaExtensionDescriptionArg>`,
        `VersionPropagator<CxxLuaExtensionDescriptionArg>`

    ------------------------------------------------------------------------

        public class CxxLuaExtensionDescription
        extends Object
        implements DescriptionWithTargetGraph<CxxLuaExtensionDescriptionArg>, ImplicitDepsInferringDescription<com.facebook.buck.features.lua.CxxLuaExtensionDescription.AbstractCxxLuaExtensionDescriptionArg>, VersionPropagator<CxxLuaExtensionDescriptionArg>, Flavored
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                Description
          -------------------------------------------------------------------------------------------------------------------------- -------------
          `CxxLuaExtensionDescription​(ToolchainProvider toolchainProvider,                           CxxBuckConfig cxxBuckConfig)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `BuildRule`           | `create               | ::: block             |
        |                       | BuildRule​(BuildRuleCr | Create a              |
        |                       | eationContextWithTarg | [`Buil                |
        |                       | etGraph context,      | dRule`](../../core/ru |
        |                       |            BuildTarge | les/BuildRule.html "i |
        |                       | t buildTarget,        | nterface in com.faceb |
        |                       |          BuildRulePar | ook.buck.core.rules") |
        |                       | ams params,           | for the given         |
        |                       |       CxxLuaExtension | [`BuildRulePara       |
        |                       | DescriptionArg args)` | ms`](../../core/rules |
        |                       |                       | /BuildRuleParams.html |
        |                       |                       |  "class in com.facebo |
        |                       |                       | ok.buck.core.rules"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `f                    |                       |
        |                       | indDepsForTargetFromC |                       |
        |                       | onstructorArgs​(BuildT |                       |
        |                       | arget buildTarget,    |                       |
        |                       |                       |                       |
        |                       |              CellName |                       |
        |                       | Resolver cellRoots,   |                       |
        |                       |                       |                       |
        |                       |               com.fac |                       |
        |                       | ebook.buck.features.l |                       |
        |                       | ua.CxxLuaExtensionDes |                       |
        |                       | cription.AbstractCxxL |                       |
        |                       | uaExtensionDescriptio |                       |
        |                       | nArg constructorArg,  |                       |
        |                       |                       |                       |
        |                       |                com.go |                       |
        |                       | ogle.common.collect.I |                       |
        |                       | mmutableCollection.Bu |                       |
        |                       | ilder<BuildTarget> ex |                       |
        |                       | traDepsBuilder,       |                       |
        |                       |                       |                       |
        |                       |           com.google. |                       |
        |                       | common.collect.Immuta |                       |
        |                       | bleCollection.Builder |                       |
        |                       | <BuildTarget> targetG |                       |
        |                       | raphOnlyDepsBuilder)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Opt                  | `f                    |                       |
        | ional<com.google.comm | lavorDomains​(TargetCo |                       |
        | on.collect.ImmutableS | nfiguration toolchain |                       |
        | et<FlavorDomain<?>>>` | TargetConfiguration)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Class<CxxLuaExte     | `get                  | ::: block             |
        | nsionDescriptionArg>` | ConstructorArgType()` | The type of the       |
        |                       |                       | constructor argument  |
        |                       |                       | that is used by this  |
        |                       |                       | description to create |
        |                       |                       | a rule                |
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
        -   []{#methods.inherited.from.class.com.facebook.buck.core.description.BaseDescription}

            ### Methods inherited from interface com.facebook.buck.core.description.[BaseDescription](../../core/description/BaseDescription.html "interface in com.facebook.buck.core.description")

            `getConfigurationDeps`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.DescriptionWithTargetGraph}

            ### Methods inherited from interface com.facebook.buck.core.rules.[DescriptionWithTargetGraph](../../core/rules/DescriptionWithTargetGraph.html "interface in com.facebook.buck.core.rules")

            `producesCacheableSubgraph`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.model.Flavored}

            ### Methods inherited from interface com.facebook.buck.core.model.[Flavored](../../core/model/Flavored.html "interface in com.facebook.buck.core.model")

            `hasFlavors`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.core.toolchain.ToolchainProvider,com.facebook.buck.cxx.config.CxxBuckConfig)}

        -   #### CxxLuaExtensionDescription

                public CxxLuaExtensionDescription​(ToolchainProvider toolchainProvider,
                                                  CxxBuckConfig cxxBuckConfig)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getConstructorArgType()}

        -   #### getConstructorArgType

            ``` methodSignature
            public Class<CxxLuaExtensionDescriptionArg> getConstructorArgType()
            ```

            ::: block
            [Description copied from
            interface: `BaseDescription`]{.descfrmTypeLabel}
            :::

            ::: block
            The type of the constructor argument that is used by this
            description to create a rule
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getConstructorArgType` in
                interface `BaseDescription<CxxLuaExtensionDescriptionArg>`

        []{#createBuildRule(com.facebook.buck.core.rules.BuildRuleCreationContextWithTargetGraph,com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.rules.BuildRuleParams,com.facebook.buck.features.lua.CxxLuaExtensionDescriptionArg)}

        -   #### createBuildRule

            ``` methodSignature
            public BuildRule createBuildRule​(BuildRuleCreationContextWithTargetGraph context,
                                             BuildTarget buildTarget,
                                             BuildRuleParams params,
                                             CxxLuaExtensionDescriptionArg args)
            ```

            ::: block
            [Description copied from
            interface: `DescriptionWithTargetGraph`]{.descfrmTypeLabel}
            :::

            ::: block
            Create a
            [`BuildRule`](../../core/rules/BuildRule.html "interface in com.facebook.buck.core.rules")
            for the given
            [`BuildRuleParams`](../../core/rules/BuildRuleParams.html "class in com.facebook.buck.core.rules").
            Note that the
            [`BuildTarget`](../../core/model/BuildTarget.html "class in com.facebook.buck.core.model")
            referred to in the `params` contains the
            [`Flavor`](../../core/model/Flavor.html "interface in com.facebook.buck.core.model")
            to create.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `createBuildRule` in
                interface `DescriptionWithTargetGraph<CxxLuaExtensionDescriptionArg>`
            :   `args` - A constructor argument, of type as returned by
                [`BaseDescription.getConstructorArgType()`](../../core/description/BaseDescription.html#getConstructorArgType()).

            [Returns:]{.returnLabel}
            :   The
                [`BuildRule`](../../core/rules/BuildRule.html "interface in com.facebook.buck.core.rules")
                that describes the default flavour of the rule being
                described.

        []{#findDepsForTargetFromConstructorArgs(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.cell.nameresolver.CellNameResolver,com.facebook.buck.features.lua.CxxLuaExtensionDescription.AbstractCxxLuaExtensionDescriptionArg,com.google.common.collect.ImmutableCollection.Builder,com.google.common.collect.ImmutableCollection.Builder)}

        -   #### findDepsForTargetFromConstructorArgs

            ``` methodSignature
            public void findDepsForTargetFromConstructorArgs​(BuildTarget buildTarget,
                                                             CellNameResolver cellRoots,
                                                             com.facebook.buck.features.lua.CxxLuaExtensionDescription.AbstractCxxLuaExtensionDescriptionArg constructorArg,
                                                             com.google.common.collect.ImmutableCollection.Builder<BuildTarget> extraDepsBuilder,
                                                             com.google.common.collect.ImmutableCollection.Builder<BuildTarget> targetGraphOnlyDepsBuilder)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `findDepsForTargetFromConstructorArgs` in
                interface `ImplicitDepsInferringDescription<com.facebook.buck.features.lua.CxxLuaExtensionDescription.AbstractCxxLuaExtensionDescriptionArg>`

        []{#flavorDomains(com.facebook.buck.core.model.TargetConfiguration)}

        -   #### flavorDomains

            ``` methodSignature
            public Optional<com.google.common.collect.ImmutableSet<FlavorDomain<?>>> flavorDomains​(TargetConfiguration toolchainTargetConfiguration)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `flavorDomains` in interface `Flavored`
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
