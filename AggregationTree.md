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
[Package]{.packageLabelInType} [com.facebook.buck.features.project.intellij.aggregation](package-summary.html)
:::

## Class AggregationTree {#class-aggregationtree .title title="Class AggregationTree"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.features.project.intellij.aggregation.AggregationTree

::: description
-   

    All Implemented Interfaces:
    :   `GraphTraversable<com.facebook.buck.features.project.intellij.aggregation.AggregationTreeNode>`

    ------------------------------------------------------------------------

        public class AggregationTree
        extends Object
        implements GraphTraversable<com.facebook.buck.features.project.intellij.aggregation.AggregationTreeNode>

    ::: block
    A tree that is responsible for managing and aggregating modules.
    The tree accepts an arbitrary number of modules each of which is
    located at a specific location.

    The tree can aggregate the modules by merging modules with the same
    aggregation tag into one module. The aggregation happens at some
    specific level.

    This data structure is based on a [prefix
    tree](https://en.wikipedia.org/wiki/Trie).
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                 Description
          ------------------------------------------------------------------------------------------- -------------
          `AggregationTree​(IjProjectConfig projectConfig,                AggregationModule module)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                                         Method                                                                                             Description
          ----------------------------------------------------------------------------------------- -------------------------------------------------------------------------------------------------- -------------
          `void`                                                                                    `addModule​(Path moduleBasePath,          AggregationModule module)`                                 
          `void`                                                                                    `aggregateModules​(int minimumPathDepth)`                                                            
          `Iterator<com.facebook.buck.features.project.intellij.aggregation.AggregationTreeNode>`   `findChildren​(com.facebook.buck.features.project.intellij.aggregation.AggregationTreeNode node)`    
          `Collection<AggregationModule>`                                                           `getModules()`                                                                                      

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

        []{#<init>(com.facebook.buck.features.project.intellij.model.IjProjectConfig,com.facebook.buck.features.project.intellij.aggregation.AggregationModule)}

        -   #### AggregationTree

                public AggregationTree​(IjProjectConfig projectConfig,
                                       AggregationModule module)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#addModule(java.nio.file.Path,com.facebook.buck.features.project.intellij.aggregation.AggregationModule)}

        -   #### addModule

            ``` methodSignature
            public void addModule​(Path moduleBasePath,
                                  AggregationModule module)
            ```

        []{#findChildren(com.facebook.buck.features.project.intellij.aggregation.AggregationTreeNode)}

        -   #### findChildren

            ``` methodSignature
            public Iterator<com.facebook.buck.features.project.intellij.aggregation.AggregationTreeNode> findChildren​(com.facebook.buck.features.project.intellij.aggregation.AggregationTreeNode node)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `findChildren` in
                interface `GraphTraversable<com.facebook.buck.features.project.intellij.aggregation.AggregationTreeNode>`

        []{#aggregateModules(int)}

        -   #### aggregateModules

            ``` methodSignature
            public void aggregateModules​(int minimumPathDepth)
            ```

        []{#getModules()}

        -   #### getModules

            ``` methodSignature
            public Collection<AggregationModule> getModules()
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
