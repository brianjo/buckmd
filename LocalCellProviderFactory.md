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
[Package]{.packageLabelInType} [com.facebook.buck.core.cell.impl](package-summary.html)
:::

## Class LocalCellProviderFactory {#class-localcellproviderfactory .title title="Class LocalCellProviderFactory"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.cell.impl.LocalCellProviderFactory

::: description
-   

    ------------------------------------------------------------------------

        public class LocalCellProviderFactory
        extends Object

    ::: block
    Creates a
    [`CellProvider`](../CellProvider.html "class in com.facebook.buck.core.cell")
    to be used in a local (non-distributed) build.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                    Description
          ------------------------------ -------------
          `LocalCellProviderFactory()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static CellProvider` | `creat                | ::: block             |
        |                       | e​(ProjectFilesystem r | Create a cell         |
        |                       | ootFilesystem,        | provider at a given   |
        |                       | BuckConfig rootConfig | root.                 |
        |                       | ,       CellConfig ro | :::                   |
        |                       | otCellConfigOverrides |                       |
        |                       | ,       com.google.co |                       |
        |                       | mmon.collect.Immutabl |                       |
        |                       | eMap<CellName,​AbsPath |                       |
        |                       | > cellPathMapping,    |                       |
        |                       |     CellPathResolver  |                       |
        |                       | rootCellCellPathResol |                       |
        |                       | ver,       BuckModule |                       |
        |                       | Manager moduleManager |                       |
        |                       | ,       ToolchainProv |                       |
        |                       | iderFactory toolchain |                       |
        |                       | ProviderFactory,      |                       |
        |                       |   ProjectFilesystemFa |                       |
        |                       | ctory projectFilesyst |                       |
        |                       | emFactory,       Unco |                       |
        |                       | nfiguredBuildTargetVi |                       |
        |                       | ewFactory unconfigure |                       |
        |                       | dBuildTargetFactory)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
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

        -   #### LocalCellProviderFactory

                public LocalCellProviderFactory()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#create(com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.config.BuckConfig,com.facebook.buck.core.cell.CellConfig,com.google.common.collect.ImmutableMap,com.facebook.buck.core.cell.CellPathResolver,com.facebook.buck.core.module.BuckModuleManager,com.facebook.buck.core.toolchain.ToolchainProviderFactory,com.facebook.buck.io.filesystem.ProjectFilesystemFactory,com.facebook.buck.core.parser.buildtargetparser.UnconfiguredBuildTargetViewFactory)}

        -   #### create

            ``` methodSignature
            public static CellProvider create​(ProjectFilesystem rootFilesystem,
                                              BuckConfig rootConfig,
                                              CellConfig rootCellConfigOverrides,
                                              com.google.common.collect.ImmutableMap<CellName,​AbsPath> cellPathMapping,
                                              CellPathResolver rootCellCellPathResolver,
                                              BuckModuleManager moduleManager,
                                              ToolchainProviderFactory toolchainProviderFactory,
                                              ProjectFilesystemFactory projectFilesystemFactory,
                                              UnconfiguredBuildTargetViewFactory unconfiguredBuildTargetFactory)
            ```

            ::: block
            Create a cell provider at a given root.
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
