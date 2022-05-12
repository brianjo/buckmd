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
[Package]{.packageLabelInType} [com.facebook.buck.core.starlark.rule](package-summary.html)
:::

## Class SkylarkDescription {#class-skylarkdescription .title title="Class SkylarkDescription"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.starlark.rule.SkylarkDescription

::: description
-   

    All Implemented Interfaces:
    :   `BaseDescription<SkylarkDescriptionArg>`,
        `Description<SkylarkDescriptionArg>`,
        `RuleDescription<SkylarkDescriptionArg>`,
        `RuleDescriptionWithInstanceName<SkylarkDescriptionArg>`

    ------------------------------------------------------------------------

        public class SkylarkDescription
        extends Object
        implements RuleDescriptionWithInstanceName<SkylarkDescriptionArg>

    ::: block
    Description for User Defined Rules. This Description runs
    user-supplied implementation functions in order to generate
    [`Action`](../../rules/actions/Action.html "interface in com.facebook.buck.core.rules.actions")s.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor              Description
          ------------------------ -------------
          `SkylarkDescription()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `Class<Sk             | `get                  | ::: block             |
        | ylarkDescriptionArg>` | ConstructorArgType()` | The type of the       |
        |                       |                       | constructor argument  |
        |                       |                       | that is used by this  |
        |                       |                       | description to create |
        |                       |                       | a rule                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getRuleName​(Skylark  |                       |
        |                       | DescriptionArg args)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `produce              | ::: block             |
        |                       | sCacheableSubgraph()` | Whether or not the    |
        |                       |                       | build rule subgraph   |
        |                       |                       | produced by this      |
        |                       |                       | `Description` is safe |
        |                       |                       | to cache in           |
        |                       |                       | [`Inc                 |
        |                       |                       | rementalActionGraphGe |
        |                       |                       | nerator`](../../model |
        |                       |                       | /actiongraph/computat |
        |                       |                       | ion/IncrementalAction |
        |                       |                       | GraphGenerator.html " |
        |                       |                       | class in com.facebook |
        |                       |                       | .buck.core.model.acti |
        |                       |                       | ongraph.computation") |
        |                       |                       | for incremental       |
        |                       |                       | action graph          |
        |                       |                       | generation.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Pr                   | `ruleImpl​(RuleAnaly   | ::: block             |
        | oviderInfoCollection` | sisContext context,   | Runs the rule         |
        |                       |        BuildTarget ta | implementation during |
        |                       | rget,         Skylark | the analysis phase.   |
        |                       | DescriptionArg args)` | :::                   |
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
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### SkylarkDescription

                public SkylarkDescription()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#producesCacheableSubgraph()}

        -   #### producesCacheableSubgraph

            ``` methodSignature
            public boolean producesCacheableSubgraph()
            ```

            ::: block
            [Description copied from
            interface: `Description`]{.descfrmTypeLabel}
            :::

            ::: block
            Whether or not the build rule subgraph produced by this
            `Description` is safe to cache in
            [`IncrementalActionGraphGenerator`](../../model/actiongraph/computation/IncrementalActionGraphGenerator.html "class in com.facebook.buck.core.model.actiongraph.computation")
            for incremental action graph generation.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `producesCacheableSubgraph` in
                interface `Description<SkylarkDescriptionArg>`

            [Specified by:]{.overrideSpecifyLabel}
            :   `producesCacheableSubgraph` in
                interface `RuleDescription<SkylarkDescriptionArg>`

        []{#ruleImpl(com.facebook.buck.core.rules.analysis.RuleAnalysisContext,com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.starlark.rule.SkylarkDescriptionArg)}

        -   #### ruleImpl

            ``` methodSignature
            public ProviderInfoCollection ruleImpl​(RuleAnalysisContext context,
                                                   BuildTarget target,
                                                   SkylarkDescriptionArg args)
                                            throws RuleAnalysisException,
                                                   ActionCreationException
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
                interface `RuleDescription<SkylarkDescriptionArg>`

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
            :   `RuleAnalysisException` - If the rule implementation
                could not run as expected. e.g. if the implementation
                method of a User Defined Rule fails to eval
            :   `ActionCreationException` - If an action cannot be
                created correctly

        []{#getRuleName(com.facebook.buck.core.starlark.rule.SkylarkDescriptionArg)}

        -   #### getRuleName

            ``` methodSignature
            public String getRuleName​(SkylarkDescriptionArg args)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getRuleName` in
                interface `RuleDescriptionWithInstanceName<SkylarkDescriptionArg>`

            [Returns:]{.returnLabel}
            :   The user friendly name of a rule. e.g. cxx_binary, or
                //foo:baz.bzl:some_rule. See
                [`DescriptionCache.getRuleType(BaseDescription)`](../../description/impl/DescriptionCache.html#getRuleType(com.facebook.buck.core.description.BaseDescription))

        []{#getConstructorArgType()}

        -   #### getConstructorArgType

            ``` methodSignature
            public Class<SkylarkDescriptionArg> getConstructorArgType()
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
                interface `BaseDescription<SkylarkDescriptionArg>`
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
