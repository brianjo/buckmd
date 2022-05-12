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
[Package]{.packageLabelInType} [com.facebook.buck.core.select](package-summary.html)
:::

## Interface SelectorListResolver {#interface-selectorlistresolver .title title="Interface SelectorListResolver"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `AbstractSelectorListResolver`, `DefaultSelectorListResolver`,
        `ThrowingSelectorListResolver`,
        `UnconfiguredSelectorListResolver`

    ------------------------------------------------------------------------

        public interface SelectorListResolver

    ::: block
    A resolver that analyzes
    [`SelectorList`](SelectorList.html "class in com.facebook.buck.core.select"),
    evaluates selectable statements and constructs the final value that
    is produced by concatenating selected values (the type of the
    elements determines the process of concatenation.)
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
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

        []{#resolveList(com.facebook.buck.core.select.SelectableConfigurationContext,com.facebook.buck.core.model.BuildTarget,java.lang.String,com.facebook.buck.core.select.SelectorList,com.facebook.buck.rules.coercer.concat.Concatable,com.facebook.buck.core.exceptions.DependencyStack)}

        -   #### resolveList

            ``` methodSignature
            @Nullable
            <T> T resolveList​(SelectableConfigurationContext configurationContext,
                              BuildTarget buildTarget,
                              String attributeName,
                              SelectorList<T> selectorList,
                              Concatable<T> concatable,
                              DependencyStack dependencyStack)
            ```

            ::: block
            Resolves the elements in a given
            [`SelectorList`](SelectorList.html "class in com.facebook.buck.core.select")
            and returns the concatenated value.
            :::

            [Type Parameters:]{.paramLabel}
            :   `T` - the type of elements stored in the provided
                selectable list

            [Parameters:]{.paramLabel}
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
