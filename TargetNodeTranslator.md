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

-   [Overview](../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../deprecated-list.html)
-   [Index](../../../../index-all.html)
-   [Help](../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.versions](package-summary.html)
:::

## Class TargetNodeTranslator {#class-targetnodetranslator .title title="Class TargetNodeTranslator"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.versions.TargetNodeTranslator

::: description
-   

    ------------------------------------------------------------------------

        public abstract class TargetNodeTranslator
        extends Object

    ::: block
    A helper class which uses reflection to translate
    [`BuildTarget`](../core/model/BuildTarget.html "class in com.facebook.buck.core.model")s
    in
    [`TargetNode`](../core/model/targetgraph/TargetNode.html "interface in com.facebook.buck.core.model.targetgraph")s.
    The API methods use an
    [`Optional`](http://docs.oracle.com/javase/7/docs/api/java/util/Optional.html?is-external=true "class or interface in java.util"){.externalLink}
    for their return types, so that
    [`Optional.empty()`](http://docs.oracle.com/javase/7/docs/api/java/util/Optional.html?is-external=true#empty() "class or interface in java.util"){.externalLink}
    can be used to signify a translation was not needed. This may allow
    some translation functions to avoid copying or creating unnecessary
    new objects.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                               Description
          ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `TargetNodeTranslator​(TypeCoercerFactory typeCoercerFactory,                     com.google.common.collect.ImmutableList<com.facebook.buck.versions.TargetTranslator<?>> translators,                     Cells cells)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                                  Method                                                                                                Description
          ---------------------------------------------------------------------------------- ----------------------------------------------------------------------------------------------------- -------------
          `abstract Optional<com.google.common.collect.ImmutableMap<BuildTarget,​Version>>`   `getSelectedVersions​(BuildTarget target)`                                                              
          `<A> Optional<A>`                                                                  `translate​(CellNameResolver cellNameResolver,          BaseName targetBaseName,          A object)`    
          `abstract Optional<BuildTarget>`                                                   `translateBuildTarget​(BuildTarget target)`                                                             
          `<A extends ConstructorArg>Optional<TargetNode<A>>`                                `translateNode​(TargetNode<A> node)`                                                                    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Abstract
          Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
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

        []{#<init>(com.facebook.buck.rules.coercer.TypeCoercerFactory,com.google.common.collect.ImmutableList,com.facebook.buck.core.cell.Cells)}

        -   #### TargetNodeTranslator

                public TargetNodeTranslator​(TypeCoercerFactory typeCoercerFactory,
                                            com.google.common.collect.ImmutableList<com.facebook.buck.versions.TargetTranslator<?>> translators,
                                            Cells cells)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#translateBuildTarget(com.facebook.buck.core.model.BuildTarget)}

        -   #### translateBuildTarget

            ``` methodSignature
            public abstract Optional<BuildTarget> translateBuildTarget​(BuildTarget target)
            ```

        []{#getSelectedVersions(com.facebook.buck.core.model.BuildTarget)}

        -   #### getSelectedVersions

            ``` methodSignature
            public abstract Optional<com.google.common.collect.ImmutableMap<BuildTarget,​Version>> getSelectedVersions​(BuildTarget target)
            ```

        []{#translate(com.facebook.buck.core.cell.nameresolver.CellNameResolver,com.facebook.buck.core.model.BaseName,java.lang.Object)}
        []{#translate(com.facebook.buck.core.cell.nameresolver.CellNameResolver,com.facebook.buck.core.model.BaseName,A)}

        -   #### translate

            ``` methodSignature
            public <A> Optional<A> translate​(CellNameResolver cellNameResolver,
                                             BaseName targetBaseName,
                                             A object)
            ```

        []{#translateNode(com.facebook.buck.core.model.targetgraph.TargetNode)}

        -   #### translateNode

            ``` methodSignature
            public <A extends ConstructorArg> Optional<TargetNode<A>> translateNode​(TargetNode<A> node)
            ```

            [Returns:]{.returnLabel}
            :   a copy of the given
                [`TargetNode`](../core/model/targetgraph/TargetNode.html "interface in com.facebook.buck.core.model.targetgraph")
                with all found
                [`BuildTarget`](../core/model/BuildTarget.html "class in com.facebook.buck.core.model")s
                translated, or
                [`Optional.empty()`](http://docs.oracle.com/javase/7/docs/api/java/util/Optional.html?is-external=true#empty() "class or interface in java.util"){.externalLink}
                if the node requires no translation.
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

-   [Overview](../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../deprecated-list.html)
-   [Index](../../../../index-all.html)
-   [Help](../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../allclasses.html)

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
