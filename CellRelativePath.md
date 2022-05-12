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

-   [Overview](../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../deprecated-list.html)
-   [Index](../../../../../index-all.html)
-   [Help](../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.core.model](package-summary.html)
:::

## Class CellRelativePath {#class-cellrelativepath .title title="Class CellRelativePath"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.model.CellRelativePath

::: description
-   

    All Implemented Interfaces:
    :   `Comparable<CellRelativePath>`

    ------------------------------------------------------------------------

        public abstract class CellRelativePath
        extends Object
        implements Comparable<CellRelativePath>

    ::: block
    A pair of
    [`CanonicalCellName`](../cell/name/CanonicalCellName.html "class in com.facebook.buck.core.cell.name")
    and
    [`ForwardRelativePath`](../path/ForwardRelativePath.html "class in com.facebook.buck.core.path")
    relative the the cell.
    This object can identify a buck package or a buck file.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor            Description
          ---------------------- -------------
          `CellRelativePath()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                Method                                                         Description
          -------------------------------- -------------------------------------------------------------- -------------
          `int`                            `compareTo​(CellRelativePath that)`                              
          `abstract CanonicalCellName`     `getCellName()`                                                 
          `abstract ForwardRelativePath`   `getPath()`                                                     
          `static CellRelativePath`        `of​(CanonicalCellName cellName,   ForwardRelativePath path)`    
          `boolean`                        `startsWith​(CellRelativePath other)`                            
          `String`                         `toString()`                                                    

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

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### CellRelativePath

                public CellRelativePath()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getCellName()}

        -   #### getCellName

            ``` methodSignature
            public abstract CanonicalCellName getCellName()
            ```

        []{#getPath()}

        -   #### getPath

            ``` methodSignature
            public abstract ForwardRelativePath getPath()
            ```

        []{#startsWith(com.facebook.buck.core.model.CellRelativePath)}

        -   #### startsWith

            ``` methodSignature
            public boolean startsWith​(CellRelativePath other)
            ```

        []{#toString()}

        -   #### toString

            ``` methodSignature
            public String toString()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `toString` in class `Object`

        []{#compareTo(com.facebook.buck.core.model.CellRelativePath)}

        -   #### compareTo

            ``` methodSignature
            public int compareTo​(CellRelativePath that)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `compareTo` in interface `Comparable<CellRelativePath>`

        []{#of(com.facebook.buck.core.cell.name.CanonicalCellName,com.facebook.buck.core.path.ForwardRelativePath)}

        -   #### of

            ``` methodSignature
            public static CellRelativePath of​(CanonicalCellName cellName,
                                              ForwardRelativePath path)
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

-   [Overview](../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../deprecated-list.html)
-   [Index](../../../../../index-all.html)
-   [Help](../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../allclasses.html)

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
