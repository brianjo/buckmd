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
[Package]{.packageLabelInType} [com.facebook.buck.core.parser.buildtargetparser](package-summary.html)
:::

## Class ParsingUnconfiguredBuildTargetViewFactory {#class-parsingunconfiguredbuildtargetviewfactory .title title="Class ParsingUnconfiguredBuildTargetViewFactory"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.parser.buildtargetparser.ParsingUnconfiguredBuildTargetViewFactory

::: description
-   

    All Implemented Interfaces:
    :   `UnconfiguredBuildTargetViewFactory`

    ------------------------------------------------------------------------

        public class ParsingUnconfiguredBuildTargetViewFactory
        extends Object
        implements UnconfiguredBuildTargetViewFactory

    ::: block
    A factory that parses a given build target name using the provided
    `BuildTargetParser`.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                     Description
          ----------------------------------------------- -------------
          `ParsingUnconfiguredBuildTargetViewFactory()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
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

        -   #### ParsingUnconfiguredBuildTargetViewFactory

                public ParsingUnconfiguredBuildTargetViewFactory()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#create(java.lang.String,com.facebook.buck.core.cell.nameresolver.CellNameResolver)}

        -   #### create

            ``` methodSignature
            public UnconfiguredBuildTarget create​(String buildTargetName,
                                                  CellNameResolver cellNameResolver)
            ```

            ::: block
            [Description copied from
            interface: `UnconfiguredBuildTargetViewFactory`]{.descfrmTypeLabel}
            :::

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

            [Specified by:]{.overrideSpecifyLabel}
            :   `create` in
                interface `UnconfiguredBuildTargetViewFactory`

            [See Also:]{.seeLabel}
            :   [`for more information about other      types of target names.`](UnconfiguredBuildTargetViewFactory.html#createForBaseName(com.facebook.buck.core.model.BaseName,java.lang.String,com.facebook.buck.core.cell.nameresolver.CellNameResolver))

        []{#createForBaseName(com.facebook.buck.core.model.BaseName,java.lang.String,com.facebook.buck.core.cell.nameresolver.CellNameResolver)}

        -   #### createForBaseName

            ``` methodSignature
            public UnconfiguredBuildTarget createForBaseName​(BaseName baseName,
                                                             String buildTargetName,
                                                             CellNameResolver cellNameResolver)
            ```

            ::: block
            [Description copied from
            interface: `UnconfiguredBuildTargetViewFactory`]{.descfrmTypeLabel}
            :::

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

            [Specified by:]{.overrideSpecifyLabel}
            :   `createForBaseName` in
                interface `UnconfiguredBuildTargetViewFactory`

        []{#createForPathRelativeToProjectRoot(com.facebook.buck.core.path.ForwardRelativePath,java.lang.String,com.facebook.buck.core.cell.nameresolver.CellNameResolver)}

        -   #### createForPathRelativeToProjectRoot

            ``` methodSignature
            public UnconfiguredBuildTarget createForPathRelativeToProjectRoot​(ForwardRelativePath pathRelativeToProjectRoot,
                                                                              String buildTargetName,
                                                                              CellNameResolver cellNameResolver)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `createForPathRelativeToProjectRoot` in
                interface `UnconfiguredBuildTargetViewFactory`

        []{#createWithWildcard(java.lang.String,com.facebook.buck.core.cell.nameresolver.CellNameResolver)}

        -   #### createWithWildcard

            ``` methodSignature
            public UnconfiguredBuildTarget createWithWildcard​(String buildTargetName,
                                                              CellNameResolver cellNameResolver)
            ```

            ::: block
            [Description copied from
            interface: `UnconfiguredBuildTargetViewFactory`]{.descfrmTypeLabel}
            :::

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

            [Specified by:]{.overrideSpecifyLabel}
            :   `createWithWildcard` in
                interface `UnconfiguredBuildTargetViewFactory`
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
