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
[Package]{.packageLabelInType} [com.facebook.buck.core.exceptions](package-summary.html)
:::

## Interface ExceptionWithHumanReadableMessage {#interface-exceptionwithhumanreadablemessage .title title="Interface ExceptionWithHumanReadableMessage"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `ActionCreationException`, `ArtifactDeclarationException`,
        `BuildFileParseException`, `BuildTargetException`,
        `BuildTargetParseException`,
        `CommandAlias.UnsupportedPlatformException`,
        `CommandLineArgException`, `CommandLineException`,
        `FlavorDomainException`, `HumanReadableException`,
        `LogDaemonException`, `MissingBuildFileException`,
        `NoSuchBuildTargetException`, `NoSuchTargetException`,
        `ProcessExecutionFailedException`, `QueryException`,
        `RuleAnalysisException`, `ToolchainInstantiationException`,
        `UnexpectedFlavorException`, `UnknownCellException`

    ------------------------------------------------------------------------

        public interface ExceptionWithHumanReadableMessage
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `def                  | `                     | ::: block             |
        | ault DependencyStack` | getDependencyStack()` | Get the dependency    |
        |                       |                       | stack associated with |
        |                       |                       | this error            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getHumanRe           |                       |
        |                       | adableErrorMessage()` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
        .tableTab}[[Default
        Methods](javascript:show(16);)[ ]{.tabEnd}]{#t5 .tableTab}
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getHumanReadableErrorMessage()}

        -   #### getHumanReadableErrorMessage

            ``` methodSignature
            String getHumanReadableErrorMessage()
            ```

            [Returns:]{.returnLabel}
            :   a human-readable error message

        []{#getDependencyStack()}

        -   #### getDependencyStack

            ``` methodSignature
            default DependencyStack getDependencyStack()
            ```

            ::: block
            Get the dependency stack associated with this error
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
