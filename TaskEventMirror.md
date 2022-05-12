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
-   [Nested](#nested.class.summary) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.jvm.java.plugin.api](package-summary.html)
:::

## Class TaskEventMirror {#class-taskeventmirror .title title="Class TaskEventMirror"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.jvm.java.plugin.api.TaskEventMirror

::: description
-   

    ------------------------------------------------------------------------

        public final class TaskEventMirror
        extends Object

    ::: block
    `TaskEvent` is included with the compiler and is thus not directly
    accessible from within Buck\'s class loader. This class is used as a
    mirror within Buck\'s class loader for a `TaskEvent` within the
    compiler\'s.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type   Class                    Description
          ------------------- ------------------------ -------------
          `static class `     `TaskEventMirror.Kind`    

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                        Description
          ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `TaskEventMirror​(Object original,                TaskEventMirror.Kind kind,                JavaFileObject sourceFile,                CompilationUnitTreeProxy compilationUnitTreeProxy,                TypeElement typeElement)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type            Method                   Description
          ---------------------------- ------------------------ -------------
          `CompilationUnitTreeProxy`   `getCompilationUnit()`    
          `TaskEventMirror.Kind`       `getKind()`               
          `Object`                     `getOriginal()`           
          `JavaFileObject`             `getSourceFile()`         
          `TypeElement`                `getTypeElement()`        

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

        []{#<init>(java.lang.Object,com.facebook.buck.jvm.java.plugin.api.TaskEventMirror.Kind,javax.tools.JavaFileObject,com.facebook.buck.jvm.java.plugin.api.CompilationUnitTreeProxy,javax.lang.model.element.TypeElement)}

        -   #### TaskEventMirror

                public TaskEventMirror​(Object original,
                                       TaskEventMirror.Kind kind,
                                       JavaFileObject sourceFile,
                                       CompilationUnitTreeProxy compilationUnitTreeProxy,
                                       TypeElement typeElement)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getOriginal()}

        -   #### getOriginal

            ``` methodSignature
            public Object getOriginal()
            ```

        []{#getKind()}

        -   #### getKind

            ``` methodSignature
            public TaskEventMirror.Kind getKind()
            ```

        []{#getSourceFile()}

        -   #### getSourceFile

            ``` methodSignature
            public JavaFileObject getSourceFile()
            ```

        []{#getCompilationUnit()}

        -   #### getCompilationUnit

            ``` methodSignature
            public CompilationUnitTreeProxy getCompilationUnit()
            ```

        []{#getTypeElement()}

        -   #### getTypeElement

            ``` methodSignature
            public TypeElement getTypeElement()
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
-   [Nested](#nested.class.summary) \| 
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
