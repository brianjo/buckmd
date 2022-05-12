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
-   [Field](#field.summary) \| 
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.android.relinker](package-summary.html)
:::

## Class Symbols {#class-symbols .title title="Class Symbols"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.android.relinker.Symbols

::: description
-   

    ------------------------------------------------------------------------

        public class Symbols
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type                                  Field         Description
          -------------------------------------------------- ------------- -------------
          `com.google.common.collect.ImmutableSet<String>`   `all`          
          `com.google.common.collect.ImmutableSet<String>`   `global`       
          `com.google.common.collect.ImmutableSet<String>`   `undefined`    

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                Method                                                                                                                                                         Description
          ---------------------------------------------------------------- -------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `static com.facebook.buck.android.relinker.Symbols.SymbolInfo`   `extractSymbolInfo​(String line)`                                                                                                                                
          `static com.google.common.collect.ImmutableSet<String>`          `getDtNeeded​(ProcessExecutor executor,            Tool objdump,            SourcePathResolverAdapter resolver,            Path lib)`                            
          `static Symbols`                                                 `getDynamicSymbols​(ProcessExecutor executor,                  Tool objdump,                  SourcePathResolverAdapter resolver,                  Path lib)`    
          `static Symbols`                                                 `getNormalSymbols​(ProcessExecutor executor,                 Tool objdump,                 SourcePathResolverAdapter resolver,                 Path lib)`        

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
          Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#field.detail}

        ### Field Detail

        []{#undefined}

        -   #### undefined

                public com.google.common.collect.ImmutableSet<String> undefined

        []{#global}

        -   #### global

                public com.google.common.collect.ImmutableSet<String> global

        []{#all}

        -   #### all

                public com.google.common.collect.ImmutableSet<String> all
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#extractSymbolInfo(java.lang.String)}

        -   #### extractSymbolInfo

            ``` methodSignature
            @Nullable
            public static com.facebook.buck.android.relinker.Symbols.SymbolInfo extractSymbolInfo​(String line)
            ```

        []{#getDynamicSymbols(com.facebook.buck.util.ProcessExecutor,com.facebook.buck.core.toolchain.tool.Tool,com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter,java.nio.file.Path)}

        -   #### getDynamicSymbols

            ``` methodSignature
            public static Symbols getDynamicSymbols​(ProcessExecutor executor,
                                                    Tool objdump,
                                                    SourcePathResolverAdapter resolver,
                                                    Path lib)
                                             throws IOException,
                                                    InterruptedException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`
            :   `InterruptedException`

        []{#getNormalSymbols(com.facebook.buck.util.ProcessExecutor,com.facebook.buck.core.toolchain.tool.Tool,com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter,java.nio.file.Path)}

        -   #### getNormalSymbols

            ``` methodSignature
            public static Symbols getNormalSymbols​(ProcessExecutor executor,
                                                   Tool objdump,
                                                   SourcePathResolverAdapter resolver,
                                                   Path lib)
                                            throws IOException,
                                                   InterruptedException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`
            :   `InterruptedException`

        []{#getDtNeeded(com.facebook.buck.util.ProcessExecutor,com.facebook.buck.core.toolchain.tool.Tool,com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter,java.nio.file.Path)}

        -   #### getDtNeeded

            ``` methodSignature
            public static com.google.common.collect.ImmutableSet<String> getDtNeeded​(ProcessExecutor executor,
                                                                                     Tool objdump,
                                                                                     SourcePathResolverAdapter resolver,
                                                                                     Path lib)
                                                                              throws IOException,
                                                                                     InterruptedException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`
            :   `InterruptedException`
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
-   [Field](#field.summary) \| 
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
-   Constr \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
