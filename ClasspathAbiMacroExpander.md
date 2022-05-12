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

## Class ClasspathAbiMacroExpander {#class-classpathabimacroexpander .title title="Class ClasspathAbiMacroExpander"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.rules.macros.AbstractMacroExpanderWithoutPrecomputedWork](AbstractMacroExpanderWithoutPrecomputedWork.html "class in com.facebook.buck.rules.macros")\<M\>

    -   -   [com.facebook.buck.rules.macros.BuildTargetMacroExpander](BuildTargetMacroExpander.html "class in com.facebook.buck.rules.macros")\<[ClasspathAbiMacro](ClasspathAbiMacro.html "class in com.facebook.buck.rules.macros")\>

        -   -   com.facebook.buck.rules.macros.ClasspathAbiMacroExpander

::: description
-   

    All Implemented Interfaces:
    :   `MacroExpander<ClasspathAbiMacro,​Object>`

    ------------------------------------------------------------------------

        public class ClasspathAbiMacroExpander
        extends BuildTargetMacroExpander<ClasspathAbiMacro>

    ::: block
    Used to expand the macro \$(classpath_abi //some:target) to the
    transitive abi\'s jars path of that target, expanding all paths to
    be absolute.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                     Description
          ------------------------------- -------------
          `ClasspathAbiMacroExpander()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type            Method                                                                                                           Description
          ---------------------------- ---------------------------------------------------------------------------------------------------------------- -------------
          `protected Arg`              `expand​(ActionGraphBuilder graphBuilder,       BuildRule inputRule)`                                              
          `protected Arg`              `expand​(SourcePathResolverAdapter resolver,       ClasspathAbiMacro macro,       BuildRule rule)`                 
          `Arg`                        `expandFrom​(BuildTarget target,           ActionGraphBuilder graphBuilder,           ClasspathAbiMacro input)`    
          `Class<ClasspathAbiMacro>`   `getInputClass()`                                                                                                 

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.rules.macros.BuildTargetMacroExpander}

            ### Methods inherited from class com.facebook.buck.rules.macros.[BuildTargetMacroExpander](BuildTargetMacroExpander.html "class in com.facebook.buck.rules.macros")

            `resolve`

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

        []{#<init>()}

        -   #### ClasspathAbiMacroExpander

                public ClasspathAbiMacroExpander()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getInputClass()}

        -   #### getInputClass

            ``` methodSignature
            public Class<ClasspathAbiMacro> getInputClass()
            ```

            [Returns:]{.returnLabel}
            :   the class for the parsed macro input type.

        []{#expand(com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter,com.facebook.buck.rules.macros.ClasspathAbiMacro,com.facebook.buck.core.rules.BuildRule)}

        -   #### expand

            ``` methodSignature
            protected Arg expand​(SourcePathResolverAdapter resolver,
                                 ClasspathAbiMacro macro,
                                 BuildRule rule)
                          throws MacroException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `expand` in
                class `BuildTargetMacroExpander<ClasspathAbiMacro>`

            [Throws:]{.throwsLabel}
            :   `MacroException`

        []{#expandFrom(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.rules.ActionGraphBuilder,com.facebook.buck.rules.macros.ClasspathAbiMacro)}

        -   #### expandFrom

            ``` methodSignature
            public Arg expandFrom​(BuildTarget target,
                                  ActionGraphBuilder graphBuilder,
                                  ClasspathAbiMacro input)
                           throws MacroException
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `expandFrom` in
                class `BuildTargetMacroExpander<ClasspathAbiMacro>`

            [Throws:]{.throwsLabel}
            :   `MacroException`

        []{#expand(com.facebook.buck.core.rules.ActionGraphBuilder,com.facebook.buck.core.rules.BuildRule)}

        -   #### expand

            ``` methodSignature
            protected Arg expand​(ActionGraphBuilder graphBuilder,
                                 BuildRule inputRule)
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
