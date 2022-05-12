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
[Package]{.packageLabelInType} [com.facebook.buck.core.rules.common](package-summary.html)
:::

## Class BuildRuleDependencyVisitors {#class-buildruledependencyvisitors .title title="Class BuildRuleDependencyVisitors"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.rules.common.BuildRuleDependencyVisitors

::: description
-   

    ------------------------------------------------------------------------

        public class BuildRuleDependencyVisitors
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `s                    | `getBu                | ::: block             |
        | tatic <T> DirectedAcy | ildRuleDirectedGraphF | Given dependencies in |
        | clicGraph<BuildRule>` | ilteredBy​(Iterable<?  | inputs builds graph   |
        |                       | extends BuildRule> in | of transitive         |
        |                       | puts,                 | dependencies          |
        |                       |                     j | filtering them by     |
        |                       | ava.util.function.Pre | instanceOf T.         |
        |                       | dicate<Object> filter | :::                   |
        |                       | ,                     |                       |
        |                       |                 java. |                       |
        |                       | util.function.Predica |                       |
        |                       | te<Object> traverse)` |                       |
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

        []{#getBuildRuleDirectedGraphFilteredBy(java.lang.Iterable,java.util.function.Predicate,java.util.function.Predicate)}

        -   #### getBuildRuleDirectedGraphFilteredBy

            ``` methodSignature
            public static <T> DirectedAcyclicGraph<BuildRule> getBuildRuleDirectedGraphFilteredBy​(Iterable<? extends BuildRule> inputs,
                                                                                                  java.util.function.Predicate<Object> filter,
                                                                                                  java.util.function.Predicate<Object> traverse)
            ```

            ::: block
            Given dependencies in inputs builds graph of transitive
            dependencies filtering them by instanceOf T.
            :::

            [Type Parameters:]{.paramLabel}
            :   `T` - class to fitler on

            [Parameters:]{.paramLabel}
            :   `inputs` - initial dependencies from which to build
                transitive closure
            :   `filter` - predicate to determine whether a node should
                be included
            :   `traverse` - predicate to determine whether this node
                should be traversed

            [Returns:]{.returnLabel}
            :   filtered BuildRule DAG of transitive dependencies

            [See Also:]{.seeLabel}
            :   [`BuildRule`](../BuildRule.html "interface in com.facebook.buck.core.rules")
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
