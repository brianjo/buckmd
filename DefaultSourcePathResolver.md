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
[Package]{.packageLabelInType} [com.facebook.buck.core.sourcepath.resolver.impl](package-summary.html)
:::

## Class DefaultSourcePathResolver {#class-defaultsourcepathresolver .title title="Class DefaultSourcePathResolver"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.core.sourcepath.resolver.impl.AbstractSourcePathResolver](AbstractSourcePathResolver.html "class in com.facebook.buck.core.sourcepath.resolver.impl")

    -   -   com.facebook.buck.core.sourcepath.resolver.impl.DefaultSourcePathResolver

::: description
-   

    All Implemented Interfaces:
    :   `SourcePathResolver`

    ------------------------------------------------------------------------

        public class DefaultSourcePathResolver
        extends AbstractSourcePathResolver
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                      Method                                                                                 Description
          ---------------------------------------------------------------------- -------------------------------------------------------------------------------------- -------------
          `static DefaultSourcePathResolver`                                     `from​(SourcePathRuleFinder ruleFinder)`                                                 
          `protected ProjectFilesystem`                                          `getBuildTargetSourcePathFilesystem​(BuildTargetSourcePath sourcePath)`                  
          `String`                                                               `getSourcePathName​(BuildTarget target,                  SourcePath sourcePath)`         
          `protected com.google.common.collect.ImmutableSortedSet<SourcePath>`   `resolveDefaultBuildTargetSourcePath​(DefaultBuildTargetSourcePath targetSourcePath)`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
          Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
          .tableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.core.sourcepath.resolver.impl.AbstractSourcePathResolver}

            ### Methods inherited from class com.facebook.buck.core.sourcepath.resolver.impl.[AbstractSourcePathResolver](AbstractSourcePathResolver.html "class in com.facebook.buck.core.sourcepath.resolver.impl")

            `createRelativeMap, filterInputsToCompareToOutput, getAbsolutePath, getAllAbsolutePaths, getFilesystem, getIdeallyRelativePath, getMappedPaths, getRelativePath, getRelativePath, getSourcePathNames, getSourcePathNames`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#from(com.facebook.buck.core.rules.SourcePathRuleFinder)}

        -   #### from

            ``` methodSignature
            public static DefaultSourcePathResolver from​(SourcePathRuleFinder ruleFinder)
            ```

        []{#getBuildTargetSourcePathFilesystem(com.facebook.buck.core.sourcepath.BuildTargetSourcePath)}

        -   #### getBuildTargetSourcePathFilesystem

            ``` methodSignature
            protected ProjectFilesystem getBuildTargetSourcePathFilesystem​(BuildTargetSourcePath sourcePath)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getBuildTargetSourcePathFilesystem` in
                class `AbstractSourcePathResolver`

        []{#resolveDefaultBuildTargetSourcePath(com.facebook.buck.core.sourcepath.DefaultBuildTargetSourcePath)}

        -   #### resolveDefaultBuildTargetSourcePath

            ``` methodSignature
            protected com.google.common.collect.ImmutableSortedSet<SourcePath> resolveDefaultBuildTargetSourcePath​(DefaultBuildTargetSourcePath targetSourcePath)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `resolveDefaultBuildTargetSourcePath` in
                class `AbstractSourcePathResolver`

        []{#getSourcePathName(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### getSourcePathName

            ``` methodSignature
            public String getSourcePathName​(BuildTarget target,
                                            SourcePath sourcePath)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getSourcePathName` in interface `SourcePathResolver`

            [Specified by:]{.overrideSpecifyLabel}
            :   `getSourcePathName` in
                class `AbstractSourcePathResolver`
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
