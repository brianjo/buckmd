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
[Package]{.packageLabelInType} [com.facebook.buck.features.dotnet](package-summary.html)
:::

## Class PrebuiltDotnetLibraryRuleDescription {#class-prebuiltdotnetlibraryruledescription .title title="Class PrebuiltDotnetLibraryRuleDescription"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.features.dotnet.PrebuiltDotnetLibraryRuleDescription

::: description
-   

    All Implemented Interfaces:
    :   `BaseDescription<PrebuiltDotnetLibraryDescriptionArg>`,
        `Description<PrebuiltDotnetLibraryDescriptionArg>`,
        `RuleDescription<PrebuiltDotnetLibraryDescriptionArg>`

    ------------------------------------------------------------------------

        public class PrebuiltDotnetLibraryRuleDescription
        extends Object
        implements RuleDescription<PrebuiltDotnetLibraryDescriptionArg>

    ::: block
    implementation for dotnet rules in the rule analysis framework.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                Description
          ------------------------------------------ -------------
          `PrebuiltDotnetLibraryRuleDescription()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `C                    | `get                  | ::: block             |
        | lass<PrebuiltDotnetLi | ConstructorArgType()` | The type of the       |
        | braryDescriptionArg>` |                       | constructor argument  |
        |                       |                       | that is used by this  |
        |                       |                       | description to create |
        |                       |                       | a rule                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Pr                   | `ruleImpl​(Ru          | ::: block             |
        | oviderInfoCollection` | leAnalysisContext con | Runs the rule         |
        |                       | text,         BuildTa | implementation during |
        |                       | rget target,          | the analysis phase.   |
        |                       | PrebuiltDotnetLibrary | :::                   |
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

            ### Methods inherited from interface com.facebook.buck.core.description.[BaseDescription](../../core/description/BaseDescription.html "interface in com.facebook.buck.core.description")

            `getConfigurationDeps`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.description.RuleDescription}

            ### Methods inherited from interface com.facebook.buck.core.description.[RuleDescription](../../core/description/RuleDescription.html "interface in com.facebook.buck.core.description")

            `producesCacheableSubgraph`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### PrebuiltDotnetLibraryRuleDescription

                public PrebuiltDotnetLibraryRuleDescription()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getConstructorArgType()}

        -   #### getConstructorArgType

            ``` methodSignature
            public Class<PrebuiltDotnetLibraryDescriptionArg> getConstructorArgType()
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
                interface `BaseDescription<PrebuiltDotnetLibraryDescriptionArg>`

        []{#ruleImpl(com.facebook.buck.core.rules.analysis.RuleAnalysisContext,com.facebook.buck.core.model.BuildTarget,com.facebook.buck.features.dotnet.PrebuiltDotnetLibraryDescriptionArg)}

        -   #### ruleImpl

            ``` methodSignature
            public ProviderInfoCollection ruleImpl​(RuleAnalysisContext context,
                                                   BuildTarget target,
                                                   PrebuiltDotnetLibraryDescriptionArg args)
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
                interface `RuleDescription<PrebuiltDotnetLibraryDescriptionArg>`

            [Parameters:]{.paramLabel}
            :   `context` - a
                [`RuleAnalysisContext`](../../core/rules/analysis/RuleAnalysisContext.html "interface in com.facebook.buck.core.rules.analysis")
                containing all the information usable by this rule for
                it\'s analysis and constructive of its corresponding
                `Provider` and
                [`BuildRule`](../../core/rules/BuildRule.html "interface in com.facebook.buck.core.rules")
                graph.
            :   `target` - the
                [`BuildTarget`](../../core/model/BuildTarget.html "class in com.facebook.buck.core.model")
                of this rule
            :   `args` - The args of type `T` that this rule uses to
                rule its analysis

            [Returns:]{.returnLabel}
            :   a
                [`ProviderInfoCollection`](../../core/rules/providers/collect/ProviderInfoCollection.html "interface in com.facebook.buck.core.rules.providers.collect")
                that contains all the `Provider` and the corresponding
                `InfoInterface` to be propagated by this rule.

            [Throws:]{.throwsLabel}
            :   `ActionCreationException` - If an action cannot be
                created correctly
            :   `RuleAnalysisException` - If the rule implementation
                could not run as expected. e.g. if the implementation
                method of a User Defined Rule fails to eval
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
