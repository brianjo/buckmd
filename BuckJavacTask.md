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
[Package]{.packageLabelInType} [com.facebook.buck.jvm.java.plugin.adapter](package-summary.html)
:::

## Class BuckJavacTask {#class-buckjavactask .title title="Class BuckJavacTask"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.sun.source.util.JavacTask

    -   -   com.facebook.buck.jvm.java.plugin.adapter.BuckJavacTask

::: description
-   

    All Implemented Interfaces:
    :   `Callable<Boolean>`, `JavaCompiler.CompilationTask`

    ```{=html}
    <!-- -->
    ```

    Direct Known Subclasses:
    :   `FrontendOnlyJavacTask`

    ------------------------------------------------------------------------

        public class BuckJavacTask
        extends com.sun.source.util.JavacTask

    ::: block
    Extends `JavacTask` with functionality that is useful for Buck:
    -   Exposes the enter method from JavacTaskImpl
    -   Pre-javac-8 support for addTaskListener/removeTaskListener
    -   Wraps
        [`Elements`](http://docs.oracle.com/javase/7/docs/api/javax/lang/model/util/Elements.html?is-external=true "class or interface in javax.lang.model.util"){.externalLink}
        with some extended functionality
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

          Constructor                                            Description
          ------------------------------------------------------ -------------
          `BuckJavacTask​(com.sun.source.util.JavacTask inner)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `void`                | `addModules​(Iterable< |                       |
        |                       | String> moduleNames)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `addPlugin​(BuckJav    |                       |
        |                       | acPlugin plugin,      |                       |
        |                       |      String... args)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `addPostEnt           |                       |
        |                       | erCallback​(java.util. |                       |
        |                       | function.Consumer<Set |                       |
        |                       | <Element>> callback)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `                     |                       |
        |                       | addTaskListener​(com.s |                       |
        |                       | un.source.util.TaskLi |                       |
        |                       | stener taskListener)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Iterabl              | `analyze()`           |                       |
        | e<? extends Element>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Boolean`             | `call()`              |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Iterabl              | `enter()`             |                       |
        | e<? extends Element>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected void`      | `                     |                       |
        |                       | finished​(com.sun.sour |                       |
        |                       | ce.util.TaskEvent e)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Iterable<? ext       | `generate()`          |                       |
        | ends JavaFileObject>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `ElementsExtended`    | `getElements()`       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.s                | `getTrees()`          |                       |
        | un.source.util.Trees` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `TypeMirror`          | `ge                   |                       |
        |                       | tTypeMirror​(Iterable< |                       |
        |                       | ? extends com.sun.sou |                       |
        |                       | rce.tree.Tree> path)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Types`               | `getTypes()`          |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected void`      | `o                    |                       |
        |                       | nPostEnter​(Set<Elemen |                       |
        |                       | t> topLevelElements)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Iterable<? extends   | `parse()`             |                       |
        |  com.sun.source.tree. |                       |                       |
        | CompilationUnitTree>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `rem                  |                       |
        |                       | oveTaskListener​(com.s |                       |
        |                       | un.source.util.TaskLi |                       |
        |                       | stener taskListener)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `setL                 |                       |
        |                       | ocale​(Locale locale)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `setProcessors​(       |                       |
        |                       | Iterable<? extends Pr |                       |
        |                       | ocessor> processors)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `                     | ::: block             |
        |                       | setTaskListener​(com.s | Sets a                |
        |                       | un.source.util.TaskLi | `TaskListener`.       |
        |                       | stener taskListener)` | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `protected void`      | `started​(com.sun.sour |                       |
        |                       | ce.util.TaskEvent e)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

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

        -   #### BuckJavacTask

                public BuckJavacTask​(com.sun.source.util.JavacTask inner)
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

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#enter()}

        -   #### enter

            ``` methodSignature
            public Iterable<? extends Element> enter()
                                              throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#setTaskListener(com.sun.source.util.TaskListener)}

        -   #### setTaskListener

            ``` methodSignature
            public void setTaskListener​(com.sun.source.util.TaskListener taskListener)
            ```

            ::: block
            Sets a `TaskListener`. Like `JavacTask`\'s implementation of
            this method, the listener does not replace listeners added
            with
            [`addTaskListener(TaskListener)`](#addTaskListener(com.sun.source.util.TaskListener)).
            Instead, it replaces only the listener provided in the
            previous call to this method, if any.
            Presumably this behavior was to enable `Plugin`s to work
            properly with build systems that were written when only a
            single `TaskListener` was supported at a time.
            :::

        []{#addTaskListener(com.sun.source.util.TaskListener)}

        -   #### addTaskListener

            ``` methodSignature
            public void addTaskListener​(com.sun.source.util.TaskListener taskListener)
            ```

        []{#removeTaskListener(com.sun.source.util.TaskListener)}

        -   #### removeTaskListener

            ``` methodSignature
            public void removeTaskListener​(com.sun.source.util.TaskListener taskListener)
            ```

        []{#getElements()}

        -   #### getElements

            ``` methodSignature
            public ElementsExtended getElements()
            ```

        []{#addPlugin(com.facebook.buck.jvm.java.plugin.adapter.BuckJavacPlugin,java.lang.String...)}

        -   #### addPlugin

            ``` methodSignature
            public void addPlugin​(BuckJavacPlugin plugin,
                                  String... args)
            ```

        []{#addPostEnterCallback(java.util.function.Consumer)}

        -   #### addPostEnterCallback

            ``` methodSignature
            public void addPostEnterCallback​(java.util.function.Consumer<Set<Element>> callback)
            ```

        []{#getTrees()}

        -   #### getTrees

            ``` methodSignature
            public com.sun.source.util.Trees getTrees()
            ```

        []{#started(com.sun.source.util.TaskEvent)}

        -   #### started

            ``` methodSignature
            protected void started​(com.sun.source.util.TaskEvent e)
            ```

        []{#finished(com.sun.source.util.TaskEvent)}

        -   #### finished

            ``` methodSignature
            protected void finished​(com.sun.source.util.TaskEvent e)
            ```

        []{#onPostEnter(java.util.Set)}

        -   #### onPostEnter

            ``` methodSignature
            protected void onPostEnter​(Set<Element> topLevelElements)
            ```

        []{#analyze()}

        -   #### analyze

            ``` methodSignature
            public Iterable<? extends Element> analyze()
                                                throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `analyze` in class `com.sun.source.util.JavacTask`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#generate()}

        -   #### generate

            ``` methodSignature
            public Iterable<? extends JavaFileObject> generate()
                                                        throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `generate` in class `com.sun.source.util.JavacTask`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#getTypeMirror(java.lang.Iterable)}

        -   #### getTypeMirror

            ``` methodSignature
            public TypeMirror getTypeMirror​(Iterable<? extends com.sun.source.tree.Tree> path)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getTypeMirror` in class `com.sun.source.util.JavacTask`

        []{#getTypes()}

        -   #### getTypes

            ``` methodSignature
            public Types getTypes()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getTypes` in class `com.sun.source.util.JavacTask`

        []{#setProcessors(java.lang.Iterable)}

        -   #### setProcessors

            ``` methodSignature
            public void setProcessors​(Iterable<? extends Processor> processors)
            ```

        []{#setLocale(java.util.Locale)}

        -   #### setLocale

            ``` methodSignature
            public void setLocale​(Locale locale)
            ```

        []{#call()}

        -   #### call

            ``` methodSignature
            public Boolean call()
            ```

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
