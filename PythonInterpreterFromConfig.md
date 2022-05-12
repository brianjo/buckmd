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
[Package]{.packageLabelInType} [com.facebook.buck.features.python.toolchain.impl](package-summary.html)
:::

## Class PythonInterpreterFromConfig {#class-pythoninterpreterfromconfig .title title="Class PythonInterpreterFromConfig"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.features.python.toolchain.impl.PythonInterpreterFromConfig

::: description
-   

    All Implemented Interfaces:
    :   `Toolchain`, `PythonInterpreter`

    ------------------------------------------------------------------------

        public class PythonInterpreterFromConfig
        extends Object
        implements PythonInterpreter
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        -   []{#fields.inherited.from.class.com.facebook.buck.features.python.toolchain.PythonInterpreter}

            ### Fields inherited from interface com.facebook.buck.features.python.toolchain.[PythonInterpreter](../PythonInterpreter.html "interface in com.facebook.buck.features.python.toolchain")

            `DEFAULT_NAME`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                      Description
          -------------------------------------------------------------------------------------------------------------------------------- -------------
          `PythonInterpreterFromConfig​(PythonBuckConfig pythonBuckConfig,                            ExecutableFinder executableFinder)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                                       Description
          ------------------- -------------------------------------------- -------------
          `Path`              `getPythonInterpreterPath()`                  
          `Path`              `getPythonInterpreterPath​(String section)`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.features.python.toolchain.PythonInterpreter}

            ### Methods inherited from interface com.facebook.buck.features.python.toolchain.[PythonInterpreter](../PythonInterpreter.html "interface in com.facebook.buck.features.python.toolchain")

            `getName`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.features.python.PythonBuckConfig,com.facebook.buck.io.ExecutableFinder)}

        -   #### PythonInterpreterFromConfig

                public PythonInterpreterFromConfig​(PythonBuckConfig pythonBuckConfig,
                                                   ExecutableFinder executableFinder)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getPythonInterpreterPath(java.lang.String)}

        -   #### getPythonInterpreterPath

            ``` methodSignature
            public Path getPythonInterpreterPath​(String section)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getPythonInterpreterPath` in
                interface `PythonInterpreter`

        []{#getPythonInterpreterPath()}

        -   #### getPythonInterpreterPath

            ``` methodSignature
            public Path getPythonInterpreterPath()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getPythonInterpreterPath` in
                interface `PythonInterpreter`

            [Returns:]{.returnLabel}
            :   the
                [`Path`](http://docs.oracle.com/javase/7/docs/api/java/nio/file/Path.html?is-external=true "class or interface in java.nio.file"){.externalLink}
                to the default python interpreter.
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
-   Field \| 
-   [Constr](#constructor.detail) \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
