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
[Package]{.packageLabelInType} [com.facebook.buck.cxx.toolchain.nativelink](package-summary.html)
:::

## Class NativeLinkableGroups {#class-nativelinkablegroups .title title="Class NativeLinkableGroups"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.cxx.toolchain.nativelink.NativeLinkableGroups

::: description
-   

    ------------------------------------------------------------------------

        public class NativeLinkableGroups
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static               | `filterConsumer​(Buil  |                       |
        |  java.util.function.C | dRuleResolver resolve |                       |
        | onsumer<BuildTarget>` | r,               java |                       |
        |                       | .util.function.Consum |                       |
        |                       | er<? super NativeLink |                       |
        |                       | ableGroup> consumer)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static Li            | `getLinkSt            |                       |
        | nker.LinkableDepType` | yle​(NativeLinkableGro |                       |
        |                       | up.Linkage preferredL |                       |
        |                       | inkage,             L |                       |
        |                       | inker.LinkableDepType |                       |
        |                       |  requestedLinkStyle)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static <T> com.googl | `getNativeL           | ::: block             |
        | e.common.collect.Immu | inkableRoots​(Iterable | Find                  |
        | tableMap<BuildTarget, | <? extends T> from,   | [`                    |
        | ​NativeLinkableGroup>` |                       | NativeLinkableGroup`] |
        |                       | java.util.function.Fu | (NativeLinkableGroup. |
        |                       | nction<? super T,​Opti | html "interface in co |
        |                       | onal<Iterable<? exten | m.facebook.buck.cxx.t |
        |                       | ds T>>> passthrough)` | oolchain.nativelink") |
        |                       |                       | nodes transitively    |
        |                       |                       | reachable from the    |
        |                       |                       | given roots.          |
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

        []{#filterConsumer(com.facebook.buck.core.rules.BuildRuleResolver,java.util.function.Consumer)}

        -   #### filterConsumer

            ``` methodSignature
            public static java.util.function.Consumer<BuildTarget> filterConsumer​(BuildRuleResolver resolver,
                                                                                  java.util.function.Consumer<? super NativeLinkableGroup> consumer)
            ```

            [Returns:]{.returnLabel}
            :   a `Consumer` which accepts
                [`BuildTarget`](../../../core/model/BuildTarget.html "class in com.facebook.buck.core.model")s
                and filter-casts them
                [`NativeLinkableGroup`](NativeLinkableGroup.html "interface in com.facebook.buck.cxx.toolchain.nativelink")s.

        []{#getNativeLinkableRoots(java.lang.Iterable,java.util.function.Function)}

        -   #### getNativeLinkableRoots

            ``` methodSignature
            public static <T> com.google.common.collect.ImmutableMap<BuildTarget,​NativeLinkableGroup> getNativeLinkableRoots​(Iterable<? extends T> from,
                                                                                                                                   java.util.function.Function<? super T,​Optional<Iterable<? extends T>>> passthrough)
            ```

            ::: block
            Find
            [`NativeLinkableGroup`](NativeLinkableGroup.html "interface in com.facebook.buck.cxx.toolchain.nativelink")
            nodes transitively reachable from the given roots.
            :::

            [Parameters:]{.paramLabel}
            :   `from` - the starting set of roots to begin the search
                from.
            :   `passthrough` - a `Function` determining acceptable
                dependencies to traverse when searching for
                [`NativeLinkableGroup`](NativeLinkableGroup.html "interface in com.facebook.buck.cxx.toolchain.nativelink")s.

            [Returns:]{.returnLabel}
            :   all the roots found as a map from
                [`BuildTarget`](../../../core/model/BuildTarget.html "class in com.facebook.buck.core.model")
                to
                [`NativeLinkableGroup`](NativeLinkableGroup.html "interface in com.facebook.buck.cxx.toolchain.nativelink").

        []{#getLinkStyle(com.facebook.buck.cxx.toolchain.nativelink.NativeLinkableGroup.Linkage,com.facebook.buck.cxx.toolchain.linker.Linker.LinkableDepType)}

        -   #### getLinkStyle

            ``` methodSignature
            public static Linker.LinkableDepType getLinkStyle​(NativeLinkableGroup.Linkage preferredLinkage,
                                                              Linker.LinkableDepType requestedLinkStyle)
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
