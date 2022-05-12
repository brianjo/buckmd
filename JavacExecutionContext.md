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
[Package]{.packageLabelInType} [com.facebook.buck.jvm.java](package-summary.html)
:::

## Interface JavacExecutionContext {#interface-javacexecutioncontext .title title="Interface JavacExecutionContext"}
:::

::: contentContainer
::: description
-   

    ------------------------------------------------------------------------

        public interface JavacExecutionContext
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                         Method                            Description
          --------------------------------------------------------- --------------------------------- -------------
          `CellPathResolver`                                        `getCellPathResolver()`            
          `ClassLoaderCache`                                        `getClassLoaderCache()`            
          `com.google.common.collect.ImmutableMap<String,​String>`   `getEnvironment()`                 
          `JavacEventSink`                                          `getEventSink()`                   
          `JavaPackageFinder`                                       `getJavaPackageFinder()`           
          `ProcessExecutor`                                         `getProcessExecutor()`             
          `ProjectFilesystem`                                       `getProjectFilesystem()`           
          `ProjectFilesystemFactory`                                `getProjectFilesystemFactory()`    
          `PrintStream`                                             `getStdErr()`                      
          `Verbosity`                                               `getVerbosity()`                   

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Abstract
          Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getEventSink()}

        -   #### getEventSink

            ``` methodSignature
            JavacEventSink getEventSink()
            ```

        []{#getStdErr()}

        -   #### getStdErr

            ``` methodSignature
            PrintStream getStdErr()
            ```

        []{#getClassLoaderCache()}

        -   #### getClassLoaderCache

            ``` methodSignature
            ClassLoaderCache getClassLoaderCache()
            ```

        []{#getVerbosity()}

        -   #### getVerbosity

            ``` methodSignature
            Verbosity getVerbosity()
            ```

        []{#getCellPathResolver()}

        -   #### getCellPathResolver

            ``` methodSignature
            CellPathResolver getCellPathResolver()
            ```

        []{#getJavaPackageFinder()}

        -   #### getJavaPackageFinder

            ``` methodSignature
            JavaPackageFinder getJavaPackageFinder()
            ```

        []{#getProjectFilesystem()}

        -   #### getProjectFilesystem

            ``` methodSignature
            ProjectFilesystem getProjectFilesystem()
            ```

        []{#getProjectFilesystemFactory()}

        -   #### getProjectFilesystemFactory

            ``` methodSignature
            ProjectFilesystemFactory getProjectFilesystemFactory()
            ```

        []{#getEnvironment()}

        -   #### getEnvironment

            ``` methodSignature
            com.google.common.collect.ImmutableMap<String,​String> getEnvironment()
            ```

        []{#getProcessExecutor()}

        -   #### getProcessExecutor

            ``` methodSignature
            ProcessExecutor getProcessExecutor()
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
