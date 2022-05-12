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
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   Constr \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.features.project.intellij](package-summary.html)
:::

## Class IjModuleGraphFactory {#class-ijmodulegraphfactory .title title="Class IjModuleGraphFactory"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.features.project.intellij.IjModuleGraphFactory

::: description
-   

    ------------------------------------------------------------------------

        public final class IjModuleGraphFactory
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type        Method                                                                                                                                                                                                                                       Description
          ------------------------ -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `static IjModuleGraph`   `from​(ProjectFilesystem projectFilesystem,     IjProjectConfig projectConfig,     TargetGraph targetGraph,     IjLibraryFactory libraryFactory,     IjModuleFactory moduleFactory,     AggregationModuleFactory aggregationModuleFactory)`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
          Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#from(com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.features.project.intellij.model.IjProjectConfig,com.facebook.buck.core.model.targetgraph.TargetGraph,com.facebook.buck.features.project.intellij.model.IjLibraryFactory,com.facebook.buck.features.project.intellij.model.IjModuleFactory,com.facebook.buck.features.project.intellij.aggregation.AggregationModuleFactory)}

        -   #### from

            ``` methodSignature
            public static IjModuleGraph from​(ProjectFilesystem projectFilesystem,
                                             IjProjectConfig projectConfig,
                                             TargetGraph targetGraph,
                                             IjLibraryFactory libraryFactory,
                                             IjModuleFactory moduleFactory,
                                             AggregationModuleFactory aggregationModuleFactory)
            ```

            [Parameters:]{.paramLabel}
            :   `projectConfig` - the project config used
            :   `targetGraph` - input graph.
            :   `libraryFactory` - library factory.
            :   `moduleFactory` - module factory.

            [Returns:]{.returnLabel}
            :   module graph corresponding to the supplied
                [`TargetGraph`](../../../core/model/targetgraph/TargetGraph.html "class in com.facebook.buck.core.model.targetgraph").
                Multiple targets from the same base path are mapped to a
                single module, therefore an IjModuleGraph edge exists
                between two modules (Ma, Mb) if a TargetGraph edge
                existed between a pair of nodes (Ta, Tb) and Ma contains
                Ta and Mb contains Tb.
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
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   Constr \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
