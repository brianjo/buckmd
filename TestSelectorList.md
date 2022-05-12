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
-   [Nested](#nested.class.summary) \| 
-   [Field](#field.summary) \| 
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
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

## Class TestSelectorList {#class-testselectorlist .title title="Class TestSelectorList"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.test.selectors.TestSelectorList

::: description
-   

    ------------------------------------------------------------------------

        public class TestSelectorList
        extends Object

    ::: block
    A collection of
    [`PatternTestSelector`](PatternTestSelector.html "class in com.facebook.buck.test.selectors")
    instances which, as a group, can decide whether or not to include a
    given
    [`TestDescription`](TestDescription.html "class in com.facebook.buck.test.selectors").
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static class `       | `Test                 | ::: block             |
        |                       | SelectorList.Builder` | Build a new           |
        |                       |                       | [`T                   |
        |                       |                       | estSelectorList`](Tes |
        |                       |                       | tSelectorList.html "c |
        |                       |                       | lass in com.facebook. |
        |                       |                       | buck.test.selectors") |
        |                       |                       | from a list of        |
        |                       |                       | strings, each of      |
        |                       |                       | which is parsed by    |
        |                       |                       | [`PatternT            |
        |                       |                       | estSelector`](Pattern |
        |                       |                       | TestSelector.html "cl |
        |                       |                       | ass in com.facebook.b |
        |                       |                       | uck.test.selectors"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type           Field     Description
          --------------------------- --------- -------------
          `static TestSelectorList`   `EMPTY`    

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static Test          | `builder()`           |                       |
        | SelectorList.Builder` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `sta                  | `empty()`             |                       |
        | tic TestSelectorList` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `TestSelector`        | `                     |                       |
        |                       | findSelector​(TestDesc |                       |
        |                       | ription description)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `List<String>`        | `getExplanation()`    |                       |
        +-----------------------+-----------------------+-----------------------+
        | `List<String>`        | `getRawSelectors()`   |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isEmpty()`           |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isIncluded​(TestDesc  |                       |
        |                       | ription description)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `po                   | ::: block             |
        |                       | ssiblyIncludesClassNa | Returns true if it is |
        |                       | me​(String className)` | \*possible\* for the  |
        |                       |                       | given classname to    |
        |                       |                       | include tests.        |
        |                       |                       | :::                   |
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
    -   []{#field.detail}

        ### Field Detail

        []{#EMPTY}

        -   #### EMPTY

                public static final TestSelectorList EMPTY
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#findSelector(com.facebook.buck.test.selectors.TestDescription)}

        -   #### findSelector

            ``` methodSignature
            public TestSelector findSelector​(TestDescription description)
            ```

        []{#isIncluded(com.facebook.buck.test.selectors.TestDescription)}

        -   #### isIncluded

            ``` methodSignature
            public boolean isIncluded​(TestDescription description)
            ```

        []{#possiblyIncludesClassName(java.lang.String)}

        -   #### possiblyIncludesClassName

            ``` methodSignature
            public boolean possiblyIncludesClassName​(String className)
            ```

            ::: block
            Returns true if it is \*possible\* for the given classname
            to include tests.
            Before we go through the hassle of loading a class, confirm
            that it\'s possible for it to run tests.
            :::

        []{#getExplanation()}

        -   #### getExplanation

            ``` methodSignature
            public List<String> getExplanation()
            ```

        []{#getRawSelectors()}

        -   #### getRawSelectors

            ``` methodSignature
            public List<String> getRawSelectors()
            ```

        []{#isEmpty()}

        -   #### isEmpty

            ``` methodSignature
            public boolean isEmpty()
            ```

        []{#empty()}

        -   #### empty

            ``` methodSignature
            public static TestSelectorList empty()
            ```

        []{#builder()}

        -   #### builder

            ``` methodSignature
            public static TestSelectorList.Builder builder()
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
-   [Nested](#nested.class.summary) \| 
-   [Field](#field.summary) \| 
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
-   Constr \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
