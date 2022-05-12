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
[Package]{.packageLabelInType} [com.facebook.buck.jvm.java.plugin.adapter](package-summary.html)
:::

## Class BuckJavacTaskProxyImpl {#class-buckjavactaskproxyimpl .title title="Class BuckJavacTaskProxyImpl"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.jvm.java.plugin.adapter.BuckJavacTaskProxyImpl

::: description
-   

    All Implemented Interfaces:
    :   `BuckJavacTaskProxy`, `Callable<Boolean>`,
        `JavaCompiler.CompilationTask`

    ```{=html}
    <!-- -->
    ```

    Direct Known Subclasses:
    :   `FrontendOnlyJavacTaskProxyImpl`

    ------------------------------------------------------------------------

        public class BuckJavacTaskProxyImpl
        extends Object
        implements BuckJavacTaskProxy

    ::: block
    NOTE: A Java8 copy of this file exists in
    ../java8/BuckJavacTaskProxyImpl.java. Please make sure to update the
    other copy when modifying this file.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                        Description
          ------------------------------------------------------------------ -------------
          `BuckJavacTaskProxyImpl​(BuckJavacTask javacTask)`                   
          `BuckJavacTaskProxyImpl​(JavaCompiler.CompilationTask javacTask)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                      Method                                                                       Description
          -------------------------------------- ---------------------------------------------------------------------------- -------------
          `void`                                 `addModules​(Iterable<String> moduleNames)`                                    
          `void`                                 `addPostEnterCallback​(java.util.function.Consumer<Set<Element>> callback)`    
          `void`                                 `addTaskListener​(BuckJavacTaskListener buckTaskListener)`                     
          `Iterable<? extends Element>`          `analyze()`                                                                   
          `Boolean`                              `call()`                                                                      
          `Iterable<? extends Element>`          `enter()`                                                                     
          `Iterable<? extends JavaFileObject>`   `generate()`                                                                  
          `ElementsExtended`                     `getElements()`                                                               
          `BuckJavacTask`                        `getInner()`                                                                  
          `Messager`                             `getMessager()`                                                               
          `Types`                                `getTypes()`                                                                  
          `Iterable<CompilationUnitTreeProxy>`   `parse()`                                                                     
          `void`                                 `removeTaskListener​(BuckJavacTaskListener buckTaskListener)`                  
          `void`                                 `setLocale​(Locale locale)`                                                    
          `void`                                 `setProcessors​(Iterable<? extends Processor> processors)`                     
          `void`                                 `setTaskListener​(BuckJavacTaskListener buckTaskListener)`                     

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
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

        []{#<init>(javax.tools.JavaCompiler.CompilationTask)}

        -   #### BuckJavacTaskProxyImpl

                public BuckJavacTaskProxyImpl​(JavaCompiler.CompilationTask javacTask)

        []{#<init>(com.facebook.buck.jvm.java.plugin.adapter.BuckJavacTask)}

        -   #### BuckJavacTaskProxyImpl

                public BuckJavacTaskProxyImpl​(BuckJavacTask javacTask)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getInner()}

        -   #### getInner

            ``` methodSignature
            public BuckJavacTask getInner()
            ```

        []{#parse()}

        -   #### parse

            ``` methodSignature
            public Iterable<CompilationUnitTreeProxy> parse()
                                                     throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `parse` in interface `BuckJavacTaskProxy`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#enter()}

        -   #### enter

            ``` methodSignature
            public Iterable<? extends Element> enter()
                                              throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `enter` in interface `BuckJavacTaskProxy`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#analyze()}

        -   #### analyze

            ``` methodSignature
            public Iterable<? extends Element> analyze()
                                                throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `analyze` in interface `BuckJavacTaskProxy`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#generate()}

        -   #### generate

            ``` methodSignature
            public Iterable<? extends JavaFileObject> generate()
                                                        throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `generate` in interface `BuckJavacTaskProxy`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#setTaskListener(com.facebook.buck.jvm.java.plugin.api.BuckJavacTaskListener)}

        -   #### setTaskListener

            ``` methodSignature
            public void setTaskListener​(BuckJavacTaskListener buckTaskListener)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `setTaskListener` in interface `BuckJavacTaskProxy`

        []{#addTaskListener(com.facebook.buck.jvm.java.plugin.api.BuckJavacTaskListener)}

        -   #### addTaskListener

            ``` methodSignature
            public void addTaskListener​(BuckJavacTaskListener buckTaskListener)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `addTaskListener` in interface `BuckJavacTaskProxy`

        []{#removeTaskListener(com.facebook.buck.jvm.java.plugin.api.BuckJavacTaskListener)}

        -   #### removeTaskListener

            ``` methodSignature
            public void removeTaskListener​(BuckJavacTaskListener buckTaskListener)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `removeTaskListener` in interface `BuckJavacTaskProxy`

        []{#addPostEnterCallback(java.util.function.Consumer)}

        -   #### addPostEnterCallback

            ``` methodSignature
            public void addPostEnterCallback​(java.util.function.Consumer<Set<Element>> callback)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `addPostEnterCallback` in interface `BuckJavacTaskProxy`

        []{#getElements()}

        -   #### getElements

            ``` methodSignature
            public ElementsExtended getElements()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getElements` in interface `BuckJavacTaskProxy`

        []{#getTypes()}

        -   #### getTypes

            ``` methodSignature
            public Types getTypes()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getTypes` in interface `BuckJavacTaskProxy`

        []{#getMessager()}

        -   #### getMessager

            ``` methodSignature
            public Messager getMessager()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getMessager` in interface `BuckJavacTaskProxy`

        []{#setProcessors(java.lang.Iterable)}

        -   #### setProcessors

            ``` methodSignature
            public void setProcessors​(Iterable<? extends Processor> processors)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `setProcessors` in
                interface `JavaCompiler.CompilationTask`

        []{#setLocale(java.util.Locale)}

        -   #### setLocale

            ``` methodSignature
            public void setLocale​(Locale locale)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `setLocale` in interface `JavaCompiler.CompilationTask`

        []{#call()}

        -   #### call

            ``` methodSignature
            public Boolean call()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `call` in interface `Callable<Boolean>`

            [Specified by:]{.overrideSpecifyLabel}
            :   `call` in interface `JavaCompiler.CompilationTask`

        []{#addModules(java.lang.Iterable)}

        -   #### addModules

            ``` methodSignature
            public void addModules​(Iterable<String> moduleNames)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `addModules` in interface `JavaCompiler.CompilationTask`
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
