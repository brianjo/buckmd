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
-   Nested \| 
-   [Field](#field.summary) \| 
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.rules.macros](package-summary.html)
:::

## Class AbsoluteOutputMacroExpander {#class-absoluteoutputmacroexpander .title title="Class AbsoluteOutputMacroExpander"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.rules.macros.AbstractMacroExpanderWithoutPrecomputedWork](AbstractMacroExpanderWithoutPrecomputedWork.html "class in com.facebook.buck.rules.macros")\<[AbsoluteOutputMacro](AbsoluteOutputMacro.html "class in com.facebook.buck.rules.macros")\>

    -   -   com.facebook.buck.rules.macros.AbsoluteOutputMacroExpander

::: description
-   

    All Implemented Interfaces:
    :   `MacroExpander<AbsoluteOutputMacro,​Object>`

    ------------------------------------------------------------------------

        public class AbsoluteOutputMacroExpander
        extends AbstractMacroExpanderWithoutPrecomputedWork<AbsoluteOutputMacro>

    ::: block
    Handles \'\$(abs_output \...)\' macro which expands to the path of a
    named supplementary output.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type                      Field        Description
          -------------------------------------- ------------ -------------
          `static AbsoluteOutputMacroExpander`   `INSTANCE`    

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type              Method                                                                                                             Description
          ------------------------------ ------------------------------------------------------------------------------------------------------------------ -------------
          `Arg`                          `expandFrom​(BuildTarget target,           ActionGraphBuilder graphBuilder,           AbsoluteOutputMacro input)`    
          `Class<AbsoluteOutputMacro>`   `getInputClass()`                                                                                                   

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.rules.macros.AbstractMacroExpanderWithoutPrecomputedWork}

            ### Methods inherited from class com.facebook.buck.rules.macros.[AbstractMacroExpanderWithoutPrecomputedWork](AbstractMacroExpanderWithoutPrecomputedWork.html "class in com.facebook.buck.rules.macros")

            `expandFrom, precomputeWorkFrom`

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
    -   []{#field.detail}

        ### Field Detail

        []{#INSTANCE}

        -   #### INSTANCE

                public static final AbsoluteOutputMacroExpander INSTANCE
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getInputClass()}

        -   #### getInputClass

            ``` methodSignature
            public Class<AbsoluteOutputMacro> getInputClass()
            ```

            [Returns:]{.returnLabel}
            :   the class for the parsed macro input type.

        []{#expandFrom(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.rules.ActionGraphBuilder,com.facebook.buck.rules.macros.AbsoluteOutputMacro)}

        -   #### expandFrom

            ``` methodSignature
            public Arg expandFrom​(BuildTarget target,
                                  ActionGraphBuilder graphBuilder,
                                  AbsoluteOutputMacro input)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `expandFrom` in
                class `AbstractMacroExpanderWithoutPrecomputedWork<AbsoluteOutputMacro>`
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
-   Nested \| 
-   [Field](#field.summary) \| 
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
-   Constr \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
