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
[Package]{.packageLabelInType} [com.facebook.buck.shell](package-summary.html)
:::

## Class CommandAliasDescription {#class-commandaliasdescription .title title="Class CommandAliasDescription"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.shell.CommandAliasDescription

::: description
-   

    All Implemented Interfaces:
    :   `BaseDescription<CommandAliasDescriptionArg>`,
        `Description<CommandAliasDescriptionArg>`,
        `DescriptionWithTargetGraph<CommandAliasDescriptionArg>`

    ------------------------------------------------------------------------

        public class CommandAliasDescription
        extends Object
        implements DescriptionWithTargetGraph<CommandAliasDescriptionArg>
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                    Description
          ---------------------------------------------- -------------
          `CommandAliasDescription​(Platform platform)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `BuildRule`           | `cre                  | ::: block             |
        |                       | ateBuildRule​(BuildRul | Create a              |
        |                       | eCreationContextWithT | [`B                   |
        |                       | argetGraph context,   | uildRule`](../core/ru |
        |                       |               BuildTa | les/BuildRule.html "i |
        |                       | rget buildTarget,     | nterface in com.faceb |
        |                       |             BuildRule | ook.buck.core.rules") |
        |                       | Params params,        | for the given         |
        |                       |          CommandAlias | [`BuildRuleP          |
        |                       | DescriptionArg args)` | arams`](../core/rules |
        |                       |                       | /BuildRuleParams.html |
        |                       |                       |  "class in com.facebo |
        |                       |                       | ok.buck.core.rules"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Class<Command        | `get                  | ::: block             |
        | AliasDescriptionArg>` | ConstructorArgType()` | The type of the       |
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

            ### Methods inherited from interface com.facebook.buck.core.description.[BaseDescription](../core/description/BaseDescription.html "interface in com.facebook.buck.core.description")

            `getConfigurationDeps`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.DescriptionWithTargetGraph}

            ### Methods inherited from interface com.facebook.buck.core.rules.[DescriptionWithTargetGraph](../core/rules/DescriptionWithTargetGraph.html "interface in com.facebook.buck.core.rules")

            `producesCacheableSubgraph`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.util.environment.Platform)}

        -   #### CommandAliasDescription

                public CommandAliasDescription​(Platform platform)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getConstructorArgType()}

        -   #### getConstructorArgType

            ``` methodSignature
            public Class<CommandAliasDescriptionArg> getConstructorArgType()
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
                interface `BaseDescription<CommandAliasDescriptionArg>`

        []{#createBuildRule(com.facebook.buck.core.rules.BuildRuleCreationContextWithTargetGraph,com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.rules.BuildRuleParams,com.facebook.buck.shell.CommandAliasDescriptionArg)}

        -   #### createBuildRule

            ``` methodSignature
            public BuildRule createBuildRule​(BuildRuleCreationContextWithTargetGraph context,
                                             BuildTarget buildTarget,
                                             BuildRuleParams params,
                                             CommandAliasDescriptionArg args)
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
                interface `DescriptionWithTargetGraph<CommandAliasDescriptionArg>`
            :   `args` - A constructor argument, of type as returned by
                [`BaseDescription.getConstructorArgType()`](../core/description/BaseDescription.html#getConstructorArgType()).

            [Returns:]{.returnLabel}
            :   The
                [`BuildRule`](../core/rules/BuildRule.html "interface in com.facebook.buck.core.rules")
                that describes the default flavour of the rule being
                described.
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