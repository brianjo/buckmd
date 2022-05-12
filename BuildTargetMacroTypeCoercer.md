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
[Package]{.packageLabelInType} [com.facebook.buck.rules.coercer](package-summary.html)
:::

## Class BuildTargetMacroTypeCoercer\<M extends [BuildTargetMacro](../macros/BuildTargetMacro.html "class in com.facebook.buck.rules.macros")\> {#class-buildtargetmacrotypecoercerm-extends-buildtargetmacro .title title="Class BuildTargetMacroTypeCoercer"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.rules.coercer.BuildTargetMacroTypeCoercer\<M\>

::: description
-   

    ------------------------------------------------------------------------

        public final class BuildTargetMacroTypeCoercer<M extends BuildTargetMacro>
        extends Object

    ::: block
    Coercer for macros which take a single
    [`BuildTarget`](../../core/model/BuildTarget.html "class in com.facebook.buck.core.model")
    arg.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static class `       | `BuildTargetMacroType | ::: block             |
        |                       | Coercer.TargetOrHost` | Should target be      |
        |                       |                       | resolved for host     |
        |                       |                       | platform or target    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                                                                                                       Description
          ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `BuildTargetMacroTypeCoercer​(TypeCoercer<UnconfiguredBuildTargetWithOutputs,​BuildTargetWithOutputs> buildTargetWithOutputsTypeCoercer,                            Class<M> mClass,                            BuildTargetMacroTypeCoercer.TargetOrHost targetOrHost,                            java.util.function.Function<BuildTargetWithOutputs,​M> factory)`    

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

        []{#<init>(com.facebook.buck.rules.coercer.TypeCoercer,java.lang.Class,com.facebook.buck.rules.coercer.BuildTargetMacroTypeCoercer.TargetOrHost,java.util.function.Function)}

        -   #### BuildTargetMacroTypeCoercer

                public BuildTargetMacroTypeCoercer​(TypeCoercer<UnconfiguredBuildTargetWithOutputs,​BuildTargetWithOutputs> buildTargetWithOutputsTypeCoercer,
                                                   Class<M> mClass,
                                                   BuildTargetMacroTypeCoercer.TargetOrHost targetOrHost,
                                                   java.util.function.Function<BuildTargetWithOutputs,​M> factory)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#hasElementClass(java.lang.Class[])}

        -   #### hasElementClass

            ``` methodSignature
            public boolean hasElementClass​(Class<?>[] types)
            ```

        []{#traverse(com.facebook.buck.core.cell.nameresolver.CellNameResolver,com.facebook.buck.rules.macros.BuildTargetMacro,com.facebook.buck.rules.coercer.TypeCoercer.Traversal)}
        []{#traverse(com.facebook.buck.core.cell.nameresolver.CellNameResolver,M,com.facebook.buck.rules.coercer.TypeCoercer.Traversal)}

        -   #### traverse

            ``` methodSignature
            public void traverse​(CellNameResolver cellRoots,
                                 M macro,
                                 TypeCoercer.Traversal traversal)
            ```

        []{#getOutputClass()}

        -   #### getOutputClass

            ``` methodSignature
            public Class<M> getOutputClass()
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
