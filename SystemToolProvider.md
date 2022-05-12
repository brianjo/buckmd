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

## Class SystemToolProvider {#class-systemtoolprovider .title title="Class SystemToolProvider"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.toolchain.toolprovider.impl.SystemToolProvider

::: description
-   

    All Implemented Interfaces:
    :   `RuleAnalysisLegacyToolProvider`, `ToolProvider`

    ------------------------------------------------------------------------

        public abstract class SystemToolProvider
        extends Object
        implements ToolProvider, RuleAnalysisLegacyToolProvider

    ::: block
    A
    [`ToolProvider`](../ToolProvider.html "interface in com.facebook.buck.core.toolchain.toolprovider")
    which returns a
    [`HashedFileTool`](../../tool/impl/HashedFileTool.html "class in com.facebook.buck.core.toolchain.tool.impl")
    found from searching the system.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor              Description
          ------------------------ -------------
          `SystemToolProvider()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type             Method                                                                                                                                                                                            Description
          ----------------------------- ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `Iterable<BuildTarget>`       `getParseTimeDeps​(TargetConfiguration targetConfiguration)`                                                                                                                                        
          `RunInfo`                     `getRunInfo​(DependencyOnlyRuleAnalysisContext context,           TargetConfiguration targetConfiguration)`                                                                                         
          `static SystemToolProvider`   `of​(ExecutableFinder executableFinder,   java.util.function.Function<Path,​SourcePath> sourcePathConverter,   Path name,   Map<String,​? extends String> environment)`                               
          `static SystemToolProvider`   `of​(ExecutableFinder executableFinder,   java.util.function.Function<Path,​SourcePath> sourcePathConverter,   Path name,   Map<String,​? extends String> environment,   Optional<String> source)`    
          `Tool`                        `resolve()`                                                                                                                                                                                        
          `Tool`                        `resolve​(BuildRuleResolver resolver,        TargetConfiguration targetConfiguration)`                                                                                                              

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
          Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
          .tableTab}[[Instance
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

        []{#<init>()}

        -   #### SystemToolProvider

                public SystemToolProvider()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#resolve()}

        -   #### resolve

            ``` methodSignature
            @Lazy
            public Tool resolve()
            ```

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

        []{#of(com.facebook.buck.io.ExecutableFinder,java.util.function.Function,java.nio.file.Path,java.util.Map,java.util.Optional)}

        -   #### of

            ``` methodSignature
            public static SystemToolProvider of​(ExecutableFinder executableFinder,
                                                java.util.function.Function<Path,​SourcePath> sourcePathConverter,
                                                Path name,
                                                Map<String,​? extends String> environment,
                                                Optional<String> source)
            ```

        []{#of(com.facebook.buck.io.ExecutableFinder,java.util.function.Function,java.nio.file.Path,java.util.Map)}

        -   #### of

            ``` methodSignature
            public static SystemToolProvider of​(ExecutableFinder executableFinder,
                                                java.util.function.Function<Path,​SourcePath> sourcePathConverter,
                                                Path name,
                                                Map<String,​? extends String> environment)
            ```
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
