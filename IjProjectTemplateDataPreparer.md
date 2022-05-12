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

-   [Overview](../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../deprecated-list.html)
-   [Index](../../../../../../index-all.html)
-   [Help](../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.features.project.intellij](package-summary.html)
:::

## Class IjProjectTemplateDataPreparer {#class-ijprojecttemplatedatapreparer .title title="Class IjProjectTemplateDataPreparer"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.features.project.intellij.IjProjectTemplateDataPreparer

::: description
-   

    ------------------------------------------------------------------------

        public class IjProjectTemplateDataPreparer
        extends Object

    ::: block
    Does the converting of abstract data structures to a format
    immediately consumable by the StringTemplate-based templates
    employed by
    [`IjProjectWriter`](IjProjectWriter.html "class in com.facebook.buck.features.project.intellij").
    This is a separate class mainly for testing convenience.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                                                                            Description
          -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `IjProjectTemplateDataPreparer​(JavaPackageFinder javaPackageFinder,                              IjModuleGraph moduleGraph,                              ProjectFilesystem projectFilesystem,                              IjProjectConfig projectConfig,                              AndroidManifestParser androidManifestParser)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                                   Method                                                                                                 Description
          ----------------------------------------------------------------------------------- ------------------------------------------------------------------------------------------------------ -------------
          `com.google.common.collect.ImmutableCollection<IjFolder>`                           `createExcludes​(IjModule module)`                                                                       
          `com.google.common.collect.ImmutableSet<Path>`                                      `createFilesystemTraversalBoundaryPathSet​(com.google.common.collect.ImmutableSet<IjModule> modules)`    
          `static com.google.common.collect.ImmutableSet<Path>`                               `createPackageLookupPathSet​(IjModuleGraph moduleGraph)`                                                 
          `static com.google.common.collect.ImmutableSet<Path>`                               `createReferencedFolderPathsSet​(com.google.common.collect.ImmutableSet<IjModule> modules)`              
          `Map<String,​Object>`                                                                `getAndroidProperties​(IjModule module)`                                                                 
          `com.google.common.collect.ImmutableList<ContentRoot>`                              `getContentRoots​(IjModule module)`                                                                      
          `com.google.common.collect.ImmutableSet<IjDependencyListBuilder.DependencyEntry>`   `getDependencies​(IjModule module)`                                                                      
          `Optional<String>`                                                                  `getFirstResourcePackageFromDependencies​(IjModule module)`                                              
          `com.google.common.collect.ImmutableSet<IjSourceFolder>`                            `getGeneratedSourceFolders​(IjModule module)`                                                            
          `com.google.common.collect.ImmutableSet<IjLibrary>`                                 `getLibrariesToBeWritten()`                                                                             
          `com.google.common.collect.ImmutableSortedSet<ModuleIndexEntry>`                    `getModuleIndexEntries()`                                                                               
          `com.google.common.collect.ImmutableSet<IjModule>`                                  `getModulesToBeWritten()`                                                                               

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
          Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
          .tableTab}[[Instance
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

        []{#<init>(com.facebook.buck.jvm.core.JavaPackageFinder,com.facebook.buck.features.project.intellij.IjModuleGraph,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.features.project.intellij.model.IjProjectConfig,com.facebook.buck.features.project.intellij.lang.android.AndroidManifestParser)}

        -   #### IjProjectTemplateDataPreparer

                public IjProjectTemplateDataPreparer​(JavaPackageFinder javaPackageFinder,
                                                     IjModuleGraph moduleGraph,
                                                     ProjectFilesystem projectFilesystem,
                                                     IjProjectConfig projectConfig,
                                                     AndroidManifestParser androidManifestParser)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#createReferencedFolderPathsSet(com.google.common.collect.ImmutableSet)}

        -   #### createReferencedFolderPathsSet

            ``` methodSignature
            public static com.google.common.collect.ImmutableSet<Path> createReferencedFolderPathsSet​(com.google.common.collect.ImmutableSet<IjModule> modules)
            ```

        []{#createFilesystemTraversalBoundaryPathSet(com.google.common.collect.ImmutableSet)}

        -   #### createFilesystemTraversalBoundaryPathSet

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<Path> createFilesystemTraversalBoundaryPathSet​(com.google.common.collect.ImmutableSet<IjModule> modules)
            ```

        []{#createPackageLookupPathSet(com.facebook.buck.features.project.intellij.IjModuleGraph)}

        -   #### createPackageLookupPathSet

            ``` methodSignature
            public static com.google.common.collect.ImmutableSet<Path> createPackageLookupPathSet​(IjModuleGraph moduleGraph)
            ```

        []{#getModulesToBeWritten()}

        -   #### getModulesToBeWritten

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<IjModule> getModulesToBeWritten()
            ```

        []{#getLibrariesToBeWritten()}

        -   #### getLibrariesToBeWritten

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<IjLibrary> getLibrariesToBeWritten()
            ```

        []{#createExcludes(com.facebook.buck.features.project.intellij.model.IjModule)}

        -   #### createExcludes

            ``` methodSignature
            public com.google.common.collect.ImmutableCollection<IjFolder> createExcludes​(IjModule module)
                                                                                   throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#getContentRoots(com.facebook.buck.features.project.intellij.model.IjModule)}

        -   #### getContentRoots

            ``` methodSignature
            public com.google.common.collect.ImmutableList<ContentRoot> getContentRoots​(IjModule module)
                                                                                 throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#getGeneratedSourceFolders(com.facebook.buck.features.project.intellij.model.IjModule)}

        -   #### getGeneratedSourceFolders

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<IjSourceFolder> getGeneratedSourceFolders​(IjModule module)
            ```

        []{#getDependencies(com.facebook.buck.features.project.intellij.model.IjModule)}

        -   #### getDependencies

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<IjDependencyListBuilder.DependencyEntry> getDependencies​(IjModule module)
            ```

        []{#getFirstResourcePackageFromDependencies(com.facebook.buck.features.project.intellij.model.IjModule)}

        -   #### getFirstResourcePackageFromDependencies

            ``` methodSignature
            public Optional<String> getFirstResourcePackageFromDependencies​(IjModule module)
            ```

        []{#getModuleIndexEntries()}

        -   #### getModuleIndexEntries

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedSet<ModuleIndexEntry> getModuleIndexEntries()
            ```

        []{#getAndroidProperties(com.facebook.buck.features.project.intellij.model.IjModule)}

        -   #### getAndroidProperties

            ``` methodSignature
            public Map<String,​Object> getAndroidProperties​(IjModule module)
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

-   [Overview](../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../deprecated-list.html)
-   [Index](../../../../../../index-all.html)
-   [Help](../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../allclasses.html)

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
