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
[Package]{.packageLabelInType} [com.facebook.buck.core.select.impl](package-summary.html)
:::

## Class SelectorFactory {#class-selectorfactory .title title="Class SelectorFactory"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.select.impl.SelectorFactory

::: description
-   

    ------------------------------------------------------------------------

        public class SelectorFactory
        extends Object

    ::: block
    Factory to create
    [`Selector`](../Selector.html "class in com.facebook.buck.core.select")
    using raw (non-coerced) data.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                Description
          ------------------------------------------------------------------------------------------ -------------
          `SelectorFactory​(UnconfiguredBuildTargetViewFactory unconfiguredBuildTargetViewFactory)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `Selector<Object>`    | `createS              | ::: block             |
        |                       | elector​(CellNameResol | Creates a new         |
        |                       | ver cellNameResolver, | Selector using the    |
        |                       |                Forwar | default error message |
        |                       | dRelativePath pathRel | when no conditions    |
        |                       | ativeToProjectRoot,   | match.                |
        |                       |              Map<Stri | :::                   |
        |                       | ng,​?> rawAttributes)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Selector<Object>`    | `cr                   | ::: block             |
        |                       | eateSelector​(CellName | Creates a             |
        |                       | Resolver cellNameReso | [`Select              |
        |                       | lver,               F | or`](../Selector.html |
        |                       | orwardRelativePath pa |  "class in com.facebo |
        |                       | thRelativeToProjectRo | ok.buck.core.select") |
        |                       | ot,               Map | by converting a given |
        |                       | <String,​?> rawAttribu | map.                  |
        |                       | tes,               St | :::                   |
        |                       | ring noMatchMessage)` |                       |
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

        []{#<init>(com.facebook.buck.core.parser.buildtargetparser.UnconfiguredBuildTargetViewFactory)}

        -   #### SelectorFactory

                public SelectorFactory​(UnconfiguredBuildTargetViewFactory unconfiguredBuildTargetViewFactory)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#createSelector(com.facebook.buck.core.cell.nameresolver.CellNameResolver,com.facebook.buck.core.path.ForwardRelativePath,java.util.Map)}

        -   #### createSelector

            ``` methodSignature
            public Selector<Object> createSelector​(CellNameResolver cellNameResolver,
                                                   ForwardRelativePath pathRelativeToProjectRoot,
                                                   Map<String,​?> rawAttributes)
            ```

            ::: block
            Creates a new Selector using the default error message when
            no conditions match.
            :::

        []{#createSelector(com.facebook.buck.core.cell.nameresolver.CellNameResolver,com.facebook.buck.core.path.ForwardRelativePath,java.util.Map,java.lang.String)}

        -   #### createSelector

            ``` methodSignature
            public Selector<Object> createSelector​(CellNameResolver cellNameResolver,
                                                   ForwardRelativePath pathRelativeToProjectRoot,
                                                   Map<String,​?> rawAttributes,
                                                   String noMatchMessage)
            ```

            ::: block
            Creates a
            [`Selector`](../Selector.html "class in com.facebook.buck.core.select")
            by converting a given map.
            :::

            [Parameters:]{.paramLabel}
            :   `rawAttributes` - a map with attributes represented in a
                format produced by build file parsers (i.e.
                non-coerced.)
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
