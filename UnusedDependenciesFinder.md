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

## Class UnusedDependenciesFinder {#class-unuseddependenciesfinder .title title="Class UnusedDependenciesFinder"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.jvm.java.UnusedDependenciesFinder

::: description
-   

    All Implemented Interfaces:
    :   `Step`

    ------------------------------------------------------------------------

        public abstract class UnusedDependenciesFinder
        extends Object
        implements Step

    ::: block
    The step that reports dependencies not used during Java compilation.
    It uses class usage map produced during compilation and compares it
    to the outputs of the dependencies specified in Java libraries. The
    entries from classpath not used during compilation are resolved to
    the corresponding targets and reported back to the user either as an
    error (which halt the build) or as a warning.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                    Description
          ------------------------------ -------------
          `UnusedDependenciesFinder()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                                                                                   Method                                       Description
          ----------------------------------------------------------------------------------------------------------------------------------- -------------------------------------------- -------------
          `StepExecutionResult`                                                                                                               `execute​(ExecutionContext context)`           
          `abstract Optional<String>`                                                                                                         `getBuildozerPath()`                          
          `abstract BuildTarget`                                                                                                              `getBuildTarget()`                            
          `abstract Path`                                                                                                                     `getDepFileRelativePath()`                    
          `abstract com.google.common.collect.ImmutableList<com.facebook.buck.jvm.java.UnusedDependenciesFinder.DependencyAndExportedDeps>`   `getDeps()`                                   
          `String`                                                                                                                            `getDescription​(ExecutionContext context)`    
          `abstract ProjectFilesystem`                                                                                                        `getProjectFilesystem()`                      
          `abstract com.google.common.collect.ImmutableList<com.facebook.buck.jvm.java.UnusedDependenciesFinder.DependencyAndExportedDeps>`   `getProvidedDeps()`                           
          `String`                                                                                                                            `getShortName()`                              
          `abstract SourcePathResolverAdapter`                                                                                                `getSourcePathResolver()`                     
          `abstract JavaBuckConfig.UnusedDependenciesAction`                                                                                  `getUnusedDependenciesAction()`               
          `abstract boolean`                                                                                                                  `isOnlyPrintCommands()`                       

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

        []{#<init>()}

        -   #### UnusedDependenciesFinder

                public UnusedDependenciesFinder()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getBuildTarget()}

        -   #### getBuildTarget

            ``` methodSignature
            public abstract BuildTarget getBuildTarget()
            ```

        []{#getProjectFilesystem()}

        -   #### getProjectFilesystem

            ``` methodSignature
            public abstract ProjectFilesystem getProjectFilesystem()
            ```

        []{#getDepFileRelativePath()}

        -   #### getDepFileRelativePath

            ``` methodSignature
            public abstract Path getDepFileRelativePath()
            ```

        []{#getDeps()}

        -   #### getDeps

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableList<com.facebook.buck.jvm.java.UnusedDependenciesFinder.DependencyAndExportedDeps> getDeps()
            ```

        []{#getProvidedDeps()}

        -   #### getProvidedDeps

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableList<com.facebook.buck.jvm.java.UnusedDependenciesFinder.DependencyAndExportedDeps> getProvidedDeps()
            ```

        []{#getSourcePathResolver()}

        -   #### getSourcePathResolver

            ``` methodSignature
            public abstract SourcePathResolverAdapter getSourcePathResolver()
            ```

        []{#getUnusedDependenciesAction()}

        -   #### getUnusedDependenciesAction

            ``` methodSignature
            public abstract JavaBuckConfig.UnusedDependenciesAction getUnusedDependenciesAction()
            ```

        []{#getBuildozerPath()}

        -   #### getBuildozerPath

            ``` methodSignature
            public abstract Optional<String> getBuildozerPath()
            ```

        []{#isOnlyPrintCommands()}

        -   #### isOnlyPrintCommands

            ``` methodSignature
            public abstract boolean isOnlyPrintCommands()
            ```

        []{#execute(com.facebook.buck.core.build.execution.context.ExecutionContext)}

        -   #### execute

            ``` methodSignature
            public StepExecutionResult execute​(ExecutionContext context)
                                        throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `execute` in interface `Step`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#getShortName()}

        -   #### getShortName

            ``` methodSignature
            public String getShortName()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getShortName` in interface `Step`

            [Returns:]{.returnLabel}
            :   a short name/description for the command, such as
                \"javac\". Should fit on one line.

        []{#getDescription(com.facebook.buck.core.build.execution.context.ExecutionContext)}

        -   #### getDescription

            ``` methodSignature
            public String getDescription​(ExecutionContext context)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getDescription` in interface `Step`
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
