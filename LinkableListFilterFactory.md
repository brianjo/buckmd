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
[Package]{.packageLabelInType} [com.facebook.buck.cxx](package-summary.html)
:::

## Class LinkableListFilterFactory {#class-linkablelistfilterfactory .title title="Class LinkableListFilterFactory"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.cxx.LinkableListFilterFactory

::: description
-   

    ------------------------------------------------------------------------

        public class LinkableListFilterFactory
        extends Object

    ::: block
    Factory for the creation of
    [`LinkableListFilter`](toolchain/nativelink/LinkableListFilter.html "interface in com.facebook.buck.cxx.toolchain.nativelink")
    which can be used to filter the libraries which an executable (e.g.,
    binary, shared library, Mach-O bundle) links against.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static Optional      | `f                    | ::: block             |
        | <LinkableListFilter>` | rom​(CxxBuckConfig cxx | Convenience method    |
        |                       | BuckConfig,     Linka | that unpacks a        |
        |                       | bleCxxConstructorArg  | [`LinkableCxxC        |
        |                       | linkableArg,     Targ | onstructorArg`](Linka |
        |                       | etGraph targetGraph)` | bleCxxConstructorArg. |
        |                       |                       | html "interface in co |
        |                       |                       | m.facebook.buck.cxx") |
        |                       |                       | and forwards the      |
        |                       |                       | call.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static Optional      | `f                    | ::: block             |
        | <LinkableListFilter>` | rom​(CxxBuckConfig cxx | Creates a             |
        |                       | BuckConfig,     Optio | [`LinkableListFilter` |
        |                       | nal<String> linkGroup | ](toolchain/nativelin |
        |                       | ,     com.google.comm | k/LinkableListFilter. |
        |                       | on.collect.ImmutableL | html "interface in co |
        |                       | ist<CxxLinkGroupMappi | m.facebook.buck.cxx.t |
        |                       | ng> mapping,     Targ | oolchain.nativelink") |
        |                       | etGraph targetGraph)` | based on a link group |
        |                       |                       | map and a target      |
        |                       |                       | graph.                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static               | `resourcePredic       | ::: block             |
        | java.util.function.Pr | ateFrom​(CxxBuckConfig | Creates a predicate   |
        | edicate<BuildTarget>` |  cxxBuckConfig,       | to filter resources   |
        |                       |                 Optio | that will be included |
        |                       | nal<String> resourceG | in an apple_bundle.   |
        |                       | roup,                 | :::                   |
        |                       |       Optional<com.go |                       |
        |                       | ogle.common.collect.I |                       |
        |                       | mmutableList<CxxLinkG |                       |
        |                       | roupMapping>> mapping |                       |
        |                       | ,                     |                       |
        |                       |   TargetGraph graph)` |                       |
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

        []{#from(com.facebook.buck.cxx.config.CxxBuckConfig,com.facebook.buck.cxx.LinkableCxxConstructorArg,com.facebook.buck.core.model.targetgraph.TargetGraph)}

        -   #### from

            ``` methodSignature
            public static Optional<LinkableListFilter> from​(CxxBuckConfig cxxBuckConfig,
                                                            LinkableCxxConstructorArg linkableArg,
                                                            TargetGraph targetGraph)
            ```

            ::: block
            Convenience method that unpacks a
            [`LinkableCxxConstructorArg`](LinkableCxxConstructorArg.html "interface in com.facebook.buck.cxx")
            and forwards the call.
            :::

        []{#from(com.facebook.buck.cxx.config.CxxBuckConfig,java.util.Optional,com.google.common.collect.ImmutableList,com.facebook.buck.core.model.targetgraph.TargetGraph)}

        -   #### from

            ``` methodSignature
            public static Optional<LinkableListFilter> from​(CxxBuckConfig cxxBuckConfig,
                                                            Optional<String> linkGroup,
                                                            com.google.common.collect.ImmutableList<CxxLinkGroupMapping> mapping,
                                                            TargetGraph targetGraph)
            ```

            ::: block
            Creates a
            [`LinkableListFilter`](toolchain/nativelink/LinkableListFilter.html "interface in com.facebook.buck.cxx.toolchain.nativelink")
            based on a link group map and a target graph. Shared
            libraries will get linked as normal and no filtering would
            occur. Static libraries will be linked according to the link
            group membership.
            :::

            [Parameters:]{.paramLabel}
            :   `cxxBuckConfig` - If link groups are not enabled in the
                config, an empty
                [`Optional`](http://docs.oracle.com/javase/7/docs/api/java/util/Optional.html?is-external=true "class or interface in java.util"){.externalLink}
                would be returned.
            :   `linkGroup` - Defines the link group of the executable
                being linked. By definition, it will be linked against
                libraries which belong to the same link group. If the
                link group is empty, the executable would linked against
                libraries which do not belong to any link groups.
            :   `mapping` - Defines the mapping which determines which
                link group specific targets belong to.
            :   `targetGraph` - The target graph which is used by the
                mapping to compute link group membership.

        []{#resourcePredicateFrom(com.facebook.buck.cxx.config.CxxBuckConfig,java.util.Optional,java.util.Optional,com.facebook.buck.core.model.targetgraph.TargetGraph)}

        -   #### resourcePredicateFrom

            ``` methodSignature
            @Nonnull
            public static java.util.function.Predicate<BuildTarget> resourcePredicateFrom​(CxxBuckConfig cxxBuckConfig,
                                                                                          Optional<String> resourceGroup,
                                                                                          Optional<com.google.common.collect.ImmutableList<CxxLinkGroupMapping>> mapping,
                                                                                          TargetGraph graph)
            ```

            ::: block
            Creates a predicate to filter resources that will be
            included in an apple_bundle.
            :::
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
