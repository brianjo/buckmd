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
[Package]{.packageLabelInType} [com.facebook.buck.features.project.intellij](package-summary.html)
:::

## Class ExportedDepsClosureResolver {#class-exporteddepsclosureresolver .title title="Class ExportedDepsClosureResolver"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.features.project.intellij.ExportedDepsClosureResolver

::: description
-   

    ------------------------------------------------------------------------

        public class ExportedDepsClosureResolver
        extends Object

    ::: block
    Calculates the transitive closure of exported deps for every node in
    a
    [`TargetGraph`](../../../core/model/targetgraph/TargetGraph.html "class in com.facebook.buck.core.model.targetgraph").
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                             Description
          ------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `ExportedDepsClosureResolver​(TargetGraph targetGraph,                            com.google.common.collect.ImmutableSet<String> ignoredTargetLabels)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                       Method                                              Description
          ------------------------------------------------------- --------------------------------------------------- -------------
          `com.google.common.collect.ImmutableSet<BuildTarget>`   `getExportedDepsClosure​(BuildTarget buildTarget)`    

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

        []{#<init>(com.facebook.buck.core.model.targetgraph.TargetGraph,com.google.common.collect.ImmutableSet)}

        -   #### ExportedDepsClosureResolver

                public ExportedDepsClosureResolver​(TargetGraph targetGraph,
                                                   com.google.common.collect.ImmutableSet<String> ignoredTargetLabels)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getExportedDepsClosure(com.facebook.buck.core.model.BuildTarget)}

        -   #### getExportedDepsClosure

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<BuildTarget> getExportedDepsClosure​(BuildTarget buildTarget)
            ```

            [Parameters:]{.paramLabel}
            :   `buildTarget` - target to process.

            [Returns:]{.returnLabel}
            :   the set of
                [`BuildTarget`](../../../core/model/BuildTarget.html "class in com.facebook.buck.core.model")s
                that must be appended to the dependencies of a node Y if
                node Y depends on X.
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