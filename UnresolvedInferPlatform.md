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
[Package]{.packageLabelInType} [com.facebook.buck.infer](package-summary.html)
:::

## Interface UnresolvedInferPlatform {#interface-unresolvedinferplatform .title title="Interface UnresolvedInferPlatform"}
:::

::: contentContainer
::: description
-   

    ------------------------------------------------------------------------

        public interface UnresolvedInferPlatform

    ::: block
    Used by descriptions to properly handle
    [`InferPlatform`](InferPlatform.html "class in com.facebook.buck.infer").
    Particularly:
    During parsing and configuration it provides information about
    parse-time deps, for instance when infer binary or infer config are
    provided by some targets that otherwise not needed for the build.

    During action graph creation it can be resolved to
    [`InferPlatform`](InferPlatform.html "class in com.facebook.buck.infer").
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static void`         | `addParseTimeDepsT    | ::: block             |
        |                       | oInferFlavored​(com.go | Helper method to add  |
        |                       | ogle.common.collect.I | parse-time deps to    |
        |                       | mmutableCollection.Bu | target graph for      |
        |                       | ilder<BuildTarget> ta | nullsafe flavored     |
        |                       | rgetGraphOnlyDepsBuil | targets.              |
        |                       | der,                  | :::                   |
        |                       |                BuildT |                       |
        |                       | arget buildTarget,    |                       |
        |                       |                       |                       |
        |                       |         UnresolvedInf |                       |
        |                       | erPlatform platform)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `I                    | `getParseTimeDeps     | ::: block             |
        | terable<BuildTarget>` | ​(TargetConfiguration  | Returns               |
        |                       | targetConfiguration)` | [`InferPl             |
        |                       |                       | atform`](InferPlatfor |
        |                       |                       | m.html "class in com. |
        |                       |                       | facebook.buck.infer") |
        |                       |                       | parse-time deps.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `InferPlatform`       | `                     | ::: block             |
        |                       | resolve​(BuildRuleReso | Resolves to the       |
        |                       | lver resolver,        | platform.             |
        |                       |  TargetConfiguration  | :::                   |
        |                       | targetConfiguration)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#resolve(com.facebook.buck.core.rules.BuildRuleResolver,com.facebook.buck.core.model.TargetConfiguration)}

        -   #### resolve

            ``` methodSignature
            InferPlatform resolve​(BuildRuleResolver resolver,
                                  TargetConfiguration targetConfiguration)
            ```

            ::: block
            Resolves to the platform.
            :::

        []{#getParseTimeDeps(com.facebook.buck.core.model.TargetConfiguration)}

        -   #### getParseTimeDeps

            ``` methodSignature
            Iterable<BuildTarget> getParseTimeDeps​(TargetConfiguration targetConfiguration)
            ```

            ::: block
            Returns
            [`InferPlatform`](InferPlatform.html "class in com.facebook.buck.infer")
            parse-time deps.
            :::

        []{#addParseTimeDepsToInferFlavored(com.google.common.collect.ImmutableCollection.Builder,com.facebook.buck.core.model.BuildTarget,com.facebook.buck.infer.UnresolvedInferPlatform)}

        -   #### addParseTimeDepsToInferFlavored

            ``` methodSignature
            static void addParseTimeDepsToInferFlavored​(com.google.common.collect.ImmutableCollection.Builder<BuildTarget> targetGraphOnlyDepsBuilder,
                                                        BuildTarget buildTarget,
                                                        UnresolvedInferPlatform platform)
            ```

            ::: block
            Helper method to add parse-time deps to target graph for
            nullsafe flavored targets.
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
