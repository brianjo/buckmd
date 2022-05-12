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

## Interface TargetTranslatable\<T\> {#interface-targettranslatablet .title title="Interface TargetTranslatable"}
:::

::: contentContainer
::: description
-   

    All Known Subinterfaces:
    :   `CcFlagsMacro`, `CcMacro`, `CxxFlagsMacro`, `CxxMacro`,
        `EnvMacro`, `Macro`, `PlatformNameMacro`

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `AbsoluteOutputMacro`, `AbstractExecutableTargetOrHostMacro`,
        `BaseLocationMacro`, `BuildTargetMacro`, `ClasspathAbiMacro`,
        `ClasspathMacro`, `CppFlagsMacro`,
        `CxxGenruleFilterAndTargetsMacro`, `CxxppFlagsMacro`,
        `ExecutableMacro`, `ExecutableTargetMacro`,
        `LdflagsSharedFilterMacro`, `LdflagsSharedMacro`,
        `LdflagsStaticFilterMacro`, `LdflagsStaticMacro`,
        `LdflagsStaticPicFilterMacro`, `LdflagsStaticPicMacro`,
        `LdMacro`, `LocationMacro`, `LocationPlatformMacro`,
        `MavenCoordinatesMacro`, `NeededCoverageSpec`, `OutputMacro`,
        `PatternMatchedCollection`, `QueryMacro`, `QueryOutputsMacro`,
        `QueryPathsMacro`, `QueryTargetsAndOutputsMacro`,
        `QueryTargetsMacro`, `SourceSet`, `SourceSortedSet`,
        `StringWithMacros`, `VersionMatchedCollection`, `WorkerMacro`

    ------------------------------------------------------------------------

        public interface TargetTranslatable<T>

    ::: block
    Interface for objects which defined how they should be translated in
    constructor args for versioning.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                                                                                                                                            Description
          ------------------- ------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `Optional<T>`       `translateTargets​(CellNameResolver cellPathResolver,                 BaseName targetBaseName,                 TargetNodeTranslator translator)`    

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

        []{#translateTargets(com.facebook.buck.core.cell.nameresolver.CellNameResolver,com.facebook.buck.core.model.BaseName,com.facebook.buck.versions.TargetNodeTranslator)}

        -   #### translateTargets

            ``` methodSignature
            Optional<T> translateTargets​(CellNameResolver cellPathResolver,
                                         BaseName targetBaseName,
                                         TargetNodeTranslator translator)
            ```

            [Returns:]{.returnLabel}
            :   if any changes are required, return the translated
                object.
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
