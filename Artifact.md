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

## Interface Artifact {#interface-artifact .title title="Interface Artifact"}
:::

::: contentContainer
::: description
-   

    All Superinterfaces:
    :   `AddsToRuleKey`, `Comparable<Artifact>`, `SkylarkArtifactApi`,
        `com.google.devtools.build.lib.skylarkinterface.SkylarkPrintable`,
        `com.google.devtools.build.lib.skylarkinterface.SkylarkValue`

    ```{=html}
    <!-- -->
    ```

    All Known Subinterfaces:
    :   `BoundArtifact`, `BuildArtifact`, `SourceArtifact`

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `SourceArtifactImpl`

    ------------------------------------------------------------------------

        public interface Artifact
        extends SkylarkArtifactApi, Comparable<Artifact>, AddsToRuleKey

    ::: block
    An
    [`Artifact`](Artifact.html "interface in com.facebook.buck.core.artifact")
    is a file used during the build stage. It can either be a source
    file for the build or a generated file from an action
    This is the interface exposed to users.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                    Method                 Description
          ---------------------------------------------------- ---------------------- -------------
          `BoundArtifact`                                      `asBound()`             
          `com.facebook.buck.core.artifact.DeclaredArtifact`   `asDeclared()`          
          `OutputArtifact`                                     `asOutputArtifact()`    
          `boolean`                                            `isBound()`             

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Abstract
          Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}

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

        []{#isBound()}

        -   #### isBound

            ``` methodSignature
            boolean isBound()
            ```

            [Returns:]{.returnLabel}
            :   whether the artifact is bound, as described above

        []{#asBound()}

        -   #### asBound

            ``` methodSignature
            BoundArtifact asBound()
            ```

            [Returns:]{.returnLabel}
            :   a view of this artifact as a
                [`BoundArtifact`](BoundArtifact.html "interface in com.facebook.buck.core.artifact")

        []{#asDeclared()}

        -   #### asDeclared

            ``` methodSignature
            com.facebook.buck.core.artifact.DeclaredArtifact asDeclared()
            ```

            [Returns:]{.returnLabel}
            :   a view of this artifact as a `DeclaredArtifact`

        []{#asOutputArtifact()}

        -   #### asOutputArtifact

            ``` methodSignature
            OutputArtifact asOutputArtifact()
            ```

            [Returns:]{.returnLabel}
            :   get this artifact as an
                [`OutputArtifact`](OutputArtifact.html "class in com.facebook.buck.core.artifact").
                Throws if cannot be converted
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
