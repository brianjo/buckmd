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
-   [Enum Constants](#enum.constant.summary) \| 
-   Field \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Enum Constants](#enum.constant.detail) \| 
-   Field \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.test.result.type](package-summary.html)
:::

## Enum ResultType {#enum-resulttype .title title="Enum ResultType"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [java.lang.Enum](http://docs.oracle.com/javase/7/docs/api/java/lang/Enum.html?is-external=true "class or interface in java.lang"){.externalLink}\<[ResultType](ResultType.html "enum in com.facebook.buck.test.result.type")\>

    -   -   com.facebook.buck.test.result.type.ResultType

::: description
-   

    All Implemented Interfaces:
    :   `Serializable`, `Comparable<ResultType>`

    ------------------------------------------------------------------------

        public enum ResultType
        extends Enum<ResultType>

    ::: block
    The kind of result
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#enum.constant.summary}

        ### Enum Constant Summary

        +-----------------------------------+-----------------------------------+
        | Enum Constant                     | Description                       |
        +===================================+===================================+
        | `ASSUMPTION_VIOLATION`            | ::: block                         |
        |                                   | The test was attempted but did    |
        |                                   | not run to completion.            |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+
        | `DISABLED`                        | ::: block                         |
        |                                   | The test was not run because it   |
        |                                   | was excluded in source code, such |
        |                                   | as with JUnit\'s                  |
        |                                   | [`Ignore`](https:                 |
        |                                   | //junit-team.github.io/junit/java |
        |                                   | doc/latest/org/junit/Ignore.html? |
        |                                   | is-external=true "class or interf |
        |                                   | ace in org.junit"){.externalLink} |
        |                                   | annotation or TestNG\'s           |
        |                                   | `Test.enabled()` field.           |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+
        | `DRY_RUN`                         | ::: block                         |
        |                                   | The test was not run because the  |
        |                                   | user chose to run tests with the  |
        |                                   | \--dry-run flag, which caused the |
        |                                   | test runner to print out the      |
        |                                   | names of tests that \*would\*     |
        |                                   | have run without actually running |
        |                                   | them.                             |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+
        | `EXCLUDED`                        | ::: block                         |
        |                                   | The test was not run because it   |
        |                                   | was excluded by the user (e.g.,   |
        |                                   | specifying                        |
        |                                   | [`TestSelectorOptions`](../../.   |
        |                                   | ./cli/TestSelectorOptions.html "c |
        |                                   | lass in com.facebook.buck.cli")). |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+
        | `FAILURE`                         | ::: block                         |
        |                                   | The test ran, but it failed with  |
        |                                   | either an assertion error or an   |
        |                                   | unexpected uncaught exception.    |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+
        | `SUCCESS`                         | ::: block                         |
        |                                   | The test ran successfully.        |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+

        : Enum Constants[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static ResultType`   | `                     | ::: block             |
        |                       | valueOf​(String name)` | Returns the enum      |
        |                       |                       | constant of this type |
        |                       |                       | with the specified    |
        |                       |                       | name.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static ResultType[]` | `values()`            | ::: block             |
        |                       |                       | Returns an array      |
        |                       |                       | containing the        |
        |                       |                       | constants of this     |
        |                       |                       | enum type, in the     |
        |                       |                       | order they are        |
        |                       |                       | declared.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Enum}

            ### Methods inherited from class java.lang.[Enum](http://docs.oracle.com/javase/7/docs/api/java/lang/Enum.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, compareTo, equals, finalize, getDeclaringClass, hashCode, name, ordinal, toString, valueOf`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `getClass, notify, notifyAll, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#enum.constant.detail}

        ### Enum Constant Detail

        []{#DRY_RUN}

        -   #### DRY_RUN

                public static final ResultType DRY_RUN

            ::: block
            The test was not run because the user chose to run tests
            with the \--dry-run flag, which caused the test runner to
            print out the names of tests that \*would\* have run without
            actually running them.
            :::

        []{#EXCLUDED}

        -   #### EXCLUDED

                public static final ResultType EXCLUDED

            ::: block
            The test was not run because it was excluded by the user
            (e.g., specifying
            [`TestSelectorOptions`](../../../cli/TestSelectorOptions.html "class in com.facebook.buck.cli")).
            :::

        []{#DISABLED}

        -   #### DISABLED

                public static final ResultType DISABLED

            ::: block
            The test was not run because it was excluded in source code,
            such as with JUnit\'s
            [`Ignore`](https://junit-team.github.io/junit/javadoc/latest/org/junit/Ignore.html?is-external=true "class or interface in org.junit"){.externalLink}
            annotation or TestNG\'s `Test.enabled()` field.
            :::

        []{#ASSUMPTION_VIOLATION}

        -   #### ASSUMPTION_VIOLATION

                public static final ResultType ASSUMPTION_VIOLATION

            ::: block
            The test was attempted but did not run to completion. It was
            aborted because a precondition/assumption of the test
            failed, see
            [`Assume`](https://junit-team.github.io/junit/javadoc/latest/org/junit/Assume.html?is-external=true "class or interface in org.junit"){.externalLink}.
            :::

        []{#FAILURE}

        -   #### FAILURE

                public static final ResultType FAILURE

            ::: block
            The test ran, but it failed with either an assertion error
            or an unexpected uncaught exception. Note that JUnit3
            distinguishes between these outcomes (FAILURE and ERROR),
            while JUnit4 does not.
            :::

        []{#SUCCESS}

        -   #### SUCCESS

                public static final ResultType SUCCESS

            ::: block
            The test ran successfully.
            :::
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#values()}

        -   #### values

            ``` methodSignature
            public static ResultType[] values()
            ```

            ::: block
            Returns an array containing the constants of this enum type,
            in the order they are declared. This method may be used to
            iterate over the constants as follows:
                for (ResultType c : ResultType.values())
                    System.out.println(c);
            :::

            [Returns:]{.returnLabel}
            :   an array containing the constants of this enum type, in
                the order they are declared

        []{#valueOf(java.lang.String)}

        -   #### valueOf

            ``` methodSignature
            public static ResultType valueOf​(String name)
            ```

            ::: block
            Returns the enum constant of this type with the specified
            name. The string must match *exactly* an identifier used to
            declare an enum constant in this type. (Extraneous
            whitespace characters are not permitted.)
            :::

            [Parameters:]{.paramLabel}
            :   `name` - the name of the enum constant to be returned.

            [Returns:]{.returnLabel}
            :   the enum constant with the specified name

            [Throws:]{.throwsLabel}
            :   `IllegalArgumentException` - if this enum type has no
                constant with the specified name
            :   `NullPointerException` - if the argument is null
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
-   [Enum Constants](#enum.constant.summary) \| 
-   Field \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Enum Constants](#enum.constant.detail) \| 
-   Field \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
