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
[Package]{.packageLabelInType} [com.facebook.buck.core.model.actiongraph.computation](package-summary.html)
:::

## Class ParallelActionGraphFactory {#class-parallelactiongraphfactory .title title="Class ParallelActionGraphFactory"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.model.actiongraph.computation.ParallelActionGraphFactory

::: description
-   

    All Implemented Interfaces:
    :   `ActionGraphFactoryDelegate`

    ------------------------------------------------------------------------

        public class ParallelActionGraphFactory
        extends Object
        implements ActionGraphFactoryDelegate
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        -   []{#nested.classes.inherited.from.class.com.facebook.buck.core.model.actiongraph.computation.ActionGraphFactoryDelegate}

            ### Nested classes/interfaces inherited from interface com.facebook.buck.core.model.actiongraph.computation.[ActionGraphFactoryDelegate](ActionGraphFactoryDelegate.html "interface in com.facebook.buck.core.model.actiongraph.computation")

            `ActionGraphFactoryDelegate.ActionGraphBuilderDecorator`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                   Description
          --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `ParallelActionGraphFactory​(java.util.function.Supplier<com.google.common.util.concurrent.ListeningExecutorService> executorSupplier,                           CellProvider cellProvider)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type         Method                                                                                                                                                                                                                                                                                                                                     Description
          ------------------------- ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ -------------
          `ActionGraphAndBuilder`   `create​(TargetNodeToBuildRuleTransformer transformer,       TargetGraph targetGraph,       com.facebook.buck.core.model.actiongraph.computation.ActionGraphFactory.ActionGraphCreationLifecycleListener actionGraphCreationLifecycleListener,       ActionGraphFactoryDelegate.ActionGraphBuilderDecorator actionGraphBuilderDecorator)`    

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

        []{#<init>(java.util.function.Supplier,com.facebook.buck.core.cell.CellProvider)}

        -   #### ParallelActionGraphFactory

                public ParallelActionGraphFactory​(java.util.function.Supplier<com.google.common.util.concurrent.ListeningExecutorService> executorSupplier,
                                                  CellProvider cellProvider)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#create(com.facebook.buck.core.rules.transformer.TargetNodeToBuildRuleTransformer,com.facebook.buck.core.model.targetgraph.TargetGraph,com.facebook.buck.core.model.actiongraph.computation.ActionGraphFactory.ActionGraphCreationLifecycleListener,com.facebook.buck.core.model.actiongraph.computation.ActionGraphFactoryDelegate.ActionGraphBuilderDecorator)}

        -   #### create

            ``` methodSignature
            public ActionGraphAndBuilder create​(TargetNodeToBuildRuleTransformer transformer,
                                                TargetGraph targetGraph,
                                                com.facebook.buck.core.model.actiongraph.computation.ActionGraphFactory.ActionGraphCreationLifecycleListener actionGraphCreationLifecycleListener,
                                                ActionGraphFactoryDelegate.ActionGraphBuilderDecorator actionGraphBuilderDecorator)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `create` in interface `ActionGraphFactoryDelegate`
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
