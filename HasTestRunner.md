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
[Package]{.packageLabelInType} [com.facebook.buck.core.test.rule](package-summary.html)
:::

## Interface HasTestRunner {#interface-hastestrunner .title title="Interface HasTestRunner"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `AppleTestDescriptionArg`, `GoTestDescriptionArg`,
        `JavaTestDescriptionArg`, `PythonTestDescriptionArg`,
        `RobolectricTestDescriptionArg`

    ------------------------------------------------------------------------

        public interface HasTestRunner

    ::: block
    This marks a Description Arg for a test rule as having a test runner
    that knows how to run the test. The test runner is declared as a
    library.
    TODO(bobyf): need a slightly better api or a new rule as a library
    doesn\'t quite make sense.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type            Method          Description
          ---------------------------- --------------- -------------
          `Optional<BuildTarget>`      `getRunner()`    
          `Optional<TestRunnerSpec>`   `getSpecs()`     

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

        []{#getRunner()}

        -   #### getRunner

            ``` methodSignature
            Optional<BuildTarget> getRunner()
            ```

            [Returns:]{.returnLabel}
            :   the target to the library containing the test runner

        []{#getSpecs()}

        -   #### getSpecs

            ``` methodSignature
            Optional<TestRunnerSpec> getSpecs()
            ```

            [Returns:]{.returnLabel}
            :   the freeform (for now) specs as required for running
                tests. For example, cmds, contacts, etc. This is
                serialized as json for for the external test runner.
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
