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
[Package]{.packageLabelInType} [com.facebook.buck.cxx.toolchain](package-summary.html)
:::

## Interface SharedLibraryInterfaceFactory {#interface-sharedlibraryinterfacefactory .title title="Interface SharedLibraryInterfaceFactory"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `MachoDylibStubRuleFactory`

    ------------------------------------------------------------------------

        public interface SharedLibraryInterfaceFactory

    ::: block
    Factory class which produces a
    [`BuildRule`](../../core/rules/BuildRule.html "interface in com.facebook.buck.core.rules")
    that generates a shared library interface.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                                                                                                                                                                                                                                                                                                                                                                                                                                                    Description
          ------------------- --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `BuildRule`         `createSharedInterfaceLibraryFromLibrary​(BuildTarget target,                                        ProjectFilesystem projectFilesystem,                                        BuildRuleResolver resolver,                                        CxxPlatform cxxPlatform,                                        SourcePath library)`                                                                                                                    
          `BuildRule`         `createSharedInterfaceLibraryFromLinkableInput​(BuildTarget target,                                              ProjectFilesystem projectFilesystem,                                              BuildRuleResolver resolver,                                              String libName,                                              Linker linker,                                              com.google.common.collect.ImmutableList<Arg> args)`    

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

        []{#createSharedInterfaceLibraryFromLibrary(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.rules.BuildRuleResolver,com.facebook.buck.cxx.toolchain.CxxPlatform,com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### createSharedInterfaceLibraryFromLibrary

            ``` methodSignature
            BuildRule createSharedInterfaceLibraryFromLibrary​(BuildTarget target,
                                                              ProjectFilesystem projectFilesystem,
                                                              BuildRuleResolver resolver,
                                                              CxxPlatform cxxPlatform,
                                                              SourcePath library)
            ```

            [Returns:]{.returnLabel}
            :   a rule building a shared library interface from an
                existing shared library.

        []{#createSharedInterfaceLibraryFromLinkableInput(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.rules.BuildRuleResolver,java.lang.String,com.facebook.buck.cxx.toolchain.linker.Linker,com.google.common.collect.ImmutableList)}

        -   #### createSharedInterfaceLibraryFromLinkableInput

            ``` methodSignature
            BuildRule createSharedInterfaceLibraryFromLinkableInput​(BuildTarget target,
                                                                    ProjectFilesystem projectFilesystem,
                                                                    BuildRuleResolver resolver,
                                                                    String libName,
                                                                    Linker linker,
                                                                    com.google.common.collect.ImmutableList<Arg> args)
            ```

            [Returns:]{.returnLabel}
            :   a rule building a shared library interface from a shared
                link line
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
