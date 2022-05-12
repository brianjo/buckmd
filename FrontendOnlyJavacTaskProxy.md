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

-   [Overview](../../../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../../index-all.html)
-   [Help](../../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.jvm.java.abi.source.api](package-summary.html)
:::

## Interface FrontendOnlyJavacTaskProxy {#interface-frontendonlyjavactaskproxy .title title="Interface FrontendOnlyJavacTaskProxy"}
:::

::: contentContainer
::: description
-   

    All Superinterfaces:
    :   `BuckJavacTaskProxy`, `Callable<Boolean>`,
        `JavaCompiler.CompilationTask`

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `FrontendOnlyJavacTaskProxyImpl`

    ------------------------------------------------------------------------

        public interface FrontendOnlyJavacTaskProxy
        extends BuckJavacTaskProxy
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                     Method                                                                                                                                                                                                                                                                                                                                       Description
          ------------------------------------- -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `static FrontendOnlyJavacTaskProxy`   `getTask​(PluginClassLoaderFactory loaderFactory,        JavaCompiler compiler,        Writer out,        JavaFileManager fileManager,        DiagnosticListener<? super JavaFileObject> diagnosticListener,        Iterable<String> options,        Iterable<String> classes,        Iterable<? extends JavaFileObject> compilationUnits)`    

          : Static Methods[ ]{.tabEnd}

        -   []{#methods.inherited.from.class.com.facebook.buck.jvm.java.plugin.api.BuckJavacTaskProxy}

            ### Methods inherited from interface com.facebook.buck.jvm.java.plugin.api.[BuckJavacTaskProxy](../../../plugin/api/BuckJavacTaskProxy.html "interface in com.facebook.buck.jvm.java.plugin.api")

            `addPostEnterCallback, addTaskListener, analyze, enter, generate, getElements, getMessager, getTypes, parse, removeTaskListener, setTaskListener`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.javax.tools.JavaCompiler.CompilationTask}

            ### Methods inherited from interface javax.tools.[JavaCompiler.CompilationTask](http://docs.oracle.com/javase/7/docs/api/javax/tools/JavaCompiler.CompilationTask.html?is-external=true "class or interface in javax.tools"){.externalLink}

            `addModules, call, setLocale, setProcessors`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getTask(com.facebook.buck.jvm.java.plugin.api.PluginClassLoaderFactory,javax.tools.JavaCompiler,java.io.Writer,javax.tools.JavaFileManager,javax.tools.DiagnosticListener,java.lang.Iterable,java.lang.Iterable,java.lang.Iterable)}

        -   #### getTask

            ``` methodSignature
            static FrontendOnlyJavacTaskProxy getTask​(PluginClassLoaderFactory loaderFactory,
                                                      JavaCompiler compiler,
                                                      Writer out,
                                                      JavaFileManager fileManager,
                                                      DiagnosticListener<? super JavaFileObject> diagnosticListener,
                                                      Iterable<String> options,
                                                      Iterable<String> classes,
                                                      Iterable<? extends JavaFileObject> compilationUnits)
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

-   [Overview](../../../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../../index-all.html)
-   [Help](../../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../../allclasses.html)

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
