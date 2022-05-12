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

## Class BuildTargetMacroExpander\<M extends [BuildTargetMacro](BuildTargetMacro.html "class in com.facebook.buck.rules.macros")\> {#class-buildtargetmacroexpanderm-extends-buildtargetmacro .title title="Class BuildTargetMacroExpander"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.rules.macros.AbstractMacroExpanderWithoutPrecomputedWork](AbstractMacroExpanderWithoutPrecomputedWork.html "class in com.facebook.buck.rules.macros")\<M\>

    -   -   com.facebook.buck.rules.macros.BuildTargetMacroExpander\<M\>

::: description
-   

    All Implemented Interfaces:
    :   `MacroExpander<M,​Object>`

    ```{=html}
    <!-- -->
    ```

    Direct Known Subclasses:
    :   `AbstractLocationMacroExpander`, `ClasspathAbiMacroExpander`,
        `ClasspathMacroExpander`, `ExecutableMacroExpander`,
        `MavenCoordinatesMacroExpander`, `WorkerMacroExpander`

    ------------------------------------------------------------------------

        public abstract class BuildTargetMacroExpander<M extends BuildTargetMacro>
        extends AbstractMacroExpanderWithoutPrecomputedWork<M>

    ::: block
    Abstract expander which resolves using a references to another
    [`BuildRule`](../../core/rules/BuildRule.html "interface in com.facebook.buck.core.rules").
    Matches either a relative or fully-qualified build target wrapped in
    \$(), unless the `$` is preceded by a backslash.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                    Description
          ------------------------------ -------------
          `BuildTargetMacroExpander()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type          Method                                                                                           Description
          -------------------------- ------------------------------------------------------------------------------------------------ -------------
          `protected abstract Arg`   `expand​(SourcePathResolverAdapter resolver,       M macro,       BuildRule rule)`                 
          `Arg`                      `expandFrom​(BuildTarget target,           ActionGraphBuilder graphBuilder,           M input)`    
          `protected BuildRule`      `resolve​(ActionGraphBuilder graphBuilder,        M input)`                                        

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Abstract
          Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
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

        -   #### BuildTargetMacroExpander

                public BuildTargetMacroExpander()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#expand(com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter,com.facebook.buck.rules.macros.BuildTargetMacro,com.facebook.buck.core.rules.BuildRule)}
        []{#expand(com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter,M,com.facebook.buck.core.rules.BuildRule)}

        -   #### expand

            ``` methodSignature
            protected abstract Arg expand​(SourcePathResolverAdapter resolver,
                                          M macro,
                                          BuildRule rule)
                                   throws MacroException
            ```

            [Throws:]{.throwsLabel}
            :   `MacroException`

        []{#resolve(com.facebook.buck.core.rules.ActionGraphBuilder,com.facebook.buck.rules.macros.BuildTargetMacro)}
        []{#resolve(com.facebook.buck.core.rules.ActionGraphBuilder,M)}

        -   #### resolve

            ``` methodSignature
            protected BuildRule resolve​(ActionGraphBuilder graphBuilder,
                                        M input)
                                 throws MacroException
            ```

            [Throws:]{.throwsLabel}
            :   `MacroException`

        []{#expandFrom(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.rules.ActionGraphBuilder,com.facebook.buck.rules.macros.BuildTargetMacro)}
        []{#expandFrom(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.rules.ActionGraphBuilder,M)}

        -   #### expandFrom

            ``` methodSignature
            public Arg expandFrom​(BuildTarget target,
                                  ActionGraphBuilder graphBuilder,
                                  M input)
                           throws MacroException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `expandFrom` in
                class `AbstractMacroExpanderWithoutPrecomputedWork<M extends BuildTargetMacro>`

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
