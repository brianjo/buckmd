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
[Package]{.packageLabelInType} [com.facebook.buck.core.model](package-summary.html)
:::

## Interface TargetConfigurationSerializer {#interface-targetconfigurationserializer .title title="Interface TargetConfigurationSerializer"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `JsonTargetConfigurationSerializer`

    ------------------------------------------------------------------------

        public interface TargetConfigurationSerializer

    ::: block
    Allows to convert
    [`TargetConfiguration`](TargetConfiguration.html "class in com.facebook.buck.core.model")
    to and from a string.
    This should be used when a
    [`TargetConfiguration`](TargetConfiguration.html "class in com.facebook.buck.core.model")
    needs to passed externally.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `TargetConfiguration` | `deserial             | ::: block             |
        |                       | ize​(String rawValue)` | Creates               |
        |                       |                       | [`Tar                 |
        |                       |                       | getConfiguration`](Ta |
        |                       |                       | rgetConfiguration.htm |
        |                       |                       | l "class in com.faceb |
        |                       |                       | ook.buck.core.model") |
        |                       |                       | from the provided     |
        |                       |                       | text representation.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `serialize            | ::: block             |
        |                       | ​(TargetConfiguration  | Converts              |
        |                       | targetConfiguration)` | [`Tar                 |
        |                       |                       | getConfiguration`](Ta |
        |                       |                       | rgetConfiguration.htm |
        |                       |                       | l "class in com.faceb |
        |                       |                       | ook.buck.core.model") |
        |                       |                       | to string.            |
        |                       |                       | :::                   |
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

        []{#serialize(com.facebook.buck.core.model.TargetConfiguration)}

        -   #### serialize

            ``` methodSignature
            String serialize​(TargetConfiguration targetConfiguration)
            ```

            ::: block
            Converts
            [`TargetConfiguration`](TargetConfiguration.html "class in com.facebook.buck.core.model")
            to string.
            :::

        []{#deserialize(java.lang.String)}

        -   #### deserialize

            ``` methodSignature
            TargetConfiguration deserialize​(String rawValue)
            ```

            ::: block
            Creates
            [`TargetConfiguration`](TargetConfiguration.html "class in com.facebook.buck.core.model")
            from the provided text representation.
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
