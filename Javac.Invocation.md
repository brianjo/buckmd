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
[Package]{.packageLabelInType} [com.facebook.buck.jvm.java](package-summary.html)
:::

## Interface Javac.Invocation {#interface-javac.invocation .title title="Interface Javac.Invocation"}
:::

::: contentContainer
::: description
-   

    All Superinterfaces:
    :   `AutoCloseable`

    ```{=html}
    <!-- -->
    ```

    Enclosing interface:
    :   [Javac](Javac.html "interface in com.facebook.buck.jvm.java")

    ------------------------------------------------------------------------

        public static interface Javac.Invocation
        extends AutoCloseable
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `int`                 | `buildClasses()`      |                       |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `buildSourceAbiJar()` | ::: block             |
        |                       |                       | Produces a source ABI |
        |                       |                       | jar.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `bui                  | ::: block             |
        |                       | ldSourceOnlyAbiJar()` | Produces a            |
        |                       |                       | source-only ABI jar.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `close()`             |                       |
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

        []{#buildSourceOnlyAbiJar()}

        -   #### buildSourceOnlyAbiJar

            ``` methodSignature
            int buildSourceOnlyAbiJar()
                               throws InterruptedException
            ```

            ::: block
            Produces a source-only ABI jar.
            [`buildClasses()`](#buildClasses()) may not be called on an
            invocation on which this has been called.
            :::

            [Throws:]{.throwsLabel}
            :   `InterruptedException`

        []{#buildSourceAbiJar()}

        -   #### buildSourceAbiJar

            ``` methodSignature
            int buildSourceAbiJar()
                           throws InterruptedException
            ```

            ::: block
            Produces a source ABI jar. Must be called before
            [`buildClasses()`](#buildClasses())
            :::

            [Throws:]{.throwsLabel}
            :   `InterruptedException`

        []{#buildClasses()}

        -   #### buildClasses

            ``` methodSignature
            int buildClasses()
                      throws InterruptedException
            ```

            [Throws:]{.throwsLabel}
            :   `InterruptedException`

        []{#close()}

        -   #### close

            ``` methodSignature
            void close()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `close` in interface `AutoCloseable`
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
