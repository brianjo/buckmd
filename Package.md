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

## Class Package {#class-package .title title="Class Package"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.model.targetgraph.impl.Package

::: description
-   

    ------------------------------------------------------------------------

        public abstract class Package
        extends Object

    ::: block
    A
    [`Package`](Package.html "class in com.facebook.buck.core.model.targetgraph.impl")
    contains attributes that are applied by default to all
    [`TargetNode`](../TargetNode.html "interface in com.facebook.buck.core.model.targetgraph")s
    contained within a build file
    [`BuildFileManifest`](../../../../parser/api/BuildFileManifest.html "class in com.facebook.buck.parser.api").
    A \`Package\` contains metadata gathered from \`PACKAGE\` files of
    the current directory/package and all parent directories/packages.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor   Description
          ------------- -------------
          `Package()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                      Method                                                                                                                                                               Description
          ---------------------------------------------------------------------- -------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `abstract com.google.common.collect.ImmutableSet<VisibilityPattern>`   `getVisibilityPatterns()`                                                                                                                                             
          `abstract com.google.common.collect.ImmutableSet<VisibilityPattern>`   `getWithinViewPatterns()`                                                                                                                                             
          `static Package`                                                       `of​(com.google.common.collect.ImmutableSet<VisibilityPattern> visibilityPatterns,   com.google.common.collect.ImmutableSet<VisibilityPattern> withinViewPatterns)`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
          Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
          .tableTab}[[Instance
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

        []{#<init>()}

        -   #### Package

                public Package()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getVisibilityPatterns()}

        -   #### getVisibilityPatterns

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableSet<VisibilityPattern> getVisibilityPatterns()
            ```

        []{#getWithinViewPatterns()}

        -   #### getWithinViewPatterns

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableSet<VisibilityPattern> getWithinViewPatterns()
            ```

        []{#of(com.google.common.collect.ImmutableSet,com.google.common.collect.ImmutableSet)}

        -   #### of

            ``` methodSignature
            public static Package of​(com.google.common.collect.ImmutableSet<VisibilityPattern> visibilityPatterns,
                                     com.google.common.collect.ImmutableSet<VisibilityPattern> withinViewPatterns)
            ```
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
