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
[Package]{.packageLabelInType} [com.facebook.buck.core.model.actiongraph](package-summary.html)
:::

## Class ActionGraphAndBuilder {#class-actiongraphandbuilder .title title="Class ActionGraphAndBuilder"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.model.actiongraph.ActionGraphAndBuilder

::: description
-   

    ------------------------------------------------------------------------

        public abstract class ActionGraphAndBuilder
        extends Object

    ::: block
    Holds an ActionGraph with the BuildRuleResolver that created it.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                 Description
          --------------------------- -------------
          `ActionGraphAndBuilder()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                 Method                                                                                                                                                Description
          ------------------------------------------------- ----------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `abstract ActionGraph`                            `getActionGraph()`                                                                                                                                     
          `abstract ActionGraphBuilder`                     `getActionGraphBuilder()`                                                                                                                              
          `abstract BuildEngineActionToBuildRuleResolver`   `getBuildEngineActionToBuildRuleResolver()`                                                                                                            
          `static ActionGraphAndBuilder`                    `of​(ActionGraph actionGraph,   ActionGraphBuilder actionGraphBuilder)`                                                                                 
          `static ActionGraphAndBuilder`                    `of​(ActionGraph actionGraph,   ActionGraphBuilder actionGraphBuilder,   BuildEngineActionToBuildRuleResolver buildEngineActionToBuildRuleResolver)`    

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

        -   #### ActionGraphAndBuilder

                public ActionGraphAndBuilder()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getActionGraph()}

        -   #### getActionGraph

            ``` methodSignature
            public abstract ActionGraph getActionGraph()
            ```

        []{#getActionGraphBuilder()}

        -   #### getActionGraphBuilder

            ``` methodSignature
            public abstract ActionGraphBuilder getActionGraphBuilder()
            ```

        []{#getBuildEngineActionToBuildRuleResolver()}

        -   #### getBuildEngineActionToBuildRuleResolver

            ``` methodSignature
            public abstract BuildEngineActionToBuildRuleResolver getBuildEngineActionToBuildRuleResolver()
            ```

        []{#of(com.facebook.buck.core.model.actiongraph.ActionGraph,com.facebook.buck.core.rules.ActionGraphBuilder)}

        -   #### of

            ``` methodSignature
            public static ActionGraphAndBuilder of​(ActionGraph actionGraph,
                                                   ActionGraphBuilder actionGraphBuilder)
            ```

        []{#of(com.facebook.buck.core.model.actiongraph.ActionGraph,com.facebook.buck.core.rules.ActionGraphBuilder,com.facebook.buck.core.build.action.resolver.BuildEngineActionToBuildRuleResolver)}

        -   #### of

            ``` methodSignature
            public static ActionGraphAndBuilder of​(ActionGraph actionGraph,
                                                   ActionGraphBuilder actionGraphBuilder,
                                                   BuildEngineActionToBuildRuleResolver buildEngineActionToBuildRuleResolver)
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
