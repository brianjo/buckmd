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

## Class SelectorListFactory {#class-selectorlistfactory .title title="Class SelectorListFactory"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.select.impl.SelectorListFactory

::: description
-   

    ------------------------------------------------------------------------

        public class SelectorListFactory
        extends Object

    ::: block
    A factory to create
    [`SelectorList`](../SelectorList.html "class in com.facebook.buck.core.select")
    from raw (non-coerced) data.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                              Description
          -------------------------------------------------------- -------------
          `SelectorListFactory​(SelectorFactory selectorFactory)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `                     | `create​(C             | ::: block             |
        | SelectorList<Object>` | ellNameResolver cellN | Create                |
        |                       | ameResolver,       Fo | [`SelectorList`]      |
        |                       | rwardRelativePath pat | (../SelectorList.html |
        |                       | hRelativeToProjectRoo |  "class in com.facebo |
        |                       | t,       ListWithSele | ok.buck.core.select") |
        |                       | cts listWithSelects)` | using the given       |
        |                       |                       | elements to create    |
        |                       |                       | Selectors.            |
        |                       |                       | :::                   |
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

        []{#<init>(com.facebook.buck.core.select.impl.SelectorFactory)}

        -   #### SelectorListFactory

                public SelectorListFactory​(SelectorFactory selectorFactory)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#create(com.facebook.buck.core.cell.nameresolver.CellNameResolver,com.facebook.buck.core.path.ForwardRelativePath,com.facebook.buck.parser.syntax.ListWithSelects)}

        -   #### create

            ``` methodSignature
            public SelectorList<Object> create​(CellNameResolver cellNameResolver,
                                               ForwardRelativePath pathRelativeToProjectRoot,
                                               ListWithSelects listWithSelects)
            ```

            ::: block
            Create
            [`SelectorList`](../SelectorList.html "class in com.facebook.buck.core.select")
            using the given elements to create Selectors.
            :::

            [Parameters:]{.paramLabel}
            :   `listWithSelects` - a list of elements in a format
                produced after parsing build files (i.e. non-coerced.)
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
