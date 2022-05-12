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
[Package]{.packageLabelInType} [com.facebook.buck.core.model](package-summary.html)
:::

## Class UnflavoredBuildTarget {#class-unflavoredbuildtarget .title title="Class UnflavoredBuildTarget"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.model.UnflavoredBuildTarget

::: description
-   

    All Implemented Interfaces:
    :   `DependencyStack.Element`, `DependencyStack.ProvidesElement`,
        `Comparable<UnflavoredBuildTarget>`

    ------------------------------------------------------------------------

        public class UnflavoredBuildTarget
        extends Object
        implements Comparable<UnflavoredBuildTarget>, DependencyStack.Element

    ::: block
    A build target in the form of
        cell//path:rule
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `int`                 | `compareTo​(Unfl       |                       |
        |                       | avoredBuildTarget o)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `equals​(Object o)`    |                       |
        +-----------------------+-----------------------+-----------------------+
        | `BaseName`            | `getBaseName()`       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `CanonicalCellName`   | `getCell()`           |                       |
        +-----------------------+-----------------------+-----------------------+
        | `CellRelativePath`    | `getCe                |                       |
        |                       | llRelativeBasePath()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `get                  |                       |
        |                       | FullyQualifiedName()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getLocalName()`      |                       |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `hashCode()`          |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static U             | `of​(Ca                | ::: block             |
        | nflavoredBuildTarget` | nonicalCellName cell, | A constructor.        |
        |                       |    BaseName baseName, | :::                   |
        |                       |    String localName)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static U             | `of​(CellRelativePath  | ::: block             |
        | nflavoredBuildTarget` | cellRelativeBasePath, | A constructor.        |
        |                       |    String shortName)` | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `toString()`          |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, finalize, getClass, notify, notifyAll, wait, wait, wait`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.exceptions.DependencyStack.Element}

            ### Methods inherited from interface com.facebook.buck.core.exceptions.[DependencyStack.Element](../exceptions/DependencyStack.Element.html "interface in com.facebook.buck.core.exceptions")

            `getElement`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getLocalName()}

        -   #### getLocalName

            ``` methodSignature
            public String getLocalName()
            ```

        []{#toString()}

        -   #### toString

            ``` methodSignature
            public String toString()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `toString` in class `Object`

        []{#hashCode()}

        -   #### hashCode

            ``` methodSignature
            public int hashCode()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `hashCode` in class `Object`

        []{#equals(java.lang.Object)}

        -   #### equals

            ``` methodSignature
            public boolean equals​(Object o)
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `equals` in class `Object`

        []{#compareTo(com.facebook.buck.core.model.UnflavoredBuildTarget)}

        -   #### compareTo

            ``` methodSignature
            public int compareTo​(UnflavoredBuildTarget o)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `compareTo` in
                interface `Comparable<UnflavoredBuildTarget>`

        []{#of(com.facebook.buck.core.model.CellRelativePath,java.lang.String)}

        -   #### of

            ``` methodSignature
            public static UnflavoredBuildTarget of​(CellRelativePath cellRelativeBasePath,
                                                   String shortName)
            ```

            ::: block
            A constructor.
            :::

        []{#of(com.facebook.buck.core.cell.name.CanonicalCellName,com.facebook.buck.core.model.BaseName,java.lang.String)}

        -   #### of

            ``` methodSignature
            public static UnflavoredBuildTarget of​(CanonicalCellName cell,
                                                   BaseName baseName,
                                                   String localName)
            ```

            ::: block
            A constructor.
            :::

        []{#getCell()}

        -   #### getCell

            ``` methodSignature
            public CanonicalCellName getCell()
            ```

        []{#getBaseName()}

        -   #### getBaseName

            ``` methodSignature
            public BaseName getBaseName()
            ```

        []{#getFullyQualifiedName()}

        -   #### getFullyQualifiedName

            ``` methodSignature
            public String getFullyQualifiedName()
            ```

        []{#getCellRelativeBasePath()}

        -   #### getCellRelativeBasePath

            ``` methodSignature
            public CellRelativePath getCellRelativeBasePath()
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
