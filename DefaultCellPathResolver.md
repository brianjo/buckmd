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
-   [Field](#field.summary) \| 
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.core.cell.impl](package-summary.html)
:::

## Class DefaultCellPathResolver {#class-defaultcellpathresolver .title title="Class DefaultCellPathResolver"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.core.cell.AbstractCellPathResolver](../AbstractCellPathResolver.html "class in com.facebook.buck.core.cell")

    -   -   com.facebook.buck.core.cell.impl.DefaultCellPathResolver

::: description
-   

    All Implemented Interfaces:
    :   `CellPathResolver`

    ------------------------------------------------------------------------

        public abstract class DefaultCellPathResolver
        extends AbstractCellPathResolver
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type   Field                    Description
          ------------------- ------------------------ -------------
          `static String`     `REPOSITORIES_SECTION`    

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                   Description
          ----------------------------- -------------
          `DefaultCellPathResolver()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `s                    | `bootstr              |                       |
        | tatic com.google.comm | apPathMapping​(AbsPath |                       |
        | on.collect.ImmutableM |  root,                |                       |
        | ap<CellName,​AbsPath>` |       Config config)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static Def           | `                     | ::: block             |
        | aultCellPathResolver` | create​(AbsPath root,  | Creates a             |
        |                       |       Config config)` | De                    |
        |                       |                       | faultCellPathResolver |
        |                       |                       | using the mappings in |
        |                       |                       | the provided          |
        |                       |                       | [`                    |
        |                       |                       | Config`](../../../uti |
        |                       |                       | l/config/Config.html  |
        |                       |                       | "class in com.faceboo |
        |                       |                       | k.buck.util.config"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static Def           | `create​(AbsPath root, |                       |
        | aultCellPathResolver` |        Map<String,​Abs |                       |
        |                       | Path> cellPaths,      |                       |
        |                       |   CellNameResolver ce |                       |
        |                       | llNameResolver,       |                       |
        |                       |  NewCellPathResolver  |                       |
        |                       | newCellPathResolver)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `getCanonicalCel      | ::: block             |
        |                       | lName​(Path cellPath)` | Returns a cell name   |
        |                       |                       | that can be used to   |
        |                       |                       | refer to the cell at  |
        |                       |                       | the given path.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `abstr                | `g                    | ::: block             |
        | act CellNameResolver` | etCellNameResolver()` | Provides access to    |
        |                       |                       | the                   |
        |                       |                       | [`CellName            |
        |                       |                       | Resolver`](../nameres |
        |                       |                       | olver/CellNameResolve |
        |                       |                       | r.html "interface in  |
        |                       |                       | com.facebook.buck.cor |
        |                       |                       | e.cell.nameresolver") |
        |                       |                       | for this cell.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Path>`      | `getCellPath​(Option   |                       |
        |                       | al<String> cellName)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `a                    | `getCellPathsByRo     |                       |
        | bstract com.google.co | otCellExternalName()` |                       |
        | mmon.collect.Immutabl |                       |                       |
        | eMap<String,​AbsPath>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google           | `getExter             | ::: block             |
        | .common.collect.Immut | nalNamesInRootCell()` | This gives the names  |
        | ableMap<Path,​String>` |                       | as they are specified |
        |                       |                       | in the root cell.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.c         | `getKnownRoots()`     |                       |
        | ommon.collect.Immutab |                       |                       |
        | leSortedSet<AbsPath>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract             | `getN                 | ::: block             |
        |  NewCellPathResolver` | ewCellPathResolver()` | Provides access to    |
        |                       |                       | the                   |
        |                       |                       | [`NewCellPat          |
        |                       |                       | hResolver`](../NewCel |
        |                       |                       | lPathResolver.html "i |
        |                       |                       | nterface in com.faceb |
        |                       |                       | ook.buck.core.cell"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.comm      | `getPathMapping()`    |                       |
        | on.collect.ImmutableM |                       |                       |
        | ap<CellName,​AbsPath>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract AbsPath`    | `getRoot()`           |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.core.cell.AbstractCellPathResolver}

            ### Methods inherited from class com.facebook.buck.core.cell.[AbstractCellPathResolver](../AbstractCellPathResolver.html "class in com.facebook.buck.core.cell")

            `getCellPathOrThrow, getCellPathOrThrow, resolveCellRelativePath`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.cell.CellPathResolver}

            ### Methods inherited from interface com.facebook.buck.core.cell.[CellPathResolver](../CellPathResolver.html "interface in com.facebook.buck.core.cell")

            `getCanonicalCellName, getCurrentCellName`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#field.detail}

        ### Field Detail

        []{#REPOSITORIES_SECTION}

        -   #### REPOSITORIES_SECTION

                public static final String REPOSITORIES_SECTION

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../constant-values.html#com.facebook.buck.core.cell.impl.DefaultCellPathResolver.REPOSITORIES_SECTION)
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### DefaultCellPathResolver

                public DefaultCellPathResolver()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getRoot()}

        -   #### getRoot

            ``` methodSignature
            public abstract AbsPath getRoot()
            ```

        []{#getCellPathsByRootCellExternalName()}

        -   #### getCellPathsByRootCellExternalName

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableMap<String,​AbsPath> getCellPathsByRootCellExternalName()
            ```

            [Returns:]{.returnLabel}
            :   absolute paths to all cells this resolver knows about.
                The key is the name of the cell in the root cell\'s
                config (this is not necessarily the canonical name).

        []{#getCellNameResolver()}

        -   #### getCellNameResolver

            ``` methodSignature
            public abstract CellNameResolver getCellNameResolver()
            ```

            ::: block
            [Description copied from
            interface: `CellPathResolver`]{.descfrmTypeLabel}
            :::

            ::: block
            Provides access to the
            [`CellNameResolver`](../nameresolver/CellNameResolver.html "interface in com.facebook.buck.core.cell.nameresolver")
            for this cell. This is to assist in migration to the new
            name/path resolvers.
            :::

        []{#getNewCellPathResolver()}

        -   #### getNewCellPathResolver

            ``` methodSignature
            public abstract NewCellPathResolver getNewCellPathResolver()
            ```

            ::: block
            [Description copied from
            interface: `CellPathResolver`]{.descfrmTypeLabel}
            :::

            ::: block
            Provides access to the
            [`NewCellPathResolver`](../NewCellPathResolver.html "interface in com.facebook.buck.core.cell").
            This is to assist in migration to the new name/path
            resolvers.
            :::

        []{#getExternalNamesInRootCell()}

        -   #### getExternalNamesInRootCell

            ``` methodSignature
            @Lazy
            public com.google.common.collect.ImmutableMap<Path,​String> getExternalNamesInRootCell()
            ```

            ::: block
            This gives the names as they are specified in the root cell.
            :::

        []{#getPathMapping()}

        -   #### getPathMapping

            ``` methodSignature
            @Lazy
            public com.google.common.collect.ImmutableMap<CellName,​AbsPath> getPathMapping()
            ```

        []{#getKnownRoots()}

        -   #### getKnownRoots

            ``` methodSignature
            @Lazy
            public com.google.common.collect.ImmutableSortedSet<AbsPath> getKnownRoots()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getKnownRoots` in interface `CellPathResolver`

            [Overrides:]{.overrideSpecifyLabel}
            :   `getKnownRoots` in class `AbstractCellPathResolver`

            [Returns:]{.returnLabel}
            :   sorted set of known roots in reverse natural order

        []{#create(com.facebook.buck.core.filesystems.AbsPath,java.util.Map,com.facebook.buck.core.cell.nameresolver.CellNameResolver,com.facebook.buck.core.cell.NewCellPathResolver)}

        -   #### create

            ``` methodSignature
            public static DefaultCellPathResolver create​(AbsPath root,
                                                         Map<String,​AbsPath> cellPaths,
                                                         CellNameResolver cellNameResolver,
                                                         NewCellPathResolver newCellPathResolver)
            ```

        []{#create(com.facebook.buck.core.filesystems.AbsPath,com.facebook.buck.util.config.Config)}

        -   #### create

            ``` methodSignature
            public static DefaultCellPathResolver create​(AbsPath root,
                                                         Config config)
            ```

            ::: block
            Creates a DefaultCellPathResolver using the mappings in the
            provided
            [`Config`](../../../util/config/Config.html "class in com.facebook.buck.util.config").
            This is the preferred way to create a
            DefaultCellPathResolver.
            :::

        []{#bootstrapPathMapping(com.facebook.buck.core.filesystems.AbsPath,com.facebook.buck.util.config.Config)}

        -   #### bootstrapPathMapping

            ``` methodSignature
            public static com.google.common.collect.ImmutableMap<CellName,​AbsPath> bootstrapPathMapping​(AbsPath root,
                                                                                                              Config config)
            ```

        []{#getCellPath(java.util.Optional)}

        -   #### getCellPath

            ``` methodSignature
            public Optional<Path> getCellPath​(Optional<String> cellName)
            ```

            [Parameters:]{.paramLabel}
            :   `cellName` - name of cell, Optional.empty() for root
                cell.

            [Returns:]{.returnLabel}
            :   Absolute path to the physical location of the cell, or
                `Optional.empty()` if the cell name cannot be resolved.

        []{#getCanonicalCellName(java.nio.file.Path)}

        -   #### getCanonicalCellName

            ``` methodSignature
            public Optional<String> getCanonicalCellName​(Path cellPath)
            ```

            ::: block
            [Description copied from
            interface: `CellPathResolver`]{.descfrmTypeLabel}
            :::

            ::: block
            Returns a cell name that can be used to refer to the cell at
            the given path.
            Returns `Optional.empty()` if the path refers to the root
            cell. Returns the lexicographically smallest name if the
            cell path has multiple names.

            Note: this is not the inverse of
            [`CellPathResolver.getCellPath(Optional)`](../CellPathResolver.html#getCellPath(java.util.Optional)),
            which returns the current, rather than the root, cell path
            if the cell name is empty.
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
-   [Field](#field.summary) \| 
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
-   [Constr](#constructor.detail) \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
