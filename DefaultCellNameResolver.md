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
[Package]{.packageLabelInType} [com.facebook.buck.core.cell.nameresolver](package-summary.html)
:::

## Class DefaultCellNameResolver {#class-defaultcellnameresolver .title title="Class DefaultCellNameResolver"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.cell.nameresolver.DefaultCellNameResolver

::: description
-   

    All Implemented Interfaces:
    :   `CellNameResolver`

    ------------------------------------------------------------------------

        public abstract class DefaultCellNameResolver
        extends Object
        implements CellNameResolver

    ::: block
    Implementation of
    [`CellNameResolver`](CellNameResolver.html "interface in com.facebook.buck.core.cell.nameresolver")
    based on the known cells mapping.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                   Description
          ----------------------------- -------------
          `DefaultCellNameResolver()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `                     | `getKnownCells()`     | ::: block             |
        | abstract com.google.c |                       | Gets the mapping for  |
        | ommon.collect.Immutab |                       | all the available     |
        | leMap<Optional<String |                       | local names.          |
        | >,​CanonicalCellName>` |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CanonicalCellName`   | `getName​(Optiona      | ::: block             |
        |                       | l<String> localName)` | Resolves the local    |
        |                       |                       | name to the           |
        |                       |                       | [`CanonicalCel        |
        |                       |                       | lName`](../name/Canon |
        |                       |                       | icalCellName.html "cl |
        |                       |                       | ass in com.facebook.b |
        |                       |                       | uck.core.cell.name"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Optiona              | `getNam               | ::: block             |
        | l<CanonicalCellName>` | eIfResolvable​(Optiona | Returns the           |
        |                       | l<String> localName)` | [`CanonicalCe         |
        |                       |                       | llName`](../name/Cano |
        |                       |                       | nicalCellName.html "c |
        |                       |                       | lass in com.facebook. |
        |                       |                       | buck.core.cell.name") |
        |                       |                       | for this local name   |
        |                       |                       | if it can be          |
        |                       |                       | resolved.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static com.faceboo   | `of​(Map<? ext         |                       |
        | k.buck.core.cell.name | ends Optional<String> |                       |
        | resolver.ImmutableDef | ,​? extends CanonicalC |                       |
        | aultCellNameResolver` | ellName> knownCells)` |                       |
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

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.cell.nameresolver.CellNameResolver}

            ### Methods inherited from interface com.facebook.buck.core.cell.nameresolver.[CellNameResolver](CellNameResolver.html "interface in com.facebook.buck.core.cell.nameresolver")

            `getCurrentCellName`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### DefaultCellNameResolver

                public DefaultCellNameResolver()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getKnownCells()}

        -   #### getKnownCells

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableMap<Optional<String>,​CanonicalCellName> getKnownCells()
            ```

            ::: block
            [Description copied from
            interface: `CellNameResolver`]{.descfrmTypeLabel}
            :::

            ::: block
            Gets the mapping for all the available local names.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getKnownCells` in interface `CellNameResolver`

        []{#getNameIfResolvable(java.util.Optional)}

        -   #### getNameIfResolvable

            ``` methodSignature
            public Optional<CanonicalCellName> getNameIfResolvable​(Optional<String> localName)
            ```

            ::: block
            [Description copied from
            interface: `CellNameResolver`]{.descfrmTypeLabel}
            :::

            ::: block
            Returns the
            [`CanonicalCellName`](../name/CanonicalCellName.html "class in com.facebook.buck.core.cell.name")
            for this local name if it can be resolved.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getNameIfResolvable` in interface `CellNameResolver`

        []{#getName(java.util.Optional)}

        -   #### getName

            ``` methodSignature
            public CanonicalCellName getName​(Optional<String> localName)
            ```

            ::: block
            [Description copied from
            interface: `CellNameResolver`]{.descfrmTypeLabel}
            :::

            ::: block
            Resolves the local name to the
            [`CanonicalCellName`](../name/CanonicalCellName.html "class in com.facebook.buck.core.cell.name").
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getName` in interface `CellNameResolver`

        []{#of(java.util.Map)}

        -   #### of

            ``` methodSignature
            public static com.facebook.buck.core.cell.nameresolver.ImmutableDefaultCellNameResolver of​(Map<? extends Optional<String>,​? extends CanonicalCellName> knownCells)
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
