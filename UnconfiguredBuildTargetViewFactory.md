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
[Package]{.packageLabelInType} [com.facebook.buck.core.parser.buildtargetparser](package-summary.html)
:::

## Interface UnconfiguredBuildTargetViewFactory {#interface-unconfiguredbuildtargetviewfactory .title title="Interface UnconfiguredBuildTargetViewFactory"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `ParsingUnconfiguredBuildTargetViewFactory`

    ------------------------------------------------------------------------

        public interface UnconfiguredBuildTargetViewFactory

    ::: block
    Creates
    [`UnconfiguredBuildTarget`](../../model/UnconfiguredBuildTarget.html "class in com.facebook.buck.core.model")
    from a raw string.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `Unc                  | `create​(St            | ::: block             |
        | onfiguredBuildTarget` | ring buildTargetName, | Given a               |
        |                       |        CellNameResolv | fully-qualified       |
        |                       | er cellNameResolver)` | target name returns   |
        |                       |                       | [`Unc                 |
        |                       |                       | onfiguredBuildTarget` |
        |                       |                       | ](../../model/Unconfi |
        |                       |                       | guredBuildTarget.html |
        |                       |                       |  "class in com.facebo |
        |                       |                       | ok.buck.core.model"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Unc                  | `crea                 | ::: block             |
        | onfiguredBuildTarget` | teForBaseName​(BaseNam | Given a target base   |
        |                       | e baseName,           | name and a target     |
        |                       |         String buildT | name returns          |
        |                       | argetName,            | [`Unc                 |
        |                       |        CellNameResolv | onfiguredBuildTarget` |
        |                       | er cellNameResolver)` | ](../../model/Unconfi |
        |                       |                       | guredBuildTarget.html |
        |                       |                       |  "class in com.facebo |
        |                       |                       | ok.buck.core.model"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Unc                  | `createForPathRelativ |                       |
        | onfiguredBuildTarget` | eToProjectRoot​(Forwar |                       |
        |                       | dRelativePath pathRel |                       |
        |                       | ativeToProjectRoot,   |                       |
        |                       |                       |                       |
        |                       |             String bu |                       |
        |                       | ildTargetName,        |                       |
        |                       |                       |                       |
        |                       |        CellNameResolv |                       |
        |                       | er cellNameResolver)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Unc                  | `createWithWi         | ::: block             |
        | onfiguredBuildTarget` | ldcard​(String buildTa | Given a target base   |
        |                       | rgetName,             | name and a target     |
        |                       |        CellNameResolv | name returns          |
        |                       | er cellNameResolver)` | [`Un                  |
        |                       |                       | configuredBuildTarget |
        |                       |                       | `](../../model/Unconf |
        |                       |                       | iguredBuildTarget.htm |
        |                       |                       | l "class in com.faceb |
        |                       |                       | ook.buck.core.model") |
        |                       |                       | with optionally       |
        |                       |                       | allowing the short    |
        |                       |                       | name to be empty.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#create(java.lang.String,com.facebook.buck.core.cell.nameresolver.CellNameResolver)}

        -   #### create

            ``` methodSignature
            UnconfiguredBuildTarget create​(String buildTargetName,
                                           CellNameResolver cellNameResolver)
            ```

            ::: block
            Given a fully-qualified target name returns
            [`UnconfiguredBuildTarget`](../../model/UnconfiguredBuildTarget.html "class in com.facebook.buck.core.model").
            A fully-qualified target name is the target name that
            uniquely identifies the target.

            Note that the cell name of the result build target can be
            different from the cell name specified in the target name.
            The build target contains a
            [`canonical cell name`](../../cell/CellPathResolver.html#getCanonicalCellName(java.nio.file.Path)).
            :::

            [See Also:]{.seeLabel}
            :   [`for more information about other      types of target names.`](#createForBaseName(com.facebook.buck.core.model.BaseName,java.lang.String,com.facebook.buck.core.cell.nameresolver.CellNameResolver))

        []{#createForBaseName(com.facebook.buck.core.model.BaseName,java.lang.String,com.facebook.buck.core.cell.nameresolver.CellNameResolver)}

        -   #### createForBaseName

            ``` methodSignature
            UnconfiguredBuildTarget createForBaseName​(BaseName baseName,
                                                      String buildTargetName,
                                                      CellNameResolver cellNameResolver)
            ```

            ::: block
            Given a target base name and a target name returns
            [`UnconfiguredBuildTarget`](../../model/UnconfiguredBuildTarget.html "class in com.facebook.buck.core.model").
            The target name may either be a fully-qualified name or a
            relative name. `baseName` is used when a relative name is
            given to correctly resolve the name of the target.

            For example, `//java/com/company/org:org` is a
            fully-qualified name. The same target is represented by a
            relative name `org` with base name `java/com/company/org`.

            Note that the cell name of the result build target can be
            different from the cell name specified in the target name.
            The build target contains a
            [`canonical cell name`](../../cell/CellPathResolver.html#getCanonicalCellName(java.nio.file.Path)).
            :::

        []{#createForPathRelativeToProjectRoot(com.facebook.buck.core.path.ForwardRelativePath,java.lang.String,com.facebook.buck.core.cell.nameresolver.CellNameResolver)}

        -   #### createForPathRelativeToProjectRoot

            ``` methodSignature
            UnconfiguredBuildTarget createForPathRelativeToProjectRoot​(ForwardRelativePath pathRelativeToProjectRoot,
                                                                       String buildTargetName,
                                                                       CellNameResolver cellNameResolver)
            ```

        []{#createWithWildcard(java.lang.String,com.facebook.buck.core.cell.nameresolver.CellNameResolver)}

        -   #### createWithWildcard

            ``` methodSignature
            UnconfiguredBuildTarget createWithWildcard​(String buildTargetName,
                                                       CellNameResolver cellNameResolver)
            ```

            ::: block
            Given a target base name and a target name returns
            [`UnconfiguredBuildTarget`](../../model/UnconfiguredBuildTarget.html "class in com.facebook.buck.core.model")
            with optionally allowing the short name to be empty.
            The target name may either be a fully-qualified name or a
            target name pattern.

            For example, `//java/com/company/org:org` is a
            fully-qualified name. `  //java/com/company/org:` is an
            example of a target with a pattern.

            Note that the cell name of the result build target can be
            different from the cell name specified in the target name.
            The build target contains a
            [`canonical cell name`](../../cell/CellPathResolver.html#getCanonicalCellName(java.nio.file.Path)).
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
