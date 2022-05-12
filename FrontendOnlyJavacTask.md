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
-   [Field](#field.summary) \| 
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.jvm.java.abi.source](package-summary.html)
:::

## Class FrontendOnlyJavacTask {#class-frontendonlyjavactask .title title="Class FrontendOnlyJavacTask"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.sun.source.util.JavacTask

    -   -   [com.facebook.buck.jvm.java.plugin.adapter.BuckJavacTask](../../plugin/adapter/BuckJavacTask.html "class in com.facebook.buck.jvm.java.plugin.adapter")

        -   -   com.facebook.buck.jvm.java.abi.source.FrontendOnlyJavacTask

::: description
-   

    All Implemented Interfaces:
    :   `Callable<Boolean>`, `JavaCompiler.CompilationTask`

    ------------------------------------------------------------------------

        public class FrontendOnlyJavacTask
        extends BuckJavacTask

    ::: block
    An implementation of `JavacTask` that implements only the frontend
    portions of the task, using only the parse phase of the underlying
    compiler and without requiring a complete classpath. This
    effectively does the same thing as the Enter phase of the compiler
    (see
    http://openjdk.java.net/groups/compiler/doc/compilation-overview/index.html),
    but applying heuristics when dependencies are missing. This
    necessarily requires some assumptions to be made about references to
    symbols defined in those dependencies. See the documentation of
    [`com.facebook.buck.jvm.java.abi.source`](package-summary.html) for
    details.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type                           Field     Description
          ------------------------------------------- --------- -------------
          `protected com.sun.source.util.JavacTask`   `inner`    

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                   Description
          ------------------------------------------------------------- -------------
          `FrontendOnlyJavacTask​(com.sun.source.util.JavacTask task)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                               Method                                                               Description
          --------------------------------------------------------------- -------------------------------------------------------------------- -------------
          `void`                                                          `addModules​(Iterable<String> moduleNames)`                            
          `Iterable<? extends Element>`                                   `analyze()`                                                           
          `Boolean`                                                       `call()`                                                              
          `Iterable<? extends Element>`                                   `enter()`                                                             
          `Iterable<? extends JavaFileObject>`                            `generate()`                                                          
          `com.facebook.buck.jvm.java.abi.source.TreeBackedElements`      `getElements()`                                                       
          `com.facebook.buck.jvm.java.abi.source.TreeBackedTrees`         `getTrees()`                                                          
          `TypeMirror`                                                    `getTypeMirror​(Iterable<? extends com.sun.source.tree.Tree> path)`    
          `com.facebook.buck.jvm.java.abi.source.TreeBackedTypes`         `getTypes()`                                                          
          `protected void`                                                `onPostEnter​(Set<Element> topLevelElements)`                          
          `Iterable<? extends com.sun.source.tree.CompilationUnitTree>`   `parse()`                                                             
          `void`                                                          `setLocale​(Locale locale)`                                            
          `void`                                                          `setProcessors​(Iterable<? extends Processor> processors)`             

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.jvm.java.plugin.adapter.BuckJavacTask}

            ### Methods inherited from class com.facebook.buck.jvm.java.plugin.adapter.[BuckJavacTask](../../plugin/adapter/BuckJavacTask.html "class in com.facebook.buck.jvm.java.plugin.adapter")

            `addPlugin, addPostEnterCallback, addTaskListener, finished, removeTaskListener, setTaskListener, started`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.sun.source.util.JavacTask}

            ### Methods inherited from class com.sun.source.util.JavacTask

            `instance`

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
    -   []{#field.detail}

        ### Field Detail

        []{#inner}

        -   #### inner

                protected final com.sun.source.util.JavacTask inner
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.sun.source.util.JavacTask)}

        -   #### FrontendOnlyJavacTask

                public FrontendOnlyJavacTask​(com.sun.source.util.JavacTask task)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#parse()}

        -   #### parse

            ``` methodSignature
            public Iterable<? extends com.sun.source.tree.CompilationUnitTree> parse()
                                                                              throws IOException
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `parse` in class `BuckJavacTask`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#enter()}

        -   #### enter

            ``` methodSignature
            public Iterable<? extends Element> enter()
                                              throws IOException
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `enter` in class `BuckJavacTask`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#analyze()}

        -   #### analyze

            ``` methodSignature
            public Iterable<? extends Element> analyze()
            ```

        []{#generate()}

        -   #### generate

            ``` methodSignature
            public Iterable<? extends JavaFileObject> generate()
            ```

        []{#getTypeMirror(java.lang.Iterable)}

        -   #### getTypeMirror

            ``` methodSignature
            public TypeMirror getTypeMirror​(Iterable<? extends com.sun.source.tree.Tree> path)
            ```

        []{#getElements()}

        -   #### getElements

            ``` methodSignature
            public com.facebook.buck.jvm.java.abi.source.TreeBackedElements getElements()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `getElements` in class `BuckJavacTask`

        []{#getTrees()}

        -   #### getTrees

            ``` methodSignature
            public com.facebook.buck.jvm.java.abi.source.TreeBackedTrees getTrees()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `getTrees` in class `BuckJavacTask`

        []{#getTypes()}

        -   #### getTypes

            ``` methodSignature
            public com.facebook.buck.jvm.java.abi.source.TreeBackedTypes getTypes()
            ```

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

        []{#onPostEnter(java.util.Set)}

        -   #### onPostEnter

            ``` methodSignature
            protected void onPostEnter​(Set<Element> topLevelElements)
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `onPostEnter` in class `BuckJavacTask`

        []{#addModules(java.lang.Iterable)}

        -   #### addModules

            ``` methodSignature
            public void addModules​(Iterable<String> moduleNames)
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
-   [Field](#field.summary) \| 
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
-   [Constr](#constructor.detail) \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
