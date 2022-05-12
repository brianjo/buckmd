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
[Package]{.packageLabelInType} [com.facebook.buck.core.toolchain.rule](package-summary.html)
:::

## Class LegacyToolchainRuleDescription {#class-legacytoolchainruledescription .title title="Class LegacyToolchainRuleDescription"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.toolchain.rule.LegacyToolchainRuleDescription

::: description
-   

    All Implemented Interfaces:
    :   `ImplicitDepsInferringDescription<LegacyToolchainDescriptionArg>`,
        `BaseDescription<LegacyToolchainDescriptionArg>`,
        `Description<LegacyToolchainDescriptionArg>`,
        `RuleDescription<LegacyToolchainDescriptionArg>`

    ------------------------------------------------------------------------

        public class LegacyToolchainRuleDescription
        extends Object
        implements RuleDescription<LegacyToolchainDescriptionArg>, ImplicitDepsInferringDescription<LegacyToolchainDescriptionArg>

    ::: block
    Description that wraps legacy toolchains by name. e.g. to allow
    access to .NET toolchains without having to re-implement them.
    \'legacy\' toolchains are ones that may do extra work behind the
    scenes in a way that is not directly able to be represented by Rule
    Analysis. This might be something like looking at the local
    environment, finding executables on the system path, etc. They are
    also used to minimmize the amount of porting work that has to be
    done up-front. Old rules can continue to use old toolchain retreival
    methods like
    [`ToolchainProvider.getByName(String,  TargetConfiguration)`](../ToolchainProvider.html#getByName(java.lang.String,com.facebook.buck.core.model.TargetConfiguration)),
    whereas new UDR/RAG rules can have a clean interface where
    [`Provider`](../../rules/providers/Provider.html "interface in com.facebook.buck.core.rules.providers")
    instances do all necessary communication about toolchains.

    We expose these currently so that new rules can use existing
    compilers, tools, etc. However in the future, these should be
    discarded in favor of proper build rules that only exist in RAG/UDR.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                             Description
          ----------------------------------------------------------------------- -------------
          `LegacyToolchainRuleDescription​(ToolchainProvider toolchainProvider)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `void`                | `findDepsForTargetFr  |                       |
        |                       | omConstructorArgs​(Bui |                       |
        |                       | ldTarget buildTarget, |                       |
        |                       |                       |                       |
        |                       |                 CellN |                       |
        |                       | ameResolver cellRoots |                       |
        |                       | ,                     |                       |
        |                       |                  Lega |                       |
        |                       | cyToolchainDescriptio |                       |
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
        | `Class<LegacyTool     | `get                  | ::: block             |
        | chainDescriptionArg>` | ConstructorArgType()` | The type of the       |
        |                       |                       | constructor argument  |
        |                       |                       | that is used by this  |
        |                       |                       | description to create |
        |                       |                       | a rule                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Pr                   | `ruleI                | ::: block             |
        | oviderInfoCollection` | mpl​(RuleAnalysisConte | Runs the rule         |
        |                       | xt context,         B | implementation during |
        |                       | uildTarget target,    | the analysis phase.   |
        |                       |       LegacyToolchain | :::                   |
        |                       | DescriptionArg args)` |                       |
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

            ### Methods inherited from interface com.facebook.buck.core.description.[BaseDescription](../../description/BaseDescription.html "interface in com.facebook.buck.core.description")

            `getConfigurationDeps`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.description.RuleDescription}

            ### Methods inherited from interface com.facebook.buck.core.description.[RuleDescription](../../description/RuleDescription.html "interface in com.facebook.buck.core.description")

            `producesCacheableSubgraph`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.core.toolchain.ToolchainProvider)}

        -   #### LegacyToolchainRuleDescription

                public LegacyToolchainRuleDescription​(ToolchainProvider toolchainProvider)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#ruleImpl(com.facebook.buck.core.rules.analysis.RuleAnalysisContext,com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.toolchain.rule.LegacyToolchainDescriptionArg)}

        -   #### ruleImpl

            ``` methodSignature
            public ProviderInfoCollection ruleImpl​(RuleAnalysisContext context,
                                                   BuildTarget target,
                                                   LegacyToolchainDescriptionArg args)
                                            throws ActionCreationException,
                                                   RuleAnalysisException
            ```

            ::: block
            [Description copied from
            interface: `RuleDescription`]{.descfrmTypeLabel}
            :::

            ::: block
            Runs the rule implementation during the analysis phase. The
            rule implementation should create the propagated `Provider`s
            and corresponding `InfoInterface`s, and register its
            corresponding actions.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `ruleImpl` in
                interface `RuleDescription<LegacyToolchainDescriptionArg>`

            [Parameters:]{.paramLabel}
            :   `context` - a
                [`RuleAnalysisContext`](../../rules/analysis/RuleAnalysisContext.html "interface in com.facebook.buck.core.rules.analysis")
                containing all the information usable by this rule for
                it\'s analysis and constructive of its corresponding
                `Provider` and
                [`BuildRule`](../../rules/BuildRule.html "interface in com.facebook.buck.core.rules")
                graph.
            :   `target` - the
                [`BuildTarget`](../../model/BuildTarget.html "class in com.facebook.buck.core.model")
                of this rule
            :   `args` - The args of type `T` that this rule uses to
                rule its analysis

            [Returns:]{.returnLabel}
            :   a
                [`ProviderInfoCollection`](../../rules/providers/collect/ProviderInfoCollection.html "interface in com.facebook.buck.core.rules.providers.collect")
                that contains all the `Provider` and the corresponding
                `InfoInterface` to be propagated by this rule.

            [Throws:]{.throwsLabel}
            :   `ActionCreationException` - If an action cannot be
                created correctly
            :   `RuleAnalysisException` - If the rule implementation
                could not run as expected. e.g. if the implementation
                method of a User Defined Rule fails to eval

        []{#getConstructorArgType()}

        -   #### getConstructorArgType

            ``` methodSignature
            public Class<LegacyToolchainDescriptionArg> getConstructorArgType()
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
                interface `BaseDescription<LegacyToolchainDescriptionArg>`

        []{#findDepsForTargetFromConstructorArgs(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.cell.nameresolver.CellNameResolver,com.facebook.buck.core.toolchain.rule.LegacyToolchainDescriptionArg,com.google.common.collect.ImmutableCollection.Builder,com.google.common.collect.ImmutableCollection.Builder)}

        -   #### findDepsForTargetFromConstructorArgs

            ``` methodSignature
            public void findDepsForTargetFromConstructorArgs​(BuildTarget buildTarget,
                                                             CellNameResolver cellRoots,
                                                             LegacyToolchainDescriptionArg constructorArg,
                                                             com.google.common.collect.ImmutableCollection.Builder<BuildTarget> extraDepsBuilder,
                                                             com.google.common.collect.ImmutableCollection.Builder<BuildTarget> targetGraphOnlyDepsBuilder)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `findDepsForTargetFromConstructorArgs` in
                interface `ImplicitDepsInferringDescription<LegacyToolchainDescriptionArg>`
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
