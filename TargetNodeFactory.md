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

-   [Overview](../../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../index-all.html)
-   [Help](../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.core.model.targetgraph.impl](package-summary.html)
:::

## Class TargetNodeFactory {#class-targetnodefactory .title title="Class TargetNodeFactory"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.model.targetgraph.impl.TargetNodeFactory

::: description
-   

    All Implemented Interfaces:
    :   `NodeCopier`

    ------------------------------------------------------------------------

        public class TargetNodeFactory
        extends Object
        implements NodeCopier
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                     Description
          --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `TargetNodeFactory​(TypeCoercerFactory typeCoercerFactory,                  CellNameResolverProvider cellNames)`                                                                                                  
          `TargetNodeFactory​(TypeCoercerFactory typeCoercerFactory,                  com.facebook.buck.core.model.targetgraph.impl.PathsChecker pathsChecker,                  CellNameResolverProvider cellNames)`        
          `TargetNodeFactory​(TypeCoercerFactory typeCoercerFactory,                  PathTypeCoercer.PathExistenceVerificationMode pathExistenceVerificationMode,                  CellNameResolverProvider cellNames)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `<T extends Construc  | `copyNodeWithFlavor   |                       |
        | torArg>TargetNode<T>` | s​(TargetNode<T> origi |                       |
        |                       | nalNode,              |                       |
        |                       |        com.google.com |                       |
        |                       | mon.collect.Immutable |                       |
        |                       | Set<Flavor> flavors)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `<T ext               | `cre                  | ::: block             |
        | ends ConstructorArg,​U | ateFromObject​(U descr | This factory method   |
        |  extends BaseDescript | iption,               | lets the wildcard be  |
        | ion<T>>TargetNode<T>` |    Object constructor | bound, so the         |
        |                       | Arg,                  | constructor can be    |
        |                       | ProjectFilesystem fil | casted to it.         |
        |                       | esystem,              | :::                   |
        |                       |     BuildTarget build |                       |
        |                       | Target,               |                       |
        |                       |    DependencyStack de |                       |
        |                       | pendencyStack,        |                       |
        |                       |           com.google. |                       |
        |                       | common.collect.Immuta |                       |
        |                       | bleSet<BuildTarget> d |                       |
        |                       | eclaredDeps,          |                       |
        |                       |         com.google.co |                       |
        |                       | mmon.collect.Immutabl |                       |
        |                       | eSortedSet<BuildTarge |                       |
        |                       | t> configurationDeps, |                       |
        |                       |                  com. |                       |
        |                       | google.common.collect |                       |
        |                       | .ImmutableSet<Visibil |                       |
        |                       | ityPattern> visibilit |                       |
        |                       | yPatterns,            |                       |
        |                       |       com.google.comm |                       |
        |                       | on.collect.ImmutableS |                       |
        |                       | et<VisibilityPattern> |                       |
        |                       |  withinViewPatterns)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `equals​(Object obj)`  |                       |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `hashCode()`          |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, finalize, getClass, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.rules.coercer.TypeCoercerFactory,com.facebook.buck.core.cell.nameresolver.CellNameResolverProvider)}

        -   #### TargetNodeFactory

                public TargetNodeFactory​(TypeCoercerFactory typeCoercerFactory,
                                         CellNameResolverProvider cellNames)

        []{#<init>(com.facebook.buck.rules.coercer.TypeCoercerFactory,com.facebook.buck.rules.coercer.PathTypeCoercer.PathExistenceVerificationMode,com.facebook.buck.core.cell.nameresolver.CellNameResolverProvider)}

        -   #### TargetNodeFactory

                public TargetNodeFactory​(TypeCoercerFactory typeCoercerFactory,
                                         PathTypeCoercer.PathExistenceVerificationMode pathExistenceVerificationMode,
                                         CellNameResolverProvider cellNames)

        []{#<init>(com.facebook.buck.rules.coercer.TypeCoercerFactory,com.facebook.buck.core.model.targetgraph.impl.PathsChecker,com.facebook.buck.core.cell.nameresolver.CellNameResolverProvider)}

        -   #### TargetNodeFactory

                public TargetNodeFactory​(TypeCoercerFactory typeCoercerFactory,
                                         com.facebook.buck.core.model.targetgraph.impl.PathsChecker pathsChecker,
                                         CellNameResolverProvider cellNames)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#createFromObject(com.facebook.buck.core.description.BaseDescription,java.lang.Object,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.exceptions.DependencyStack,com.google.common.collect.ImmutableSet,com.google.common.collect.ImmutableSortedSet,com.google.common.collect.ImmutableSet,com.google.common.collect.ImmutableSet)}
        []{#createFromObject(U,java.lang.Object,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.exceptions.DependencyStack,com.google.common.collect.ImmutableSet,com.google.common.collect.ImmutableSortedSet,com.google.common.collect.ImmutableSet,com.google.common.collect.ImmutableSet)}

        -   #### createFromObject

            ``` methodSignature
            public <T extends ConstructorArg,​U extends BaseDescription<T>> TargetNode<T> createFromObject​(U description,
                                                                                                                Object constructorArg,
                                                                                                                ProjectFilesystem filesystem,
                                                                                                                BuildTarget buildTarget,
                                                                                                                DependencyStack dependencyStack,
                                                                                                                com.google.common.collect.ImmutableSet<BuildTarget> declaredDeps,
                                                                                                                com.google.common.collect.ImmutableSortedSet<BuildTarget> configurationDeps,
                                                                                                                com.google.common.collect.ImmutableSet<VisibilityPattern> visibilityPatterns,
                                                                                                                com.google.common.collect.ImmutableSet<VisibilityPattern> withinViewPatterns)
                                                                                                         throws NoSuchBuildTargetException
            ```

            ::: block
            This factory method lets the wildcard be bound, so the
            constructor can be casted to it.
            This does no checking that the type of `constructorArg` is
            correct, since `  Description` does not hold the Class of
            the constructor arg.

            See [Wildcard Capture and Helper
            Methods](https://docs.oracle.com/javase/tutorial/java/generics/capture.html).
            :::

            [Throws:]{.throwsLabel}
            :   `NoSuchBuildTargetException`

        []{#copyNodeWithFlavors(com.facebook.buck.core.model.targetgraph.TargetNode,com.google.common.collect.ImmutableSet)}

        -   #### copyNodeWithFlavors

            ``` methodSignature
            public <T extends ConstructorArg> TargetNode<T> copyNodeWithFlavors​(TargetNode<T> originalNode,
                                                                                com.google.common.collect.ImmutableSet<Flavor> flavors)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `copyNodeWithFlavors` in interface `NodeCopier`

        []{#equals(java.lang.Object)}

        -   #### equals

            ``` methodSignature
            public boolean equals​(Object obj)
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `equals` in class `Object`

        []{#hashCode()}

        -   #### hashCode

            ``` methodSignature
            public int hashCode()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `hashCode` in class `Object`
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

-   [Overview](../../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../index-all.html)
-   [Help](../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../allclasses.html)

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
