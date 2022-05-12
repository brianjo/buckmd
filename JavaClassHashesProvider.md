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
[Package]{.packageLabelInType} [com.facebook.buck.jvm.core](package-summary.html)
:::

## Interface JavaClassHashesProvider {#interface-javaclasshashesprovider .title title="Interface JavaClassHashesProvider"}
:::

::: contentContainer
::: description
-   

    All Superinterfaces:
    :   `AddsToRuleKey`

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `DefaultJavaClassHashesProvider`

    ------------------------------------------------------------------------

        public interface JavaClassHashesProvider
        extends AddsToRuleKey

    ::: block
    Provider that can load java class hashes from the filesystem.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `c                    | `                     |                       |
        | om.google.common.coll | getClassNamesToHashes |                       |
        | ect.ImmutableSortedMa | ​(ProjectFilesystem fi |                       |
        | p<String,​com.google.c | lesystem,             |                       |
        | ommon.hash.HashCode>` |           SourcePathR |                       |
        |                       | esolverAdapter source |                       |
        |                       | PathResolverAdapter)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `invalidate()`        | ::: block             |
        |                       |                       | Invalidates a state   |
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

        []{#getClassNamesToHashes(com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter)}

        -   #### getClassNamesToHashes

            ``` methodSignature
            com.google.common.collect.ImmutableSortedMap<String,​com.google.common.hash.HashCode> getClassNamesToHashes​(ProjectFilesystem filesystem,
                                                                                                                             SourcePathResolverAdapter sourcePathResolverAdapter)
            ```

        []{#invalidate()}

        -   #### invalidate

            ``` methodSignature
            void invalidate()
            ```

            ::: block
            Invalidates a state
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
