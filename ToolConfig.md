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
[Package]{.packageLabelInType} [com.facebook.buck.rules.tool.config](package-summary.html)
:::

## Class ToolConfig {#class-toolconfig .title title="Class ToolConfig"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.rules.tool.config.ToolConfig

::: description
-   

    All Implemented Interfaces:
    :   `ConfigView<BuckConfig>`

    ------------------------------------------------------------------------

        public abstract class ToolConfig
        extends Object
        implements ConfigView<BuckConfig>
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor      Description
          ---------------- -------------
          `ToolConfig()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type          Method                                                                                                                                                              Description
          -------------------------- ------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `abstract BuckConfig`      `getDelegate()`                                                                                                                                                      
          `Optional<Tool>`           `getPrebuiltTool​(String section,                String field,                java.util.function.Function<String,​Path> valueToPathMapper)`                            
          `Tool`                     `getRequiredTool​(String section,                String field,                BuildRuleResolver resolver,                TargetConfiguration targetConfiguration)`    
          `Optional<Tool>`           `getTool​(String section,        String field,        BuildRuleResolver resolver,        TargetConfiguration targetConfiguration)`                                    
          `Optional<ToolProvider>`   `getToolProvider​(String section,                String field)`                                                                                                       
          `Optional<ToolProvider>`   `getToolProvider​(String section,                String field,                java.util.function.Function<String,​Path> valueToPathMapper)`                            
          `static ToolConfig`        `of​(BuckConfig delegate)`                                                                                                                                            

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
          Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
          .tableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Abstract
          Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
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

        -   #### ToolConfig

                public ToolConfig()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getDelegate()}

        -   #### getDelegate

            ``` methodSignature
            public abstract BuckConfig getDelegate()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getDelegate` in interface `ConfigView<BuckConfig>`

        []{#of(com.facebook.buck.core.config.BuckConfig)}

        -   #### of

            ``` methodSignature
            public static ToolConfig of​(BuckConfig delegate)
            ```

        []{#getToolProvider(java.lang.String,java.lang.String)}

        -   #### getToolProvider

            ``` methodSignature
            public Optional<ToolProvider> getToolProvider​(String section,
                                                          String field)
            ```

            [Returns:]{.returnLabel}
            :   a
                [`Tool`](../../../core/toolchain/tool/Tool.html "interface in com.facebook.buck.core.toolchain.tool")
                identified by a \@{link BuildTarget} or
                [`Path`](http://docs.oracle.com/javase/7/docs/api/java/nio/file/Path.html?is-external=true "class or interface in java.nio.file"){.externalLink}
                reference by the given section:field, if set.

        []{#getToolProvider(java.lang.String,java.lang.String,java.util.function.Function)}

        -   #### getToolProvider

            ``` methodSignature
            public Optional<ToolProvider> getToolProvider​(String section,
                                                          String field,
                                                          java.util.function.Function<String,​Path> valueToPathMapper)
            ```

            [Returns:]{.returnLabel}
            :   a
                [`Tool`](../../../core/toolchain/tool/Tool.html "interface in com.facebook.buck.core.toolchain.tool")
                identified by a \@{link BuildTarget} or
                [`Path`](http://docs.oracle.com/javase/7/docs/api/java/nio/file/Path.html?is-external=true "class or interface in java.nio.file"){.externalLink}
                reference by the given section:field, if set.

        []{#getPrebuiltTool(java.lang.String,java.lang.String,java.util.function.Function)}

        -   #### getPrebuiltTool

            ``` methodSignature
            public Optional<Tool> getPrebuiltTool​(String section,
                                                  String field,
                                                  java.util.function.Function<String,​Path> valueToPathMapper)
            ```

            [Returns:]{.returnLabel}
            :   a
                [`Tool`](../../../core/toolchain/tool/Tool.html "interface in com.facebook.buck.core.toolchain.tool")
                identified by a
                [`Path`](http://docs.oracle.com/javase/7/docs/api/java/nio/file/Path.html?is-external=true "class or interface in java.nio.file"){.externalLink}
                reference by the given section:field, if set. This does
                not allow the tool to be provided by a \@{link
                BuildTarget}.

        []{#getTool(java.lang.String,java.lang.String,com.facebook.buck.core.rules.BuildRuleResolver,com.facebook.buck.core.model.TargetConfiguration)}

        -   #### getTool

            ``` methodSignature
            public Optional<Tool> getTool​(String section,
                                          String field,
                                          BuildRuleResolver resolver,
                                          TargetConfiguration targetConfiguration)
            ```

        []{#getRequiredTool(java.lang.String,java.lang.String,com.facebook.buck.core.rules.BuildRuleResolver,com.facebook.buck.core.model.TargetConfiguration)}

        -   #### getRequiredTool

            ``` methodSignature
            public Tool getRequiredTool​(String section,
                                        String field,
                                        BuildRuleResolver resolver,
                                        TargetConfiguration targetConfiguration)
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
