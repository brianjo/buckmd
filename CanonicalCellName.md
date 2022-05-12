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
[Package]{.packageLabelInType} [com.facebook.buck.core.cell.name](package-summary.html)
:::

## Class CanonicalCellName {#class-canonicalcellname .title title="Class CanonicalCellName"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.cell.name.CanonicalCellName

::: description
-   

    All Implemented Interfaces:
    :   `Comparable<CanonicalCellName>`

    ------------------------------------------------------------------------

        @Immutable(prehash=true,
                   builder=false,
                   copy=false,
                   intern=true)
        public abstract class CanonicalCellName
        extends Object
        implements Comparable<CanonicalCellName>

    ::: block
    Provides a canonical identifier for a
    [`Cell`](../Cell.html "interface in com.facebook.buck.core.cell").
    There is a 1-1 mapping between these.
    These should not be constructed by users and instead should only be
    acquired from a
    [`Cell`](../Cell.html "interface in com.facebook.buck.core.cell") or
    via a
    [`CellNameResolver`](../nameresolver/CellNameResolver.html "interface in com.facebook.buck.core.cell.nameresolver").
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor             Description
          ----------------------- -------------
          `CanonicalCellName()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `int`                 | `compareTo​(           |                       |
        |                       | CanonicalCellName o)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstr                | `getLegacyName()`     | ::: block             |
        | act Optional<String>` |                       | Returns the           |
        |                       |                       | underlying name in    |
        |                       |                       | the legacy            |
        |                       |                       | `Optional<String>`    |
        |                       |                       | format.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getName()`           | ::: block             |
        |                       |                       | Returns the name in a |
        |                       |                       | human-readable form.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `stat                 | `of​(Op                |                       |
        | ic CanonicalCellName` | tional<String> name)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `stat                 | `rootCell()`          |                       |
        | ic CanonicalCellName` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `toString()`          |                       |
        +-----------------------+-----------------------+-----------------------+
        | `stat                 | `unsafeNotACell()`    | ::: block             |
        | ic CanonicalCellName` |                       | This cell object is   |
        |                       |                       | used when there\'s no |
        |                       |                       | cell, but             |
        |                       |                       | [`Can                 |
        |                       |                       | onicalCellName`](Cano |
        |                       |                       | nicalCellName.html "c |
        |                       |                       | lass in com.facebook. |
        |                       |                       | buck.core.cell.name") |
        |                       |                       | object is needed.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `stat                 | `unsafeOf​(Op          | ::: block             |
        | ic CanonicalCellName` | tional<String> name)` | Used for creating     |
        |                       |                       | CanonicalCellName in  |
        |                       |                       | places where we       |
        |                       |                       | aren\'t guaranteed to |
        |                       |                       | be handling           |
        |                       |                       | canonicalization      |
        |                       |                       | correctly.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `stat                 | `unsafeRootCell()`    | ::: block             |
        | ic CanonicalCellName` |                       | This should be used   |
        |                       |                       | to mark places that   |
        |                       |                       | are hardcoding the    |
        |                       |                       | root cell\'s          |
        |                       |                       | canonical name in a   |
        |                       |                       | way that doesn\'t     |
        |                       |                       | ensure that it\'s     |
        |                       |                       | correct.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

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

        -   #### CanonicalCellName

                public CanonicalCellName()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#rootCell()}

        -   #### rootCell

            ``` methodSignature
            public static CanonicalCellName rootCell()
            ```

        []{#unsafeNotACell()}

        -   #### unsafeNotACell

            ``` methodSignature
            public static CanonicalCellName unsafeNotACell()
            ```

            ::: block
            This cell object is used when there\'s no cell, but
            [`CanonicalCellName`](CanonicalCellName.html "class in com.facebook.buck.core.cell.name")
            object is needed. This cell name is never resolved
            successfully to a cell.
            :::

        []{#unsafeRootCell()}

        -   #### unsafeRootCell

            ``` methodSignature
            public static CanonicalCellName unsafeRootCell()
            ```

            ::: block
            This should be used to mark places that are hardcoding the
            root cell\'s canonical name in a way that doesn\'t ensure
            that it\'s correct.
            :::

        []{#getLegacyName()}

        -   #### getLegacyName

            ``` methodSignature
            public abstract Optional<String> getLegacyName()
            ```

            ::: block
            Returns the underlying name in the legacy `Optional<String>`
            format.
            :::

        []{#getName()}

        -   #### getName

            ``` methodSignature
            public String getName()
            ```

            ::: block
            Returns the name in a human-readable form.
            :::

        []{#compareTo(com.facebook.buck.core.cell.name.CanonicalCellName)}

        -   #### compareTo

            ``` methodSignature
            public int compareTo​(CanonicalCellName o)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `compareTo` in interface `Comparable<CanonicalCellName>`

        []{#toString()}

        -   #### toString

            ``` methodSignature
            public String toString()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `toString` in class `Object`

        []{#of(java.util.Optional)}

        -   #### of

            ``` methodSignature
            public static CanonicalCellName of​(Optional<String> name)
            ```

        []{#unsafeOf(java.util.Optional)}

        -   #### unsafeOf

            ``` methodSignature
            public static CanonicalCellName unsafeOf​(Optional<String> name)
            ```

            ::: block
            Used for creating CanonicalCellName in places where we
            aren\'t guaranteed to be handling canonicalization
            correctly. This is only used to mark those places so that
            they are easier to find, the behavior is unchanged.
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
