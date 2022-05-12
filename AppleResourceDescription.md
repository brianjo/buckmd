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
[Package]{.packageLabelInType} [com.facebook.buck.apple](package-summary.html)
:::

## Class AppleResourceDescription {#class-appleresourcedescription .title title="Class AppleResourceDescription"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.apple.AppleResourceDescription

::: description
-   

    All Implemented Interfaces:
    :   `HasAppleBundleResourcesDescription<AppleResourceDescriptionArg>`,
        `BaseDescription<AppleResourceDescriptionArg>`,
        `Description<AppleResourceDescriptionArg>`, `Flavored`,
        `DescriptionWithTargetGraph<AppleResourceDescriptionArg>`

    ------------------------------------------------------------------------

        public class AppleResourceDescription
        extends Object
        implements DescriptionWithTargetGraph<AppleResourceDescriptionArg>, Flavored, HasAppleBundleResourcesDescription<AppleResourceDescriptionArg>

    ::: block
    Description for an apple_resource rule which copies resource files
    to the built bundle.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                    Description
          ------------------------------ -------------
          `AppleResourceDescription()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `void`                | `addAppleBu           |                       |
        |                       | ndleResources​(AppleBu |                       |
        |                       | ndleResources.Builder |                       |
        |                       |  builder,             |                       |
        |                       |             TargetNod |                       |
        |                       | e<AppleResourceDescri |                       |
        |                       | ptionArg> targetNode, |                       |
        |                       |                       |                       |
        |                       |    ProjectFilesystem  |                       |
        |                       | filesystem,           |                       |
        |                       |               BuildRu |                       |
        |                       | leResolver resolver)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `BuildRule`           | `crea                 | ::: block             |
        |                       | teBuildRule​(BuildRule | Create a              |
        |                       | CreationContextWithTa | [`B                   |
        |                       | rgetGraph context,    | uildRule`](../core/ru |
        |                       |              BuildTar | les/BuildRule.html "i |
        |                       | get buildTarget,      | nterface in com.faceb |
        |                       |            BuildRuleP | ook.buck.core.rules") |
        |                       | arams params,         | for the given         |
        |                       |         AppleResource | [`BuildRuleP          |
        |                       | DescriptionArg args)` | arams`](../core/rules |
        |                       |                       | /BuildRuleParams.html |
        |                       |                       |  "class in com.facebo |
        |                       |                       | ok.buck.core.rules"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Class<AppleRes       | `get                  | ::: block             |
        | ourceDescriptionArg>` | ConstructorArgType()` | The type of the       |
        |                       |                       | constructor argument  |
        |                       |                       | that is used by this  |
        |                       |                       | description to create |
        |                       |                       | a rule                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `h                    |                       |
        |                       | asFlavors​(com.google. |                       |
        |                       | common.collect.Immuta |                       |
        |                       | bleSet<Flavor> flavor |                       |
        |                       | s,           TargetCo |                       |
        |                       | nfiguration toolchain |                       |
        |                       | TargetConfiguration)` |                       |
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

            ### Methods inherited from interface com.facebook.buck.core.description.[BaseDescription](../core/description/BaseDescription.html "interface in com.facebook.buck.core.description")

            `getConfigurationDeps`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.DescriptionWithTargetGraph}

            ### Methods inherited from interface com.facebook.buck.core.rules.[DescriptionWithTargetGraph](../core/rules/DescriptionWithTargetGraph.html "interface in com.facebook.buck.core.rules")

            `producesCacheableSubgraph`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.model.Flavored}

            ### Methods inherited from interface com.facebook.buck.core.model.[Flavored](../core/model/Flavored.html "interface in com.facebook.buck.core.model")

            `flavorDomains`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### AppleResourceDescription

                public AppleResourceDescription()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getConstructorArgType()}

        -   #### getConstructorArgType

            ``` methodSignature
            public Class<AppleResourceDescriptionArg> getConstructorArgType()
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
                interface `BaseDescription<AppleResourceDescriptionArg>`

        []{#createBuildRule(com.facebook.buck.core.rules.BuildRuleCreationContextWithTargetGraph,com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.rules.BuildRuleParams,com.facebook.buck.apple.AppleResourceDescriptionArg)}

        -   #### createBuildRule

            ``` methodSignature
            public BuildRule createBuildRule​(BuildRuleCreationContextWithTargetGraph context,
                                             BuildTarget buildTarget,
                                             BuildRuleParams params,
                                             AppleResourceDescriptionArg args)
            ```

            ::: block
            [Description copied from
            interface: `DescriptionWithTargetGraph`]{.descfrmTypeLabel}
            :::

            ::: block
            Create a
            [`BuildRule`](../core/rules/BuildRule.html "interface in com.facebook.buck.core.rules")
            for the given
            [`BuildRuleParams`](../core/rules/BuildRuleParams.html "class in com.facebook.buck.core.rules").
            Note that the
            [`BuildTarget`](../core/model/BuildTarget.html "class in com.facebook.buck.core.model")
            referred to in the `params` contains the
            [`Flavor`](../core/model/Flavor.html "interface in com.facebook.buck.core.model")
            to create.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `createBuildRule` in
                interface `DescriptionWithTargetGraph<AppleResourceDescriptionArg>`
            :   `args` - A constructor argument, of type as returned by
                [`BaseDescription.getConstructorArgType()`](../core/description/BaseDescription.html#getConstructorArgType()).

            [Returns:]{.returnLabel}
            :   The
                [`BuildRule`](../core/rules/BuildRule.html "interface in com.facebook.buck.core.rules")
                that describes the default flavour of the rule being
                described.

        []{#hasFlavors(com.google.common.collect.ImmutableSet,com.facebook.buck.core.model.TargetConfiguration)}

        -   #### hasFlavors

            ``` methodSignature
            public boolean hasFlavors​(com.google.common.collect.ImmutableSet<Flavor> flavors,
                                      TargetConfiguration toolchainTargetConfiguration)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `hasFlavors` in interface `Flavored`

            [Parameters:]{.paramLabel}
            :   `flavors` - The set of
                [`Flavor`](../core/model/Flavor.html "interface in com.facebook.buck.core.model")s
                to consider. All must match.

            [Returns:]{.returnLabel}
            :   Whether a
                [`BuildRule`](../core/rules/BuildRule.html "interface in com.facebook.buck.core.rules")
                of the given
                [`Flavor`](../core/model/Flavor.html "interface in com.facebook.buck.core.model")
                can be created.

        []{#addAppleBundleResources(com.facebook.buck.apple.AppleBundleResources.Builder,com.facebook.buck.core.model.targetgraph.TargetNode,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.rules.BuildRuleResolver)}

        -   #### addAppleBundleResources

            ``` methodSignature
            public void addAppleBundleResources​(AppleBundleResources.Builder builder,
                                                TargetNode<AppleResourceDescriptionArg> targetNode,
                                                ProjectFilesystem filesystem,
                                                BuildRuleResolver resolver)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `addAppleBundleResources` in
                interface `HasAppleBundleResourcesDescription<AppleResourceDescriptionArg>`
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
