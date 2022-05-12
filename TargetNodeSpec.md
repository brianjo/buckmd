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
-   [Nested](#nested.class.summary) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.parser.spec](package-summary.html)
:::

## Interface TargetNodeSpec {#interface-targetnodespec .title title="Interface TargetNodeSpec"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `BuildTargetSpec`, `TargetNodePredicateSpec`

    ------------------------------------------------------------------------

        public interface TargetNodeSpec

    ::: block
    A specification used by the parser to match
    [`TargetNode`](../../core/model/targetgraph/TargetNode.html "interface in com.facebook.buck.core.model.targetgraph")
    objects.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type   Interface                     Description
          ------------------- ----------------------------- -------------
          `static class `     `TargetNodeSpec.TargetType`    

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `com.google.common    | `filter​(Ite           |                       |
        | .collect.ImmutableMap | rable<TargetNodeMaybe |                       |
        | <BuildTarget,​TargetNo | Incompatible> nodes)` |                       |
        | deMaybeIncompatible>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `BuildFileSpec`       | `getBuildFileSpec()`  |                       |
        +-----------------------+-----------------------+-----------------------+
        | `BuildTargetPattern`  | `getBuildTarg         | ::: block             |
        |                       | etPattern​(Cell cell)` | Convert from a legacy |
        |                       |                       | [`TargetNodeSpec`](Ta |
        |                       |                       | rgetNodeSpec.html "in |
        |                       |                       | terface in com.facebo |
        |                       |                       | ok.buck.parser.spec") |
        |                       |                       | to a new-hotness      |
        |                       |                       | [`BuildTargetPatter   |
        |                       |                       | n`](../../core/parser |
        |                       |                       | /buildtargetpattern/B |
        |                       |                       | uildTargetPattern.htm |
        |                       |                       | l "class in com.faceb |
        |                       |                       | ook.buck.core.parser. |
        |                       |                       | buildtargetpattern"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Targe                | `getTargetType()`     |                       |
        | tNodeSpec.TargetType` |                       |                       |
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

        []{#getTargetType()}

        -   #### getTargetType

            ``` methodSignature
            TargetNodeSpec.TargetType getTargetType()
            ```

            [Returns:]{.returnLabel}
            :   whether spec is a single target requested by a name or a
                list of targets requested with recursive spec (i.e. \...
                )

        []{#filter(java.lang.Iterable)}

        -   #### filter

            ``` methodSignature
            com.google.common.collect.ImmutableMap<BuildTarget,​TargetNodeMaybeIncompatible> filter​(Iterable<TargetNodeMaybeIncompatible> nodes)
            ```

            [Returns:]{.returnLabel}
            :   the targets which should be built according to this spec

        []{#getBuildFileSpec()}

        -   #### getBuildFileSpec

            ``` methodSignature
            BuildFileSpec getBuildFileSpec()
            ```

            [Returns:]{.returnLabel}
            :   a
                [`BuildFileSpec`](BuildFileSpec.html "class in com.facebook.buck.parser.spec")
                representing the build files to parse to search for
                specific build target.

        []{#getBuildTargetPattern(com.facebook.buck.core.cell.Cell)}

        -   #### getBuildTargetPattern

            ``` methodSignature
            BuildTargetPattern getBuildTargetPattern​(Cell cell)
            ```

            ::: block
            Convert from a legacy
            [`TargetNodeSpec`](TargetNodeSpec.html "interface in com.facebook.buck.parser.spec")
            to a new-hotness
            [`BuildTargetPattern`](../../core/parser/buildtargetpattern/BuildTargetPattern.html "class in com.facebook.buck.core.parser.buildtargetpattern").
            This conversion is imperfect and best-effort. If possible,
            use
            [`BuildTargetPatternParser.parse(String, CellNameResolver)`](../../core/parser/buildtargetpattern/BuildTargetPatternParser.html#parse(java.lang.String,com.facebook.buck.core.cell.nameresolver.CellNameResolver))
            to create a
            [`BuildTargetPattern`](../../core/parser/buildtargetpattern/BuildTargetPattern.html "class in com.facebook.buck.core.parser.buildtargetpattern")
            instead.

            This conversion is lossy. Some attributes, such as whether
            test targets should be included, are not reflected in the
            result.
            :::

            [Parameters:]{.paramLabel}
            :   `cell` - this
                [`TargetNodeSpec`](TargetNodeSpec.html "interface in com.facebook.buck.parser.spec")\'s
                cell. Some implementations of
                [`TargetNodeSpec`](TargetNodeSpec.html "interface in com.facebook.buck.parser.spec")
                do not store a cell name, so `cell` provides the name.

            [Returns:]{.returnLabel}
            :   a pattern matching the same targets as this pattern.

            [Throws:]{.throwsLabel}
            :   `IllegalArgumentException` - `cell` refers to a cell
                different from this
                [`TargetNodeSpec`](TargetNodeSpec.html "interface in com.facebook.buck.parser.spec")\'s
                cell. This exception is best-effort.
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
-   [Nested](#nested.class.summary) \| 
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
