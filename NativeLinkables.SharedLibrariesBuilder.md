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
[Package]{.packageLabelInType} [com.facebook.buck.cxx.toolchain.nativelink](package-summary.html)
:::

## Class NativeLinkables.SharedLibrariesBuilder {#class-nativelinkables.sharedlibrariesbuilder .title title="Class NativeLinkables.SharedLibrariesBuilder"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.cxx.toolchain.nativelink.NativeLinkables.SharedLibrariesBuilder

::: description
-   

    Enclosing class:
    :   [NativeLinkables](NativeLinkables.html "class in com.facebook.buck.cxx.toolchain.nativelink")

    ------------------------------------------------------------------------

        public static class NativeLinkables.SharedLibrariesBuilder
        extends Object

    ::: block
    Builds a map of shared library names to paths from
    [`NativeLinkable`](NativeLinkable.html "interface in com.facebook.buck.cxx.toolchain.nativelink")s,
    throwing a useful error on duplicates.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                  Description
          ---------------------------- -------------
          `SharedLibrariesBuilder()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `NativeLinkables.Sh   | `                     | ::: block             |
        | aredLibrariesBuilder` | addAll​(ActionGraphBui | Adds libraries from   |
        |                       | lder graphBuilder,    | the given             |
        |                       |     Collection<Native | [`Na                  |
        |                       | Linkable> linkables)` | tiveLinkableGroup`](N |
        |                       |                       | ativeLinkableGroup.ht |
        |                       |                       | ml "interface in com. |
        |                       |                       | facebook.buck.cxx.too |
        |                       |                       | lchain.nativelink")s, |
        |                       |                       | potentially in        |
        |                       |                       | parallel.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `c                    | `build()`             |                       |
        | om.google.common.coll |                       |                       |
        | ect.ImmutableSortedMa |                       |                       |
        | p<String,​SourcePath>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+

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

        []{#<init>()}

        -   #### SharedLibrariesBuilder

                public SharedLibrariesBuilder()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#addAll(com.facebook.buck.core.rules.ActionGraphBuilder,java.util.Collection)}

        -   #### addAll

            ``` methodSignature
            public NativeLinkables.SharedLibrariesBuilder addAll​(ActionGraphBuilder graphBuilder,
                                                                 Collection<NativeLinkable> linkables)
            ```

            ::: block
            Adds libraries from the given
            [`NativeLinkableGroup`](NativeLinkableGroup.html "interface in com.facebook.buck.cxx.toolchain.nativelink")s,
            potentially in parallel.
            :::

        []{#build()}

        -   #### build

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedMap<String,​SourcePath> build()
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
