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
[Package]{.packageLabelInType} [com.facebook.buck.jvm.java.abi.source.api](package-summary.html)
:::

## Class ErrorSuppressingDiagnosticListener {#class-errorsuppressingdiagnosticlistener .title title="Class ErrorSuppressingDiagnosticListener"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.jvm.java.abi.source.api.ErrorSuppressingDiagnosticListener

::: description
-   

    All Implemented Interfaces:
    :   `DiagnosticListener<JavaFileObject>`

    ------------------------------------------------------------------------

        public class ErrorSuppressingDiagnosticListener
        extends Object
        implements DiagnosticListener<JavaFileObject>

    ::: block
    When running the compiler with some dependencies missing (as when
    generating ABIs from source), by default it will abort after the
    last round of annotation processing because it believes there are
    missing types. This diagnostic listener tricks the compiler into
    ignoring those errors (which it marks as \"recoverable\") so that
    the compiler will keep going and run one more enter phase after
    annotation processing. We must be careful to not allow it to run
    further, because the analyze phase will not be happy to have missing
    types.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                              Description
          ---------------------------------------------------------------------------------------- -------------
          `ErrorSuppressingDiagnosticListener​(DiagnosticListener<? super JavaFileObject> inner)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                                                      Description
          ------------------- ----------------------------------------------------------- -------------
          `void`              `report​(Diagnostic<? extends JavaFileObject> diagnostic)`    
          `void`              `setTask​(JavaCompiler.CompilationTask task)`                 

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

        []{#<init>(javax.tools.DiagnosticListener)}

        -   #### ErrorSuppressingDiagnosticListener

                public ErrorSuppressingDiagnosticListener​(DiagnosticListener<? super JavaFileObject> inner)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#setTask(javax.tools.JavaCompiler.CompilationTask)}

        -   #### setTask

            ``` methodSignature
            public void setTask​(JavaCompiler.CompilationTask task)
            ```

        []{#report(javax.tools.Diagnostic)}

        -   #### report

            ``` methodSignature
            public void report​(Diagnostic<? extends JavaFileObject> diagnostic)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `report` in
                interface `DiagnosticListener<JavaFileObject>`
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
