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
[Package]{.packageLabelInType} [com.facebook.buck.jvm.java](package-summary.html)
:::

## Class JavaLibraryDescription {#class-javalibrarydescription .title title="Class JavaLibraryDescription"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.jvm.java.JavaLibraryDescription

::: description
-   

    All Implemented Interfaces:
    :   `ImplicitDepsInferringDescription<JavaLibraryDescriptionArg>`,
        `BaseDescription<JavaLibraryDescriptionArg>`,
        `Description<JavaLibraryDescriptionArg>`, `Flavored`,
        `DescriptionWithTargetGraph<JavaLibraryDescriptionArg>`,
        `VersionPropagator<JavaLibraryDescriptionArg>`

    ------------------------------------------------------------------------

        public class JavaLibraryDescription
        extends Object
        implements DescriptionWithTargetGraph<JavaLibraryDescriptionArg>, Flavored, VersionPropagator<JavaLibraryDescriptionArg>, ImplicitDepsInferringDescription<JavaLibraryDescriptionArg>
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type     Class                              Description
          --------------------- ---------------------------------- -------------
          `static interface `   `JavaLibraryDescription.CoreArg`    

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                          Description
          -------------------------------------------------------------------------------------------------------------------- -------------
          `JavaLibraryDescription​(ToolchainProvider toolchainProvider,                       JavaBuckConfig javaBuckConfig)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `BuildRule`           | `cr                   | ::: block             |
        |                       | eateBuildRule​(BuildRu | Create a              |
        |                       | leCreationContextWith | [`Buil                |
        |                       | TargetGraph context,  | dRule`](../../core/ru |
        |                       |                BuildT | les/BuildRule.html "i |
        |                       | arget buildTarget,    | nterface in com.faceb |
        |                       |              BuildRul | ook.buck.core.rules") |
        |                       | eParams params,       | for the given         |
        |                       |           JavaLibrary | [`BuildRulePara       |
        |                       | DescriptionArg args)` | ms`](../../core/rules |
        |                       |                       | /BuildRuleParams.html |
        |                       |                       |  "class in com.facebo |
        |                       |                       | ok.buck.core.rules"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `findDepsForTarg      |                       |
        |                       | etFromConstructorArgs |                       |
        |                       | ​(BuildTarget buildTar |                       |
        |                       | get,                  |                       |
        |                       |                     C |                       |
        |                       | ellNameResolver cellR |                       |
        |                       | oots,                 |                       |
        |                       |                       |                       |
        |                       | JavaLibraryDescriptio |                       |
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
        | `Class<JavaLi         | `get                  | ::: block             |
        | braryDescriptionArg>` | ConstructorArgType()` | The type of the       |
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

            `flavorDomains`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.core.toolchain.ToolchainProvider,com.facebook.buck.jvm.java.JavaBuckConfig)}

        -   #### JavaLibraryDescription

                public JavaLibraryDescription​(ToolchainProvider toolchainProvider,
                                              JavaBuckConfig javaBuckConfig)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

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
                [`Flavor`](../../core/model/Flavor.html "interface in com.facebook.buck.core.model")s
                to consider. All must match.

            [Returns:]{.returnLabel}
            :   Whether a
                [`BuildRule`](../../core/rules/BuildRule.html "interface in com.facebook.buck.core.rules")
                of the given
                [`Flavor`](../../core/model/Flavor.html "interface in com.facebook.buck.core.model")
                can be created.

        []{#getConstructorArgType()}

        -   #### getConstructorArgType

            ``` methodSignature
            public Class<JavaLibraryDescriptionArg> getConstructorArgType()
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
                interface `BaseDescription<JavaLibraryDescriptionArg>`

        []{#createBuildRule(com.facebook.buck.core.rules.BuildRuleCreationContextWithTargetGraph,com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.rules.BuildRuleParams,com.facebook.buck.jvm.java.JavaLibraryDescriptionArg)}

        -   #### createBuildRule

            ``` methodSignature
            public BuildRule createBuildRule​(BuildRuleCreationContextWithTargetGraph context,
                                             BuildTarget buildTarget,
                                             BuildRuleParams params,
                                             JavaLibraryDescriptionArg args)
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
                interface `DescriptionWithTargetGraph<JavaLibraryDescriptionArg>`
            :   `args` - A constructor argument, of type as returned by
                [`BaseDescription.getConstructorArgType()`](../../core/description/BaseDescription.html#getConstructorArgType()).

            [Returns:]{.returnLabel}
            :   The
                [`BuildRule`](../../core/rules/BuildRule.html "interface in com.facebook.buck.core.rules")
                that describes the default flavour of the rule being
                described.

        []{#findDepsForTargetFromConstructorArgs(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.cell.nameresolver.CellNameResolver,com.facebook.buck.jvm.java.JavaLibraryDescriptionArg,com.google.common.collect.ImmutableCollection.Builder,com.google.common.collect.ImmutableCollection.Builder)}

        -   #### findDepsForTargetFromConstructorArgs

            ``` methodSignature
            public void findDepsForTargetFromConstructorArgs​(BuildTarget buildTarget,
                                                             CellNameResolver cellRoots,
                                                             JavaLibraryDescriptionArg constructorArg,
                                                             com.google.common.collect.ImmutableCollection.Builder<BuildTarget> extraDepsBuilder,
                                                             com.google.common.collect.ImmutableCollection.Builder<BuildTarget> targetGraphOnlyDepsBuilder)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `findDepsForTargetFromConstructorArgs` in
                interface `ImplicitDepsInferringDescription<JavaLibraryDescriptionArg>`
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
