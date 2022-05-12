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
[Package]{.packageLabelInType} [com.facebook.buck.test.selectors](package-summary.html)
:::

## Interface TestSelector {#interface-testselector .title title="Interface TestSelector"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `PatternTestSelector`, `SimpleTestSelector`

    ------------------------------------------------------------------------

        public interface TestSelector

    ::: block
    A way of matching a test-method in a test-class, and saying whether
    or not to include any matches in a test run.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `boolean`             | `containsClassPa      |                       |
        |                       | th​(String classPath)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getExplanation()`    |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getRawSelector()`    |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isInclusive()`       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isMatchAnyClass()`   |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isMatchAnyMethod()`  |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `matches​(TestDesc     | ::: block             |
        |                       | ription description)` | Whether this          |
        |                       |                       | [`TestSelector`](Tes  |
        |                       |                       | tSelector.html "inter |
        |                       |                       | face in com.facebook. |
        |                       |                       | buck.test.selectors") |
        |                       |                       | matches the given     |
        |                       |                       | [`                    |
        |                       |                       | TestDescription`](Tes |
        |                       |                       | tDescription.html "cl |
        |                       |                       | ass in com.facebook.b |
        |                       |                       | uck.test.selectors"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `matchesClassNa       |                       |
        |                       | me​(String className)` |                       |
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

        []{#getRawSelector()}

        -   #### getRawSelector

            ``` methodSignature
            String getRawSelector()
            ```

        []{#getExplanation()}

        -   #### getExplanation

            ``` methodSignature
            String getExplanation()
            ```

        []{#isInclusive()}

        -   #### isInclusive

            ``` methodSignature
            boolean isInclusive()
            ```

        []{#isMatchAnyClass()}

        -   #### isMatchAnyClass

            ``` methodSignature
            boolean isMatchAnyClass()
            ```

        []{#isMatchAnyMethod()}

        -   #### isMatchAnyMethod

            ``` methodSignature
            boolean isMatchAnyMethod()
            ```

        []{#matches(com.facebook.buck.test.selectors.TestDescription)}

        -   #### matches

            ``` methodSignature
            boolean matches​(TestDescription description)
            ```

            ::: block
            Whether this
            [`TestSelector`](TestSelector.html "interface in com.facebook.buck.test.selectors")
            matches the given
            [`TestDescription`](TestDescription.html "class in com.facebook.buck.test.selectors").
            A class or method name being null in the
            [`TestDescription`](TestDescription.html "class in com.facebook.buck.test.selectors")
            means that it will match anything.
            :::

            [Parameters:]{.paramLabel}
            :   `description` - the
                [`TestDescription`](TestDescription.html "class in com.facebook.buck.test.selectors")
                to match

            [Returns:]{.returnLabel}
            :   true if this selector matches the given
                [`TestDescription`](TestDescription.html "class in com.facebook.buck.test.selectors")

        []{#matchesClassName(java.lang.String)}

        -   #### matchesClassName

            ``` methodSignature
            boolean matchesClassName​(String className)
            ```

            [Returns:]{.returnLabel}
            :   true if the given className matches this selector

        []{#containsClassPath(java.lang.String)}

        -   #### containsClassPath

            ``` methodSignature
            boolean containsClassPath​(String classPath)
            ```

            [Returns:]{.returnLabel}
            :   true if the given classpath may be required by any
                classes that matches this selector
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
