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
[Package]{.packageLabelInType} [com.facebook.buck.features.filebundler](package-summary.html)
:::

## Class FileBundler {#class-filebundler .title title="Class FileBundler"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.features.filebundler.FileBundler

::: description
-   

    Direct Known Subclasses:
    :   `CopyingFileBundler`

    ------------------------------------------------------------------------

        public abstract class FileBundler
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                  Description
          ---------------------------------------------------------------------------- -------------
          `FileBundler​(ProjectFilesystem filesystem,            BuildTarget target)`    
          `FileBundler​(Path basePath)`                                                  

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type           Method                                                                                                                                                                                                                                                                                                             Description
          --------------------------- ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ -------------
          `protected abstract void`   `addCopySteps​(ProjectFilesystem filesystem,             BuildCellRelativePathFactory buildCellRelativePathFactory,             com.google.common.collect.ImmutableList.Builder<Step> steps,             Path relativePath,             Path absolutePath,             Path destination)`                            
          `void`                      `copy​(ProjectFilesystem filesystem,     BuildCellRelativePathFactory buildCellRelativePathFactory,     com.google.common.collect.ImmutableList.Builder<Step> steps,     Path destinationDir,     com.google.common.collect.ImmutableSortedSet<SourcePath> toCopy,     SourcePathResolverAdapter pathResolver)`      
          `void`                      `copy​(ProjectFilesystem filesystem,     BuildCellRelativePathFactory buildCellRelativePathFactory,     com.google.common.collect.ImmutableList.Builder<Step> steps,     Path destinationDir,     Iterable<SourcePath> toCopy,     SourcePathResolverAdapter pathResolver,     PatternsMatcher entriesToExclude)`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Abstract
          Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
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

        []{#<init>(com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.model.BuildTarget)}

        -   #### FileBundler

                public FileBundler​(ProjectFilesystem filesystem,
                                   BuildTarget target)

        []{#<init>(java.nio.file.Path)}

        -   #### FileBundler

                public FileBundler​(Path basePath)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#copy(com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.rules.modern.BuildCellRelativePathFactory,com.google.common.collect.ImmutableList.Builder,java.nio.file.Path,com.google.common.collect.ImmutableSortedSet,com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter)}

        -   #### copy

            ``` methodSignature
            public void copy​(ProjectFilesystem filesystem,
                             BuildCellRelativePathFactory buildCellRelativePathFactory,
                             com.google.common.collect.ImmutableList.Builder<Step> steps,
                             Path destinationDir,
                             com.google.common.collect.ImmutableSortedSet<SourcePath> toCopy,
                             SourcePathResolverAdapter pathResolver)
            ```

        []{#copy(com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.rules.modern.BuildCellRelativePathFactory,com.google.common.collect.ImmutableList.Builder,java.nio.file.Path,java.lang.Iterable,com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter,com.facebook.buck.util.PatternsMatcher)}

        -   #### copy

            ``` methodSignature
            public void copy​(ProjectFilesystem filesystem,
                             BuildCellRelativePathFactory buildCellRelativePathFactory,
                             com.google.common.collect.ImmutableList.Builder<Step> steps,
                             Path destinationDir,
                             Iterable<SourcePath> toCopy,
                             SourcePathResolverAdapter pathResolver,
                             PatternsMatcher entriesToExclude)
            ```

        []{#addCopySteps(com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.rules.modern.BuildCellRelativePathFactory,com.google.common.collect.ImmutableList.Builder,java.nio.file.Path,java.nio.file.Path,java.nio.file.Path)}

        -   #### addCopySteps

            ``` methodSignature
            protected abstract void addCopySteps​(ProjectFilesystem filesystem,
                                                 BuildCellRelativePathFactory buildCellRelativePathFactory,
                                                 com.google.common.collect.ImmutableList.Builder<Step> steps,
                                                 Path relativePath,
                                                 Path absolutePath,
                                                 Path destination)
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
