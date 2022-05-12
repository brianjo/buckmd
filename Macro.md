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
[Package]{.packageLabelInType} [com.facebook.buck.rules.macros](package-summary.html)
:::

## Interface Macro {#interface-macro .title title="Interface Macro"}
:::

::: contentContainer
::: description
-   

    All Superinterfaces:
    :   `TargetTranslatable<Macro>`

    ```{=html}
    <!-- -->
    ```

    All Known Subinterfaces:
    :   `CcFlagsMacro`, `CcMacro`, `CxxFlagsMacro`, `CxxMacro`,
        `EnvMacro`, `PlatformNameMacro`

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
        `MavenCoordinatesMacro`, `OutputMacro`, `QueryMacro`,
        `QueryOutputsMacro`, `QueryPathsMacro`,
        `QueryTargetsAndOutputsMacro`, `QueryTargetsMacro`,
        `WorkerMacro`

    ------------------------------------------------------------------------

        public interface Macro
        extends TargetTranslatable<Macro>

    ::: block
    Base class for strongly typed macros.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type           Method                                                                                                                                            Description
          --------------------------- ------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `Class<? extends Macro>`    `getMacroClass()`                                                                                                                                  
          `default Optional<Macro>`   `translateTargets​(CellNameResolver cellPathResolver,                 BaseName targetBaseName,                 TargetNodeTranslator translator)`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Abstract
          Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
          .tableTab}[[Default
          Methods](javascript:show(16);)[ ]{.tabEnd}]{#t5 .tableTab}
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getMacroClass()}

        -   #### getMacroClass

            ``` methodSignature
            Class<? extends Macro> getMacroClass()
            ```

        []{#translateTargets(com.facebook.buck.core.cell.nameresolver.CellNameResolver,com.facebook.buck.core.model.BaseName,com.facebook.buck.versions.TargetNodeTranslator)}

        -   #### translateTargets

            ``` methodSignature
            default Optional<Macro> translateTargets​(CellNameResolver cellPathResolver,
                                                     BaseName targetBaseName,
                                                     TargetNodeTranslator translator)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `translateTargets` in
                interface `TargetTranslatable<Macro>`

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
