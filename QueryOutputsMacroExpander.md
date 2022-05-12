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

## Class QueryOutputsMacroExpander {#class-queryoutputsmacroexpander .title title="Class QueryOutputsMacroExpander"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.rules.macros.QueryMacroExpander](QueryMacroExpander.html "class in com.facebook.buck.rules.macros")\<[QueryOutputsMacro](QueryOutputsMacro.html "class in com.facebook.buck.rules.macros")\>

    -   -   com.facebook.buck.rules.macros.QueryOutputsMacroExpander

::: description
-   

    All Implemented Interfaces:
    :   `MacroExpander<QueryOutputsMacro,​QueryMacroExpander.QueryResults>`

    ------------------------------------------------------------------------

        public class QueryOutputsMacroExpander
        extends QueryMacroExpander<QueryOutputsMacro>

    ::: block
    Used to expand the macro \$(query_outputs
    \"some(query(:expression))\") to the set of the outputs of the
    targets matching the query. Example queries
           '$(query_outputs "deps(:foo)")'
           '$(query_outputs "filter(bar, classpath(:bar))")'
           '$(query_outputs "attrfilter(annotation_processors, com.foo.Processor, deps(:app))")'
         
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        -   []{#nested.classes.inherited.from.class.com.facebook.buck.rules.macros.QueryMacroExpander}

            ### Nested classes/interfaces inherited from class com.facebook.buck.rules.macros.[QueryMacroExpander](QueryMacroExpander.html "class in com.facebook.buck.rules.macros")

            `QueryMacroExpander.QueryResults`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                            Description
          ------------------------------------------------------ -------------
          `QueryOutputsMacroExpander​(TargetGraph targetGraph)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type            Method                                                                                                                                                                      Description
          ---------------------------- --------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `Arg`                        `expandFrom​(BuildTarget target,           ActionGraphBuilder graphBuilder,           QueryOutputsMacro input,           QueryMacroExpander.QueryResults precomputedWork)`    
          `Class<QueryOutputsMacro>`   `getInputClass()`                                                                                                                                                            

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.rules.macros.QueryMacroExpander}

            ### Methods inherited from class com.facebook.buck.rules.macros.[QueryMacroExpander](QueryMacroExpander.html "class in com.facebook.buck.rules.macros")

            `precomputeWorkFrom`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.core.model.targetgraph.TargetGraph)}

        -   #### QueryOutputsMacroExpander

                public QueryOutputsMacroExpander​(TargetGraph targetGraph)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getInputClass()}

        -   #### getInputClass

            ``` methodSignature
            public Class<QueryOutputsMacro> getInputClass()
            ```

            [Returns:]{.returnLabel}
            :   the class for the parsed macro input type.

        []{#expandFrom(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.rules.ActionGraphBuilder,com.facebook.buck.rules.macros.QueryOutputsMacro,com.facebook.buck.rules.macros.QueryMacroExpander.QueryResults)}

        -   #### expandFrom

            ``` methodSignature
            public Arg expandFrom​(BuildTarget target,
                                  ActionGraphBuilder graphBuilder,
                                  QueryOutputsMacro input,
                                  QueryMacroExpander.QueryResults precomputedWork)
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
