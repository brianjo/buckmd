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

-   [Overview](../../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../index-all.html)
-   [Help](../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.core.rules.providers.annotations](package-summary.html)
:::

## Annotation Type ImmutableInfo {#annotation-type-immutableinfo .title title="Annotation Type ImmutableInfo"}
:::

::: contentContainer
::: description
-   

    ------------------------------------------------------------------------

        @Target({TYPE,PACKAGE,ANNOTATION_TYPE})
        @Retention(RUNTIME)
        public @interface ImmutableInfo

    ::: block
    Annotation marking a class as an immutable built in implementation
    of
    [`ProviderInfo`](../ProviderInfo.html "interface in com.facebook.buck.core.rules.providers").
    This uses the immutable library to generate an implementation class
    that conforms to the requirements of providers declared in java.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#annotation.type.required.element.summary}

        ### Required Element Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Required Element      | Description           |
        +=======================+=======================+=======================+
        | `String[]`            | `args`                | ::: block             |
        |                       |                       | TODO this is here     |
        |                       |                       | because java          |
        |                       |                       | reflection doesn\'t   |
        |                       |                       | expose parameter      |
        |                       |                       | names, and methods    |
        |                       |                       | can\'t be retrieved   |
        |                       |                       | in order of           |
        |                       |                       | declaration.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Required Elements[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#annotation.type.optional.element.summary}

        ### Optional Element Summary

          Modifier and Type   Optional Element         Description
          ------------------- ------------------------ -------------
          `String[]`          `defaultSkylarkValues`    
          `String[]`          `noneable`                

          : Optional Elements[ ]{.tabEnd}
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#annotation.type.element.detail}

        ### Element Detail

        []{#args()}

        -   #### args

                String[] args

            ::: block
            TODO this is here because java reflection doesn\'t expose
            parameter names, and methods can\'t be retrieved in order of
            declaration. We should just have some custom annotation
            processor to generate this.
            :::

            [Returns:]{.returnLabel}
            :   an array of Strings that represent the names of the
                constructor parameters in order of declared methods.
                This should be in the lower underscore naming convention
                for python.
    :::

    ::: {.section role="region"}
    -   []{#defaultSkylarkValues()}
        -   #### defaultSkylarkValues

                String[] defaultSkylarkValues

            [Returns:]{.returnLabel}
            :   an array of string representations of default values to
                use in the Starlark interpreter if a kwarg is not
                provided.

            ```{=html}
            <!-- -->
            ```

            Default:
            :   {}
    :::

    ::: {.section role="region"}
    -   []{#noneable()}
        -   #### noneable

                String[] noneable

            [Returns:]{.returnLabel}
            :   an array of fields that should be noneable

            ```{=html}
            <!-- -->
            ```

            Default:
            :   {}
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

-   [Overview](../../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../index-all.html)
-   [Help](../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../allclasses.html)

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
