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
[Package]{.packageLabelInType} [com.facebook.buck.jvm.kotlin](package-summary.html)
:::

## Class JarBackedReflectedKotlinc {#class-jarbackedreflectedkotlinc .title title="Class JarBackedReflectedKotlinc"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.jvm.kotlin.JarBackedReflectedKotlinc

::: description
-   

    All Implemented Interfaces:
    :   `AddsToRuleKey`, `Tool`, `Kotlinc`

    ------------------------------------------------------------------------

        public class JarBackedReflectedKotlinc
        extends Object
        implements Kotlinc
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                         Method                                                                                                                                                                                                                                                                                                                                                                                                               Description
          --------------------------------------------------------- -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `int`                                                     `buildWithClasspath​(ExecutionContext context,                   BuildTarget invokingRule,                   com.google.common.collect.ImmutableList<String> options,                   com.google.common.collect.ImmutableSortedSet<Path> kotlinSourceFilePaths,                   Path pathToSrcsList,                   Optional<Path> workingDirectory,                   ProjectFilesystem projectFilesystem)`    
          `com.google.common.collect.ImmutableList<Path>`           `getAdditionalClasspathEntries​(SourcePathResolverAdapter sourcePathResolverAdapter)`                                                                                                                                                                                                                                                                                                                                  
          `Path`                                                    `getAnnotationProcessorPath​(SourcePathResolverAdapter sourcePathResolverAdapter)`                                                                                                                                                                                                                                                                                                                                     
          `com.google.common.collect.ImmutableList<String>`         `getCommandPrefix​(SourcePathResolverAdapter resolver)`                                                                                                                                                                                                                                                                                                                                                                
          `String`                                                  `getDescription​(com.google.common.collect.ImmutableList<String> options,               com.google.common.collect.ImmutableSortedSet<Path> javaSourceFilePaths,               Path pathToSrcsList)`                                                                                                                                                                                                                    
          `com.google.common.collect.ImmutableMap<String,​String>`   `getEnvironment​(SourcePathResolverAdapter resolver)`                                                                                                                                                                                                                                                                                                                                                                  
          `String`                                                  `getShortName()`                                                                                                                                                                                                                                                                                                                                                                                                      
          `Path`                                                    `getStdlibPath​(SourcePathResolverAdapter sourcePathResolverAdapter)`                                                                                                                                                                                                                                                                                                                                                  
          `com.facebook.buck.jvm.kotlin.KotlincVersion`             `getVersion()`                                                                                                                                                                                                                                                                                                                                                                                                        

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.jvm.kotlin.Kotlinc}

            ### Methods inherited from interface com.facebook.buck.jvm.kotlin.[Kotlinc](Kotlinc.html "interface in com.facebook.buck.jvm.kotlin")

            `getExpandedSourcePaths`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getVersion()}

        -   #### getVersion

            ``` methodSignature
            public com.facebook.buck.jvm.kotlin.KotlincVersion getVersion()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getVersion` in interface `Kotlinc`

        []{#getDescription(com.google.common.collect.ImmutableList,com.google.common.collect.ImmutableSortedSet,java.nio.file.Path)}

        -   #### getDescription

            ``` methodSignature
            public String getDescription​(com.google.common.collect.ImmutableList<String> options,
                                         com.google.common.collect.ImmutableSortedSet<Path> javaSourceFilePaths,
                                         Path pathToSrcsList)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getDescription` in interface `Kotlinc`

        []{#getShortName()}

        -   #### getShortName

            ``` methodSignature
            public String getShortName()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getShortName` in interface `Kotlinc`

        []{#getAnnotationProcessorPath(com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter)}

        -   #### getAnnotationProcessorPath

            ``` methodSignature
            public Path getAnnotationProcessorPath​(SourcePathResolverAdapter sourcePathResolverAdapter)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getAnnotationProcessorPath` in interface `Kotlinc`

        []{#getStdlibPath(com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter)}

        -   #### getStdlibPath

            ``` methodSignature
            public Path getStdlibPath​(SourcePathResolverAdapter sourcePathResolverAdapter)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getStdlibPath` in interface `Kotlinc`

        []{#getAdditionalClasspathEntries(com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter)}

        -   #### getAdditionalClasspathEntries

            ``` methodSignature
            public com.google.common.collect.ImmutableList<Path> getAdditionalClasspathEntries​(SourcePathResolverAdapter sourcePathResolverAdapter)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getAdditionalClasspathEntries` in interface `Kotlinc`

        []{#getCommandPrefix(com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter)}

        -   #### getCommandPrefix

            ``` methodSignature
            public com.google.common.collect.ImmutableList<String> getCommandPrefix​(SourcePathResolverAdapter resolver)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getCommandPrefix` in interface `Tool`

            [Returns:]{.returnLabel}
            :   the prefix command use to run this tool.

        []{#buildWithClasspath(com.facebook.buck.core.build.execution.context.ExecutionContext,com.facebook.buck.core.model.BuildTarget,com.google.common.collect.ImmutableList,com.google.common.collect.ImmutableSortedSet,java.nio.file.Path,java.util.Optional,com.facebook.buck.io.filesystem.ProjectFilesystem)}

        -   #### buildWithClasspath

            ``` methodSignature
            public int buildWithClasspath​(ExecutionContext context,
                                          BuildTarget invokingRule,
                                          com.google.common.collect.ImmutableList<String> options,
                                          com.google.common.collect.ImmutableSortedSet<Path> kotlinSourceFilePaths,
                                          Path pathToSrcsList,
                                          Optional<Path> workingDirectory,
                                          ProjectFilesystem projectFilesystem)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `buildWithClasspath` in interface `Kotlinc`

        []{#getEnvironment(com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter)}

        -   #### getEnvironment

            ``` methodSignature
            public com.google.common.collect.ImmutableMap<String,​String> getEnvironment​(SourcePathResolverAdapter resolver)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getEnvironment` in interface `Tool`

            [Returns:]{.returnLabel}
            :   the list of environment variables to set when running
                the command.
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
