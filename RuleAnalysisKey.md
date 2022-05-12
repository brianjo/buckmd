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
-   [Field](#field.summary) \| 
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.core.rules.analysis](package-summary.html)
:::

## Class RuleAnalysisKey {#class-ruleanalysiskey .title title="Class RuleAnalysisKey"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.rules.analysis.RuleAnalysisKey

::: description
-   

    All Implemented Interfaces:
    :   `ComputeKey<RuleAnalysisResult>`

    ------------------------------------------------------------------------

        public abstract class RuleAnalysisKey
        extends Object
        implements ComputeKey<RuleAnalysisResult>

    ::: block
    The key of a computation of the
    [`TargetGraph`](../../model/targetgraph/TargetGraph.html "class in com.facebook.buck.core.model.targetgraph")
    to its corresponding `Provider`s and
    [`ActionAnalysisData`](action/ActionAnalysisData.html "interface in com.facebook.buck.core.rules.analysis.action").
    This key will be used to indicate which rule\'s analysis we are
    currently interested in.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type                                    Field          Description
          ---------------------------------------------------- -------------- -------------
          `static ComputationIdentifier<RuleAnalysisResult>`   `IDENTIFIER`    

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor           Description
          --------------------- -------------
          `RuleAnalysisKey()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `                     | `getBuildTarget()`    | ::: block             |
        | abstract BuildTarget` |                       | TODO(bobyf) this      |
        |                       |                       | really should be a    |
        |                       |                       | ConfiguredBuildTarget |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getIdentifier()`     |                       |
        | ComputationIdentifier |                       |                       |
        | <RuleAnalysisResult>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `st                   | `of​(Buil              |                       |
        | atic RuleAnalysisKey` | dTarget buildTarget)` |                       |
        +-----------------------+-----------------------+-----------------------+

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
    -   []{#field.detail}

        ### Field Detail

        []{#IDENTIFIER}

        -   #### IDENTIFIER

                public static final ComputationIdentifier<RuleAnalysisResult> IDENTIFIER
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### RuleAnalysisKey

                public RuleAnalysisKey()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getBuildTarget()}

        -   #### getBuildTarget

            ``` methodSignature
            public abstract BuildTarget getBuildTarget()
            ```

            ::: block
            TODO(bobyf) this really should be a ConfiguredBuildTarget
            :::

            [Returns:]{.returnLabel}
            :   the
                [`BuildTarget`](../../model/BuildTarget.html "class in com.facebook.buck.core.model")
                of this key

        []{#getIdentifier()}

        -   #### getIdentifier

            ``` methodSignature
            public ComputationIdentifier<RuleAnalysisResult> getIdentifier()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getIdentifier` in
                interface `ComputeKey<RuleAnalysisResult>`

            [Returns:]{.returnLabel}
            :   the identifier of this key. This identifier is used to
                map all keys of the same
                [`ComputationIdentifier`](../../graph/transformation/model/ComputationIdentifier.html "interface in com.facebook.buck.core.graph.transformation.model")
                to the same
                [`GraphComputation`](../../graph/transformation/GraphComputation.html "interface in com.facebook.buck.core.graph.transformation").

        []{#of(com.facebook.buck.core.model.BuildTarget)}

        -   #### of

            ``` methodSignature
            public static RuleAnalysisKey of​(BuildTarget buildTarget)
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
-   [Field](#field.summary) \| 
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
-   [Constr](#constructor.detail) \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
