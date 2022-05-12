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
[Package]{.packageLabelInType} [com.facebook.buck.test.config](package-summary.html)
:::

## Class TestBuckConfig {#class-testbuckconfig .title title="Class TestBuckConfig"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.test.config.TestBuckConfig

::: description
-   

    All Implemented Interfaces:
    :   `ConfigView<BuckConfig>`

    ------------------------------------------------------------------------

        public abstract class TestBuckConfig
        extends Object
        implements ConfigView<BuckConfig>
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor          Description
          -------------------- -------------
          `TestBuckConfig()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `Optional<com.goo     | `g                    |                       |
        | gle.common.collect.Im | etCoverageExcludes()` |                       |
        | mutableList<String>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<com.goo     | `g                    |                       |
        | gle.common.collect.Im | etCoverageIncludes()` |                       |
        | mutableList<String>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.go               | `getDefaultRawExcl    | ::: block             |
        | ogle.common.collect.I | udedLabelSelectors()` | Return Strings so as  |
        | mmutableList<String>` |                       | to avoid a dependency |
        |                       |                       | on                    |
        |                       |                       | [`LabelSelector`](    |
        |                       |                       | ../../cli/LabelSelect |
        |                       |                       | or.html "class in com |
        |                       |                       | .facebook.buck.cli")! |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Long>`      | `getDefaul            | ::: block             |
        |                       | tTestRuleTimeoutMs()` | The timeout to apply  |
        |                       |                       | to entire test rules. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `long`                | `getDefaul            |                       |
        |                       | tTestTimeoutMillis()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract BuckConfig` | `getDelegate()`       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<com.goo     | `get                  |                       |
        | gle.common.collect.Im | ExternalTestRunner()` |                       |
        | mutableList<String>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `getNumTestThreads()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `TestRe               | `getResu              |                       |
        | sultSummaryVerbosity` | ltSummaryVerbosity()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isBuildingFi         |                       |
        |                       | lteredTestsEnabled()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isInclNoLoca         |                       |
        |                       | tionClassesEnabled()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isPar                |                       |
        |                       | allelExternalTestSpec |                       |
        |                       | ComputationEnabled()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `s                    | `of​(                  |                       |
        | tatic TestBuckConfig` | BuckConfig delegate)` |                       |
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

        -   #### TestBuckConfig

                public TestBuckConfig()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getDelegate()}

        -   #### getDelegate

            ``` methodSignature
            public abstract BuckConfig getDelegate()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getDelegate` in interface `ConfigView<BuckConfig>`

        []{#of(com.facebook.buck.core.config.BuckConfig)}

        -   #### of

            ``` methodSignature
            public static TestBuckConfig of​(BuckConfig delegate)
            ```

        []{#isParallelExternalTestSpecComputationEnabled()}

        -   #### isParallelExternalTestSpecComputationEnabled

            ``` methodSignature
            @Lazy
            public boolean isParallelExternalTestSpecComputationEnabled()
            ```

        []{#getDefaultTestTimeoutMillis()}

        -   #### getDefaultTestTimeoutMillis

            ``` methodSignature
            @Lazy
            public long getDefaultTestTimeoutMillis()
            ```

        []{#getDefaultRawExcludedLabelSelectors()}

        -   #### getDefaultRawExcludedLabelSelectors

            ``` methodSignature
            @Lazy
            public com.google.common.collect.ImmutableList<String> getDefaultRawExcludedLabelSelectors()
            ```

            ::: block
            Return Strings so as to avoid a dependency on
            [`LabelSelector`](../../cli/LabelSelector.html "class in com.facebook.buck.cli")!
            :::

        []{#getNumTestThreads()}

        -   #### getNumTestThreads

            ``` methodSignature
            @Lazy
            public int getNumTestThreads()
            ```

            [Returns:]{.returnLabel}
            :   the number of threads Buck should use for testing. This
                will use the test.threads setting if it exists.
                Otherwise, this will use the build parallelization
                settings if not configured.

        []{#getResultSummaryVerbosity()}

        -   #### getResultSummaryVerbosity

            ``` methodSignature
            public TestResultSummaryVerbosity getResultSummaryVerbosity()
            ```

        []{#getExternalTestRunner()}

        -   #### getExternalTestRunner

            ``` methodSignature
            public Optional<com.google.common.collect.ImmutableList<String>> getExternalTestRunner()
            ```

        []{#getDefaultTestRuleTimeoutMs()}

        -   #### getDefaultTestRuleTimeoutMs

            ``` methodSignature
            public Optional<Long> getDefaultTestRuleTimeoutMs()
            ```

            ::: block
            The timeout to apply to entire test rules.
            :::

        []{#isInclNoLocationClassesEnabled()}

        -   #### isInclNoLocationClassesEnabled

            ``` methodSignature
            public boolean isInclNoLocationClassesEnabled()
            ```

        []{#getCoverageIncludes()}

        -   #### getCoverageIncludes

            ``` methodSignature
            public Optional<com.google.common.collect.ImmutableList<String>> getCoverageIncludes()
            ```

        []{#getCoverageExcludes()}

        -   #### getCoverageExcludes

            ``` methodSignature
            public Optional<com.google.common.collect.ImmutableList<String>> getCoverageExcludes()
            ```

        []{#isBuildingFilteredTestsEnabled()}

        -   #### isBuildingFilteredTestsEnabled

            ``` methodSignature
            public boolean isBuildingFilteredTestsEnabled()
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
