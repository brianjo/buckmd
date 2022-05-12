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

-   [Overview](../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../deprecated-list.html)
-   [Index](../../../../../../index-all.html)
-   [Help](../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.core.description.metadata](package-summary.html)
:::

## Interface MetadataProvidingDescription\<T\> {#interface-metadataprovidingdescriptiont .title title="Interface MetadataProvidingDescription"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `AppleBinaryDescription`, `AppleBundleDescription`,
        `AppleLibraryDescription`, `AppleTestDescription`,
        `CgoLibraryDescription`, `CxxBinaryDescription`,
        `CxxLibraryDescription`, `CxxTestDescription`,
        `GoLibraryDescription`, `GoTestDescription`,
        `PrebuiltAppleFrameworkDescription`,
        `PrebuiltGoLibraryDescription`, `PythonLibraryDescription`

    ------------------------------------------------------------------------

        public interface MetadataProvidingDescription<T>
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                                                                                                                                                                                                                                                                                                 Description
          ------------------- ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ -------------
          `<U> Optional<U>`   `createMetadata​(BuildTarget buildTarget,               ActionGraphBuilder graphBuilder,               CellPathResolver cellRoots,               T args,               Optional<com.google.common.collect.ImmutableMap<BuildTarget,​Version>> selectedVersions,               Class<U> metadataClass)`    

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

        []{#createMetadata(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.rules.ActionGraphBuilder,com.facebook.buck.core.cell.CellPathResolver,java.lang.Object,java.util.Optional,java.lang.Class)}
        []{#createMetadata(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.rules.ActionGraphBuilder,com.facebook.buck.core.cell.CellPathResolver,T,java.util.Optional,java.lang.Class)}

        -   #### createMetadata

            ``` methodSignature
            <U> Optional<U> createMetadata​(BuildTarget buildTarget,
                                           ActionGraphBuilder graphBuilder,
                                           CellPathResolver cellRoots,
                                           T args,
                                           Optional<com.google.common.collect.ImmutableMap<BuildTarget,​Version>> selectedVersions,
                                           Class<U> metadataClass)
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

-   [Overview](../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../deprecated-list.html)
-   [Index](../../../../../../index-all.html)
-   [Help](../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../allclasses.html)

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
