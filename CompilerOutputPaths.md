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

## Class CompilerOutputPaths {#class-compileroutputpaths .title title="Class CompilerOutputPaths"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.jvm.java.CompilerOutputPaths

::: description
-   

    ------------------------------------------------------------------------

        public abstract class CompilerOutputPaths
        extends Object

    ::: block
    Provides access to the various output paths for a java library.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor               Description
          ------------------------- -------------
          `CompilerOutputPaths()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type              Method                                                                                       Description
          ------------------------------ -------------------------------------------------------------------------------------------- -------------
          `abstract Optional<Path>`      `getAbiJarPath()`                                                                             
          `static Path`                  `getAbiJarPath​(BuildTarget buildTarget,              ProjectFilesystem filesystem)`           
          `abstract Path`                `getAnnotationPath()`                                                                         
          `static Optional<Path>`        `getAnnotationPath​(ProjectFilesystem filesystem,                  BuildTarget target)`        
          `abstract Path`                `getClassesDir()`                                                                             
          `static Path`                  `getClassesDir​(BuildTarget target,              ProjectFilesystem filesystem)`                
          `static Path`                  `getDepFilePath​(BuildTarget target,               ProjectFilesystem filesystem)`              
          `abstract Path`                `getOutputJarDirPath()`                                                                       
          `static Path`                  `getOutputJarDirPath​(BuildTarget target,                    ProjectFilesystem filesystem)`    
          `abstract Optional<Path>`      `getOutputJarPath()`                                                                          
          `static Path`                  `getOutputJarPath​(BuildTarget target,                 ProjectFilesystem filesystem)`          
          `abstract Path`                `getPathToSourcesList()`                                                                      
          `abstract Path`                `getWorkingDirectory()`                                                                       
          `static CompilerOutputPaths`   `of​(BuildTarget target,   ProjectFilesystem filesystem)`                                      

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
          Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
          .tableTab}[[Instance
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

        []{#<init>()}

        -   #### CompilerOutputPaths

                public CompilerOutputPaths()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getClassesDir()}

        -   #### getClassesDir

            ``` methodSignature
            public abstract Path getClassesDir()
            ```

        []{#getOutputJarDirPath()}

        -   #### getOutputJarDirPath

            ``` methodSignature
            public abstract Path getOutputJarDirPath()
            ```

        []{#getAbiJarPath()}

        -   #### getAbiJarPath

            ``` methodSignature
            public abstract Optional<Path> getAbiJarPath()
            ```

        []{#getAnnotationPath()}

        -   #### getAnnotationPath

            ``` methodSignature
            public abstract Path getAnnotationPath()
            ```

        []{#getPathToSourcesList()}

        -   #### getPathToSourcesList

            ``` methodSignature
            public abstract Path getPathToSourcesList()
            ```

        []{#getWorkingDirectory()}

        -   #### getWorkingDirectory

            ``` methodSignature
            public abstract Path getWorkingDirectory()
            ```

        []{#getOutputJarPath()}

        -   #### getOutputJarPath

            ``` methodSignature
            public abstract Optional<Path> getOutputJarPath()
            ```

        []{#of(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem)}

        -   #### of

            ``` methodSignature
            public static CompilerOutputPaths of​(BuildTarget target,
                                                 ProjectFilesystem filesystem)
            ```

        []{#getDepFilePath(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem)}

        -   #### getDepFilePath

            ``` methodSignature
            public static Path getDepFilePath​(BuildTarget target,
                                              ProjectFilesystem filesystem)
            ```

        []{#getClassesDir(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem)}

        -   #### getClassesDir

            ``` methodSignature
            public static Path getClassesDir​(BuildTarget target,
                                             ProjectFilesystem filesystem)
            ```

        []{#getOutputJarDirPath(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem)}

        -   #### getOutputJarDirPath

            ``` methodSignature
            public static Path getOutputJarDirPath​(BuildTarget target,
                                                   ProjectFilesystem filesystem)
            ```

        []{#getAnnotationPath(com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.model.BuildTarget)}

        -   #### getAnnotationPath

            ``` methodSignature
            public static Optional<Path> getAnnotationPath​(ProjectFilesystem filesystem,
                                                           BuildTarget target)
            ```

        []{#getAbiJarPath(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem)}

        -   #### getAbiJarPath

            ``` methodSignature
            public static Path getAbiJarPath​(BuildTarget buildTarget,
                                             ProjectFilesystem filesystem)
            ```

        []{#getOutputJarPath(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem)}

        -   #### getOutputJarPath

            ``` methodSignature
            public static Path getOutputJarPath​(BuildTarget target,
                                                ProjectFilesystem filesystem)
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
