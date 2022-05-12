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

-   [Overview](../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../deprecated-list.html)
-   [Index](../../../../index-all.html)
-   [Help](../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.testrunner](package-summary.html)
:::

## Class BuckBlockJUnit4ClassRunner {#class-buckblockjunit4classrunner .title title="Class BuckBlockJUnit4ClassRunner"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [org.junit.runner.Runner](https://junit-team.github.io/junit/javadoc/latest/org/junit/runner/Runner.html?is-external=true "class or interface in org.junit.runner"){.externalLink}

    -   -   [org.junit.runners.ParentRunner](https://junit-team.github.io/junit/javadoc/latest/org/junit/runners/ParentRunner.html?is-external=true "class or interface in org.junit.runners"){.externalLink}\<[FrameworkMethod](https://junit-team.github.io/junit/javadoc/latest/org/junit/runners/model/FrameworkMethod.html?is-external=true "class or interface in org.junit.runners.model"){.externalLink}\>

        -   -   [org.junit.runners.BlockJUnit4ClassRunner](https://junit-team.github.io/junit/javadoc/latest/org/junit/runners/BlockJUnit4ClassRunner.html?is-external=true "class or interface in org.junit.runners"){.externalLink}

            -   -   com.facebook.buck.testrunner.BuckBlockJUnit4ClassRunner

::: description
-   

    All Implemented Interfaces:
    :   `Describable`, `Filterable`, `Sortable`

    ------------------------------------------------------------------------

        public class BuckBlockJUnit4ClassRunner
        extends BlockJUnit4ClassRunner

    ::: block
    JUnit-4-compatible test class runner that supports the concept of a
    \"default timeout.\" If the value of `defaultTestTimeoutMillis`
    passed to the constructor is non-zero, then it will be used in place
    of
    [`Test.timeout()`](https://junit-team.github.io/junit/javadoc/latest/org/junit/Test.html?is-external=true#timeout() "class or interface in org.junit"){.externalLink}
    if
    [`Test.timeout()`](https://junit-team.github.io/junit/javadoc/latest/org/junit/Test.html?is-external=true#timeout() "class or interface in org.junit"){.externalLink}
    returns zero.
    The superclass,
    [`BlockJUnit4ClassRunner`](https://junit-team.github.io/junit/javadoc/latest/org/junit/runners/BlockJUnit4ClassRunner.html?is-external=true "class or interface in org.junit.runners"){.externalLink},
    was introduced in JUnit 4.5 as a published API that was designed to
    be extended.

    This runner also creates Descriptions that allow JUnitRunner to
    filter which test-methods to run and should be forced into the test
    code path whenever test-selectors are in use.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                             Description
          ------------------------------------------------------------------------------------------------------- -------------
          `BuckBlockJUnit4ClassRunner​(Class<?> klass,                           long defaultTestTimeoutMillis)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `protected void`      | `collectIni           | ::: block             |
        |                       | tializationErrors​(Lis | Override default init |
        |                       | t<Throwable> errors)` | error collector so    |
        |                       |                       | that class without    |
        |                       |                       | any test methods will |
        |                       |                       | pass                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `protected Object`    | `createTest()`        |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected Statement` | `methodBlock​(Fra      | ::: block             |
        |                       | meworkMethod method)` | Override the default  |
        |                       |                       | timeout behavior so   |
        |                       |                       | that when no timeout  |
        |                       |                       | is specified in the   |
        |                       |                       | [`Test`](https://ju   |
        |                       |                       | nit-team.github.io/ju |
        |                       |                       | nit/javadoc/latest/or |
        |                       |                       | g/junit/Test.html?is- |
        |                       |                       | external=true "class  |
        |                       |                       | or interface in org.j |
        |                       |                       | unit"){.externalLink} |
        |                       |                       | annotation, the       |
        |                       |                       | timeout specified by  |
        |                       |                       | the constructor will  |
        |                       |                       | be used (if it has    |
        |                       |                       | been set).            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.org.junit.runners.BlockJUnit4ClassRunner}

            ### Methods inherited from class org.junit.runners.[BlockJUnit4ClassRunner](https://junit-team.github.io/junit/javadoc/latest/org/junit/runners/BlockJUnit4ClassRunner.html?is-external=true "class or interface in org.junit.runners"){.externalLink}

            `computeTestMethods, describeChild, getChildren, getTestRules, isIgnored, methodInvoker, possiblyExpectingExceptions, rules, runChild, testName, validateConstructor, validateFields, validateInstanceMethods, validateNoNonStaticInnerClass, validateOnlyOneConstructor, validateTestMethods, validateZeroArgConstructor, withAfters, withBefores, withPotentialTimeout`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.org.junit.runners.ParentRunner}

            ### Methods inherited from class org.junit.runners.[ParentRunner](https://junit-team.github.io/junit/javadoc/latest/org/junit/runners/ParentRunner.html?is-external=true "class or interface in org.junit.runners"){.externalLink}

            `childrenInvoker, classBlock, classRules, createTestClass, filter, getDescription, getName, getRunnerAnnotations, getTestClass, run, runLeaf, setScheduler, sort, validatePublicVoidNoArgMethods, withAfterClasses, withBeforeClasses`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.org.junit.runner.Runner}

            ### Methods inherited from class org.junit.runner.[Runner](https://junit-team.github.io/junit/javadoc/latest/org/junit/runner/Runner.html?is-external=true "class or interface in org.junit.runner"){.externalLink}

            `testCount`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(java.lang.Class,long)}

        -   #### BuckBlockJUnit4ClassRunner

                public BuckBlockJUnit4ClassRunner​(Class<?> klass,
                                                  long defaultTestTimeoutMillis)
                                           throws InitializationError

            [Throws:]{.throwsLabel}
            :   `InitializationError`
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#createTest()}

        -   #### createTest

            ``` methodSignature
            protected Object createTest()
                                 throws Exception
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `createTest` in class `BlockJUnit4ClassRunner`

            [Throws:]{.throwsLabel}
            :   `Exception`

        []{#methodBlock(org.junit.runners.model.FrameworkMethod)}

        -   #### methodBlock

            ``` methodSignature
            protected Statement methodBlock​(FrameworkMethod method)
            ```

            ::: block
            Override the default timeout behavior so that when no
            timeout is specified in the
            [`Test`](https://junit-team.github.io/junit/javadoc/latest/org/junit/Test.html?is-external=true "class or interface in org.junit"){.externalLink}
            annotation, the timeout specified by the constructor will be
            used (if it has been set).
            :::

            [Overrides:]{.overrideSpecifyLabel}
            :   `methodBlock` in class `BlockJUnit4ClassRunner`

        []{#collectInitializationErrors(java.util.List)}

        -   #### collectInitializationErrors

            ``` methodSignature
            protected void collectInitializationErrors​(List<Throwable> errors)
            ```

            ::: block
            Override default init error collector so that class without
            any test methods will pass
            :::

            [Overrides:]{.overrideSpecifyLabel}
            :   `collectInitializationErrors` in
                class `BlockJUnit4ClassRunner`
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

-   [Overview](../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../deprecated-list.html)
-   [Index](../../../../index-all.html)
-   [Help](../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../allclasses.html)

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
