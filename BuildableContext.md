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
[Package]{.packageLabelInType} [com.facebook.buck.core.build.buildable.context](package-summary.html)
:::

## Interface BuildableContext {#interface-buildablecontext .title title="Interface BuildableContext"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `DefaultBuildableContext`, `RecordArtifactVerifier`

    ------------------------------------------------------------------------

        public interface BuildableContext

    ::: block
    Context object that is specific to an individual
    [`BuildRule`](../../../rules/BuildRule.html "interface in com.facebook.buck.core.rules").
    This differs from
    [`BuildContext`](../../context/BuildContext.html "class in com.facebook.buck.core.build.context")
    in that a
    [`BuildContext`](../../context/BuildContext.html "class in com.facebook.buck.core.build.context")
    is a context that is shared by all
    [`BuildRule`](../../../rules/BuildRule.html "interface in com.facebook.buck.core.rules")s
    whereas a new
    [`BuildableContext`](BuildableContext.html "interface in com.facebook.buck.core.build.buildable.context")
    is created for each call to
    [`BuildRule.getBuildSteps(com.facebook.buck.core.build.context.BuildContext,  BuildableContext)`](../../../rules/BuildRule.html#getBuildSteps(com.facebook.buck.core.build.context.BuildContext,com.facebook.buck.core.build.buildable.context.BuildableContext)).
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                                  Description
          ------------------- --------------------------------------- -------------
          `void`              `recordArtifact​(Path pathToArtifact)`    

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

        []{#recordArtifact(java.nio.file.Path)}

        -   #### recordArtifact

            ``` methodSignature
            void recordArtifact​(Path pathToArtifact)
            ```

            [See Also:]{.seeLabel}
            :   [`BuildInfoRecorder.recordArtifact(Path)`](../../engine/buildinfo/BuildInfoRecorder.html#recordArtifact(java.nio.file.Path))
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
