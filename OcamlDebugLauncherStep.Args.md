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
[Package]{.packageLabelInType} [com.facebook.buck.features.ocaml](package-summary.html)
:::

## Class OcamlDebugLauncherStep.Args {#class-ocamldebuglauncherstep.args .title title="Class OcamlDebugLauncherStep.Args"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.features.ocaml.OcamlDebugLauncherStep.Args

::: description
-   

    All Implemented Interfaces:
    :   `AddsToRuleKey`

    ```{=html}
    <!-- -->
    ```

    Enclosing class:
    :   [OcamlDebugLauncherStep](OcamlDebugLauncherStep.html "class in com.facebook.buck.features.ocaml")

    ------------------------------------------------------------------------

        public static class OcamlDebugLauncherStep.Args
        extends Object
        implements AddsToRuleKey
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type                                        Field                          Description
          -------------------------------------------------------- ------------------------------ -------------
          `com.google.common.collect.ImmutableList<String>`        `bytecodeIncludeFlags`          
          `Path`                                                   `bytecodeOutput`                
          `Tool`                                                   `ocamlDebug`                    
          `com.google.common.collect.ImmutableSortedSet<String>`   `transitiveBytecodeIncludes`    

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                    Description
          ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ -------------
          `Args​(Tool ocamlDebug,     Path bytecodeOutput,     com.google.common.collect.ImmutableSortedSet<String> transitiveBytecodeIncludes,     List<String> bytecodeIncludeFlags)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method          Description
          ------------------- --------------- -------------
          `Path`              `getOutput()`    

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
    -   []{#field.detail}

        ### Field Detail

        []{#ocamlDebug}

        -   #### ocamlDebug

                public final Tool ocamlDebug

        []{#bytecodeOutput}

        -   #### bytecodeOutput

                public final Path bytecodeOutput

        []{#transitiveBytecodeIncludes}

        -   #### transitiveBytecodeIncludes

                public final com.google.common.collect.ImmutableSortedSet<String> transitiveBytecodeIncludes

        []{#bytecodeIncludeFlags}

        -   #### bytecodeIncludeFlags

                public final com.google.common.collect.ImmutableList<String> bytecodeIncludeFlags
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.core.toolchain.tool.Tool,java.nio.file.Path,com.google.common.collect.ImmutableSortedSet,java.util.List)}

        -   #### Args

                public Args​(Tool ocamlDebug,
                            Path bytecodeOutput,
                            com.google.common.collect.ImmutableSortedSet<String> transitiveBytecodeIncludes,
                            List<String> bytecodeIncludeFlags)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getOutput()}

        -   #### getOutput

            ``` methodSignature
            public Path getOutput()
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
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
