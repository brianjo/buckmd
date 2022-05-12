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

## Class TestSelectorList.Builder {#class-testselectorlist.builder .title title="Class TestSelectorList.Builder"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.test.selectors.TestSelectorList.Builder

::: description
-   

    Enclosing class:
    :   [TestSelectorList](TestSelectorList.html "class in com.facebook.buck.test.selectors")

    ------------------------------------------------------------------------

        public static class TestSelectorList.Builder
        extends Object

    ::: block
    Build a new
    [`TestSelectorList`](TestSelectorList.html "class in com.facebook.buck.test.selectors")
    from a list of strings, each of which is parsed by
    [`PatternTestSelector`](PatternTestSelector.html "class in com.facebook.buck.test.selectors").
    If any of the selectors is an inclusive selector, everything else
    will be excluded. Conversely, if all of the selectors are exclusive,
    then everything else will be included by default.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Modifier       Constructor   Description
          -------------- ------------- -------------
          `protected `   `Builder()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type            Method                                                   Description
          ---------------------------- -------------------------------------------------------- -------------
          `TestSelectorList.Builder`   `addBase64EncodedTestSelector​(String b64Selector)`        
          `TestSelectorList.Builder`   `addRawSelectors​(String... rawSelectors)`                 
          `TestSelectorList.Builder`   `addRawSelectors​(Collection<String> rawTestSelectors)`    
          `TestSelectorList.Builder`   `addSimpleTestSelector​(String simpleSelector)`            
          `TestSelectorList`           `build()`                                                 

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

        []{#<init>()}

        -   #### Builder

                protected Builder()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#addRawSelectors(java.lang.String...)}

        -   #### addRawSelectors

            ``` methodSignature
            public TestSelectorList.Builder addRawSelectors​(String... rawSelectors)
            ```

        []{#addRawSelectors(java.util.Collection)}

        -   #### addRawSelectors

            ``` methodSignature
            public TestSelectorList.Builder addRawSelectors​(Collection<String> rawTestSelectors)
            ```

        []{#addSimpleTestSelector(java.lang.String)}

        -   #### addSimpleTestSelector

            ``` methodSignature
            public TestSelectorList.Builder addSimpleTestSelector​(String simpleSelector)
            ```

        []{#addBase64EncodedTestSelector(java.lang.String)}

        -   #### addBase64EncodedTestSelector

            ``` methodSignature
            public TestSelectorList.Builder addBase64EncodedTestSelector​(String b64Selector)
            ```

        []{#build()}

        -   #### build

            ``` methodSignature
            public TestSelectorList build()
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
