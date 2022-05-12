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
[Package]{.packageLabelInType} [com.facebook.buck.features.python](package-summary.html)
:::

## Interface PythonComponents.Resolved {#interface-pythoncomponents.resolved .title title="Interface PythonComponents.Resolved"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `PythonMappedComponents.Resolved`

    ```{=html}
    <!-- -->
    ```

    Enclosing interface:
    :   [PythonComponents](PythonComponents.html "interface in com.facebook.buck.features.python")

    ------------------------------------------------------------------------

        public static interface PythonComponents.Resolved

    ::: block
    Resolve this
    [`PythonComponents`](PythonComponents.html "interface in com.facebook.buck.features.python")
    into a class usable by
    [`Step`](../../step/Step.html "interface in com.facebook.buck.step")s.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Interface             | Description           |
        +=======================+=======================+=======================+
        | `static interface `   | `Py                   | ::: block             |
        |                       | thonComponents.Resolv | A `BiConsumer` which  |
        |                       | ed.ComponentConsumer` | throws a              |
        |                       |                       | [`IOException`](http  |
        |                       |                       | ://docs.oracle.com/ja |
        |                       |                       | vase/7/docs/api/java/ |
        |                       |                       | io/IOException.html?i |
        |                       |                       | s-external=true "clas |
        |                       |                       | s or interface in jav |
        |                       |                       | a.io"){.externalLink} |
        |                       |                       | for use by executing  |
        |                       |                       | [`Step                |
        |                       |                       | `](../../step/Step.ht |
        |                       |                       | ml "interface in com. |
        |                       |                       | facebook.buck.step")s |
        |                       |                       | to process the        |
        |                       |                       | [`Path`](http://doc   |
        |                       |                       | s.oracle.com/javase/7 |
        |                       |                       | /docs/api/java/nio/fi |
        |                       |                       | le/Path.html?is-exter |
        |                       |                       | nal=true "class or in |
        |                       |                       | terface in java.nio.f |
        |                       |                       | ile"){.externalLink}s |
        |                       |                       | to the components     |
        |                       |                       | from this object.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `void`                | `forEachPythonC       | ::: block             |
        |                       | omponent​(PythonCompon | Called by executing   |
        |                       | ents.Resolved.Compone | [`Step                |
        |                       | ntConsumer consumer)` | `](../../step/Step.ht |
        |                       |                       | ml "interface in com. |
        |                       |                       | facebook.buck.step")s |
        |                       |                       | to iterate over the   |
        |                       |                       | components owned by   |
        |                       |                       | this                  |
        |                       |                       | [`PythonC             |
        |                       |                       | omponents`](PythonCom |
        |                       |                       | ponents.html "interfa |
        |                       |                       | ce in com.facebook.bu |
        |                       |                       | ck.features.python"). |
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

        []{#forEachPythonComponent(com.facebook.buck.features.python.PythonComponents.Resolved.ComponentConsumer)}

        -   #### forEachPythonComponent

            ``` methodSignature
            void forEachPythonComponent​(PythonComponents.Resolved.ComponentConsumer consumer)
                                 throws IOException
            ```

            ::: block
            Called by executing
            [`Step`](../../step/Step.html "interface in com.facebook.buck.step")s
            to iterate over the components owned by this
            [`PythonComponents`](PythonComponents.html "interface in com.facebook.buck.features.python").
            :::

            [Throws:]{.throwsLabel}
            :   `IOException`
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
