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
[Package]{.packageLabelInType} [com.facebook.buck.rules.coercer](package-summary.html)
:::

## Interface TypeCoercerFactory {#interface-typecoercerfactory .title title="Interface TypeCoercerFactory"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `DefaultTypeCoercerFactory`

    ------------------------------------------------------------------------

        public interface TypeCoercerFactory
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `<T extends DataTrans | `getC                 | ::: block             |
        | ferObject>DataTransfe | onstructorArgDescript | Returns an            |
        | rObjectDescriptor<T>` | or​(Class<T> dtoType)` | unpopulated DTO       |
        |                       |                       | object, and the build |
        |                       |                       | method which must be  |
        |                       |                       | called with it when   |
        |                       |                       | it is finished being  |
        |                       |                       | populated.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `t                    |                       |
        | <T> TypeCoercer<?,​T>` | ypeCoercerForType​(com |                       |
        |                       | .google.common.reflec |                       |
        |                       | t.TypeToken<T> type)` |                       |
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

        []{#typeCoercerForType(com.google.common.reflect.TypeToken)}

        -   #### typeCoercerForType

            ``` methodSignature
            <T> TypeCoercer<?,​T> typeCoercerForType​(com.google.common.reflect.TypeToken<T> type)
            ```

        []{#getConstructorArgDescriptor(java.lang.Class)}

        -   #### getConstructorArgDescriptor

            ``` methodSignature
            <T extends DataTransferObject> DataTransferObjectDescriptor<T> getConstructorArgDescriptor​(Class<T> dtoType)
            ```

            ::: block
            Returns an unpopulated DTO object, and the build method
            which must be called with it when it is finished being
            populated.
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
