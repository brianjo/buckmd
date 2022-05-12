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

## Class AbstractMacroExpanderWithoutPrecomputedWork\<T\> {#class-abstractmacroexpanderwithoutprecomputedworkt .title title="Class AbstractMacroExpanderWithoutPrecomputedWork"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.rules.macros.AbstractMacroExpanderWithoutPrecomputedWork\<T\>

::: description
-   

    All Implemented Interfaces:
    :   `MacroExpander<T,​Object>`

    ```{=html}
    <!-- -->
    ```

    Direct Known Subclasses:
    :   `AbsoluteOutputMacroExpander`, `BuildTargetMacroExpander`,
        `EnvironmentVariableMacroExpander`, `OutputMacroExpander`,
        `SimpleMacroExpander`

    ------------------------------------------------------------------------

        public abstract class AbstractMacroExpanderWithoutPrecomputedWork<T>
        extends Object
        implements MacroExpander<T,​Object>
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                       Description
          ------------------------------------------------- -------------
          `AbstractMacroExpanderWithoutPrecomputedWork()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                                                                                                                                                                 Description
          ------------------- ---------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `abstract Arg`      `expandFrom​(BuildTarget target,           ActionGraphBuilder graphBuilder,           T input)`                                                                          
          `Arg`               `expandFrom​(BuildTarget target,           ActionGraphBuilder graphBuilder,           T input,           Object precomputedWork)`                                        
          `Object`            `precomputeWorkFrom​(BuildTarget target,                   CellNameResolver cellNames,                   ActionGraphBuilder graphBuilder,                   T input)`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Abstract
          Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
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

            `getInputClass`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### AbstractMacroExpanderWithoutPrecomputedWork

                public AbstractMacroExpanderWithoutPrecomputedWork()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#precomputeWorkFrom(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.cell.nameresolver.CellNameResolver,com.facebook.buck.core.rules.ActionGraphBuilder,java.lang.Object)}
        []{#precomputeWorkFrom(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.cell.nameresolver.CellNameResolver,com.facebook.buck.core.rules.ActionGraphBuilder,T)}

        -   #### precomputeWorkFrom

            ``` methodSignature
            public final Object precomputeWorkFrom​(BuildTarget target,
                                                   CellNameResolver cellNames,
                                                   ActionGraphBuilder graphBuilder,
                                                   T input)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `precomputeWorkFrom` in
                interface `MacroExpander<T,​Object>`

            [Returns:]{.returnLabel}
            :   the precomputed work that can be re-used between
                invocations

        []{#expandFrom(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.rules.ActionGraphBuilder,java.lang.Object,java.lang.Object)}
        []{#expandFrom(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.rules.ActionGraphBuilder,T,java.lang.Object)}

        -   #### expandFrom

            ``` methodSignature
            public final Arg expandFrom​(BuildTarget target,
                                        ActionGraphBuilder graphBuilder,
                                        T input,
                                        Object precomputedWork)
                                 throws MacroException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `expandFrom` in interface `MacroExpander<T,​Object>`

            [Throws:]{.throwsLabel}
            :   `MacroException`

        []{#expandFrom(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.rules.ActionGraphBuilder,java.lang.Object)}
        []{#expandFrom(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.rules.ActionGraphBuilder,T)}

        -   #### expandFrom

            ``` methodSignature
            public abstract Arg expandFrom​(BuildTarget target,
                                           ActionGraphBuilder graphBuilder,
                                           T input)
                                    throws MacroException
            ```

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
