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

## Interface WrapsException {#interface-wrapsexception .title title="Interface WrapsException"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `BuckUncheckedExecutionException`, `BuildRuleFailedException`,
        `StepFailedException`

    ------------------------------------------------------------------------

        public interface WrapsException

    ::: block
    This interface indicates that an exception is just used to wrap
    another and isn\'t the true root cause of the problem. This is used
    to present the exception in a more user-friendly way.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static Throwable`    | `getRootCause​(        | ::: block             |
        |                       | Throwable throwable)` | Unwraps exception to  |
        |                       |                       | the root cause.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Static Methods[ ]{.tabEnd}
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getRootCause(java.lang.Throwable)}

        -   #### getRootCause

            ``` methodSignature
            static Throwable getRootCause​(Throwable throwable)
            ```

            ::: block
            Unwraps exception to the root cause.
            TODO(cjhopman): This behavior is slightly different than
            that in ErrorLogger as it doesn\'t unwrap the
            non-WrapsException exceptions that ErrorLogger does.
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
