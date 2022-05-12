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
[Package]{.packageLabelInType} [com.facebook.buck.remoteexecution](package-summary.html)
:::

## Interface UploadDataSupplier {#interface-uploaddatasupplier .title title="Interface UploadDataSupplier"}
:::

::: contentContainer
::: description
-   

    ------------------------------------------------------------------------

        public interface UploadDataSupplier

    ::: block
    Used for wrapping access to data for uploads.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `default String`      | `describe()`          | ::: block             |
        |                       |                       | Describe what data is |
        |                       |                       | being uploaded.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `InputStream`         | `get()`               |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Protocol.Digest`     | `getDigest()`         |                       |
        +-----------------------+-----------------------+-----------------------+
        | `stati                | `of​(String            | ::: block             |
        | c UploadDataSupplier` | name,   Protocol.Dige | Create a simple       |
        |                       | st digest,   Throwing | UploadDataSupplier.   |
        |                       | Supplier<InputStream, | :::                   |
        |                       | ​IOException> stream)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
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

        []{#describe()}

        -   #### describe

            ``` methodSignature
            default String describe()
            ```

            ::: block
            Describe what data is being uploaded. It may be helpful to
            include the size/hash/contents of the data. If doing so,
            those values should be recomputed (one major use of
            including that data would be to diagnose cases where the
            server claims that the data doesn\'t match the digest).
            :::

        []{#get()}

        -   #### get

            ``` methodSignature
            InputStream get()
                     throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#getDigest()}

        -   #### getDigest

            ``` methodSignature
            Protocol.Digest getDigest()
            ```

        []{#of(java.lang.String,com.facebook.buck.remoteexecution.interfaces.Protocol.Digest,com.facebook.buck.util.function.ThrowingSupplier)}

        -   #### of

            ``` methodSignature
            static UploadDataSupplier of​(String name,
                                         Protocol.Digest digest,
                                         ThrowingSupplier<InputStream,​IOException> stream)
            ```

            ::: block
            Create a simple UploadDataSupplier.
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
