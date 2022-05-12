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
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   [Constr](#constructor.detail) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.android.relinker](package-summary.html)
:::

## Class NativeRelinker {#class-nativerelinker .title title="Class NativeRelinker"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.android.relinker.NativeRelinker

::: description
-   

    ------------------------------------------------------------------------

        public class NativeRelinker
        extends Object

    ::: block
    When linking shared libraries, by default, all symbols are exported
    from the library. In a particular application, though, many of those
    symbols may never be used. Ideally, in each apk, each shared library
    would only export the minimal set of symbols that are used by other
    libraries in the apk. This would allow the linker to remove any dead
    code within the library (the linker can strip all code that is
    unreachable from the set of exported symbols).
    The native relinker tries to remedy the situation. When enabled for
    an apk, the native relinker will take the set of libraries in the
    apk and relink them in reverse order telling the linker to only
    export those symbols that are referenced by a higher library.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                Description
          ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `NativeRelinker​(BuildTarget buildTarget,               ProjectFilesystem projectFilesystem,               CellPathResolver cellPathResolver,               SourcePathResolverAdapter resolver,               SourcePathRuleFinder ruleFinder,               CxxBuckConfig cxxBuckConfig,               com.google.common.collect.ImmutableMap<TargetCpuType,​NdkCxxPlatform> nativePlatforms,               com.google.common.collect.ImmutableMap<AndroidLinkableMetadata,​SourcePath> linkableLibs,               com.google.common.collect.ImmutableMap<AndroidLinkableMetadata,​SourcePath> linkableLibsAssets,               com.google.common.collect.ImmutableList<Pattern> symbolPatternWhitelist)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                                            Method                      Description
          -------------------------------------------------------------------------------------------- --------------------------- -------------
          `com.google.common.collect.ImmutableMap<AndroidLinkableMetadata,​SourcePath>`                 `getRelinkedLibs()`          
          `com.google.common.collect.ImmutableMap<AndroidLinkableMetadata,​SourcePath>`                 `getRelinkedLibsAssets()`    
          `com.google.common.collect.ImmutableList<com.facebook.buck.android.relinker.RelinkerRule>`   `getRules()`                 

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.cell.CellPathResolver,com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter,com.facebook.buck.core.rules.SourcePathRuleFinder,com.facebook.buck.cxx.config.CxxBuckConfig,com.google.common.collect.ImmutableMap,com.google.common.collect.ImmutableMap,com.google.common.collect.ImmutableMap,com.google.common.collect.ImmutableList)}

        -   #### NativeRelinker

                public NativeRelinker​(BuildTarget buildTarget,
                                      ProjectFilesystem projectFilesystem,
                                      CellPathResolver cellPathResolver,
                                      SourcePathResolverAdapter resolver,
                                      SourcePathRuleFinder ruleFinder,
                                      CxxBuckConfig cxxBuckConfig,
                                      com.google.common.collect.ImmutableMap<TargetCpuType,​NdkCxxPlatform> nativePlatforms,
                                      com.google.common.collect.ImmutableMap<AndroidLinkableMetadata,​SourcePath> linkableLibs,
                                      com.google.common.collect.ImmutableMap<AndroidLinkableMetadata,​SourcePath> linkableLibsAssets,
                                      com.google.common.collect.ImmutableList<Pattern> symbolPatternWhitelist)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getRelinkedLibs()}

        -   #### getRelinkedLibs

            ``` methodSignature
            public com.google.common.collect.ImmutableMap<AndroidLinkableMetadata,​SourcePath> getRelinkedLibs()
            ```

        []{#getRelinkedLibsAssets()}

        -   #### getRelinkedLibsAssets

            ``` methodSignature
            public com.google.common.collect.ImmutableMap<AndroidLinkableMetadata,​SourcePath> getRelinkedLibsAssets()
            ```

        []{#getRules()}

        -   #### getRules

            ``` methodSignature
            public com.google.common.collect.ImmutableList<com.facebook.buck.android.relinker.RelinkerRule> getRules()
            ```
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
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   [Constr](#constructor.detail) \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
