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
[Package]{.packageLabelInType} [com.facebook.buck.rules.keys](package-summary.html)
:::

## Class InputBasedRuleKeyFactory {#class-inputbasedrulekeyfactory .title title="Class InputBasedRuleKeyFactory"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.rules.keys.InputBasedRuleKeyFactory

::: description
-   

    All Implemented Interfaces:
    :   `RuleKeyFactory<RuleKey>`

    ------------------------------------------------------------------------

        public class InputBasedRuleKeyFactory
        extends Object
        implements RuleKeyFactory<RuleKey>

    ::: block
    A factory for generating input-based
    [`RuleKey`](../../core/rulekey/RuleKey.html "class in com.facebook.buck.core.rulekey")s.
    :::

    [See Also:]{.seeLabel}
    :   [`SupportsInputBasedRuleKey`](../../core/rules/attr/SupportsInputBasedRuleKey.html "interface in com.facebook.buck.core.rules.attr")
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type           Class                                         Description
          --------------------------- --------------------------------------------- -------------
          `protected static class `   `InputBasedRuleKeyFactory.Result<RULE_KEY>`    

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                                       Description
          ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `InputBasedRuleKeyFactory​(RuleKeyFieldLoader ruleKeyFieldLoader,                         FileHashLoader hashLoader,                         SourcePathRuleFinder ruleFinder,                         long inputSizeLimit,                         Optional<ThriftRuleKeyLogger> ruleKeyLogger)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `RuleKey`             | `build​(Build          | ::: block             |
        |                       | EngineAction action)` | Creates a new         |
        |                       |                       | `RULE_KEY` for the    |
        |                       |                       | given                 |
        |                       |                       | [`BuildEngineAct      |
        |                       |                       | ion`](../../core/buil |
        |                       |                       | d/action/BuildEngineA |
        |                       |                       | ction.html "interface |
        |                       |                       |  in com.facebook.buck |
        |                       |                       | .core.build.action"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Long>`      | `getInputSizeLimit()` |                       |
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
        -   []{#methods.inherited.from.class.com.facebook.buck.rules.keys.RuleKeyFactory}

            ### Methods inherited from interface com.facebook.buck.rules.keys.[RuleKeyFactory](RuleKeyFactory.html "interface in com.facebook.buck.rules.keys")

            `getFromCache`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.rules.keys.RuleKeyFieldLoader,com.facebook.buck.util.hashing.FileHashLoader,com.facebook.buck.core.rules.SourcePathRuleFinder,long,java.util.Optional)}

        -   #### InputBasedRuleKeyFactory

                public InputBasedRuleKeyFactory​(RuleKeyFieldLoader ruleKeyFieldLoader,
                                                FileHashLoader hashLoader,
                                                SourcePathRuleFinder ruleFinder,
                                                long inputSizeLimit,
                                                Optional<ThriftRuleKeyLogger> ruleKeyLogger)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getInputSizeLimit()}

        -   #### getInputSizeLimit

            ``` methodSignature
            public Optional<Long> getInputSizeLimit()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getInputSizeLimit` in
                interface `RuleKeyFactory<RuleKey>`

        []{#build(com.facebook.buck.core.build.action.BuildEngineAction)}

        -   #### build

            ``` methodSignature
            public RuleKey build​(BuildEngineAction action)
            ```

            ::: block
            [Description copied from
            interface: `RuleKeyFactory`]{.descfrmTypeLabel}
            :::

            ::: block
            Creates a new `RULE_KEY` for the given
            [`BuildEngineAction`](../../core/build/action/BuildEngineAction.html "interface in com.facebook.buck.core.build.action").
            In most cases `  RULE_KEY` is going to be
            [`RuleKey`](../../core/rulekey/RuleKey.html "class in com.facebook.buck.core.rulekey"),
            but it can be anything really.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `build` in interface `RuleKeyFactory<RuleKey>`

            [Parameters:]{.paramLabel}
            :   `action` - The build rule to create the key for.

            [Returns:]{.returnLabel}
            :   A rule key.
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