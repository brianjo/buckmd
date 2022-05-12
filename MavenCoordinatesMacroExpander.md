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

## Class MavenCoordinatesMacroExpander {#class-mavencoordinatesmacroexpander .title title="Class MavenCoordinatesMacroExpander"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.rules.macros.AbstractMacroExpanderWithoutPrecomputedWork](AbstractMacroExpanderWithoutPrecomputedWork.html "class in com.facebook.buck.rules.macros")\<M\>

    -   -   [com.facebook.buck.rules.macros.BuildTargetMacroExpander](BuildTargetMacroExpander.html "class in com.facebook.buck.rules.macros")\<[MavenCoordinatesMacro](MavenCoordinatesMacro.html "class in com.facebook.buck.rules.macros")\>

        -   -   com.facebook.buck.rules.macros.MavenCoordinatesMacroExpander

::: description
-   

    All Implemented Interfaces:
    :   `MacroExpander<MavenCoordinatesMacro,​Object>`

    ------------------------------------------------------------------------

        public class MavenCoordinatesMacroExpander
        extends BuildTargetMacroExpander<MavenCoordinatesMacro>

    ::: block
    Resolves to the maven coordinates for a build target referencing a
    [`HasMavenCoordinates`](../../jvm/core/HasMavenCoordinates.html "interface in com.facebook.buck.jvm.core").
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                         Description
          ----------------------------------- -------------
          `MavenCoordinatesMacroExpander()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                Method                                                                                                    Description
          -------------------------------- --------------------------------------------------------------------------------------------------------- -------------
          `Arg`                            `expand​(SourcePathResolverAdapter resolver,       MavenCoordinatesMacro ignored,       BuildRule rule)`    
          `Class<MavenCoordinatesMacro>`   `getInputClass()`                                                                                          
          `protected String`               `getMavenCoordinates​(BuildRule rule)`                                                                      

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

        []{#<init>()}

        -   #### MavenCoordinatesMacroExpander

                public MavenCoordinatesMacroExpander()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getInputClass()}

        -   #### getInputClass

            ``` methodSignature
            public Class<MavenCoordinatesMacro> getInputClass()
            ```

            [Returns:]{.returnLabel}
            :   the class for the parsed macro input type.

        []{#getMavenCoordinates(com.facebook.buck.core.rules.BuildRule)}

        -   #### getMavenCoordinates

            ``` methodSignature
            protected String getMavenCoordinates​(BuildRule rule)
                                          throws MacroException
            ```

            [Throws:]{.throwsLabel}
            :   `MacroException`

        []{#expand(com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter,com.facebook.buck.rules.macros.MavenCoordinatesMacro,com.facebook.buck.core.rules.BuildRule)}

        -   #### expand

            ``` methodSignature
            public Arg expand​(SourcePathResolverAdapter resolver,
                              MavenCoordinatesMacro ignored,
                              BuildRule rule)
                       throws MacroException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `expand` in
                class `BuildTargetMacroExpander<MavenCoordinatesMacro>`

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
