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

-   [Overview](../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../deprecated-list.html)
-   [Index](../../../../../index-all.html)
-   [Help](../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.rules.macros](package-summary.html)
:::

## Class QueryMacroExpander\<T extends [QueryMacro](QueryMacro.html "class in com.facebook.buck.rules.macros")\> {#class-querymacroexpandert-extends-querymacro .title title="Class QueryMacroExpander"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.rules.macros.QueryMacroExpander\<T\>

::: description
-   

    All Implemented Interfaces:
    :   `MacroExpander<T,​QueryMacroExpander.QueryResults>`

    ```{=html}
    <!-- -->
    ```

    Direct Known Subclasses:
    :   `QueryOutputsMacroExpander`, `QueryPathsMacroExpander`,
        `QueryTargetsAndOutputsMacroExpander`,
        `QueryTargetsMacroExpander`

    ------------------------------------------------------------------------

        public abstract class QueryMacroExpander<T extends QueryMacro>
        extends Object
        implements MacroExpander<T,​QueryMacroExpander.QueryResults>

    ::: block
    Abstract base class for the query_targets and query_outputs macros
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type           Class                               Description
          --------------------------- ----------------------------------- -------------
          `protected static class `   `QueryMacroExpander.QueryResults`    

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                     Description
          ----------------------------------------------- -------------
          `QueryMacroExpander​(TargetGraph targetGraph)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                   Method                                                                                                                                                                 Description
          ----------------------------------- ---------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `QueryMacroExpander.QueryResults`   `precomputeWorkFrom​(BuildTarget target,                   CellNameResolver cellNames,                   ActionGraphBuilder graphBuilder,                   T input)`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.rules.macros.MacroExpander}

            ### Methods inherited from interface com.facebook.buck.rules.macros.[MacroExpander](MacroExpander.html "interface in com.facebook.buck.rules.macros")

            `expandFrom, getInputClass`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.core.model.targetgraph.TargetGraph)}

        -   #### QueryMacroExpander

                public QueryMacroExpander​(TargetGraph targetGraph)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#precomputeWorkFrom(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.cell.nameresolver.CellNameResolver,com.facebook.buck.core.rules.ActionGraphBuilder,com.facebook.buck.rules.macros.QueryMacro)}
        []{#precomputeWorkFrom(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.cell.nameresolver.CellNameResolver,com.facebook.buck.core.rules.ActionGraphBuilder,T)}

        -   #### precomputeWorkFrom

            ``` methodSignature
            public QueryMacroExpander.QueryResults precomputeWorkFrom​(BuildTarget target,
                                                                      CellNameResolver cellNames,
                                                                      ActionGraphBuilder graphBuilder,
                                                                      T input)
                                                               throws MacroException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `precomputeWorkFrom` in
                interface `MacroExpander<T extends QueryMacro,​QueryMacroExpander.QueryResults>`

            [Returns:]{.returnLabel}
            :   the precomputed work that can be re-used between
                invocations

            [Throws:]{.throwsLabel}
            :   `MacroException`
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

-   [Overview](../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../deprecated-list.html)
-   [Index](../../../../../index-all.html)
-   [Help](../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../allclasses.html)

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
