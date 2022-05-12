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
[Package]{.packageLabelInType} [com.facebook.buck.cxx.toolchain](package-summary.html)
:::

## Class CompilerProvider {#class-compilerprovider .title title="Class CompilerProvider"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.cxx.toolchain.CxxToolProvider](CxxToolProvider.html "class in com.facebook.buck.cxx.toolchain")\<[Compiler](Compiler.html "interface in com.facebook.buck.cxx.toolchain")\>

    -   -   com.facebook.buck.cxx.toolchain.CompilerProvider

::: description
-   

    ------------------------------------------------------------------------

        public class CompilerProvider
        extends CxxToolProvider<Compiler>
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        -   []{#nested.classes.inherited.from.class.com.facebook.buck.cxx.toolchain.CxxToolProvider}

            ### Nested classes/interfaces inherited from class com.facebook.buck.cxx.toolchain.[CxxToolProvider](CxxToolProvider.html "class in com.facebook.buck.cxx.toolchain")

            `CxxToolProvider.Type`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                            Description
          ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ -------------
          `CompilerProvider​(ToolProvider toolProvider,                 CxxToolProvider.Type type,                 ToolType toolType,                 boolean preferDependencyTree)`                                                                               
          `CompilerProvider​(ToolProvider toolProvider,                 java.util.function.Supplier<CxxToolProvider.Type> type,                 ToolType toolType,                 boolean preferDependencyTree)`                                                  
          `CompilerProvider​(ToolProvider toolProvider,                 java.util.function.Supplier<CxxToolProvider.Type> type,                 ToolType toolType,                 boolean preferDependencyTree,                 boolean useUnixPathSeparator)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type      Method                                               Description
          ---------------------- ---------------------------------------------------- -------------
          `protected Compiler`   `build​(CxxToolProvider.Type type,      Tool tool)`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.cxx.toolchain.CxxToolProvider}

            ### Methods inherited from class com.facebook.buck.cxx.toolchain.[CxxToolProvider](CxxToolProvider.html "class in com.facebook.buck.cxx.toolchain")

            `getParseTimeDeps, getToolType, getUseUnixPathSeparator, resolve`

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
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.core.toolchain.toolprovider.ToolProvider,com.facebook.buck.cxx.toolchain.CxxToolProvider.Type,com.facebook.buck.cxx.toolchain.ToolType,boolean)}

        -   #### CompilerProvider

                public CompilerProvider​(ToolProvider toolProvider,
                                        CxxToolProvider.Type type,
                                        ToolType toolType,
                                        boolean preferDependencyTree)

        []{#<init>(com.facebook.buck.core.toolchain.toolprovider.ToolProvider,java.util.function.Supplier,com.facebook.buck.cxx.toolchain.ToolType,boolean)}

        -   #### CompilerProvider

                public CompilerProvider​(ToolProvider toolProvider,
                                        java.util.function.Supplier<CxxToolProvider.Type> type,
                                        ToolType toolType,
                                        boolean preferDependencyTree)

        []{#<init>(com.facebook.buck.core.toolchain.toolprovider.ToolProvider,java.util.function.Supplier,com.facebook.buck.cxx.toolchain.ToolType,boolean,boolean)}

        -   #### CompilerProvider

                public CompilerProvider​(ToolProvider toolProvider,
                                        java.util.function.Supplier<CxxToolProvider.Type> type,
                                        ToolType toolType,
                                        boolean preferDependencyTree,
                                        boolean useUnixPathSeparator)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#build(com.facebook.buck.cxx.toolchain.CxxToolProvider.Type,com.facebook.buck.core.toolchain.tool.Tool)}

        -   #### build

            ``` methodSignature
            protected Compiler build​(CxxToolProvider.Type type,
                                     Tool tool)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `build` in class `CxxToolProvider<Compiler>`
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
