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
[Package]{.packageLabelInType} [com.facebook.buck.test.selectors](package-summary.html)
:::

## Class SimpleTestSelector {#class-simpletestselector .title title="Class SimpleTestSelector"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.test.selectors.SimpleTestSelector

::: description
-   

    All Implemented Interfaces:
    :   `TestSelector`

    ------------------------------------------------------------------------

        public class SimpleTestSelector
        extends Object
        implements TestSelector

    ::: block
    A
    [`TestDescription`](TestDescription.html "class in com.facebook.buck.test.selectors")
    will match if this selector\'s class-part is identical to the
    TestDescriptions class name (same for the method name).
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                   Description
          ----------------------------------------------------------------------------- -------------
          `SimpleTestSelector​(String className,                   String methodName)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
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
        | `boolean`             | `matchesClassName​(S   |                       |
        |                       | tring thatClassName)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
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

        []{#<init>(java.lang.String,java.lang.String)}

        -   #### SimpleTestSelector

                public SimpleTestSelector​(String className,
                                          String methodName)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getRawSelector()}

        -   #### getRawSelector

            ``` methodSignature
            public String getRawSelector()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getRawSelector` in interface `TestSelector`

        []{#getExplanation()}

        -   #### getExplanation

            ``` methodSignature
            public String getExplanation()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getExplanation` in interface `TestSelector`

        []{#isInclusive()}

        -   #### isInclusive

            ``` methodSignature
            public boolean isInclusive()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `isInclusive` in interface `TestSelector`

        []{#isMatchAnyClass()}

        -   #### isMatchAnyClass

            ``` methodSignature
            public boolean isMatchAnyClass()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `isMatchAnyClass` in interface `TestSelector`

        []{#isMatchAnyMethod()}

        -   #### isMatchAnyMethod

            ``` methodSignature
            public boolean isMatchAnyMethod()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `isMatchAnyMethod` in interface `TestSelector`

        []{#matches(com.facebook.buck.test.selectors.TestDescription)}

        -   #### matches

            ``` methodSignature
            public boolean matches​(TestDescription description)
            ```

            ::: block
            [Description copied from
            interface: `TestSelector`]{.descfrmTypeLabel}
            :::

            ::: block
            Whether this
            [`TestSelector`](TestSelector.html "interface in com.facebook.buck.test.selectors")
            matches the given
            [`TestDescription`](TestDescription.html "class in com.facebook.buck.test.selectors").
            A class or method name being null in the
            [`TestDescription`](TestDescription.html "class in com.facebook.buck.test.selectors")
            means that it will match anything.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `matches` in interface `TestSelector`

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
            public boolean matchesClassName​(String thatClassName)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `matchesClassName` in interface `TestSelector`

            [Returns:]{.returnLabel}
            :   true if the given className matches this selector

        []{#containsClassPath(java.lang.String)}

        -   #### containsClassPath

            ``` methodSignature
            public boolean containsClassPath​(String classPath)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `containsClassPath` in interface `TestSelector`

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
