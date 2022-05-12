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
[Package]{.packageLabelInType} [com.facebook.buck.parser.spec](package-summary.html)
:::

## Class BuildTargetSpec {#class-buildtargetspec .title title="Class BuildTargetSpec"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.parser.spec.BuildTargetSpec

::: description
-   

    All Implemented Interfaces:
    :   `TargetNodeSpec`

    ------------------------------------------------------------------------

        public abstract class BuildTargetSpec
        extends Object
        implements TargetNodeSpec

    ::: block
    Matches a
    [`TargetNode`](../../core/model/targetgraph/TargetNode.html "interface in com.facebook.buck.core.model.targetgraph")
    that corresponds to a single build target
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        -   []{#nested.classes.inherited.from.class.com.facebook.buck.parser.spec.TargetNodeSpec}

            ### Nested classes/interfaces inherited from interface com.facebook.buck.parser.spec.[TargetNodeSpec](TargetNodeSpec.html "interface in com.facebook.buck.parser.spec")

            `TargetNodeSpec.TargetType`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor           Description
          --------------------- -------------
          `BuildTargetSpec()`    

          : Constructors[ ]{.tabEnd}
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
        | `st                   | `from​(Unconfigure     | ::: block             |
        | atic BuildTargetSpec` | dBuildTarget target)` | Create new instance   |
        |                       |                       | of                    |
        |                       |                       | [`BuildTargetSpec`]   |
        |                       |                       | (BuildTargetSpec.html |
        |                       |                       |  "class in com.facebo |
        |                       |                       | ok.buck.parser.spec") |
        |                       |                       | and automatically     |
        |                       |                       | resolve               |
        |                       |                       | [`BuildFileSpec       |
        |                       |                       | `](BuildFileSpec.html |
        |                       |                       |  "class in com.facebo |
        |                       |                       | ok.buck.parser.spec") |
        |                       |                       | based on              |
        |                       |                       | [`Unconfi             |
        |                       |                       | guredBuildTarget`](.. |
        |                       |                       | /../core/model/Unconf |
        |                       |                       | iguredBuildTarget.htm |
        |                       |                       | l "class in com.faceb |
        |                       |                       | ook.buck.core.model") |
        |                       |                       | properties.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `st                   | `from​(Unconfigured    | ::: block             |
        | atic BuildTargetSpec` | BuildTargetWithOutput | Returns a new         |
        |                       | s targetWithOutputs)` | instance of           |
        |                       |                       | [`BuildTargetSpec`]   |
        |                       |                       | (BuildTargetSpec.html |
        |                       |                       |  "class in com.facebo |
        |                       |                       | ok.buck.parser.spec") |
        |                       |                       | and automatically     |
        |                       |                       | resolve               |
        |                       |                       | [`BuildFileSpec       |
        |                       |                       | `](BuildFileSpec.html |
        |                       |                       |  "class in com.facebo |
        |                       |                       | ok.buck.parser.spec") |
        |                       |                       | based on              |
        |                       |                       | [`Unconfi             |
        |                       |                       | guredBuildTarget`](.. |
        |                       |                       | /../core/model/Unconf |
        |                       |                       | iguredBuildTarget.htm |
        |                       |                       | l "class in com.faceb |
        |                       |                       | ook.buck.core.model") |
        |                       |                       | properties.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ab                   | `getBuildFileSpec()`  |                       |
        | stract BuildFileSpec` |                       |                       |
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
        | `Unc                  | `getUncon             |                       |
        | onfiguredBuildTarget` | figuredBuildTarget()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `ab                   | `ge                   |                       |
        | stract UnconfiguredBu | tUnconfiguredBuildTar |                       |
        | ildTargetWithOutputs` | getViewWithOutputs()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `st                   | `of​(UnconfiguredBuild | ::: block             |
        | atic BuildTargetSpec` | Target unconfiguredBu | Returns a             |
        |                       | ildTarget,   BuildFil | `BuildTargetSpec`     |
        |                       | eSpec buildFileSpec)` | with an empty output  |
        |                       |                       | label.                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `toString()`          |                       |
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

        -   #### BuildTargetSpec

                public BuildTargetSpec()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getUnconfiguredBuildTargetViewWithOutputs()}

        -   #### getUnconfiguredBuildTargetViewWithOutputs

            ``` methodSignature
            public abstract UnconfiguredBuildTargetWithOutputs getUnconfiguredBuildTargetViewWithOutputs()
            ```

            [Returns:]{.returnLabel}
            :   Build target to match with this spec and its output
                label, if any

        []{#getUnconfiguredBuildTarget()}

        -   #### getUnconfiguredBuildTarget

            ``` methodSignature
            public UnconfiguredBuildTarget getUnconfiguredBuildTarget()
            ```

        []{#of(com.facebook.buck.core.model.UnconfiguredBuildTarget,com.facebook.buck.parser.spec.BuildFileSpec)}

        -   #### of

            ``` methodSignature
            public static BuildTargetSpec of​(UnconfiguredBuildTarget unconfiguredBuildTarget,
                                             BuildFileSpec buildFileSpec)
            ```

            ::: block
            Returns a `BuildTargetSpec` with an empty output label.
            :::

        []{#getBuildFileSpec()}

        -   #### getBuildFileSpec

            ``` methodSignature
            public abstract BuildFileSpec getBuildFileSpec()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getBuildFileSpec` in interface `TargetNodeSpec`

            [Returns:]{.returnLabel}
            :   a
                [`BuildFileSpec`](BuildFileSpec.html "class in com.facebook.buck.parser.spec")
                representing the build files to parse to search for
                specific build target.

        []{#from(com.facebook.buck.core.model.UnconfiguredBuildTargetWithOutputs)}

        -   #### from

            ``` methodSignature
            public static BuildTargetSpec from​(UnconfiguredBuildTargetWithOutputs targetWithOutputs)
            ```

            ::: block
            Returns a new instance of
            [`BuildTargetSpec`](BuildTargetSpec.html "class in com.facebook.buck.parser.spec")
            and automatically resolve
            [`BuildFileSpec`](BuildFileSpec.html "class in com.facebook.buck.parser.spec")
            based on
            [`UnconfiguredBuildTarget`](../../core/model/UnconfiguredBuildTarget.html "class in com.facebook.buck.core.model")
            properties. The returned
            [`BuildTargetSpec`](BuildTargetSpec.html "class in com.facebook.buck.parser.spec")
            may carry a non-empty output label through
            [`UnconfiguredBuildTargetWithOutputs`](../../core/model/UnconfiguredBuildTargetWithOutputs.html "class in com.facebook.buck.core.model").
            :::

            [Parameters:]{.paramLabel}
            :   `targetWithOutputs` - Build target to match

        []{#from(com.facebook.buck.core.model.UnconfiguredBuildTarget)}

        -   #### from

            ``` methodSignature
            public static BuildTargetSpec from​(UnconfiguredBuildTarget target)
            ```

            ::: block
            Create new instance of
            [`BuildTargetSpec`](BuildTargetSpec.html "class in com.facebook.buck.parser.spec")
            and automatically resolve
            [`BuildFileSpec`](BuildFileSpec.html "class in com.facebook.buck.parser.spec")
            based on
            [`UnconfiguredBuildTarget`](../../core/model/UnconfiguredBuildTarget.html "class in com.facebook.buck.core.model")
            properties. The returned
            [`BuildTargetSpec`](BuildTargetSpec.html "class in com.facebook.buck.parser.spec")
            carries an empty output label.
            :::

            [Parameters:]{.paramLabel}
            :   `target` - Build target to match

        []{#getTargetType()}

        -   #### getTargetType

            ``` methodSignature
            public TargetNodeSpec.TargetType getTargetType()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getTargetType` in interface `TargetNodeSpec`

            [Returns:]{.returnLabel}
            :   whether spec is a single target requested by a name or a
                list of targets requested with recursive spec (i.e. \...
                )

        []{#filter(java.lang.Iterable)}

        -   #### filter

            ``` methodSignature
            public com.google.common.collect.ImmutableMap<BuildTarget,​TargetNodeMaybeIncompatible> filter​(Iterable<TargetNodeMaybeIncompatible> nodes)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `filter` in interface `TargetNodeSpec`

            [Returns:]{.returnLabel}
            :   the targets which should be built according to this spec

        []{#getBuildTargetPattern(com.facebook.buck.core.cell.Cell)}

        -   #### getBuildTargetPattern

            ``` methodSignature
            public BuildTargetPattern getBuildTargetPattern​(Cell cell)
            ```

            ::: block
            [Description copied from
            interface: `TargetNodeSpec`]{.descfrmTypeLabel}
            :::

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

            [Specified by:]{.overrideSpecifyLabel}
            :   `getBuildTargetPattern` in interface `TargetNodeSpec`

            [Parameters:]{.paramLabel}
            :   `cell` - this
                [`TargetNodeSpec`](TargetNodeSpec.html "interface in com.facebook.buck.parser.spec")\'s
                cell. Some implementations of
                [`TargetNodeSpec`](TargetNodeSpec.html "interface in com.facebook.buck.parser.spec")
                do not store a cell name, so `cell` provides the name.

            [Returns:]{.returnLabel}
            :   a pattern matching the same targets as this pattern.

        []{#toString()}

        -   #### toString

            ``` methodSignature
            public String toString()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `toString` in class `Object`
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
