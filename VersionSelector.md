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
[Package]{.packageLabelInType} [com.facebook.buck.versions](package-summary.html)
:::

## Interface VersionSelector {#interface-versionselector .title title="Interface VersionSelector"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `VersionUniverseVersionSelector`

    ------------------------------------------------------------------------

        public interface VersionSelector

    ::: block
    Interface for selecting versions for a versioned sub-graph
    represented by a root node and its version domain.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                               Method                                                                                                                                           Description
          --------------------------------------------------------------- ------------------------------------------------------------------------------------------------------------------------------------------------ -------------
          `com.google.common.collect.ImmutableMap<BuildTarget,​Version>`   `resolve​(BuildTarget root,        com.google.common.collect.ImmutableMap<BuildTarget,​com.google.common.collect.ImmutableSet<Version>> domain)`    

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

        []{#resolve(com.facebook.buck.core.model.BuildTarget,com.google.common.collect.ImmutableMap)}

        -   #### resolve

            ``` methodSignature
            com.google.common.collect.ImmutableMap<BuildTarget,​Version> resolve​(BuildTarget root,
                                                                                      com.google.common.collect.ImmutableMap<BuildTarget,​com.google.common.collect.ImmutableSet<Version>> domain)
                                                                               throws VersionException
            ```

            [Parameters:]{.paramLabel}
            :   `root` - the root of the versioned sub-graph.
            :   `domain` - the versioned nodes and their version domain.

            [Returns:]{.returnLabel}
            :   the map of versioned nodes to their selected versions.

            [Throws:]{.throwsLabel}
            :   `VersionException`
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
