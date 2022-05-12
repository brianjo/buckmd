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

-   [Overview](../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../deprecated-list.html)
-   [Index](../../../../../../index-all.html)
-   [Help](../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.cxx.toolchain.nativelink](package-summary.html)
:::

## Class NativeLinkables {#class-nativelinkables .title title="Class NativeLinkables"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.cxx.toolchain.nativelink.NativeLinkables

::: description
-   

    ------------------------------------------------------------------------

        public class NativeLinkables
        extends Object

    ::: block
    Utility functions for interacting with
    [`NativeLinkable`](NativeLinkable.html "interface in com.facebook.buck.cxx.toolchain.nativelink")
    objects.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static class `       | `NativeLinkables.Sh   | ::: block             |
        |                       | aredLibrariesBuilder` | Builds a map of       |
        |                       |                       | shared library names  |
        |                       |                       | to paths from         |
        |                       |                       | [`NativeLinkabl       |
        |                       |                       | e`](NativeLinkable.ht |
        |                       |                       | ml "interface in com. |
        |                       |                       | facebook.buck.cxx.too |
        |                       |                       | lchain.nativelink")s, |
        |                       |                       | throwing a useful     |
        |                       |                       | error on duplicates.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static Li            | `getLinkSt            | ::: block             |
        | nker.LinkableDepType` | yle​(NativeLinkableGro | Determine the final   |
        |                       | up.Linkage preferredL | [`Linker.             |
        |                       | inkage,             L | LinkableDepType`](../ |
        |                       | inker.LinkableDepType | linker/Linker.Linkabl |
        |                       |  requestedLinkStyle)` | eDepType.html "enum i |
        |                       |                       | n com.facebook.buck.c |
        |                       |                       | xx.toolchain.linker") |
        |                       |                       | given a preferred and |
        |                       |                       | requested linkage.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static Li            | `g                    | ::: block             |
        | nker.LinkableDepType` | etLinkStyle​(NativeLin | Determine the final   |
        |                       | kableGroup.Linkage pr | [`Linker.             |
        |                       | eferredLinkage,       | LinkableDepType`](../ |
        |                       |        Linker.Linkabl | linker/Linker.Linkabl |
        |                       | eDepType requestedLin | eDepType.html "enum i |
        |                       | kStyle,             O | n com.facebook.buck.c |
        |                       | ptional<PicType> picT | xx.toolchain.linker") |
        |                       | ypeForSharedLinking)` | given a preferred and |
        |                       |                       | requested linkage.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static               | `getNativeLinkableI   | ::: block             |
        |  NativeLinkableInput` | nput​(Linker.LinkableD | Get the               |
        |                       | epType linkStyle,     | [`NativeLinkableInp   |
        |                       |                    Na | ut`](NativeLinkableIn |
        |                       | tiveLinkable nativeLi | put.html "class in co |
        |                       | nkable,               | m.facebook.buck.cxx.t |
        |                       |          ActionGraphB | oolchain.nativelink") |
        |                       | uilder graphBuilder,  | for a                 |
        |                       |                       | [`NativeLinkab        |
        |                       |  TargetConfiguration  | le`](NativeLinkable.h |
        |                       | targetConfiguration)` | tml "interface in com |
        |                       |                       | .facebook.buck.cxx.to |
        |                       |                       | olchain.nativelink"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static com           | `getNativeLinkables   | ::: block             |
        | .google.common.collec | ​(ActionGraphBuilder g | Extract from the      |
        | t.ImmutableList<? ext | raphBuilder,          | dependency graph all  |
        | ends NativeLinkable>` |           Iterable<?  | the libraries which   |
        |                       | extends NativeLinkabl | must be considered    |
        |                       | e> inputs,            | for linking.          |
        |                       |         Linker.Linkab | :::                   |
        |                       | leDepType linkStyle)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static com           | `getNativeLinkab      | ::: block             |
        | .google.common.collec | les​(ActionGraphBuilde | Extract from the      |
        | t.ImmutableList<? ext | r graphBuilder,       | dependency graph all  |
        | ends NativeLinkable>` |              Iterable | the libraries which   |
        |                       | <? extends NativeLink | must be considered    |
        |                       | able> inputs,         | for linking.          |
        |                       |            Linker.Lin | :::                   |
        |                       | kableDepType linkStyl |                       |
        |                       | e,                    |                       |
        |                       | java.util.function.Pr |                       |
        |                       | edicate<? super Nativ |                       |
        |                       | eLinkable> traverse)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static com           | `getNati              | ::: block             |
        | .google.common.collec | veLinkables​(ActionGra | Extract from the      |
        | t.ImmutableList<? ext | phBuilder graphBuilde | dependency graph all  |
        | ends NativeLinkable>` | r,                    | the libraries which   |
        |                       | Iterable<? extends Na | must be considered    |
        |                       | tiveLinkable> inputs, | for linking.          |
        |                       |                    Li | :::                   |
        |                       | nker.LinkableDepType  |                       |
        |                       | linkStyle,            |                       |
        |                       |         java.util.fun |                       |
        |                       | ction.Predicate<? sup |                       |
        |                       | er NativeLinkable> tr |                       |
        |                       | averse,               |                       |
        |                       |      Optional<Linkabl |                       |
        |                       | eListFilter> filter)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static com           | `getNativeL           | ::: block             |
        | .google.common.collec | inkables​(ActionGraphB | Extract from the      |
        | t.ImmutableList<? ext | uilder graphBuilder,  | dependency graph all  |
        | ends NativeLinkable>` |                   Ite | the libraries which   |
        |                       | rable<? extends Nativ | must be considered    |
        |                       | eLinkable> inputs,    | for linking.          |
        |                       |                 Linke | :::                   |
        |                       | r.LinkableDepType lin |                       |
        |                       | kStyle,               |                       |
        |                       |      Optional<Linkabl |                       |
        |                       | eListFilter> filter)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static com           | `getT                 |                       |
        | .google.common.collec | opoSortedNativeLinkab |                       |
        | t.ImmutableList<? ext | les​(Iterable<? extend |                       |
        | ends NativeLinkable>` | s NativeLinkable> roo |                       |
        |                       | ts,                   |                       |
        |                       |            Topologica |                       |
        |                       | lSort.Traversable<Nat |                       |
        |                       | iveLinkable> depsFn)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static               | `getT                 | ::: block             |
        |  NativeLinkableInput` | ransitiveNativeLinkab | Collect up and merge  |
        |                       | leInput​(ActionGraphBu | all                   |
        |                       | ilder graphBuilder,   | [`NativeLinkableInp   |
        |                       |                       | ut`](NativeLinkableIn |
        |                       |           TargetConfi | put.html "class in co |
        |                       | guration targetConfig | m.facebook.buck.cxx.t |
        |                       | uration,              | oolchain.nativelink") |
        |                       |                     I | objects from          |
        |                       | terable<? extends Nat | transitively          |
        |                       | iveLinkable> roots,   | traversing all        |
        |                       |                       | unbroken dependency   |
        |                       |           Linker.Link | chains of             |
        |                       | ableDepType depType)` | [`NativeLinka         |
        |                       |                       | ble`](NativeLinkable. |
        |                       |                       | html "interface in co |
        |                       |                       | m.facebook.buck.cxx.t |
        |                       |                       | oolchain.nativelink") |
        |                       |                       | objects found via the |
        |                       |                       | passed in             |
        |                       |                       | [`NativeLinka         |
        |                       |                       | ble`](NativeLinkable. |
        |                       |                       | html "interface in co |
        |                       |                       | m.facebook.buck.cxx.t |
        |                       |                       | oolchain.nativelink") |
        |                       |                       | roots.                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static com           | `getTra               | ::: block             |
        | .google.common.collec | nsitiveNativeLinkable | Collect up and merge  |
        | t.ImmutableList<? ext | s​(ActionGraphBuilder  | all                   |
        | ends NativeLinkable>` | graphBuilder,         | [`NativeLinkableInp   |
        |                       |                       | ut`](NativeLinkableIn |
        |                       | Iterable<? extends Na | put.html "class in co |
        |                       | tiveLinkable> roots)` | m.facebook.buck.cxx.t |
        |                       |                       | oolchain.nativelink") |
        |                       |                       | objects from          |
        |                       |                       | transitively          |
        |                       |                       | traversing all        |
        |                       |                       | unbroken dependency   |
        |                       |                       | chains of             |
        |                       |                       | [`NativeLinka         |
        |                       |                       | ble`](NativeLinkable. |
        |                       |                       | html "interface in co |
        |                       |                       | m.facebook.buck.cxx.t |
        |                       |                       | oolchain.nativelink") |
        |                       |                       | objects found via the |
        |                       |                       | passed in             |
        |                       |                       | [`NativeLinka         |
        |                       |                       | ble`](NativeLinkable. |
        |                       |                       | html "interface in co |
        |                       |                       | m.facebook.buck.cxx.t |
        |                       |                       | oolchain.nativelink") |
        |                       |                       | roots.                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static c             | `getTransitiveSharedL | ::: block             |
        | om.google.common.coll | ibraries​(ActionGraphB | Collect all the       |
        | ect.ImmutableSortedMa | uilder graphBuilder,  | shared libraries      |
        | p<String,​SourcePath>` |                       | generated by          |
        |                       |        Iterable<? ext | [`NativeLinkab        |
        |                       | ends NativeLinkable>  | le`](NativeLinkable.h |
        |                       | roots,                | tml "interface in com |
        |                       |               boolean | .facebook.buck.cxx.to |
        |                       |  alwaysIncludeRoots)` | olchain.nativelink")s |
        |                       |                       | found by transitively |
        |                       |                       | traversing all        |
        |                       |                       | unbroken dependency   |
        |                       |                       | chains of             |
        |                       |                       | [`NativeLinka         |
        |                       |                       | ble`](NativeLinkable. |
        |                       |                       | html "interface in co |
        |                       |                       | m.facebook.buck.cxx.t |
        |                       |                       | oolchain.nativelink") |
        |                       |                       | objects found via the |
        |                       |                       | passed in             |
        |                       |                       | [`NativeLinka         |
        |                       |                       | ble`](NativeLinkable. |
        |                       |                       | html "interface in co |
        |                       |                       | m.facebook.buck.cxx.t |
        |                       |                       | oolchain.nativelink") |
        |                       |                       | roots.                |
        |                       |                       | :::                   |
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

        []{#getTopoSortedNativeLinkables(java.lang.Iterable,com.facebook.buck.core.util.graph.TopologicalSort.Traversable)}

        -   #### getTopoSortedNativeLinkables

            ``` methodSignature
            public static com.google.common.collect.ImmutableList<? extends NativeLinkable> getTopoSortedNativeLinkables​(Iterable<? extends NativeLinkable> roots,
                                                                                                                         TopologicalSort.Traversable<NativeLinkable> depsFn)
            ```

            [Returns:]{.returnLabel}
            :   the nodes found from traversing the given roots in
                topologically sorted order.

        []{#getNativeLinkables(com.facebook.buck.core.rules.ActionGraphBuilder,java.lang.Iterable,com.facebook.buck.cxx.toolchain.linker.Linker.LinkableDepType,java.util.function.Predicate,java.util.Optional)}

        -   #### getNativeLinkables

            ``` methodSignature
            public static com.google.common.collect.ImmutableList<? extends NativeLinkable> getNativeLinkables​(ActionGraphBuilder graphBuilder,
                                                                                                               Iterable<? extends NativeLinkable> inputs,
                                                                                                               Linker.LinkableDepType linkStyle,
                                                                                                               java.util.function.Predicate<? super NativeLinkable> traverse,
                                                                                                               Optional<LinkableListFilter> filter)
            ```

            ::: block
            Extract from the dependency graph all the libraries which
            must be considered for linking.
            Traversal proceeds depending on whether each dependency is
            to be statically or dynamically linked.
            :::

            [Parameters:]{.paramLabel}
            :   `linkStyle` - how dependencies should be linked, if
                their preferred_linkage is
                `      NativeLinkable.Linkage.ANY`.

        []{#getNativeLinkables(com.facebook.buck.core.rules.ActionGraphBuilder,java.lang.Iterable,com.facebook.buck.cxx.toolchain.linker.Linker.LinkableDepType,java.util.function.Predicate)}

        -   #### getNativeLinkables

            ``` methodSignature
            public static com.google.common.collect.ImmutableList<? extends NativeLinkable> getNativeLinkables​(ActionGraphBuilder graphBuilder,
                                                                                                               Iterable<? extends NativeLinkable> inputs,
                                                                                                               Linker.LinkableDepType linkStyle,
                                                                                                               java.util.function.Predicate<? super NativeLinkable> traverse)
            ```

            ::: block
            Extract from the dependency graph all the libraries which
            must be considered for linking.
            :::

        []{#getNativeLinkables(com.facebook.buck.core.rules.ActionGraphBuilder,java.lang.Iterable,com.facebook.buck.cxx.toolchain.linker.Linker.LinkableDepType)}

        -   #### getNativeLinkables

            ``` methodSignature
            public static com.google.common.collect.ImmutableList<? extends NativeLinkable> getNativeLinkables​(ActionGraphBuilder graphBuilder,
                                                                                                               Iterable<? extends NativeLinkable> inputs,
                                                                                                               Linker.LinkableDepType linkStyle)
            ```

            ::: block
            Extract from the dependency graph all the libraries which
            must be considered for linking.
            :::

        []{#getNativeLinkables(com.facebook.buck.core.rules.ActionGraphBuilder,java.lang.Iterable,com.facebook.buck.cxx.toolchain.linker.Linker.LinkableDepType,java.util.Optional)}

        -   #### getNativeLinkables

            ``` methodSignature
            public static com.google.common.collect.ImmutableList<? extends NativeLinkable> getNativeLinkables​(ActionGraphBuilder graphBuilder,
                                                                                                               Iterable<? extends NativeLinkable> inputs,
                                                                                                               Linker.LinkableDepType linkStyle,
                                                                                                               Optional<LinkableListFilter> filter)
            ```

            ::: block
            Extract from the dependency graph all the libraries which
            must be considered for linking.
            :::

        []{#getLinkStyle(com.facebook.buck.cxx.toolchain.nativelink.NativeLinkableGroup.Linkage,com.facebook.buck.cxx.toolchain.linker.Linker.LinkableDepType,java.util.Optional)}

        -   #### getLinkStyle

            ``` methodSignature
            public static Linker.LinkableDepType getLinkStyle​(NativeLinkableGroup.Linkage preferredLinkage,
                                                              Linker.LinkableDepType requestedLinkStyle,
                                                              Optional<PicType> picTypeForSharedLinking)
            ```

            ::: block
            Determine the final
            [`Linker.LinkableDepType`](../linker/Linker.LinkableDepType.html "enum in com.facebook.buck.cxx.toolchain.linker")
            given a preferred and requested linkage.
            :::

        []{#getLinkStyle(com.facebook.buck.cxx.toolchain.nativelink.NativeLinkableGroup.Linkage,com.facebook.buck.cxx.toolchain.linker.Linker.LinkableDepType)}

        -   #### getLinkStyle

            ``` methodSignature
            public static Linker.LinkableDepType getLinkStyle​(NativeLinkableGroup.Linkage preferredLinkage,
                                                              Linker.LinkableDepType requestedLinkStyle)
            ```

            ::: block
            Determine the final
            [`Linker.LinkableDepType`](../linker/Linker.LinkableDepType.html "enum in com.facebook.buck.cxx.toolchain.linker")
            given a preferred and requested linkage.
            :::

        []{#getNativeLinkableInput(com.facebook.buck.cxx.toolchain.linker.Linker.LinkableDepType,com.facebook.buck.cxx.toolchain.nativelink.NativeLinkable,com.facebook.buck.core.rules.ActionGraphBuilder,com.facebook.buck.core.model.TargetConfiguration)}

        -   #### getNativeLinkableInput

            ``` methodSignature
            public static NativeLinkableInput getNativeLinkableInput​(Linker.LinkableDepType linkStyle,
                                                                     NativeLinkable nativeLinkable,
                                                                     ActionGraphBuilder graphBuilder,
                                                                     TargetConfiguration targetConfiguration)
            ```

            ::: block
            Get the
            [`NativeLinkableInput`](NativeLinkableInput.html "class in com.facebook.buck.cxx.toolchain.nativelink")
            for a
            [`NativeLinkable`](NativeLinkable.html "interface in com.facebook.buck.cxx.toolchain.nativelink").
            :::

        []{#getTransitiveNativeLinkableInput(com.facebook.buck.core.rules.ActionGraphBuilder,com.facebook.buck.core.model.TargetConfiguration,java.lang.Iterable,com.facebook.buck.cxx.toolchain.linker.Linker.LinkableDepType)}

        -   #### getTransitiveNativeLinkableInput

            ``` methodSignature
            public static NativeLinkableInput getTransitiveNativeLinkableInput​(ActionGraphBuilder graphBuilder,
                                                                               TargetConfiguration targetConfiguration,
                                                                               Iterable<? extends NativeLinkable> roots,
                                                                               Linker.LinkableDepType depType)
            ```

            ::: block
            Collect up and merge all
            [`NativeLinkableInput`](NativeLinkableInput.html "class in com.facebook.buck.cxx.toolchain.nativelink")
            objects from transitively traversing all unbroken dependency
            chains of
            [`NativeLinkable`](NativeLinkable.html "interface in com.facebook.buck.cxx.toolchain.nativelink")
            objects found via the passed in
            [`NativeLinkable`](NativeLinkable.html "interface in com.facebook.buck.cxx.toolchain.nativelink")
            roots.
            :::

        []{#getTransitiveNativeLinkables(com.facebook.buck.core.rules.ActionGraphBuilder,java.lang.Iterable)}

        -   #### getTransitiveNativeLinkables

            ``` methodSignature
            public static com.google.common.collect.ImmutableList<? extends NativeLinkable> getTransitiveNativeLinkables​(ActionGraphBuilder graphBuilder,
                                                                                                                         Iterable<? extends NativeLinkable> roots)
            ```

            ::: block
            Collect up and merge all
            [`NativeLinkableInput`](NativeLinkableInput.html "class in com.facebook.buck.cxx.toolchain.nativelink")
            objects from transitively traversing all unbroken dependency
            chains of
            [`NativeLinkable`](NativeLinkable.html "interface in com.facebook.buck.cxx.toolchain.nativelink")
            objects found via the passed in
            [`NativeLinkable`](NativeLinkable.html "interface in com.facebook.buck.cxx.toolchain.nativelink")
            roots.
            :::

        []{#getTransitiveSharedLibraries(com.facebook.buck.core.rules.ActionGraphBuilder,java.lang.Iterable,boolean)}

        -   #### getTransitiveSharedLibraries

            ``` methodSignature
            public static com.google.common.collect.ImmutableSortedMap<String,​SourcePath> getTransitiveSharedLibraries​(ActionGraphBuilder graphBuilder,
                                                                                                                             Iterable<? extends NativeLinkable> roots,
                                                                                                                             boolean alwaysIncludeRoots)
            ```

            ::: block
            Collect all the shared libraries generated by
            [`NativeLinkable`](NativeLinkable.html "interface in com.facebook.buck.cxx.toolchain.nativelink")s
            found by transitively traversing all unbroken dependency
            chains of
            [`NativeLinkable`](NativeLinkable.html "interface in com.facebook.buck.cxx.toolchain.nativelink")
            objects found via the passed in
            [`NativeLinkable`](NativeLinkable.html "interface in com.facebook.buck.cxx.toolchain.nativelink")
            roots.
            :::

            [Parameters:]{.paramLabel}
            :   `alwaysIncludeRoots` - whether to include shared
                libraries from roots, even if they prefer static
                linkage.

            [Returns:]{.returnLabel}
            :   a mapping of library name to the library
                [`SourcePath`](../../../core/sourcepath/SourcePath.html "interface in com.facebook.buck.core.sourcepath").
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

-   [Overview](../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../deprecated-list.html)
-   [Index](../../../../../../index-all.html)
-   [Help](../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../allclasses.html)

<div>

<div>

JavaScript is disabled on your browser.

</div>

</div>

<div>

-   Summary: 
-   [Nested](#nested.class.summary) \| 
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
