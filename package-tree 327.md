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
-   Tree
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

[]{#skip.navbar.top}
:::
:::

::: navPadding
 
:::
:::

::: {role="main"}
::: header
# Hierarchy For Package com.facebook.buck.rules.macros {#hierarchy-for-package-com.facebook.buck.rules.macros .title}

[Package Hierarchies:]{.packageHierarchyLabel}

-   [All Packages](../../../../../overview-tree.html)
:::

::: contentContainer
::: {.section role="region"}
## Class Hierarchy {#class-hierarchy title="Class Hierarchy"}

-   java.lang.[[Object]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}
    -   com.facebook.buck.rules.macros.[[AbsoluteOutputMacro]{.typeNameLink}](AbsoluteOutputMacro.html "class in com.facebook.buck.rules.macros")
        (implements
        com.facebook.buck.rules.macros.[Macro](Macro.html "interface in com.facebook.buck.rules.macros"))
    -   com.facebook.buck.rules.macros.[[AbstractMacroExpanderWithoutPrecomputedWork]{.typeNameLink}](AbstractMacroExpanderWithoutPrecomputedWork.html "class in com.facebook.buck.rules.macros")\<T\>
        (implements
        com.facebook.buck.rules.macros.[MacroExpander](MacroExpander.html "interface in com.facebook.buck.rules.macros")\<T,​P\>)
        -   com.facebook.buck.rules.macros.[[AbsoluteOutputMacroExpander]{.typeNameLink}](AbsoluteOutputMacroExpander.html "class in com.facebook.buck.rules.macros")
        -   com.facebook.buck.rules.macros.[[BuildTargetMacroExpander]{.typeNameLink}](BuildTargetMacroExpander.html "class in com.facebook.buck.rules.macros")\<M\>
            -   com.facebook.buck.rules.macros.[[AbstractLocationMacroExpander]{.typeNameLink}](AbstractLocationMacroExpander.html "class in com.facebook.buck.rules.macros")\<T\>
                -   com.facebook.buck.rules.macros.[[LocationMacroExpander]{.typeNameLink}](LocationMacroExpander.html "class in com.facebook.buck.rules.macros")
                -   com.facebook.buck.rules.macros.[[LocationPlatformMacroExpander]{.typeNameLink}](LocationPlatformMacroExpander.html "class in com.facebook.buck.rules.macros")
            -   com.facebook.buck.rules.macros.[[ClasspathAbiMacroExpander]{.typeNameLink}](ClasspathAbiMacroExpander.html "class in com.facebook.buck.rules.macros")
            -   com.facebook.buck.rules.macros.[[ClasspathMacroExpander]{.typeNameLink}](ClasspathMacroExpander.html "class in com.facebook.buck.rules.macros")
            -   com.facebook.buck.rules.macros.[[ExecutableMacroExpander]{.typeNameLink}](ExecutableMacroExpander.html "class in com.facebook.buck.rules.macros")\<M\>
            -   com.facebook.buck.rules.macros.[[MavenCoordinatesMacroExpander]{.typeNameLink}](MavenCoordinatesMacroExpander.html "class in com.facebook.buck.rules.macros")
            -   com.facebook.buck.rules.macros.[[WorkerMacroExpander]{.typeNameLink}](WorkerMacroExpander.html "class in com.facebook.buck.rules.macros")
        -   com.facebook.buck.rules.macros.[[EnvironmentVariableMacroExpander]{.typeNameLink}](EnvironmentVariableMacroExpander.html "class in com.facebook.buck.rules.macros")
        -   com.facebook.buck.rules.macros.[[OutputMacroExpander]{.typeNameLink}](OutputMacroExpander.html "class in com.facebook.buck.rules.macros")
        -   com.facebook.buck.rules.macros.[[SimpleMacroExpander]{.typeNameLink}](SimpleMacroExpander.html "class in com.facebook.buck.rules.macros")\<M\>
            -   com.facebook.buck.rules.macros.[[ArgExpander]{.typeNameLink}](ArgExpander.html "class in com.facebook.buck.rules.macros")\<M\>
            -   com.facebook.buck.rules.macros.[[StringExpander]{.typeNameLink}](StringExpander.html "class in com.facebook.buck.rules.macros")\<M\>
    -   com.facebook.buck.rules.macros.[[BuildTargetMacro]{.typeNameLink}](BuildTargetMacro.html "class in com.facebook.buck.rules.macros")
        (implements
        com.facebook.buck.rules.macros.[Macro](Macro.html "interface in com.facebook.buck.rules.macros"))
        -   com.facebook.buck.rules.macros.[[AbstractExecutableTargetOrHostMacro]{.typeNameLink}](AbstractExecutableTargetOrHostMacro.html "class in com.facebook.buck.rules.macros")
            -   com.facebook.buck.rules.macros.[[ExecutableMacro]{.typeNameLink}](ExecutableMacro.html "class in com.facebook.buck.rules.macros")
            -   com.facebook.buck.rules.macros.[[ExecutableTargetMacro]{.typeNameLink}](ExecutableTargetMacro.html "class in com.facebook.buck.rules.macros")
        -   com.facebook.buck.rules.macros.[[BaseLocationMacro]{.typeNameLink}](BaseLocationMacro.html "class in com.facebook.buck.rules.macros")
            -   com.facebook.buck.rules.macros.[[LocationMacro]{.typeNameLink}](LocationMacro.html "class in com.facebook.buck.rules.macros")
            -   com.facebook.buck.rules.macros.[[LocationPlatformMacro]{.typeNameLink}](LocationPlatformMacro.html "class in com.facebook.buck.rules.macros")
        -   com.facebook.buck.rules.macros.[[ClasspathAbiMacro]{.typeNameLink}](ClasspathAbiMacro.html "class in com.facebook.buck.rules.macros")
        -   com.facebook.buck.rules.macros.[[ClasspathMacro]{.typeNameLink}](ClasspathMacro.html "class in com.facebook.buck.rules.macros")
        -   com.facebook.buck.rules.macros.[[MavenCoordinatesMacro]{.typeNameLink}](MavenCoordinatesMacro.html "class in com.facebook.buck.rules.macros")
        -   com.facebook.buck.rules.macros.[[WorkerMacro]{.typeNameLink}](WorkerMacro.html "class in com.facebook.buck.rules.macros")
    -   com.facebook.buck.rules.macros.[[CxxGenruleFilterAndTargetsMacro]{.typeNameLink}](CxxGenruleFilterAndTargetsMacro.html "class in com.facebook.buck.rules.macros")
        (implements
        com.facebook.buck.rules.macros.[Macro](Macro.html "interface in com.facebook.buck.rules.macros"))
        -   com.facebook.buck.rules.macros.[[CppFlagsMacro]{.typeNameLink}](CppFlagsMacro.html "class in com.facebook.buck.rules.macros")
        -   com.facebook.buck.rules.macros.[[CxxppFlagsMacro]{.typeNameLink}](CxxppFlagsMacro.html "class in com.facebook.buck.rules.macros")
        -   com.facebook.buck.rules.macros.[[LdflagsSharedFilterMacro]{.typeNameLink}](LdflagsSharedFilterMacro.html "class in com.facebook.buck.rules.macros")
        -   com.facebook.buck.rules.macros.[[LdflagsSharedMacro]{.typeNameLink}](LdflagsSharedMacro.html "class in com.facebook.buck.rules.macros")
        -   com.facebook.buck.rules.macros.[[LdflagsStaticFilterMacro]{.typeNameLink}](LdflagsStaticFilterMacro.html "class in com.facebook.buck.rules.macros")
        -   com.facebook.buck.rules.macros.[[LdflagsStaticMacro]{.typeNameLink}](LdflagsStaticMacro.html "class in com.facebook.buck.rules.macros")
        -   com.facebook.buck.rules.macros.[[LdflagsStaticPicFilterMacro]{.typeNameLink}](LdflagsStaticPicFilterMacro.html "class in com.facebook.buck.rules.macros")
        -   com.facebook.buck.rules.macros.[[LdflagsStaticPicMacro]{.typeNameLink}](LdflagsStaticPicMacro.html "class in com.facebook.buck.rules.macros")
    -   com.facebook.buck.rules.macros.[[FunctionMacroReplacer]{.typeNameLink}](FunctionMacroReplacer.html "class in com.facebook.buck.rules.macros")\<T\>
        (implements
        com.facebook.buck.core.macros.[MacroReplacer](../../core/macros/MacroReplacer.html "interface in com.facebook.buck.core.macros")\<T\>)
    -   com.facebook.buck.rules.macros.ImmutableMacroContainer.Builder
        -   com.facebook.buck.rules.macros.[[MacroContainer.Builder]{.typeNameLink}](MacroContainer.Builder.html "class in com.facebook.buck.rules.macros")
    -   com.facebook.buck.rules.macros.[[LdMacro]{.typeNameLink}](LdMacro.html "class in com.facebook.buck.rules.macros")
        (implements
        com.facebook.buck.rules.macros.[Macro](Macro.html "interface in com.facebook.buck.rules.macros"))
    -   com.facebook.buck.rules.macros.[[MacroContainer]{.typeNameLink}](MacroContainer.html "class in com.facebook.buck.rules.macros")
    -   com.facebook.buck.rules.macros.[[OutputMacro]{.typeNameLink}](OutputMacro.html "class in com.facebook.buck.rules.macros")
        (implements
        com.facebook.buck.rules.macros.[Macro](Macro.html "interface in com.facebook.buck.rules.macros"))
    -   com.facebook.buck.rules.args.[[ProxyArg]{.typeNameLink}](../args/ProxyArg.html "class in com.facebook.buck.rules.args")
        (implements
        com.facebook.buck.rules.args.[Arg](../args/Arg.html "interface in com.facebook.buck.rules.args"))
        -   com.facebook.buck.rules.macros.[[WorkerMacroArg]{.typeNameLink}](WorkerMacroArg.html "class in com.facebook.buck.rules.macros")
    -   com.facebook.buck.rules.macros.[[QueryMacro]{.typeNameLink}](QueryMacro.html "class in com.facebook.buck.rules.macros")
        (implements
        com.facebook.buck.rules.macros.[Macro](Macro.html "interface in com.facebook.buck.rules.macros"))
        -   com.facebook.buck.rules.macros.[[QueryOutputsMacro]{.typeNameLink}](QueryOutputsMacro.html "class in com.facebook.buck.rules.macros")
        -   com.facebook.buck.rules.macros.[[QueryPathsMacro]{.typeNameLink}](QueryPathsMacro.html "class in com.facebook.buck.rules.macros")
        -   com.facebook.buck.rules.macros.[[QueryTargetsAndOutputsMacro]{.typeNameLink}](QueryTargetsAndOutputsMacro.html "class in com.facebook.buck.rules.macros")
        -   com.facebook.buck.rules.macros.[[QueryTargetsMacro]{.typeNameLink}](QueryTargetsMacro.html "class in com.facebook.buck.rules.macros")
    -   com.facebook.buck.rules.macros.[[QueryMacroExpander]{.typeNameLink}](QueryMacroExpander.html "class in com.facebook.buck.rules.macros")\<T\>
        (implements
        com.facebook.buck.rules.macros.[MacroExpander](MacroExpander.html "interface in com.facebook.buck.rules.macros")\<T,​P\>)
        -   com.facebook.buck.rules.macros.[[QueryOutputsMacroExpander]{.typeNameLink}](QueryOutputsMacroExpander.html "class in com.facebook.buck.rules.macros")
        -   com.facebook.buck.rules.macros.[[QueryPathsMacroExpander]{.typeNameLink}](QueryPathsMacroExpander.html "class in com.facebook.buck.rules.macros")
        -   com.facebook.buck.rules.macros.[[QueryTargetsAndOutputsMacroExpander]{.typeNameLink}](QueryTargetsAndOutputsMacroExpander.html "class in com.facebook.buck.rules.macros")
        -   com.facebook.buck.rules.macros.[[QueryTargetsMacroExpander]{.typeNameLink}](QueryTargetsMacroExpander.html "class in com.facebook.buck.rules.macros")
    -   com.facebook.buck.rules.macros.[[QueryMacroExpander.QueryResults]{.typeNameLink}](QueryMacroExpander.QueryResults.html "class in com.facebook.buck.rules.macros")
    -   com.facebook.buck.rules.macros.[[StringWithMacros]{.typeNameLink}](StringWithMacros.html "class in com.facebook.buck.rules.macros")
        (implements
        com.facebook.buck.util.string.[StringMatcher](../../util/string/StringMatcher.html "interface in com.facebook.buck.util.string"),
        com.facebook.buck.versions.[TargetTranslatable](../../versions/TargetTranslatable.html "interface in com.facebook.buck.versions")\<T\>)
    -   com.facebook.buck.rules.macros.[[StringWithMacrosConverter]{.typeNameLink}](StringWithMacrosConverter.html "class in com.facebook.buck.rules.macros")
:::

::: {.section role="region"}
## Interface Hierarchy {#interface-hierarchy title="Interface Hierarchy"}

-   com.facebook.buck.rules.macros.[[MacroExpander]{.typeNameLink}](MacroExpander.html "interface in com.facebook.buck.rules.macros")\<T,​P\>
-   com.facebook.buck.versions.[[TargetTranslatable]{.typeNameLink}](../../versions/TargetTranslatable.html "interface in com.facebook.buck.versions")\<T\>
    -   com.facebook.buck.rules.macros.[[Macro]{.typeNameLink}](Macro.html "interface in com.facebook.buck.rules.macros")
        -   com.facebook.buck.rules.macros.[[CcFlagsMacro]{.typeNameLink}](CcFlagsMacro.html "interface in com.facebook.buck.rules.macros")
        -   com.facebook.buck.rules.macros.[[CcMacro]{.typeNameLink}](CcMacro.html "interface in com.facebook.buck.rules.macros")
        -   com.facebook.buck.rules.macros.[[CxxFlagsMacro]{.typeNameLink}](CxxFlagsMacro.html "interface in com.facebook.buck.rules.macros")
        -   com.facebook.buck.rules.macros.[[CxxMacro]{.typeNameLink}](CxxMacro.html "interface in com.facebook.buck.rules.macros")
        -   com.facebook.buck.rules.macros.[[EnvMacro]{.typeNameLink}](EnvMacro.html "interface in com.facebook.buck.rules.macros")
        -   com.facebook.buck.rules.macros.[[PlatformNameMacro]{.typeNameLink}](PlatformNameMacro.html "interface in com.facebook.buck.rules.macros")
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
-   Tree
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

[]{#skip.navbar.bottom}
:::
