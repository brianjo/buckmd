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
[Package]{.packageLabelInType} [com.facebook.buck.rules.coercer](package-summary.html)
:::

## Class NeededCoverageSpec {#class-neededcoveragespec .title title="Class NeededCoverageSpec"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.rules.coercer.NeededCoverageSpec

::: description
-   

    All Implemented Interfaces:
    :   `TargetTranslatable<NeededCoverageSpec>`

    ------------------------------------------------------------------------

        public abstract class NeededCoverageSpec
        extends Object
        implements TargetTranslatable<NeededCoverageSpec>
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor              Description
          ------------------------ -------------
          `NeededCoverageSpec()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `                     | `getBuildTarget()`    |                       |
        | abstract BuildTarget` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract int`        | `getNeededCover       | ::: block             |
        |                       | ageRatioPercentage()` | Gets the coverage     |
        |                       |                       | ratio that is         |
        |                       |                       | required for a test   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `abstr                | `getPathName()`       |                       |
        | act Optional<String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `stati                | `of​(int nee           |                       |
        | c NeededCoverageSpec` | dedCoverageRatioPerce |                       |
        |                       | ntage,   BuildTarget  |                       |
        |                       | buildTarget,   Option |                       |
        |                       | al<String> pathName)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional             | `translateTargets     |                       |
        | <NeededCoverageSpec>` | ​(CellNameResolver cel |                       |
        |                       | lPathResolver,        |                       |
        |                       |           BaseName ta |                       |
        |                       | rgetBaseName,         |                       |
        |                       |          TargetNodeTr |                       |
        |                       | anslator translator)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `NeededCoverageSpec`  | `withBuildTarget      |                       |
        |                       | ​(BuildTarget target)` |                       |
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
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### NeededCoverageSpec

                public NeededCoverageSpec()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getNeededCoverageRatioPercentage()}

        -   #### getNeededCoverageRatioPercentage

            ``` methodSignature
            public abstract int getNeededCoverageRatioPercentage()
            ```

            ::: block
            Gets the coverage ratio that is required for a test
            :::

            [Returns:]{.returnLabel}
            :   The coverage ratio required for the build target,
                represented in a percentage integer (e.g., return value
                42 means 42% coverage ratio)

        []{#getBuildTarget()}

        -   #### getBuildTarget

            ``` methodSignature
            public abstract BuildTarget getBuildTarget()
            ```

        []{#getPathName()}

        -   #### getPathName

            ``` methodSignature
            public abstract Optional<String> getPathName()
            ```

        []{#of(int,com.facebook.buck.core.model.BuildTarget,java.util.Optional)}

        -   #### of

            ``` methodSignature
            public static NeededCoverageSpec of​(int neededCoverageRatioPercentage,
                                                BuildTarget buildTarget,
                                                Optional<String> pathName)
            ```

        []{#translateTargets(com.facebook.buck.core.cell.nameresolver.CellNameResolver,com.facebook.buck.core.model.BaseName,com.facebook.buck.versions.TargetNodeTranslator)}

        -   #### translateTargets

            ``` methodSignature
            public Optional<NeededCoverageSpec> translateTargets​(CellNameResolver cellPathResolver,
                                                                 BaseName targetBaseName,
                                                                 TargetNodeTranslator translator)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `translateTargets` in
                interface `TargetTranslatable<NeededCoverageSpec>`

            [Returns:]{.returnLabel}
            :   if any changes are required, return the translated
                object.

        []{#withBuildTarget(com.facebook.buck.core.model.BuildTarget)}

        -   #### withBuildTarget

            ``` methodSignature
            public NeededCoverageSpec withBuildTarget​(BuildTarget target)
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
