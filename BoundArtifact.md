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

## Interface BoundArtifact {#interface-boundartifact .title title="Interface BoundArtifact"}
:::

::: contentContainer
::: description
-   

    All Superinterfaces:
    :   `AddsToRuleKey`, `Artifact`, `Comparable<Artifact>`,
        `SkylarkArtifactApi`,
        `com.google.devtools.build.lib.skylarkinterface.SkylarkPrintable`,
        `com.google.devtools.build.lib.skylarkinterface.SkylarkValue`

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `SourceArtifactImpl`

    ------------------------------------------------------------------------

        public interface BoundArtifact
        extends Artifact

    ::: block
    Represents an
    [`Artifact`](Artifact.html "interface in com.facebook.buck.core.artifact")
    that will be materialized by the action execution phase. This can
    either be a source file or a file produced by an action.
    A bound artifact is only either an
    [`SourceArtifact`](SourceArtifact.html "interface in com.facebook.buck.core.artifact")
    or
    [`BuildArtifact`](BuildArtifact.html "interface in com.facebook.buck.core.artifact")

    This interface is not intended to be used by users, but only by the
    framework.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                Description
          ------------------- --------------------- -------------
          `BuildArtifact`     `asBuildArtifact()`    
          `SourceArtifact`    `asSource()`           
          `SourcePath`        `getSourcePath()`      

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

        []{#asSource()}

        -   #### asSource

            ``` methodSignature
            @Nullable
            SourceArtifact asSource()
            ```

            [Returns:]{.returnLabel}
            :   this artifact as a
                [`SourceArtifact`](SourceArtifact.html "interface in com.facebook.buck.core.artifact"),
                null if this is not a
                [`SourceArtifact`](SourceArtifact.html "interface in com.facebook.buck.core.artifact")

        []{#asBuildArtifact()}

        -   #### asBuildArtifact

            ``` methodSignature
            @Nullable
            BuildArtifact asBuildArtifact()
            ```

            [Returns:]{.returnLabel}
            :   this artifact as a
                [`BuildArtifact`](BuildArtifact.html "interface in com.facebook.buck.core.artifact"),
                null if this is not a
                [`BuildArtifact`](BuildArtifact.html "interface in com.facebook.buck.core.artifact")

        []{#getSourcePath()}

        -   #### getSourcePath

            ``` methodSignature
            SourcePath getSourcePath()
            ```

            [Returns:]{.returnLabel}
            :   the
                [`SourcePath`](../sourcepath/SourcePath.html "interface in com.facebook.buck.core.sourcepath")
                that represents where this artifact is.
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
