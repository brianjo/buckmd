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

## Class RootCellFactory {#class-rootcellfactory .title title="Class RootCellFactory"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.cell.impl.RootCellFactory

::: description
-   

    ------------------------------------------------------------------------

        public class RootCellFactory
        extends Object

    ::: block
    Creates a root cell, i.e. a cell that is representing the current
    repository.
    The root cell is different from other cells: it doesn\'t require a
    path to the repository directory since the root of the provided
    filesystem is considered to be the root of the cell. Its name is
    also empty.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor           Description
          --------------------- -------------
          `RootCellFactory()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         Description
          ------------------- ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ -------------
          `static Cell`       `create​(com.google.common.collect.ImmutableSortedSet<AbsPath> knownRoots,       CellProvider cellProvider,       NewCellPathResolver newCellPathResolver,       CellPathResolver rootCellCellPathResolver,       ProjectFilesystem rootFilesystem,       BuckModuleManager moduleManager,       org.pf4j.PluginManager pluginManager,       BuckConfig rootConfig,       com.google.common.collect.ImmutableMap<String,​String> environment,       ProcessExecutor processExecutor,       ExecutableFinder executableFinder)`    

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

        -   #### RootCellFactory

                public RootCellFactory()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#create(com.google.common.collect.ImmutableSortedSet,com.facebook.buck.core.cell.CellProvider,com.facebook.buck.core.cell.NewCellPathResolver,com.facebook.buck.core.cell.CellPathResolver,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.module.BuckModuleManager,org.pf4j.PluginManager,com.facebook.buck.core.config.BuckConfig,com.google.common.collect.ImmutableMap,com.facebook.buck.util.ProcessExecutor,com.facebook.buck.io.ExecutableFinder)}

        -   #### create

            ``` methodSignature
            public static Cell create​(com.google.common.collect.ImmutableSortedSet<AbsPath> knownRoots,
                                      CellProvider cellProvider,
                                      NewCellPathResolver newCellPathResolver,
                                      CellPathResolver rootCellCellPathResolver,
                                      ProjectFilesystem rootFilesystem,
                                      BuckModuleManager moduleManager,
                                      org.pf4j.PluginManager pluginManager,
                                      BuckConfig rootConfig,
                                      com.google.common.collect.ImmutableMap<String,​String> environment,
                                      ProcessExecutor processExecutor,
                                      ExecutableFinder executableFinder)
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
