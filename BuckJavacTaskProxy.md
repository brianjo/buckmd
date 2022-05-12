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
[Package]{.packageLabelInType} [com.facebook.buck.jvm.java.plugin.api](package-summary.html)
:::

## Interface BuckJavacTaskProxy {#interface-buckjavactaskproxy .title title="Interface BuckJavacTaskProxy"}
:::

::: contentContainer
::: description
-   

    All Superinterfaces:
    :   `Callable<Boolean>`, `JavaCompiler.CompilationTask`

    ```{=html}
    <!-- -->
    ```

    All Known Subinterfaces:
    :   `FrontendOnlyJavacTaskProxy`

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `BuckJavacTaskProxyImpl`, `FrontendOnlyJavacTaskProxyImpl`

    ------------------------------------------------------------------------

        public interface BuckJavacTaskProxy
        extends JavaCompiler.CompilationTask

    ::: block
    `JavacTask` is included with the compiler and is thus not directly
    accessible from within Buck\'s class loader. This interface is used
    as a proxy within Buck\'s class loader to allow access to
    commonly-used methods.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                      Method                                                                                                                                                                                                                                                                                                                                       Description
          -------------------------------------- -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `void`                                 `addPostEnterCallback​(java.util.function.Consumer<Set<Element>> callback)`                                                                                                                                                                                                                                                                    
          `void`                                 `addTaskListener​(BuckJavacTaskListener taskListener)`                                                                                                                                                                                                                                                                                         
          `Iterable<? extends Element>`          `analyze()`                                                                                                                                                                                                                                                                                                                                   
          `Iterable<? extends Element>`          `enter()`                                                                                                                                                                                                                                                                                                                                     
          `Iterable<? extends JavaFileObject>`   `generate()`                                                                                                                                                                                                                                                                                                                                  
          `ElementsExtended`                     `getElements()`                                                                                                                                                                                                                                                                                                                               
          `Messager`                             `getMessager()`                                                                                                                                                                                                                                                                                                                               
          `static BuckJavacTaskProxy`            `getTask​(PluginClassLoaderFactory loaderFactory,        JavaCompiler compiler,        Writer out,        JavaFileManager fileManager,        DiagnosticListener<? super JavaFileObject> diagnosticListener,        Iterable<String> options,        Iterable<String> classes,        Iterable<? extends JavaFileObject> compilationUnits)`    
          `Types`                                `getTypes()`                                                                                                                                                                                                                                                                                                                                  
          `Iterable<CompilationUnitTreeProxy>`   `parse()`                                                                                                                                                                                                                                                                                                                                     
          `void`                                 `removeTaskListener​(BuckJavacTaskListener taskListener)`                                                                                                                                                                                                                                                                                      
          `void`                                 `setTaskListener​(BuckJavacTaskListener taskListener)`                                                                                                                                                                                                                                                                                         

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
          Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
          .tableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Abstract
          Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}

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
            static BuckJavacTaskProxy getTask​(PluginClassLoaderFactory loaderFactory,
                                              JavaCompiler compiler,
                                              Writer out,
                                              JavaFileManager fileManager,
                                              DiagnosticListener<? super JavaFileObject> diagnosticListener,
                                              Iterable<String> options,
                                              Iterable<String> classes,
                                              Iterable<? extends JavaFileObject> compilationUnits)
            ```

        []{#parse()}

        -   #### parse

            ``` methodSignature
            Iterable<CompilationUnitTreeProxy> parse()
                                              throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#enter()}

        -   #### enter

            ``` methodSignature
            Iterable<? extends Element> enter()
                                       throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#analyze()}

        -   #### analyze

            ``` methodSignature
            Iterable<? extends Element> analyze()
                                         throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#generate()}

        -   #### generate

            ``` methodSignature
            Iterable<? extends JavaFileObject> generate()
                                                 throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#setTaskListener(com.facebook.buck.jvm.java.plugin.api.BuckJavacTaskListener)}

        -   #### setTaskListener

            ``` methodSignature
            void setTaskListener​(BuckJavacTaskListener taskListener)
            ```

        []{#addTaskListener(com.facebook.buck.jvm.java.plugin.api.BuckJavacTaskListener)}

        -   #### addTaskListener

            ``` methodSignature
            void addTaskListener​(BuckJavacTaskListener taskListener)
            ```

        []{#removeTaskListener(com.facebook.buck.jvm.java.plugin.api.BuckJavacTaskListener)}

        -   #### removeTaskListener

            ``` methodSignature
            void removeTaskListener​(BuckJavacTaskListener taskListener)
            ```

        []{#addPostEnterCallback(java.util.function.Consumer)}

        -   #### addPostEnterCallback

            ``` methodSignature
            void addPostEnterCallback​(java.util.function.Consumer<Set<Element>> callback)
            ```

        []{#getElements()}

        -   #### getElements

            ``` methodSignature
            ElementsExtended getElements()
            ```

        []{#getTypes()}

        -   #### getTypes

            ``` methodSignature
            Types getTypes()
            ```

        []{#getMessager()}

        -   #### getMessager

            ``` methodSignature
            Messager getMessager()
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
