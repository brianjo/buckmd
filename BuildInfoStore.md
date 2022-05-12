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
[Package]{.packageLabelInType} [com.facebook.buck.core.build.engine.buildinfo](package-summary.html)
:::

## Interface BuildInfoStore {#interface-buildinfostore .title title="Interface BuildInfoStore"}
:::

::: contentContainer
::: description
-   

    All Superinterfaces:
    :   `AutoCloseable`, `Closeable`

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `SQLiteBuildInfoStore`

    ------------------------------------------------------------------------

        public interface BuildInfoStore
        extends Closeable

    ::: block
    Repository of build metadata.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                         Method                                                                                 Description
          --------------------------------------------------------- -------------------------------------------------------------------------------------- -------------
          `void`                                                    `close()`                                                                               
          `void`                                                    `deleteMetadata​(BuildTarget buildTarget)`                                               
          `com.google.common.collect.ImmutableMap<String,​String>`   `getAllMetadata​(BuildTarget buildTarget)`                                               
          `Optional<String>`                                        `readMetadata​(BuildTarget buildTarget,             String key)`                         
          `void`                                                    `updateMetadata​(BuildTarget buildTarget,               Map<String,​String> metadata)`    

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

        []{#readMetadata(com.facebook.buck.core.model.BuildTarget,java.lang.String)}

        -   #### readMetadata

            ``` methodSignature
            Optional<String> readMetadata​(BuildTarget buildTarget,
                                          String key)
            ```

        []{#close()}

        -   #### close

            ``` methodSignature
            void close()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `close` in interface `AutoCloseable`

            [Specified by:]{.overrideSpecifyLabel}
            :   `close` in interface `Closeable`

        []{#getAllMetadata(com.facebook.buck.core.model.BuildTarget)}

        -   #### getAllMetadata

            ``` methodSignature
            com.google.common.collect.ImmutableMap<String,​String> getAllMetadata​(BuildTarget buildTarget)
                                                                                throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#updateMetadata(com.facebook.buck.core.model.BuildTarget,java.util.Map)}

        -   #### updateMetadata

            ``` methodSignature
            void updateMetadata​(BuildTarget buildTarget,
                                Map<String,​String> metadata)
                         throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#deleteMetadata(com.facebook.buck.core.model.BuildTarget)}

        -   #### deleteMetadata

            ``` methodSignature
            void deleteMetadata​(BuildTarget buildTarget)
                         throws IOException
            ```

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
