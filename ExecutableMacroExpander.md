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

## Class ExecutableMacroExpander\<M extends [AbstractExecutableTargetOrHostMacro](AbstractExecutableTargetOrHostMacro.html "class in com.facebook.buck.rules.macros")\> {#class-executablemacroexpanderm-extends-abstractexecutabletargetorhostmacro .title title="Class ExecutableMacroExpander"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.rules.macros.AbstractMacroExpanderWithoutPrecomputedWork](AbstractMacroExpanderWithoutPrecomputedWork.html "class in com.facebook.buck.rules.macros")\<M\>

    -   -   [com.facebook.buck.rules.macros.BuildTargetMacroExpander](BuildTargetMacroExpander.html "class in com.facebook.buck.rules.macros")\<M\>

        -   -   com.facebook.buck.rules.macros.ExecutableMacroExpander\<M\>

::: description
-   

    All Implemented Interfaces:
    :   `MacroExpander<M,​Object>`

    ------------------------------------------------------------------------

        public class ExecutableMacroExpander<M extends AbstractExecutableTargetOrHostMacro>
        extends BuildTargetMacroExpander<M>

    ::: block
    Resolves to the executable command for a build target referencing a
    [`BinaryBuildRule`](../../core/rules/tool/BinaryBuildRule.html "interface in com.facebook.buck.core.rules.tool").
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                      Description
          ------------------------------------------------ -------------
          `ExecutableMacroExpander​(Class<M> macroClass)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                                                                              Description
          ------------------- ----------------------------------------------------------------------------------- -------------
          `protected Arg`     `expand​(SourcePathResolverAdapter resolver,       M macro,       BuildRule rule)`    
          `Class<M>`          `getInputClass()`                                                                    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.rules.macros.BuildTargetMacroExpander}

            ### Methods inherited from class com.facebook.buck.rules.macros.[BuildTargetMacroExpander](BuildTargetMacroExpander.html "class in com.facebook.buck.rules.macros")

            `expandFrom, resolve`

        ```{=html}
        <!-- -->
        ```
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
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(java.lang.Class)}

        -   #### ExecutableMacroExpander

                public ExecutableMacroExpander​(Class<M> macroClass)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getInputClass()}

        -   #### getInputClass

            ``` methodSignature
            public Class<M> getInputClass()
            ```

            [Returns:]{.returnLabel}
            :   the class for the parsed macro input type.

        []{#expand(com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter,com.facebook.buck.rules.macros.AbstractExecutableTargetOrHostMacro,com.facebook.buck.core.rules.BuildRule)}
        []{#expand(com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter,M,com.facebook.buck.core.rules.BuildRule)}

        -   #### expand

            ``` methodSignature
            protected Arg expand​(SourcePathResolverAdapter resolver,
                                 M macro,
                                 BuildRule rule)
                          throws MacroException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `expand` in
                class `BuildTargetMacroExpander<M extends AbstractExecutableTargetOrHostMacro>`

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
