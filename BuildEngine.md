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
[Package]{.packageLabelInType} [com.facebook.buck.core.build.engine](package-summary.html)
:::

## Interface BuildEngine {#interface-buildengine .title title="Interface BuildEngine"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `CachingBuildEngine`

    ------------------------------------------------------------------------

        public interface BuildEngine

    ::: block
    A build engine is responsible for building a given build rule, which
    includes all its transitive dependencies.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type   Interface                         Description
          ------------------- --------------------------------- -------------
          `static class `     `BuildEngine.BuildEngineResult`    

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `BuildEngi            | `                     | ::: block             |
        | ne.BuildEngineResult` | build​(BuildEngineBuil | Build the given build |
        |                       | dContext buildContext | rule and return a     |
        |                       | ,      ExecutionConte | future to the build   |
        |                       | xt executionContext,  | rule success.         |
        |                       |      BuildRule rule)` | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `BuildResult`         | `ge                   | ::: block             |
        |                       | tBuildRuleResult​(Buil | Returns the build     |
        |                       | dTarget buildTarget)` | result of the build   |
        |                       |                       | rule associated with  |
        |                       |                       | the given build       |
        |                       |                       | target.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `get                  | ::: block             |
        |                       | NumRulesToBuild​(Itera | Calculate the total   |
        |                       | ble<BuildRule> rule)` | number of transitive  |
        |                       |                       | build rules processed |
        |                       |                       | from the given roots. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isRuleBuilt​(Buil     | ::: block             |
        |                       | dTarget buildTarget)` | Returns whether the   |
        |                       |                       | build rule associated |
        |                       |                       | with the build target |
        |                       |                       | has been successfully |
        |                       |                       | built.                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `ter                  | ::: block             |
        |                       | minateBuildWithFailur | Marks build as failed |
        |                       | e​(Throwable failure)` | with the given        |
        |                       |                       | Throwable.            |
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

        []{#getNumRulesToBuild(java.lang.Iterable)}

        -   #### getNumRulesToBuild

            ``` methodSignature
            int getNumRulesToBuild​(Iterable<BuildRule> rule)
            ```

            ::: block
            Calculate the total number of transitive build rules
            processed from the given roots.
            :::

        []{#build(com.facebook.buck.core.build.engine.BuildEngineBuildContext,com.facebook.buck.core.build.execution.context.ExecutionContext,com.facebook.buck.core.rules.BuildRule)}

        -   #### build

            ``` methodSignature
            BuildEngine.BuildEngineResult build​(BuildEngineBuildContext buildContext,
                                                ExecutionContext executionContext,
                                                BuildRule rule)
            ```

            ::: block
            Build the given build rule and return a future to the build
            rule success.
            :::

        []{#getBuildRuleResult(com.facebook.buck.core.model.BuildTarget)}

        -   #### getBuildRuleResult

            ``` methodSignature
            @Nullable
            BuildResult getBuildRuleResult​(BuildTarget buildTarget)
                                    throws ExecutionException,
                                           InterruptedException
            ```

            ::: block
            Returns the build result of the build rule associated with
            the given build target. Returns `null` if the build rule has
            not yet been built.
            :::

            [Throws:]{.throwsLabel}
            :   `ExecutionException`
            :   `InterruptedException`

        []{#isRuleBuilt(com.facebook.buck.core.model.BuildTarget)}

        -   #### isRuleBuilt

            ``` methodSignature
            boolean isRuleBuilt​(BuildTarget buildTarget)
                         throws InterruptedException
            ```

            ::: block
            Returns whether the build rule associated with the build
            target has been successfully built.
            :::

            [Throws:]{.throwsLabel}
            :   `InterruptedException`

        []{#terminateBuildWithFailure(java.lang.Throwable)}

        -   #### terminateBuildWithFailure

            ``` methodSignature
            void terminateBuildWithFailure​(Throwable failure)
            ```

            ::: block
            Marks build as failed with the given Throwable. If keepGoing
            == false, any pending steps will be terminated before
            starting.
            :::

            [Parameters:]{.paramLabel}
            :   `failure` -
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
