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

## Class AggregationModule {#class-aggregationmodule .title title="Class AggregationModule"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.features.project.intellij.aggregation.AggregationModule

::: description
-   

    ------------------------------------------------------------------------

        public abstract class AggregationModule
        extends Object

    ::: block
    Represents a module during aggregation.
    This module is used only for aggregation and discarded after. It
    contains a minimal information necessary to create
    [`IjModule`](../model/IjModule.html "class in com.facebook.buck.features.project.intellij.model").
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor             Description
          ----------------------- -------------
          `AggregationModule()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `abstract String`     | `getAggregationTag()` | ::: block             |
        |                       |                       | Uniquely identifies   |
        |                       |                       | the type of this      |
        |                       |                       | module for            |
        |                       |                       | aggregation purpose.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `abstract com         | `getExcludes()`       | ::: block             |
        | .google.common.collec |                       | A set of paths that   |
        | t.ImmutableSet<Path>` |                       | need to be excluded   |
        |                       |                       | from the final        |
        |                       |                       | [`IjModule`](.        |
        |                       |                       | ./model/IjModule.html |
        |                       |                       |  "class in com.facebo |
        |                       |                       | ok.buck.features.proj |
        |                       |                       | ect.intellij.model"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `abstract Path`       | `getModuleBasePath()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `a                    | `getModuleType()`     |                       |
        | bstract IjModuleType` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract com.googl   | `getTargets()`        |                       |
        | e.common.collect.Immu |                       |                       |
        | tableSet<TargetNode>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}

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

        -   #### AggregationModule

                public AggregationModule()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getTargets()}

        -   #### getTargets

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableSet<TargetNode> getTargets()
            ```

        []{#getModuleBasePath()}

        -   #### getModuleBasePath

            ``` methodSignature
            public abstract Path getModuleBasePath()
            ```

            [Returns:]{.returnLabel}
            :   path to the top-most directory the module is responsible
                for. This is also where the corresponding .iml file is
                located.

        []{#getAggregationTag()}

        -   #### getAggregationTag

            ``` methodSignature
            public abstract String getAggregationTag()
            ```

            ::: block
            Uniquely identifies the type of this module for aggregation
            purpose.
            Modules with the same aggregation tag can be aggregated into
            one module.
            :::

        []{#getModuleType()}

        -   #### getModuleType

            ``` methodSignature
            public abstract IjModuleType getModuleType()
            ```

        []{#getExcludes()}

        -   #### getExcludes

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableSet<Path> getExcludes()
            ```

            ::: block
            A set of paths that need to be excluded from the final
            [`IjModule`](../model/IjModule.html "class in com.facebook.buck.features.project.intellij.model").
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
