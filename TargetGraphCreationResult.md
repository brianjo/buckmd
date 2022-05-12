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
[Package]{.packageLabelInType} [com.facebook.buck.core.model.targetgraph](package-summary.html)
:::

## Class TargetGraphCreationResult {#class-targetgraphcreationresult .title title="Class TargetGraphCreationResult"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.model.targetgraph.TargetGraphCreationResult

::: description
-   

    ------------------------------------------------------------------------

        public abstract class TargetGraphCreationResult
        extends Object

    ::: block
    Contains information produced as a result of the phase of target
    graph creation.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                     Description
          ------------------------------- -------------
          `TargetGraphCreationResult()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `abstract com.google  | `getBuildTargets()`   | ::: block             |
        | .common.collect.Immut |                       | Top level targets of  |
        | ableSet<BuildTarget>` |                       | the target graph.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getTargetGraph()`    | ::: block             |
        | abstract TargetGraph` |                       | A graph of transitive |
        |                       |                       | dependencies of the   |
        |                       |                       | top level targets     |
        |                       |                       | from                  |
        |                       |                       | [`getBuildTargets()`] |
        |                       |                       | (#getBuildTargets()). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static Targe         | `of​(TargetGra         |                       |
        | tGraphCreationResult` | ph targetGraph,   com |                       |
        |                       | .google.common.collec |                       |
        |                       | t.ImmutableSet<BuildT |                       |
        |                       | arget> buildTargets)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Targe                | `withBuildTargets​(    | ::: block             |
        | tGraphCreationResult` | Iterable<? extends Bu | Copies this object    |
        |                       | ildTarget> elements)` | with replacing the    |
        |                       |                       | top level targets.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Targe                | `withTargetGraph​(Targ | ::: block             |
        | tGraphCreationResult` | etGraph targetGraph)` | Copies this object    |
        |                       |                       | with replacing the    |
        |                       |                       | target graph.         |
        |                       |                       | :::                   |
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
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### TargetGraphCreationResult

                public TargetGraphCreationResult()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getTargetGraph()}

        -   #### getTargetGraph

            ``` methodSignature
            public abstract TargetGraph getTargetGraph()
            ```

            ::: block
            A graph of transitive dependencies of the top level targets
            from [`getBuildTargets()`](#getBuildTargets()).
            :::

        []{#getBuildTargets()}

        -   #### getBuildTargets

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableSet<BuildTarget> getBuildTargets()
            ```

            ::: block
            Top level targets of the target graph.
            A top level target is a target requested by a client during
            target graph creation request.

            Note that top level targets are not equal to the nodes
            without incoming edges. A top level target can be in a
            transitive dependencies of another top level target and can
            have incoming edges.
            :::

        []{#withTargetGraph(com.facebook.buck.core.model.targetgraph.TargetGraph)}

        -   #### withTargetGraph

            ``` methodSignature
            public TargetGraphCreationResult withTargetGraph​(TargetGraph targetGraph)
            ```

            ::: block
            Copies this object with replacing the target graph.
            :::

        []{#withBuildTargets(java.lang.Iterable)}

        -   #### withBuildTargets

            ``` methodSignature
            public TargetGraphCreationResult withBuildTargets​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Copies this object with replacing the top level targets.
            :::

        []{#of(com.facebook.buck.core.model.targetgraph.TargetGraph,com.google.common.collect.ImmutableSet)}

        -   #### of

            ``` methodSignature
            public static TargetGraphCreationResult of​(TargetGraph targetGraph,
                                                       com.google.common.collect.ImmutableSet<BuildTarget> buildTargets)
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
