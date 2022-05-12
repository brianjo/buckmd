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
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
-   [Constr](#constructor.detail) \| 
-   Method

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
[Package]{.packageLabelInType} [com.facebook.buck.features.ocaml](package-summary.html)
:::

## Class OcamlCCompileStep.Args {#class-ocamlccompilestep.args .title title="Class OcamlCCompileStep.Args"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.features.ocaml.OcamlCCompileStep.Args

::: description
-   

    All Implemented Interfaces:
    :   `AddsToRuleKey`

    ```{=html}
    <!-- -->
    ```

    Enclosing class:
    :   [OcamlCCompileStep](OcamlCCompileStep.html "class in com.facebook.buck.features.ocaml")

    ------------------------------------------------------------------------

        public static class OcamlCCompileStep.Args
        extends Object
        implements AddsToRuleKey

    ::: block
    OcamlCCompile rule args.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type                                         Field             Description
          --------------------------------------------------------- ----------------- -------------
          `BuildTarget`                                             `buildTarget`      
          `com.google.common.collect.ImmutableList<String>`         `cCompiler`        
          `com.google.common.collect.ImmutableList<Arg>`            `cFlags`           
          `com.google.common.collect.ImmutableMap<String,​String>`   `environment`      
          `com.google.common.collect.ImmutableList<CxxHeaders>`     `includes`         
          `SourcePath`                                              `input`            
          `Tool`                                                    `ocamlCompiler`    
          `Path`                                                    `output`           
          `Optional<String>`                                        `stdlib`           

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                                                                                                                                    Description
          ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `Args​(BuildTarget buildTarget,     com.google.common.collect.ImmutableMap<String,​String> environment,     com.google.common.collect.ImmutableList<String> cCompiler,     Tool ocamlCompiler,     Optional<String> stdlib,     Path output,     SourcePath input,     com.google.common.collect.ImmutableList<Arg> cFlags,     com.google.common.collect.ImmutableList<CxxHeaders> includes)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#field.detail}

        ### Field Detail

        []{#buildTarget}

        -   #### buildTarget

                public final BuildTarget buildTarget

        []{#environment}

        -   #### environment

                public final com.google.common.collect.ImmutableMap<String,​String> environment

        []{#ocamlCompiler}

        -   #### ocamlCompiler

                public final Tool ocamlCompiler

        []{#cCompiler}

        -   #### cCompiler

                public final com.google.common.collect.ImmutableList<String> cCompiler

        []{#cFlags}

        -   #### cFlags

                public final com.google.common.collect.ImmutableList<Arg> cFlags

        []{#stdlib}

        -   #### stdlib

                public final Optional<String> stdlib

        []{#output}

        -   #### output

                public final Path output

        []{#input}

        -   #### input

                public final SourcePath input

        []{#includes}

        -   #### includes

                public final com.google.common.collect.ImmutableList<CxxHeaders> includes
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.core.model.BuildTarget,com.google.common.collect.ImmutableMap,com.google.common.collect.ImmutableList,com.facebook.buck.core.toolchain.tool.Tool,java.util.Optional,java.nio.file.Path,com.facebook.buck.core.sourcepath.SourcePath,com.google.common.collect.ImmutableList,com.google.common.collect.ImmutableList)}

        -   #### Args

                public Args​(BuildTarget buildTarget,
                            com.google.common.collect.ImmutableMap<String,​String> environment,
                            com.google.common.collect.ImmutableList<String> cCompiler,
                            Tool ocamlCompiler,
                            Optional<String> stdlib,
                            Path output,
                            SourcePath input,
                            com.google.common.collect.ImmutableList<Arg> cFlags,
                            com.google.common.collect.ImmutableList<CxxHeaders> includes)
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
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
-   [Constr](#constructor.detail) \| 
-   Method

</div>

[]{#skip.navbar.bottom}
:::
