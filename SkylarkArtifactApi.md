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
[Package]{.packageLabelInType} [com.facebook.buck.core.starlark.rule.artifact](package-summary.html)
:::

## Interface SkylarkArtifactApi {#interface-skylarkartifactapi .title title="Interface SkylarkArtifactApi"}
:::

::: contentContainer
::: description
-   

    All Superinterfaces:
    :   `com.google.devtools.build.lib.skylarkinterface.SkylarkPrintable`,
        `com.google.devtools.build.lib.skylarkinterface.SkylarkValue`

    ```{=html}
    <!-- -->
    ```

    All Known Subinterfaces:
    :   `Artifact`, `BoundArtifact`, `BuildArtifact`, `SourceArtifact`

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `SourceArtifactImpl`

    ------------------------------------------------------------------------

        public interface SkylarkArtifactApi
        extends com.google.devtools.build.lib.skylarkinterface.SkylarkValue

    ::: block
    Helper struct fields that should be available to users of Artifact
    inside of user defined rules
    Note, that unlike
    https://docs.bazel.build/versions/master/skylark/lib/File.html, we
    do not presently expose root, dirname, or path to give a fully
    constructed path from the repository root. Should this be necessary
    in the future, we may expose those things.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type            Method                                                                              Description
          ---------------------------- ----------------------------------------------------------------------------------- -------------
          `SkylarkOutputArtifactApi`   `asSkylarkOutputArtifact​(com.google.devtools.build.lib.events.Location location)`    
          `String`                     `getBasename()`                                                                      
          `String`                     `getExtension()`                                                                     
          `Object`                     `getOwner()`                                                                         
          `String`                     `getShortPath()`                                                                     
          `default boolean`            `isImmutable()`                                                                      
          `boolean`                    `isSource()`                                                                         

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Abstract
          Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
          .tableTab}[[Default
          Methods](javascript:show(16);)[ ]{.tabEnd}]{#t5 .tableTab}

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

        []{#getBasename()}

        -   #### getBasename

            ``` methodSignature
            String getBasename()
            ```

        []{#getExtension()}

        -   #### getExtension

            ``` methodSignature
            String getExtension()
            ```

        []{#isSource()}

        -   #### isSource

            ``` methodSignature
            boolean isSource()
            ```

        []{#getOwner()}

        -   #### getOwner

            ``` methodSignature
            Object getOwner()
            ```

        []{#getShortPath()}

        -   #### getShortPath

            ``` methodSignature
            String getShortPath()
            ```

        []{#asSkylarkOutputArtifact(com.google.devtools.build.lib.events.Location)}

        -   #### asSkylarkOutputArtifact

            ``` methodSignature
            SkylarkOutputArtifactApi asSkylarkOutputArtifact​(com.google.devtools.build.lib.events.Location location)
                                                      throws com.google.devtools.build.lib.syntax.EvalException
            ```

            [Throws:]{.throwsLabel}
            :   `com.google.devtools.build.lib.syntax.EvalException`

        []{#isImmutable()}

        -   #### isImmutable

            ``` methodSignature
            default boolean isImmutable()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `isImmutable` in
                interface `com.google.devtools.build.lib.skylarkinterface.SkylarkValue`
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
