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

## Class BuildTargetMacro {#class-buildtargetmacro .title title="Class BuildTargetMacro"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.rules.macros.BuildTargetMacro

::: description
-   

    All Implemented Interfaces:
    :   `Macro`, `TargetTranslatable<Macro>`

    ```{=html}
    <!-- -->
    ```

    Direct Known Subclasses:
    :   `AbstractExecutableTargetOrHostMacro`, `BaseLocationMacro`,
        `ClasspathAbiMacro`, `ClasspathMacro`, `MavenCoordinatesMacro`,
        `WorkerMacro`

    ------------------------------------------------------------------------

        public abstract class BuildTargetMacro
        extends Object
        implements Macro

    ::: block
    Base class for macros wrapping a single
    [`BuildTarget`](../../core/model/BuildTarget.html "class in com.facebook.buck.core.model").
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor            Description
          ---------------------- -------------
          `BuildTargetMacro()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                       Method                                                                                                                                            Description
          --------------------------------------- ------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `boolean`                               `equals​(Object another)`                                                                                                                           
          `BuildTarget`                           `getTarget()`                                                                                                                                      
          `abstract BuildTargetWithOutputs`       `getTargetWithOutputs()`                                                                                                                           
          `int`                                   `hashCode()`                                                                                                                                       
          `Optional<Macro>`                       `translateTargets​(CellNameResolver cellPathResolver,                 BaseName targetBaseName,                 TargetNodeTranslator translator)`    
          `protected abstract BuildTargetMacro`   `withTargetWithOutputs​(BuildTargetWithOutputs target)`                                                                                             

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Abstract
          Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, finalize, getClass, notify, notifyAll, toString, wait, wait, wait`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.rules.macros.Macro}

            ### Methods inherited from interface com.facebook.buck.rules.macros.[Macro](Macro.html "interface in com.facebook.buck.rules.macros")

            `getMacroClass`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### BuildTargetMacro

                public BuildTargetMacro()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getTargetWithOutputs()}

        -   #### getTargetWithOutputs

            ``` methodSignature
            public abstract BuildTargetWithOutputs getTargetWithOutputs()
            ```

        []{#getTarget()}

        -   #### getTarget

            ``` methodSignature
            public BuildTarget getTarget()
            ```

        []{#withTargetWithOutputs(com.facebook.buck.core.model.BuildTargetWithOutputs)}

        -   #### withTargetWithOutputs

            ``` methodSignature
            protected abstract BuildTargetMacro withTargetWithOutputs​(BuildTargetWithOutputs target)
            ```

            [Returns:]{.returnLabel}
            :   a copy of this
                [`BuildTargetMacro`](BuildTargetMacro.html "class in com.facebook.buck.rules.macros")
                with the given
                [`BuildTargetWithOutputs`](../../core/model/BuildTargetWithOutputs.html "class in com.facebook.buck.core.model").

        []{#translateTargets(com.facebook.buck.core.cell.nameresolver.CellNameResolver,com.facebook.buck.core.model.BaseName,com.facebook.buck.versions.TargetNodeTranslator)}

        -   #### translateTargets

            ``` methodSignature
            public final Optional<Macro> translateTargets​(CellNameResolver cellPathResolver,
                                                          BaseName targetBaseName,
                                                          TargetNodeTranslator translator)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `translateTargets` in interface `Macro`

            [Specified by:]{.overrideSpecifyLabel}
            :   `translateTargets` in
                interface `TargetTranslatable<Macro>`

            [Returns:]{.returnLabel}
            :   if any changes are required, return the translated
                object.

        []{#hashCode()}

        -   #### hashCode

            ``` methodSignature
            public int hashCode()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `hashCode` in class `Object`

        []{#equals(java.lang.Object)}

        -   #### equals

            ``` methodSignature
            public boolean equals​(@Nullable
                                  Object another)
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `equals` in class `Object`
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
