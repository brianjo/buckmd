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

## Class PatternTestSelector {#class-patterntestselector .title title="Class PatternTestSelector"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.test.selectors.PatternTestSelector

::: description
-   

    All Implemented Interfaces:
    :   `TestSelector`

    ------------------------------------------------------------------------

        public class PatternTestSelector
        extends Object
        implements TestSelector

    ::: block
    A
    [`TestDescription`](TestDescription.html "class in com.facebook.buck.test.selectors")
    will match if this selector\'s class-part is a substring of the
    [`TestDescription`](TestDescription.html "class in com.facebook.buck.test.selectors")\'s
    full class-name, or if this selector\'s class-name, when interpreted
    as a java.util.regex regular-expression, matches the
    [`TestDescription`](TestDescription.html "class in com.facebook.buck.test.selectors")\'s
    full class-name.
    (The same rules apply for the method-name as well. If this
    selector\'s class-part or method-part are null, all class-names or
    method-names will match.)
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static TestSelector` | `buildFro             | ::: block             |
        |                       | mSelectorString​(Strin | Build a               |
        |                       | g rawSelectorString)` | [`Pattern             |
        |                       |                       | TestSelector`](Patter |
        |                       |                       | nTestSelector.html "c |
        |                       |                       | lass in com.facebook. |
        |                       |                       | buck.test.selectors") |
        |                       |                       | from the given        |
        |                       |                       | String.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
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

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
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
    -   []{#method.detail}

        ### Method Detail

        []{#buildFromSelectorString(java.lang.String)}

        -   #### buildFromSelectorString

            ``` methodSignature
            public static TestSelector buildFromSelectorString​(String rawSelectorString)
            ```

            ::: block
            Build a
            [`PatternTestSelector`](PatternTestSelector.html "class in com.facebook.buck.test.selectors")
            from the given String. Selector strings should be of the
            form \"\[is-exclusive\]\[class-part\]#\[method-part\]\". If
            \"\[is-exclusive\]\" is a \"!\" then this selector will
            exclude tests, otherwise it will include tests.
            If the class-part (or method-part) are omitted, then all
            classes or methods will match. Consequently \"#\" means
            \"include everything\" and \"!#\" means \"exclude
            everything\".

            If the selector string doesn\'t contain a \"#\" at all, it
            is interpreted as a class-part.
            :::

            [Parameters:]{.paramLabel}
            :   `rawSelectorString` - An unparsed selector string.

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
            public boolean matchesClassName​(String className)
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
