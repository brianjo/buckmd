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
[Package]{.packageLabelInType} [com.facebook.buck.core.artifact](package-summary.html)
:::

## Interface BuildArtifact {#interface-buildartifact .title title="Interface BuildArtifact"}
:::

::: contentContainer
::: description
-   

    All Superinterfaces:
    :   `AddsToRuleKey`, `Artifact`, `Comparable<Artifact>`,
        `SkylarkArtifactApi`,
        `com.google.devtools.build.lib.skylarkinterface.SkylarkPrintable`,
        `com.google.devtools.build.lib.skylarkinterface.SkylarkValue`

    ------------------------------------------------------------------------

        public interface BuildArtifact
        extends Artifact

    ::: block
    Represents an
    [`Artifact`](Artifact.html "interface in com.facebook.buck.core.artifact")
    that is materialized by an
    [`Action`](../rules/actions/Action.html "interface in com.facebook.buck.core.rules.actions").
    This is not intended to be exposed to users, but used only by the
    build engine.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                 Method                 Description
          --------------------------------- ---------------------- -------------
          `ActionAnalysisDataKey`           `getActionDataKey()`    
          `Path`                            `getOutputPath()`       
          `ExplicitBuildTargetSourcePath`   `getSourcePath()`       

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Abstract
          Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.core.artifact.Artifact}

            ### Methods inherited from interface com.facebook.buck.core.artifact.[Artifact](Artifact.html "interface in com.facebook.buck.core.artifact")

            `asBound, asDeclared, asOutputArtifact, isBound`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Comparable}

            ### Methods inherited from interface java.lang.[Comparable](http://docs.oracle.com/javase/7/docs/api/java/lang/Comparable.html?is-external=true "class or interface in java.lang"){.externalLink}

            `compareTo`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.starlark.rule.artifact.SkylarkArtifactApi}

            ### Methods inherited from interface com.facebook.buck.core.starlark.rule.artifact.[SkylarkArtifactApi](../starlark/rule/artifact/SkylarkArtifactApi.html "interface in com.facebook.buck.core.starlark.rule.artifact")

            `asSkylarkOutputArtifact, getBasename, getExtension, getOwner, getShortPath, isImmutable, isSource`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.google.devtools.build.lib.skylarkinterface.SkylarkPrintable}

            ### Methods inherited from interface com.google.devtools.build.lib.skylarkinterface.SkylarkPrintable

            `debugPrint, repr, str`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.google.devtools.build.lib.skylarkinterface.SkylarkValue}

            ### Methods inherited from interface com.google.devtools.build.lib.skylarkinterface.SkylarkValue

            `isHashable`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getActionDataKey()}

        -   #### getActionDataKey

            ``` methodSignature
            @Parameter
            @Nullable
            ActionAnalysisDataKey getActionDataKey()
            ```

            [Returns:]{.returnLabel}
            :   the key to the
                [`ActionAnalysisData`](../rules/analysis/action/ActionAnalysisData.html "interface in com.facebook.buck.core.rules.analysis.action")
                that owns this artifact. This is null if this is a
                legacy artifact (one that refers to a source path of an
                old BuildRule.

        []{#getSourcePath()}

        -   #### getSourcePath

            ``` methodSignature
            ExplicitBuildTargetSourcePath getSourcePath()
            ```

            [Returns:]{.returnLabel}
            :   the path to the artifact

        []{#getOutputPath()}

        -   #### getOutputPath

            ``` methodSignature
            Path getOutputPath()
            ```

            [Returns:]{.returnLabel}
            :   the path the user intends to write to relative to the
                assigned package path.
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
