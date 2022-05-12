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
[Package]{.packageLabelInType} [com.facebook.buck.core.cell](package-summary.html)
:::

## Class DefaultNewCellPathResolver {#class-defaultnewcellpathresolver .title title="Class DefaultNewCellPathResolver"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.cell.DefaultNewCellPathResolver

::: description
-   

    All Implemented Interfaces:
    :   `NewCellPathResolver`

    ------------------------------------------------------------------------

        public abstract class DefaultNewCellPathResolver
        extends Object
        implements NewCellPathResolver

    ::: block
    Implementation of
    [`NewCellPathResolver`](NewCellPathResolver.html "interface in com.facebook.buck.core.cell")
    based on the path to name map (this is assumed to be 1-1).
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                      Description
          -------------------------------- -------------
          `DefaultNewCellPathResolver()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `CanonicalCellName`   | `getCanonica          |                       |
        |                       | lCellName​(Path path)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Path`                | `getCellPath​(Canonic  | ::: block             |
        |                       | alCellName cellName)` | Note: unlike          |
        |                       |                       | [`CellPathRes         |
        |                       |                       | olver.getCellPath(Opt |
        |                       |                       | ional)`](CellPathReso |
        |                       |                       | lver.html#getCellPath |
        |                       |                       | (java.util.Optional)) |
        |                       |                       | this function always  |
        |                       |                       | returns a value.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static c             | `of​(Map               |                       |
        | om.facebook.buck.core | <? extends AbsPath,​?  |                       |
        | .cell.ImmutableDefaul | extends CanonicalCell |                       |
        | tNewCellPathResolver` | Name> pathToNameMap)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
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

        -   #### DefaultNewCellPathResolver

                public DefaultNewCellPathResolver()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getCellPath(com.facebook.buck.core.cell.name.CanonicalCellName)}

        -   #### getCellPath

            ``` methodSignature
            public Path getCellPath​(CanonicalCellName cellName)
            ```

            ::: block
            [Description copied from
            interface: `NewCellPathResolver`]{.descfrmTypeLabel}
            :::

            ::: block
            Note: unlike
            [`CellPathResolver.getCellPath(Optional)`](CellPathResolver.html#getCellPath(java.util.Optional))
            this function always returns a value. Existence/visibility
            of the cell is enforced when the
            [`CanonicalCellName`](name/CanonicalCellName.html "class in com.facebook.buck.core.cell.name")
            is resolved.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getCellPath` in interface `NewCellPathResolver`

            [Parameters:]{.paramLabel}
            :   `cellName` - Canonical name of the cell.

            [Returns:]{.returnLabel}
            :   Absolute path to the physical root of the cell.

        []{#getCanonicalCellName(java.nio.file.Path)}

        -   #### getCanonicalCellName

            ``` methodSignature
            public CanonicalCellName getCanonicalCellName​(Path path)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getCanonicalCellName` in
                interface `NewCellPathResolver`

            [Parameters:]{.paramLabel}
            :   `path` - Absolute path to the physical root of the cell.

            [Returns:]{.returnLabel}
            :   Canonical name of the cell.

        []{#of(java.util.Map)}

        -   #### of

            ``` methodSignature
            public static com.facebook.buck.core.cell.ImmutableDefaultNewCellPathResolver of​(Map<? extends AbsPath,​? extends CanonicalCellName> pathToNameMap)
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
