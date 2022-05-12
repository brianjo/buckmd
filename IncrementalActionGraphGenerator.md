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
[Package]{.packageLabelInType} [com.facebook.buck.core.model.actiongraph.computation](package-summary.html)
:::

## Class IncrementalActionGraphGenerator {#class-incrementalactiongraphgenerator .title title="Class IncrementalActionGraphGenerator"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.model.actiongraph.computation.IncrementalActionGraphGenerator

::: description
-   

    ------------------------------------------------------------------------

        public class IncrementalActionGraphGenerator
        extends Object

    ::: block
    Provides a way to incrementally construct a new
    [`ActionGraphBuilder`](../../../rules/ActionGraphBuilder.html "interface in com.facebook.buck.core.rules")
    from a previous one.
    This works by grabbing all the build rules from the previous
    [`ActionGraphBuilder`](../../../rules/ActionGraphBuilder.html "interface in com.facebook.buck.core.rules")
    with unflavored targets that were not invalidated when doing a
    target graph walk to check for changes.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                           Description
          ------------------------------------- -------------
          `IncrementalActionGraphGenerator()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `void`                | `populateActionGr     | ::: block             |
        |                       | aphBuilderWithCachedR | Populates the given   |
        |                       | ules​(BuckEventBus eve | [                     |
        |                       | ntBus,                | `ActionGraphBuilder`] |
        |                       |                       | (../../../rules/Actio |
        |                       |       TargetGraph tar | nGraphBuilder.html "i |
        |                       | getGraph,             | nterface in com.faceb |
        |                       |                       | ook.buck.core.rules") |
        |                       |          ActionGraphB | with the rules from   |
        |                       | uilder graphBuilder)` | the previously used   |
        |                       |                       | [                     |
        |                       |                       | `ActionGraphBuilder`] |
        |                       |                       | (../../../rules/Actio |
        |                       |                       | nGraphBuilder.html "i |
        |                       |                       | nterface in com.faceb |
        |                       |                       | ook.buck.core.rules") |
        |                       |                       | that are deemed       |
        |                       |                       | usable after checking |
        |                       |                       | for invalidations     |
        |                       |                       | with a target graph   |
        |                       |                       | walk.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

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

        []{#<init>()}

        -   #### IncrementalActionGraphGenerator

                public IncrementalActionGraphGenerator()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#populateActionGraphBuilderWithCachedRules(com.facebook.buck.event.BuckEventBus,com.facebook.buck.core.model.targetgraph.TargetGraph,com.facebook.buck.core.rules.ActionGraphBuilder)}

        -   #### populateActionGraphBuilderWithCachedRules

            ``` methodSignature
            public void populateActionGraphBuilderWithCachedRules​(BuckEventBus eventBus,
                                                                  TargetGraph targetGraph,
                                                                  ActionGraphBuilder graphBuilder)
            ```

            ::: block
            Populates the given
            [`ActionGraphBuilder`](../../../rules/ActionGraphBuilder.html "interface in com.facebook.buck.core.rules")
            with the rules from the previously used
            [`ActionGraphBuilder`](../../../rules/ActionGraphBuilder.html "interface in com.facebook.buck.core.rules")
            that are deemed usable after checking for invalidations with
            a target graph walk.
            :::
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
