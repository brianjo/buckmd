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
[Package]{.packageLabelInType} [com.facebook.buck.rules.coercer](package-summary.html)
:::

## Class CxxGenruleFilterAndTargetsMacroTypeCoercer\<M extends [CxxGenruleFilterAndTargetsMacro](../macros/CxxGenruleFilterAndTargetsMacro.html "class in com.facebook.buck.rules.macros")\> {#class-cxxgenrulefilterandtargetsmacrotypecoercerm-extends-cxxgenrulefilterandtargetsmacro .title title="Class CxxGenruleFilterAndTargetsMacroTypeCoercer"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.rules.coercer.CxxGenruleFilterAndTargetsMacroTypeCoercer\<M\>

::: description
-   

    ------------------------------------------------------------------------

        public class CxxGenruleFilterAndTargetsMacroTypeCoercer<M extends CxxGenruleFilterAndTargetsMacro>
        extends Object

    ::: block
    Coercer for `cxx_genrule` flag-based macros.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          Description
          ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ -------------
          `CxxGenruleFilterAndTargetsMacroTypeCoercer​(Optional<TypeCoercer<Pattern,​Pattern>> patternTypeCoercer,                                           TypeCoercer<com.google.common.collect.ImmutableList<UnconfiguredBuildTarget>,​com.google.common.collect.ImmutableList<BuildTarget>> buildTargetsTypeCoercer,                                           Class<M> clazz,                                           java.util.function.BiFunction<Optional<Pattern>,​com.google.common.collect.ImmutableList<BuildTarget>,​M> factory)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                                                                                                                                                                                                                                                                                         Description
          ------------------- ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `M`                 `coerce​(CellNameResolver cellNameResolver,       ProjectFilesystem filesystem,       ForwardRelativePath pathRelativeToProjectRoot,       TargetConfiguration targetConfiguration,       TargetConfiguration hostConfiguration,       com.google.common.collect.ImmutableList<String> args)`    
          `Class<M>`          `getOutputClass()`                                                                                                                                                                                                                                                                              
          `boolean`           `hasElementClass​(Class<?>[] types)`                                                                                                                                                                                                                                                             
          `void`              `traverse​(CellNameResolver cellRoots,         M macro,         TypeCoercer.Traversal traversal)`                                                                                                                                                                                                

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(java.util.Optional,com.facebook.buck.rules.coercer.TypeCoercer,java.lang.Class,java.util.function.BiFunction)}

        -   #### CxxGenruleFilterAndTargetsMacroTypeCoercer

                public CxxGenruleFilterAndTargetsMacroTypeCoercer​(Optional<TypeCoercer<Pattern,​Pattern>> patternTypeCoercer,
                                                                  TypeCoercer<com.google.common.collect.ImmutableList<UnconfiguredBuildTarget>,​com.google.common.collect.ImmutableList<BuildTarget>> buildTargetsTypeCoercer,
                                                                  Class<M> clazz,
                                                                  java.util.function.BiFunction<Optional<Pattern>,​com.google.common.collect.ImmutableList<BuildTarget>,​M> factory)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getOutputClass()}

        -   #### getOutputClass

            ``` methodSignature
            public Class<M> getOutputClass()
            ```

        []{#hasElementClass(java.lang.Class[])}

        -   #### hasElementClass

            ``` methodSignature
            public boolean hasElementClass​(Class<?>[] types)
            ```

        []{#traverse(com.facebook.buck.core.cell.nameresolver.CellNameResolver,com.facebook.buck.rules.macros.CxxGenruleFilterAndTargetsMacro,com.facebook.buck.rules.coercer.TypeCoercer.Traversal)}
        []{#traverse(com.facebook.buck.core.cell.nameresolver.CellNameResolver,M,com.facebook.buck.rules.coercer.TypeCoercer.Traversal)}

        -   #### traverse

            ``` methodSignature
            public void traverse​(CellNameResolver cellRoots,
                                 M macro,
                                 TypeCoercer.Traversal traversal)
            ```

        []{#coerce(com.facebook.buck.core.cell.nameresolver.CellNameResolver,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.path.ForwardRelativePath,com.facebook.buck.core.model.TargetConfiguration,com.facebook.buck.core.model.TargetConfiguration,com.google.common.collect.ImmutableList)}

        -   #### coerce

            ``` methodSignature
            public M coerce​(CellNameResolver cellNameResolver,
                            ProjectFilesystem filesystem,
                            ForwardRelativePath pathRelativeToProjectRoot,
                            TargetConfiguration targetConfiguration,
                            TargetConfiguration hostConfiguration,
                            com.google.common.collect.ImmutableList<String> args)
                     throws CoerceFailedException
            ```

            [Throws:]{.throwsLabel}
            :   `CoerceFailedException`
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
