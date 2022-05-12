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
-   [Field](#field.summary) \| 
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.core.select](package-summary.html)
:::

## Class AbstractSelectorListResolver {#class-abstractselectorlistresolver .title title="Class AbstractSelectorListResolver"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.select.AbstractSelectorListResolver

::: description
-   

    All Implemented Interfaces:
    :   `SelectorListResolver`

    ```{=html}
    <!-- -->
    ```

    Direct Known Subclasses:
    :   `DefaultSelectorListResolver`,
        `UnconfiguredSelectorListResolver`

    ------------------------------------------------------------------------

        public abstract class AbstractSelectorListResolver
        extends Object
        implements SelectorListResolver

    ::: block
    Provides base functionality for selector list resolvers.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type           Field          Description
          --------------------------- -------------- -------------
          `protected static Object`   `NULL_VALUE`    

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Modifier       Constructor                                                             Description
          -------------- ----------------------------------------------------------------------- -------------
          `protected `   `AbstractSelectorListResolver​(SelectableResolver selectableResolver)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `p                    | `assertNotMu          | ::: block             |
        | rotected static void` | ltipleMatches​(Map<Sel | Assertion that        |
        |                       | ectable,​?> matchingCo | ensures that the      |
        |                       | nditions,             | current configuration |
        |                       |              String a | doesn\'t match        |
        |                       | ttributeName,         | multiple select       |
        |                       |                  Buil | dictionary keys       |
        |                       | dTarget buildTarget)` | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `p                    | `assertSele           | ::: block             |
        | rotected static void` | ctorHasDefault​(BuildT | Assertion for the     |
        |                       | arget buildTarget,    | selector to contain   |
        |                       |                       | \"DEFAULT\" as key    |
        |                       |  DependencyStack depe | inside the            |
        |                       | ndencyStack,          | dictionary.           |
        |                       |                 Strin | :::                   |
        |                       | g attributeName,      |                       |
        |                       |                     S |                       |
        |                       | elector<?> selector)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected <T> Ma     | `findMat              | ::: block             |
        | p<Selectable,​Object>` | chingConditions​(Selec | Returns the value for |
        |                       | tableConfigurationCon | which the current     |
        |                       | text configurationCon | configuration matches |
        |                       | text,                 | the key inside the    |
        |                       |        Selector<T> se | select dictionary     |
        |                       | lector,               | :::                   |
        |                       |          DependencySt |                       |
        |                       | ack dependencyStack)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `<T> T`               | `reso                 | ::: block             |
        |                       | lveList​(SelectableCon | Resolves the elements |
        |                       | figurationContext con | in a given            |
        |                       | figurationContext,    | [`SelectorLis         |
        |                       |          BuildTarget  | t`](SelectorList.html |
        |                       | buildTarget,          |  "class in com.facebo |
        |                       |    String attributeNa | ok.buck.core.select") |
        |                       | me,            Select | and returns the       |
        |                       | orList<T> selectorLis | concatenated value.   |
        |                       | t,            Concata | :::                   |
        |                       | ble<T> concatable,    |                       |
        |                       |          DependencySt |                       |
        |                       | ack dependencyStack)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `prot                 | `                     |                       |
        | ected abstract <T> T` | resolveSelector​(Selec |                       |
        |                       | tableConfigurationCon |                       |
        |                       | text configurationCon |                       |
        |                       | text,                 |                       |
        |                       | BuildTarget buildTarg |                       |
        |                       | et,                De |                       |
        |                       | pendencyStack depende |                       |
        |                       | ncyStack,             |                       |
        |                       |     String attributeN |                       |
        |                       | ame,                S |                       |
        |                       | elector<T> selector)` |                       |
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
    -   []{#field.detail}

        ### Field Detail

        []{#NULL_VALUE}

        -   #### NULL_VALUE

                protected static final Object NULL_VALUE
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.core.select.SelectableResolver)}

        -   #### AbstractSelectorListResolver

                protected AbstractSelectorListResolver​(SelectableResolver selectableResolver)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#resolveList(com.facebook.buck.core.select.SelectableConfigurationContext,com.facebook.buck.core.model.BuildTarget,java.lang.String,com.facebook.buck.core.select.SelectorList,com.facebook.buck.rules.coercer.concat.Concatable,com.facebook.buck.core.exceptions.DependencyStack)}

        -   #### resolveList

            ``` methodSignature
            @Nullable
            public <T> T resolveList​(SelectableConfigurationContext configurationContext,
                                     BuildTarget buildTarget,
                                     String attributeName,
                                     SelectorList<T> selectorList,
                                     Concatable<T> concatable,
                                     DependencyStack dependencyStack)
            ```

            ::: block
            [Description copied from
            interface: `SelectorListResolver`]{.descfrmTypeLabel}
            :::

            ::: block
            Resolves the elements in a given
            [`SelectorList`](SelectorList.html "class in com.facebook.buck.core.select")
            and returns the concatenated value.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `resolveList` in interface `SelectorListResolver`

            [Type Parameters:]{.paramLabel}
            :   `T` - the type of elements stored in the provided
                selectable list
            :   `buildTarget` - the build target that contains the given
                list in its arguments
            :   `attributeName` - the name of the attribute that holds
                the given selector list
            :   `selectorList` - a list with selectable elements
            :   `concatable` - to be used when concatenating select
                items (e. g. lists or strings)
            :   `dependencyStack` - used to provide error stacks

            [Returns:]{.returnLabel}
            :   an object produced by concatenating resolved elements of
                the given list or `null` if the list is resolved to an
                absent element

        []{#resolveSelector(com.facebook.buck.core.select.SelectableConfigurationContext,com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.exceptions.DependencyStack,java.lang.String,com.facebook.buck.core.select.Selector)}

        -   #### resolveSelector

            ``` methodSignature
            @Nullable
            protected abstract <T> T resolveSelector​(SelectableConfigurationContext configurationContext,
                                                     BuildTarget buildTarget,
                                                     DependencyStack dependencyStack,
                                                     String attributeName,
                                                     Selector<T> selector)
            ```

        []{#findMatchingConditions(com.facebook.buck.core.select.SelectableConfigurationContext,com.facebook.buck.core.select.Selector,com.facebook.buck.core.exceptions.DependencyStack)}

        -   #### findMatchingConditions

            ``` methodSignature
            protected <T> Map<Selectable,​Object> findMatchingConditions​(SelectableConfigurationContext configurationContext,
                                                                              Selector<T> selector,
                                                                              DependencyStack dependencyStack)
            ```

            ::: block
            Returns the value for which the current configuration
            matches the key inside the select dictionary
            :::

        []{#assertNotMultipleMatches(java.util.Map,java.lang.String,com.facebook.buck.core.model.BuildTarget)}

        -   #### assertNotMultipleMatches

            ``` methodSignature
            protected static void assertNotMultipleMatches​(Map<Selectable,​?> matchingConditions,
                                                           String attributeName,
                                                           BuildTarget buildTarget)
            ```

            ::: block
            Assertion that ensures that the current configuration
            doesn\'t match multiple select dictionary keys
            :::

        []{#assertSelectorHasDefault(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.exceptions.DependencyStack,java.lang.String,com.facebook.buck.core.select.Selector)}

        -   #### assertSelectorHasDefault

            ``` methodSignature
            protected static void assertSelectorHasDefault​(BuildTarget buildTarget,
                                                           DependencyStack dependencyStack,
                                                           String attributeName,
                                                           Selector<?> selector)
            ```

            ::: block
            Assertion for the selector to contain \"DEFAULT\" as key
            inside the dictionary.
            :::
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
-   [Field](#field.summary) \| 
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
-   [Constr](#constructor.detail) \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
