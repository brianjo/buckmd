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
[Package]{.packageLabelInType} [com.facebook.buck.features.ocaml](package-summary.html)
:::

## Class OcamlBuildRulesGenerator {#class-ocamlbuildrulesgenerator .title title="Class OcamlBuildRulesGenerator"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.features.ocaml.OcamlBuildRulesGenerator

::: description
-   

    ------------------------------------------------------------------------

        public class OcamlBuildRulesGenerator
        extends Object

    ::: block
    A generator of fine-grained OCaml build rules
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 Description
          --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `OcamlBuildRulesGenerator​(BuildTarget buildTarget,                         ProjectFilesystem projectFilesystem,                         BuildRuleParams params,                         ActionGraphBuilder graphBuilder,                         com.facebook.buck.features.ocaml.OcamlBuildContext ocamlContext,                         com.google.common.collect.ImmutableMap<Path,​com.google.common.collect.ImmutableList<Path>> mlInput,                         com.google.common.collect.ImmutableList<SourcePath> cInput,                         Compiler cCompiler,                         Linker cxxLinker,                         boolean bytecodeOnly,                         boolean buildNativePlugin)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type      Method                                                                                                    Description
          ---------------------- --------------------------------------------------------------------------------------------------------- -------------
          `static BuildTarget`   `addBytecodeFlavor​(BuildTarget target)`                                                                    
          `static BuildTarget`   `addDebugFlavor​(BuildTarget target)`                                                                       
          `static BuildTarget`   `createCCompileBuildTarget​(BuildTarget target,                          String name)`                      
          `static BuildTarget`   `createMLBytecodeCompileBuildTarget​(BuildTarget target,                                   String name)`    
          `static BuildTarget`   `createMLNativeCompileBuildTarget​(BuildTarget target,                                 String name)`        

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
          Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
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

        []{#<init>(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.rules.BuildRuleParams,com.facebook.buck.core.rules.ActionGraphBuilder,com.facebook.buck.features.ocaml.OcamlBuildContext,com.google.common.collect.ImmutableMap,com.google.common.collect.ImmutableList,com.facebook.buck.cxx.toolchain.Compiler,com.facebook.buck.cxx.toolchain.linker.Linker,boolean,boolean)}

        -   #### OcamlBuildRulesGenerator

                public OcamlBuildRulesGenerator​(BuildTarget buildTarget,
                                                ProjectFilesystem projectFilesystem,
                                                BuildRuleParams params,
                                                ActionGraphBuilder graphBuilder,
                                                com.facebook.buck.features.ocaml.OcamlBuildContext ocamlContext,
                                                com.google.common.collect.ImmutableMap<Path,​com.google.common.collect.ImmutableList<Path>> mlInput,
                                                com.google.common.collect.ImmutableList<SourcePath> cInput,
                                                Compiler cCompiler,
                                                Linker cxxLinker,
                                                boolean bytecodeOnly,
                                                boolean buildNativePlugin)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#createCCompileBuildTarget(com.facebook.buck.core.model.BuildTarget,java.lang.String)}

        -   #### createCCompileBuildTarget

            ``` methodSignature
            public static BuildTarget createCCompileBuildTarget​(BuildTarget target,
                                                                String name)
            ```

        []{#addDebugFlavor(com.facebook.buck.core.model.BuildTarget)}

        -   #### addDebugFlavor

            ``` methodSignature
            public static BuildTarget addDebugFlavor​(BuildTarget target)
            ```

        []{#addBytecodeFlavor(com.facebook.buck.core.model.BuildTarget)}

        -   #### addBytecodeFlavor

            ``` methodSignature
            public static BuildTarget addBytecodeFlavor​(BuildTarget target)
            ```

        []{#createMLNativeCompileBuildTarget(com.facebook.buck.core.model.BuildTarget,java.lang.String)}

        -   #### createMLNativeCompileBuildTarget

            ``` methodSignature
            public static BuildTarget createMLNativeCompileBuildTarget​(BuildTarget target,
                                                                       String name)
            ```

        []{#createMLBytecodeCompileBuildTarget(com.facebook.buck.core.model.BuildTarget,java.lang.String)}

        -   #### createMLBytecodeCompileBuildTarget

            ``` methodSignature
            public static BuildTarget createMLBytecodeCompileBuildTarget​(BuildTarget target,
                                                                         String name)
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
