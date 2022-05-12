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
[Package]{.packageLabelInType} [com.facebook.buck.parser.detector](package-summary.html)
:::

## Class TargetConfigurationDetectorFactory {#class-targetconfigurationdetectorfactory .title title="Class TargetConfigurationDetectorFactory"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.parser.detector.TargetConfigurationDetectorFactory

::: description
-   

    ------------------------------------------------------------------------

        public class TargetConfigurationDetectorFactory
        extends Object

    ::: block
    Utility to create
    [`TargetConfigurationDetector`](TargetConfigurationDetector.html "class in com.facebook.buck.parser.detector")
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static TargetC       | `empty()`             | ::: block             |
        | onfigurationDetector` |                       | Target configuration  |
        |                       |                       | that detects to none  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static TargetC       | `fromBuckConfig​(      | ::: block             |
        | onfigurationDetector` | ParserConfig parserCo | Configure detector    |
        |                       | nfig,               U | using provided        |
        |                       | nconfiguredBuildTarge | `.buckconfig`         |
        |                       | tViewFactory unconfig | :::                   |
        |                       | uredBuildTargetViewFa |                       |
        |                       | ctory,                |                       |
        |                       | CellPathResolver cell |                       |
        |                       | PathResolver,         |                       |
        |                       |        CellNameResolv |                       |
        |                       | er cellNameResolver)` |                       |
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
    -   []{#method.detail}

        ### Method Detail

        []{#fromBuckConfig(com.facebook.buck.parser.config.ParserConfig,com.facebook.buck.core.parser.buildtargetparser.UnconfiguredBuildTargetViewFactory,com.facebook.buck.core.cell.CellPathResolver,com.facebook.buck.core.cell.nameresolver.CellNameResolver)}

        -   #### fromBuckConfig

            ``` methodSignature
            public static TargetConfigurationDetector fromBuckConfig​(ParserConfig parserConfig,
                                                                     UnconfiguredBuildTargetViewFactory unconfiguredBuildTargetViewFactory,
                                                                     CellPathResolver cellPathResolver,
                                                                     CellNameResolver cellNameResolver)
            ```

            ::: block
            Configure detector using provided `.buckconfig`
            :::

        []{#empty()}

        -   #### empty

            ``` methodSignature
            public static TargetConfigurationDetector empty()
            ```

            ::: block
            Target configuration that detects to none
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
