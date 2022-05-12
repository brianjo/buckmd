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

-   [Overview](../../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../index-all.html)
-   [Help](../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.core.toolchain.toolprovider.impl](package-summary.html)
:::

## Class BinaryBuildRuleToolProvider {#class-binarybuildruletoolprovider .title title="Class BinaryBuildRuleToolProvider"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.toolchain.toolprovider.impl.BinaryBuildRuleToolProvider

::: description
-   

    All Implemented Interfaces:
    :   `RuleAnalysisLegacyToolProvider`, `ToolProvider`

    ------------------------------------------------------------------------

        public class BinaryBuildRuleToolProvider
        extends Object
        implements ToolProvider, RuleAnalysisLegacyToolProvider

    ::: block
    A
    [`ToolProvider`](../ToolProvider.html "interface in com.facebook.buck.core.toolchain.toolprovider")
    which provides the
    [`Tool`](../../tool/Tool.html "interface in com.facebook.buck.core.toolchain.tool")
    object of the
    [`BinaryBuildRule`](../../../rules/tool/BinaryBuildRule.html "interface in com.facebook.buck.core.rules.tool")
    references by a given
    [`BuildTarget`](../../../model/BuildTarget.html "class in com.facebook.buck.core.model").
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                               Description
          --------------------------------------------------------------------------------------------------------- -------------
          `BinaryBuildRuleToolProvider​(UnconfiguredBuildTarget target,                            String source)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type         Method                                                                                                       Description
          ------------------------- ------------------------------------------------------------------------------------------------------------ -------------
          `Iterable<BuildTarget>`   `getParseTimeDeps​(TargetConfiguration targetConfiguration)`                                                   
          `RunInfo`                 `getRunInfo​(DependencyOnlyRuleAnalysisContext context,           TargetConfiguration targetConfiguration)`    
          `Tool`                    `resolve​(BuildRuleResolver resolver,        TargetConfiguration targetConfiguration)`                         

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.core.model.UnconfiguredBuildTarget,java.lang.String)}

        -   #### BinaryBuildRuleToolProvider

                public BinaryBuildRuleToolProvider​(UnconfiguredBuildTarget target,
                                                   String source)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#resolve(com.facebook.buck.core.rules.BuildRuleResolver,com.facebook.buck.core.model.TargetConfiguration)}

        -   #### resolve

            ``` methodSignature
            public Tool resolve​(BuildRuleResolver resolver,
                                TargetConfiguration targetConfiguration)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `resolve` in interface `ToolProvider`

            [Returns:]{.returnLabel}
            :   the provided
                [`Tool`](../../tool/Tool.html "interface in com.facebook.buck.core.toolchain.tool")
                object.

        []{#getParseTimeDeps(com.facebook.buck.core.model.TargetConfiguration)}

        -   #### getParseTimeDeps

            ``` methodSignature
            public Iterable<BuildTarget> getParseTimeDeps​(TargetConfiguration targetConfiguration)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getParseTimeDeps` in interface `ToolProvider`

            [Returns:]{.returnLabel}
            :   any dependencies required at parse time to support the
                provided tool.

        []{#getRunInfo(com.facebook.buck.core.rules.analysis.context.DependencyOnlyRuleAnalysisContext,com.facebook.buck.core.model.TargetConfiguration)}

        -   #### getRunInfo

            ``` methodSignature
            public RunInfo getRunInfo​(DependencyOnlyRuleAnalysisContext context,
                                      TargetConfiguration targetConfiguration)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getRunInfo` in
                interface `RuleAnalysisLegacyToolProvider`

            [Returns:]{.returnLabel}
            :   a
                [`RunInfo`](../../../rules/providers/lib/RunInfo.html "class in com.facebook.buck.core.rules.providers.lib")
                that will execute a given tool
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

-   [Overview](../../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../index-all.html)
-   [Help](../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../allclasses.html)

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
