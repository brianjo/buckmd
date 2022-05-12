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
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   Constr \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.apple](package-summary.html)
:::

## Class Flavors {#class-flavors .title title="Class Flavors"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.apple.Flavors

::: description
-   

    ------------------------------------------------------------------------

        public class Flavors
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static               | `containsF            |                       |
        | java.util.function.Pr | lavor​(Flavor flavor)` |                       |
        | edicate<BuildTarget>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static               | `containsFlavors​(Fla  |                       |
        | java.util.function.Pr | vorDomain<?> domain)` |                       |
        | edicate<BuildTarget>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `st                   | `pro                  | ::: block             |
        | atic com.google.commo | pagateFlavorDomains​(B | Propagate flavors     |
        | n.collect.ImmutableSo | uildTarget target,    | represented by the    |
        | rtedSet<BuildTarget>` |                     I | given                 |
        |                       | terable<FlavorDomain< | [`Fla                 |
        |                       | ?>> domains,          | vorDomain`](../core/m |
        |                       |               Iterabl | odel/FlavorDomain.htm |
        |                       | e<BuildTarget> deps)` | l "class in com.faceb |
        |                       |                       | ook.buck.core.model") |
        |                       |                       | objects from a parent |
        |                       |                       | target to its         |
        |                       |                       | dependencies.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static com.google.c  | `propagat             | ::: block             |
        | ommon.collect.FluentI | eFlavorsInDomainIfNot | Propagate a build     |
        | terable<BuildTarget>` | Present​(FlavorDomain< | target\'s flavors in  |
        |                       | ?> domain,            | a certain domain to a |
        |                       |                       | list of other build   |
        |                       |      BuildTarget buil | targets.              |
        |                       | dTarget,              | :::                   |
        |                       |                       |                       |
        |                       |    com.google.common. |                       |
        |                       | collect.FluentIterabl |                       |
        |                       | e<BuildTarget> deps)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#containsFlavors(com.facebook.buck.core.model.FlavorDomain)}

        -   #### containsFlavors

            ``` methodSignature
            public static java.util.function.Predicate<BuildTarget> containsFlavors​(FlavorDomain<?> domain)
            ```

        []{#containsFlavor(com.facebook.buck.core.model.Flavor)}

        -   #### containsFlavor

            ``` methodSignature
            public static java.util.function.Predicate<BuildTarget> containsFlavor​(Flavor flavor)
            ```

        []{#propagateFlavorDomains(com.facebook.buck.core.model.BuildTarget,java.lang.Iterable,java.lang.Iterable)}

        -   #### propagateFlavorDomains

            ``` methodSignature
            public static com.google.common.collect.ImmutableSortedSet<BuildTarget> propagateFlavorDomains​(BuildTarget target,
                                                                                                           Iterable<FlavorDomain<?>> domains,
                                                                                                           Iterable<BuildTarget> deps)
            ```

            ::: block
            Propagate flavors represented by the given
            [`FlavorDomain`](../core/model/FlavorDomain.html "class in com.facebook.buck.core.model")
            objects from a parent target to its dependencies.
            :::

        []{#propagateFlavorsInDomainIfNotPresent(com.facebook.buck.core.model.FlavorDomain,com.facebook.buck.core.model.BuildTarget,com.google.common.collect.FluentIterable)}

        -   #### propagateFlavorsInDomainIfNotPresent

            ``` methodSignature
            public static com.google.common.collect.FluentIterable<BuildTarget> propagateFlavorsInDomainIfNotPresent​(FlavorDomain<?> domain,
                                                                                                                     BuildTarget buildTarget,
                                                                                                                     com.google.common.collect.FluentIterable<BuildTarget> deps)
            ```

            ::: block
            Propagate a build target\'s flavors in a certain domain to a
            list of other build targets.
            :::

            [Parameters:]{.paramLabel}
            :   `domain` - the flavor domain to be propagated.
            :   `buildTarget` - the build target containing the flavors
                to be propagated
            :   `deps` - list of BuildTargetPaths to propagate the
                flavors to. If a target already contains one or more
                flavors in domain, it is left unchanged.

            [Returns:]{.returnLabel}
            :   the list of BuildTargetPaths with any flavors
                propagated.
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
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   Constr \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
