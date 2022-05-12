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
[Package]{.packageLabelInType} [com.facebook.buck.jvm.java](package-summary.html)
:::

## Class CompilerParameters.Builder {#class-compilerparameters.builder .title title="Class CompilerParameters.Builder"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.jvm.java.ImmutableCompilerParameters.Builder

    -   -   com.facebook.buck.jvm.java.CompilerParameters.Builder

::: description
-   

    Enclosing class:
    :   [CompilerParameters](CompilerParameters.html "class in com.facebook.buck.jvm.java")

    ------------------------------------------------------------------------

        public static class CompilerParameters.Builder
        extends com.facebook.buck.jvm.java.ImmutableCompilerParameters.Builder
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor   Description
          ------------- -------------
          `Builder()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type              Method                                                                                                                                                                                                               Description
          ------------------------------ -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `CompilerParameters.Builder`   `setClasspathEntriesSourcePaths​(Collection<SourcePath> compileTimeClasspathSourcePaths,                               SourcePathResolverAdapter resolver)`                                                            
          `CompilerParameters.Builder`   `setScratchPaths​(BuildTarget target,                ProjectFilesystem projectFilesystem)`                                                                                                                             
          `CompilerParameters.Builder`   `setSourceFileSourcePaths​(com.google.common.collect.ImmutableSortedSet<SourcePath> srcs,                         ProjectFilesystem projectFilesystem,                         SourcePathResolverAdapter resolver)`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.jvm.java.ImmutableCompilerParameters.Builder}

            ### Methods inherited from class com.facebook.buck.jvm.java.ImmutableCompilerParameters.Builder

            `build, from, setAbiCompatibilityMode, setAbiGenerationMode, setClasspathEntries, setOutputPaths, setShouldTrackClassUsage, setShouldTrackJavacPhaseEvents, setSourceFilePaths, setSourceOnlyAbiRuleInfoFactory`

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
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### Builder

                public Builder()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#setScratchPaths(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem)}

        -   #### setScratchPaths

            ``` methodSignature
            public CompilerParameters.Builder setScratchPaths​(BuildTarget target,
                                                              ProjectFilesystem projectFilesystem)
            ```

        []{#setSourceFileSourcePaths(com.google.common.collect.ImmutableSortedSet,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter)}

        -   #### setSourceFileSourcePaths

            ``` methodSignature
            public CompilerParameters.Builder setSourceFileSourcePaths​(com.google.common.collect.ImmutableSortedSet<SourcePath> srcs,
                                                                       ProjectFilesystem projectFilesystem,
                                                                       SourcePathResolverAdapter resolver)
            ```

        []{#setClasspathEntriesSourcePaths(java.util.Collection,com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter)}

        -   #### setClasspathEntriesSourcePaths

            ``` methodSignature
            public CompilerParameters.Builder setClasspathEntriesSourcePaths​(Collection<SourcePath> compileTimeClasspathSourcePaths,
                                                                             SourcePathResolverAdapter resolver)
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
