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
-   [Required](#annotation.type.required.element.summary) \| 
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

## Annotation Type ExcludeFromRuleKey {#annotation-type-excludefromrulekey .title title="Annotation Type ExcludeFromRuleKey"}
:::

::: contentContainer
::: description
-   

    ------------------------------------------------------------------------

        @Retention(RUNTIME)
        @Target({FIELD,METHOD})
        public @interface ExcludeFromRuleKey

    ::: block
    Marks a field/method of a class explicitly excluded from rulekeys.
    Usage of this should be very rare. In general, we consider uses of
    it to indicate likely correctness problems. Instead annotate the
    field with
    @[`AddToRuleKey`](AddToRuleKey.html "annotation in com.facebook.buck.core.rulekey").
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#annotation.type.required.element.summary}

        ### Required Element Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Required Element      | Description           |
        +=======================+=======================+=======================+
        | `Class<? extends C    | `inputs`              | ::: block             |
        | ustomFieldInputsTag>` |                       | Indicates how inputs  |
        |                       |                       | should be derived     |
        |                       |                       | from this field.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Cla                  | `serialization`       | ::: block             |
        | ss<? extends CustomFi |                       | Indicates how         |
        | eldSerializationTag>` |                       | serialization of this |
        |                       |                       | field should be       |
        |                       |                       | handled.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Required Elements[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#annotation.type.optional.element.summary}

        ### Optional Element Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Optional Element      | Description           |
        +=======================+=======================+=======================+
        | `Class<? extends      | `deps`                | ::: block             |
        |  CustomFieldDepsTag>` |                       | Indicates how deps    |
        |                       |                       | should be derived     |
        |                       |                       | from this field.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `reason`              | ::: block             |
        |                       |                       | This indicates the    |
        |                       |                       | reason we exclude a   |
        |                       |                       | value from rulekeys.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `shouldReport`        | ::: block             |
        |                       |                       | We really do think    |
        |                       |                       | that using this       |
        |                       |                       | annotation indicates  |
        |                       |                       | a likely source of    |
        |                       |                       | problems.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Optional Elements[ ]{.tabEnd}
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#annotation.type.element.detail}

        ### Element Detail

        []{#serialization()}

        -   #### serialization

                Class<? extends CustomFieldSerializationTag> serialization

            ::: block
            Indicates how serialization of this field should be handled.
            For default serialization, use
            [`DefaultFieldSerialization`](DefaultFieldSerialization.html "class in com.facebook.buck.core.rulekey")
            If serialization cannot possibly be supported, use
            [`ThrowingSerialization`](ThrowingSerialization.html "class in com.facebook.buck.core.rulekey").
            :::
    :::

    ::: {.section role="region"}
    -   []{#inputs()}
        -   #### inputs

                Class<? extends CustomFieldInputsTag> inputs

            ::: block
            Indicates how inputs should be derived from this field. For
            default inputs derivation, use
            [`DefaultFieldInputs`](DefaultFieldInputs.html "class in com.facebook.buck.core.rulekey").
            If this field should not contribute to inputs, use
            [`IgnoredFieldInputs`](IgnoredFieldInputs.html "class in com.facebook.buck.core.rulekey").
            :::
    :::

    ::: {.section role="region"}
    -   []{#reason()}
        -   #### reason

                String reason

            ::: block
            This indicates the reason we exclude a value from rulekeys.
            It\'s currently only used for logging.
            :::

            Default:
            :   \"\"
    :::

    ::: {.section role="region"}
    -   []{#deps()}
        -   #### deps

                Class<? extends CustomFieldDepsTag> deps

            ::: block
            Indicates how deps should be derived from this field. For
            default deps derivation, use
            [`DefaultFieldDeps`](DefaultFieldDeps.html "class in com.facebook.buck.core.rulekey").
            If this field should not contribute to deps, use
            [`IgnoredFieldDeps`](IgnoredFieldDeps.html "class in com.facebook.buck.core.rulekey").
            If you would like to provide custom logic, see
            `CustomFieldDeps`.
            :::

            Default:
            :   com.facebook.buck.core.rulekey.IgnoredFieldDeps.class
    :::

    ::: {.section role="region"}
    -   []{#shouldReport()}
        -   #### shouldReport

                boolean shouldReport

            ::: block
            We really do think that using this annotation indicates a
            likely source of problems. By default, the first time we
            encounter such an annotated field/method, we will log that
            information to the buck log.
            :::

            Default:
            :   true
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
-   [Required](#annotation.type.required.element.summary) \| 
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
