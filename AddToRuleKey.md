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
-   Field \| 
-   Required \| 
-   [Optional](#annotation.type.optional.element.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   [Element](#annotation.type.element.detail)

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
[Package]{.packageLabelInType} [com.facebook.buck.core.rulekey](package-summary.html)
:::

## Annotation Type AddToRuleKey {#annotation-type-addtorulekey .title title="Annotation Type AddToRuleKey"}
:::

::: contentContainer
::: description
-   

    ------------------------------------------------------------------------

        @Retention(RUNTIME)
        @Target({FIELD,METHOD})
        public @interface AddToRuleKey

    ::: block
    Indicates that a field or method of a class should be added to
    rulekeys when an instance of that class is added to a rulekey.
    This annotation also indicates that we should derive inputs, deps
    and serialization automatically from this field/method.

    Annotating a method with \@AddToRuleKey should only be used for
    Immutable objects.

    In general, this should be added to all fields unless there\'s a
    good reason not to add it. In that case, annotated the field/method
    with
    @[`ExcludeFromRuleKey`](ExcludeFromRuleKey.html "annotation in com.facebook.buck.core.rulekey")
    to indicate that not adding it to the keys is intentional.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#annotation.type.optional.element.summary}

        ### Optional Element Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Optional Element      | Description           |
        +=======================+=======================+=======================+
        | `boolean`             | `stringify`           | ::: block             |
        |                       |                       | This causes us to add |
        |                       |                       | the value to the      |
        |                       |                       | rulekey in its        |
        |                       |                       | stringified form      |
        |                       |                       | (i.e.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Optional Elements[ ]{.tabEnd}
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#annotation.type.element.detail}

        ### Element Detail

        []{#stringify()}

        -   #### stringify

                boolean stringify

            ::: block
            This causes us to add the value to the rulekey in its
            stringified form (i.e. we call toString() on it).
            :::

            Default:
            :   false
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
-   Field \| 
-   Required \| 
-   [Optional](#annotation.type.optional.element.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   [Element](#annotation.type.element.detail)

</div>

[]{#skip.navbar.bottom}
:::
