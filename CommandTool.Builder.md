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
[Package]{.packageLabelInType} [com.facebook.buck.core.toolchain.tool.impl](package-summary.html)
:::

## Class CommandTool.Builder {#class-commandtool.builder .title title="Class CommandTool.Builder"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.toolchain.tool.impl.CommandTool.Builder

::: description
-   

    Enclosing class:
    :   [CommandTool](CommandTool.html "class in com.facebook.buck.core.toolchain.tool.impl")

    ------------------------------------------------------------------------

        public static class CommandTool.Builder
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                          Description
          ------------------------------------ -------------
          `Builder()`                           
          `Builder​(Tool baseTool)`              
          `Builder​(Optional<Tool> baseTool)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `CommandTool.Builder` | `addArg​(Arg arg)`     | ::: block             |
        |                       |                       | Adds an argument.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CommandTool.Builder` | `addArg​(String arg)`  |                       |
        +-----------------------+-----------------------+-----------------------+
        | `CommandTool.Builder` | `addEnv​(String        | ::: block             |
        |                       |  key,       Arg arg)` | Adds an environment   |
        |                       |                       | variable key=arg.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CommandTool.Builder` | `addEnv​(String ke     |                       |
        |                       | y,       String val)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `CommandTool.Builder` | `addInput​(S           |                       |
        |                       | ourcePath... inputs)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `CommandTool.Builder` | `addInpu              | ::: block             |
        |                       | ts​(Iterable<? extends | Adds additional       |
        |                       |  SourcePath> inputs)` | non-argument inputs   |
        |                       |                       | to the tool.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CommandTool.Builder` | `addNonHashableInp    |                       |
        |                       | ut​(SourcePath input)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `CommandTool`         | `build()`             |                       |
        +-----------------------+-----------------------+-----------------------+

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

        []{#<init>(java.util.Optional)}

        -   #### Builder

                public Builder​(Optional<Tool> baseTool)

        []{#<init>(com.facebook.buck.core.toolchain.tool.Tool)}

        -   #### Builder

                public Builder​(Tool baseTool)

        []{#<init>()}

        -   #### Builder

                public Builder()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#addArg(com.facebook.buck.rules.args.Arg)}

        -   #### addArg

            ``` methodSignature
            public CommandTool.Builder addArg​(Arg arg)
            ```

            ::: block
            Adds an argument.
            :::

        []{#addArg(java.lang.String)}

        -   #### addArg

            ``` methodSignature
            public CommandTool.Builder addArg​(String arg)
            ```

        []{#addEnv(java.lang.String,com.facebook.buck.rules.args.Arg)}

        -   #### addEnv

            ``` methodSignature
            public CommandTool.Builder addEnv​(String key,
                                              Arg arg)
            ```

            ::: block
            Adds an environment variable key=arg.
            :::

        []{#addEnv(java.lang.String,java.lang.String)}

        -   #### addEnv

            ``` methodSignature
            public CommandTool.Builder addEnv​(String key,
                                              String val)
            ```

        []{#addInputs(java.lang.Iterable)}

        -   #### addInputs

            ``` methodSignature
            public CommandTool.Builder addInputs​(Iterable<? extends SourcePath> inputs)
            ```

            ::: block
            Adds additional non-argument inputs to the tool.
            :::

        []{#addInput(com.facebook.buck.core.sourcepath.SourcePath...)}

        -   #### addInput

            ``` methodSignature
            public CommandTool.Builder addInput​(SourcePath... inputs)
            ```

        []{#addNonHashableInput(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### addNonHashableInput

            ``` methodSignature
            public CommandTool.Builder addNonHashableInput​(SourcePath input)
            ```

        []{#build()}

        -   #### build

            ``` methodSignature
            public CommandTool build()
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
