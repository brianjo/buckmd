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

-   [Overview](../../../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../../index-all.html)
-   [Help](../../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.features.project.intellij.lang.java](package-summary.html)
:::

## Class JavaLibraryRuleHelper {#class-javalibraryrulehelper .title title="Class JavaLibraryRuleHelper"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.features.project.intellij.lang.java.JavaLibraryRuleHelper

::: description
-   

    ------------------------------------------------------------------------

        public class JavaLibraryRuleHelper
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static <T ex         | `addCompiledSha       |                       |
        | tends JavaLibraryDesc | dowIfNeeded​(IjProject |                       |
        | ription.CoreArg>void` | Config projectConfig, |                       |
        |                       |                       |                       |
        |                       |      TargetNode<T> ta |                       |
        |                       | rgetNode,             |                       |
        |                       |               ModuleB |                       |
        |                       | uildContext context)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static <T ex         | `addLanguageAg        | ::: block             |
        | tends JavaLibraryDesc | gregationKeyIfNeeded​( | Helper method to add  |
        | ription.CoreArg>void` | IjProjectConfig proje | aggregation key of    |
        |                       | ctConfig,             | JAVA_LANGUAGE_LEVEL   |
        |                       |                       | if the target         |
        |                       |  TargetNode<T> target | specifies a language  |
        |                       | ,                     | level                 |
        |                       |               Aggrega | :::                   |
        |                       | tionContext context)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static <T ex         | `addNonSourceBuildTa  |                       |
        | tends JavaLibraryDesc | rgets​(TargetNode<T> t |                       |
        | ription.CoreArg>void` | argetNode,            |                       |
        |                       |               ModuleB |                       |
        |                       | uildContext context)` |                       |
        +-----------------------+-----------------------+-----------------------+

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

        []{#addCompiledShadowIfNeeded(com.facebook.buck.features.project.intellij.model.IjProjectConfig,com.facebook.buck.core.model.targetgraph.TargetNode,com.facebook.buck.features.project.intellij.ModuleBuildContext)}

        -   #### addCompiledShadowIfNeeded

            ``` methodSignature
            public static <T extends JavaLibraryDescription.CoreArg> void addCompiledShadowIfNeeded​(IjProjectConfig projectConfig,
                                                                                                    TargetNode<T> targetNode,
                                                                                                    ModuleBuildContext context)
            ```

        []{#addNonSourceBuildTargets(com.facebook.buck.core.model.targetgraph.TargetNode,com.facebook.buck.features.project.intellij.ModuleBuildContext)}

        -   #### addNonSourceBuildTargets

            ``` methodSignature
            public static <T extends JavaLibraryDescription.CoreArg> void addNonSourceBuildTargets​(TargetNode<T> targetNode,
                                                                                                   ModuleBuildContext context)
            ```

        []{#addLanguageAggregationKeyIfNeeded(com.facebook.buck.features.project.intellij.model.IjProjectConfig,com.facebook.buck.core.model.targetgraph.TargetNode,com.facebook.buck.features.project.intellij.aggregation.AggregationContext)}

        -   #### addLanguageAggregationKeyIfNeeded

            ``` methodSignature
            public static <T extends JavaLibraryDescription.CoreArg> void addLanguageAggregationKeyIfNeeded​(IjProjectConfig projectConfig,
                                                                                                            TargetNode<T> target,
                                                                                                            AggregationContext context)
            ```

            ::: block
            Helper method to add aggregation key of JAVA_LANGUAGE_LEVEL
            if the target specifies a language level
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

-   [Overview](../../../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../../index-all.html)
-   [Help](../../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../../allclasses.html)

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
