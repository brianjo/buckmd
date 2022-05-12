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

-   [Overview](../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../deprecated-list.html)
-   [Index](../../../../index-all.html)
-   [Help](../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.shell](package-summary.html)
:::

## Interface WorkerTool {#interface-workertool .title title="Interface WorkerTool"}
:::

::: contentContainer
::: description
-   

    All Superinterfaces:
    :   `AddsToRuleKey`

    ------------------------------------------------------------------------

        public interface WorkerTool
        extends AddsToRuleKey

    ::: block
    Worker tool definition
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `com.google.          | `getInstanceKey()`    |                       |
        | common.hash.HashCode` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `getMaxWorkers()`     |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Path`                | `getTempDir​(ProjectFi | ::: block             |
        |                       | lesystem filesystem)` | Returns temp dir for  |
        |                       |                       | this WorkerTool and   |
        |                       |                       | provided filesystem   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Tool`                | `getTool()`           |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isAsync()`           |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isPersistent()`      |                       |
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

        []{#getTool()}

        -   #### getTool

            ``` methodSignature
            Tool getTool()
            ```

        []{#getTempDir(com.facebook.buck.io.filesystem.ProjectFilesystem)}

        -   #### getTempDir

            ``` methodSignature
            Path getTempDir​(ProjectFilesystem filesystem)
            ```

            ::: block
            Returns temp dir for this WorkerTool and provided filesystem
            :::

        []{#getMaxWorkers()}

        -   #### getMaxWorkers

            ``` methodSignature
            int getMaxWorkers()
            ```

        []{#isPersistent()}

        -   #### isPersistent

            ``` methodSignature
            boolean isPersistent()
            ```

        []{#getInstanceKey()}

        -   #### getInstanceKey

            ``` methodSignature
            com.google.common.hash.HashCode getInstanceKey()
            ```

        []{#isAsync()}

        -   #### isAsync

            ``` methodSignature
            boolean isAsync()
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

-   [Overview](../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../deprecated-list.html)
-   [Index](../../../../index-all.html)
-   [Help](../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../allclasses.html)

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
