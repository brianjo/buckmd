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
[Package]{.packageLabelInType} [com.facebook.buck.features.python](package-summary.html)
:::

## Class PythonUtil {#class-pythonutil .title title="Class PythonUtil"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.features.python.PythonUtil

::: description
-   

    ------------------------------------------------------------------------

        public class PythonUtil
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                        Method                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         Description
          ------------------------------------------------------------------------ ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `static void`                                                            `forEachModule​(BuildTarget target,              ActionGraphBuilder graphBuilder,              PythonPlatform pythonPlatform,              CxxPlatform cxxPlatform,              String parameter,              Path baseModule,              SourceSortedSet items,              PatternMatchedCollection<SourceSortedSet> platformItems,              Optional<VersionMatchedCollection<SourceSortedSet>> versionItems,              Optional<com.google.common.collect.ImmutableMap<BuildTarget,​Version>> versions,              java.util.function.BiConsumer<Path,​SourcePath> consumer)`    
          `static void`                                                            `forEachSrc​(BuildTarget target,           ActionGraphBuilder graphBuilder,           PythonPlatform pythonPlatform,           CxxPlatform cxxPlatform,           Optional<com.google.common.collect.ImmutableMap<BuildTarget,​Version>> versions,           com.facebook.buck.features.python.PythonLibraryDescription.CoreArg args,           java.util.function.BiConsumer<Path,​SourcePath> consumer)`                                                                                                                                                                                         
          `static Path`                                                            `getBasePath​(BuildTarget target,            Optional<String> override)`                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         
          `static com.google.common.collect.ImmutableList<BuildTarget>`            `getDeps​(PythonPlatform pythonPlatform,        CxxPlatform cxxPlatform,        com.google.common.collect.ImmutableSortedSet<BuildTarget> deps,        PatternMatchedCollection<com.google.common.collect.ImmutableSortedSet<BuildTarget>> platformDeps)`                                                                                                                                                                                                                                                                                                                                        
          `static boolean`                                                         `isModuleExt​(String ext)`                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       
          `static com.google.common.collect.ImmutableSortedMap<Path,​SourcePath>`   `parseModules​(BuildTarget target,             ActionGraphBuilder graphBuilder,             PythonPlatform pythonPlatform,             CxxPlatform cxxPlatform,             Optional<com.google.common.collect.ImmutableMap<BuildTarget,​Version>> versions,             com.facebook.buck.features.python.PythonLibraryDescription.CoreArg args)`                                                                                                                                                                                                                                                
          `static com.google.common.collect.ImmutableSortedMap<Path,​SourcePath>`   `parseResources​(BuildTarget target,               ActionGraphBuilder graphBuilder,               PythonPlatform pythonPlatform,               CxxPlatform cxxPlatform,               Optional<com.google.common.collect.ImmutableMap<BuildTarget,​Version>> versions,               com.facebook.buck.features.python.PythonLibraryDescription.CoreArg args)`                                                                                                                                                                                                                                    
          `static com.google.common.collect.ImmutableSortedMap<Path,​SourcePath>`   `parseSources​(BuildTarget target,             ActionGraphBuilder graphBuilder,             PythonPlatform pythonPlatform,             CxxPlatform cxxPlatform,             Optional<com.google.common.collect.ImmutableMap<BuildTarget,​Version>> versions,             com.facebook.buck.features.python.PythonLibraryDescription.CoreArg args)`                                                                                                                                                                                                                                                

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
    -   []{#method.detail}

        ### Method Detail

        []{#isModuleExt(java.lang.String)}

        -   #### isModuleExt

            ``` methodSignature
            public static boolean isModuleExt​(String ext)
            ```

        []{#getDeps(com.facebook.buck.features.python.toolchain.PythonPlatform,com.facebook.buck.cxx.toolchain.CxxPlatform,com.google.common.collect.ImmutableSortedSet,com.facebook.buck.rules.coercer.PatternMatchedCollection)}

        -   #### getDeps

            ``` methodSignature
            public static com.google.common.collect.ImmutableList<BuildTarget> getDeps​(PythonPlatform pythonPlatform,
                                                                                       CxxPlatform cxxPlatform,
                                                                                       com.google.common.collect.ImmutableSortedSet<BuildTarget> deps,
                                                                                       PatternMatchedCollection<com.google.common.collect.ImmutableSortedSet<BuildTarget>> platformDeps)
            ```

        []{#forEachModule(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.rules.ActionGraphBuilder,com.facebook.buck.features.python.toolchain.PythonPlatform,com.facebook.buck.cxx.toolchain.CxxPlatform,java.lang.String,java.nio.file.Path,com.facebook.buck.rules.coercer.SourceSortedSet,com.facebook.buck.rules.coercer.PatternMatchedCollection,java.util.Optional,java.util.Optional,java.util.function.BiConsumer)}

        -   #### forEachModule

            ``` methodSignature
            public static void forEachModule​(BuildTarget target,
                                             ActionGraphBuilder graphBuilder,
                                             PythonPlatform pythonPlatform,
                                             CxxPlatform cxxPlatform,
                                             String parameter,
                                             Path baseModule,
                                             SourceSortedSet items,
                                             PatternMatchedCollection<SourceSortedSet> platformItems,
                                             Optional<VersionMatchedCollection<SourceSortedSet>> versionItems,
                                             Optional<com.google.common.collect.ImmutableMap<BuildTarget,​Version>> versions,
                                             java.util.function.BiConsumer<Path,​SourcePath> consumer)
            ```

        []{#forEachSrc(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.rules.ActionGraphBuilder,com.facebook.buck.features.python.toolchain.PythonPlatform,com.facebook.buck.cxx.toolchain.CxxPlatform,java.util.Optional,com.facebook.buck.features.python.PythonLibraryDescription.CoreArg,java.util.function.BiConsumer)}

        -   #### forEachSrc

            ``` methodSignature
            public static void forEachSrc​(BuildTarget target,
                                          ActionGraphBuilder graphBuilder,
                                          PythonPlatform pythonPlatform,
                                          CxxPlatform cxxPlatform,
                                          Optional<com.google.common.collect.ImmutableMap<BuildTarget,​Version>> versions,
                                          com.facebook.buck.features.python.PythonLibraryDescription.CoreArg args,
                                          java.util.function.BiConsumer<Path,​SourcePath> consumer)
            ```

        []{#parseSources(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.rules.ActionGraphBuilder,com.facebook.buck.features.python.toolchain.PythonPlatform,com.facebook.buck.cxx.toolchain.CxxPlatform,java.util.Optional,com.facebook.buck.features.python.PythonLibraryDescription.CoreArg)}

        -   #### parseSources

            ``` methodSignature
            public static com.google.common.collect.ImmutableSortedMap<Path,​SourcePath> parseSources​(BuildTarget target,
                                                                                                           ActionGraphBuilder graphBuilder,
                                                                                                           PythonPlatform pythonPlatform,
                                                                                                           CxxPlatform cxxPlatform,
                                                                                                           Optional<com.google.common.collect.ImmutableMap<BuildTarget,​Version>> versions,
                                                                                                           com.facebook.buck.features.python.PythonLibraryDescription.CoreArg args)
            ```

        []{#parseModules(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.rules.ActionGraphBuilder,com.facebook.buck.features.python.toolchain.PythonPlatform,com.facebook.buck.cxx.toolchain.CxxPlatform,java.util.Optional,com.facebook.buck.features.python.PythonLibraryDescription.CoreArg)}

        -   #### parseModules

            ``` methodSignature
            public static com.google.common.collect.ImmutableSortedMap<Path,​SourcePath> parseModules​(BuildTarget target,
                                                                                                           ActionGraphBuilder graphBuilder,
                                                                                                           PythonPlatform pythonPlatform,
                                                                                                           CxxPlatform cxxPlatform,
                                                                                                           Optional<com.google.common.collect.ImmutableMap<BuildTarget,​Version>> versions,
                                                                                                           com.facebook.buck.features.python.PythonLibraryDescription.CoreArg args)
            ```

        []{#parseResources(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.rules.ActionGraphBuilder,com.facebook.buck.features.python.toolchain.PythonPlatform,com.facebook.buck.cxx.toolchain.CxxPlatform,java.util.Optional,com.facebook.buck.features.python.PythonLibraryDescription.CoreArg)}

        -   #### parseResources

            ``` methodSignature
            public static com.google.common.collect.ImmutableSortedMap<Path,​SourcePath> parseResources​(BuildTarget target,
                                                                                                             ActionGraphBuilder graphBuilder,
                                                                                                             PythonPlatform pythonPlatform,
                                                                                                             CxxPlatform cxxPlatform,
                                                                                                             Optional<com.google.common.collect.ImmutableMap<BuildTarget,​Version>> versions,
                                                                                                             com.facebook.buck.features.python.PythonLibraryDescription.CoreArg args)
            ```

        []{#getBasePath(com.facebook.buck.core.model.BuildTarget,java.util.Optional)}

        -   #### getBasePath

            ``` methodSignature
            public static Path getBasePath​(BuildTarget target,
                                           Optional<String> override)
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
