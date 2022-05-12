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

-   [Overview](../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../deprecated-list.html)
-   [Index](../../../../index-all.html)
-   [Help](../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.android](package-summary.html)
:::

## Class ConcatStep {#class-concatstep .title title="Class ConcatStep"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.android.ConcatStep

::: description
-   

    All Implemented Interfaces:
    :   `Step`

    ------------------------------------------------------------------------

        public class ConcatStep
        extends Object
        implements Step

    ::: block
    Takes in a list of files and outputs a concatenation of them in the
    same directory. Used for solid compression into a single .xz. Does
    NOT delete source files after concatenating.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type   Field          Description
          ------------------- -------------- -------------
          `static String`     `SHORT_NAME`    

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

        +-----------------------------------+-----------------------------------+
        | Constructor                       | Description                       |
        +===================================+===================================+
        | `ConcatStep​(Proj                  | ::: block                         |
        | ectFilesystem filesystem,         | Use this constructor if the files |
        |    com.google.common.collect.Immu | to concatenate are not known at   |
        | tableList.Builder<Path> inputsBui | the time of step creation.        |
        | lder,           Path outputPath)` | :::                               |
        +-----------------------------------+-----------------------------------+
        | `                                 | ::: block                         |
        | ConcatStep​(ProjectFilesystem file | Use this constructor if the files |
        | system,           com.google.comm | to concatenate are known at the   |
        | on.collect.ImmutableList<Path> in | time of step creation.            |
        | puts,           Path outputPath)` | :::                               |
        +-----------------------------------+-----------------------------------+

        : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type       Method                                       Description
          ----------------------- -------------------------------------------- -------------
          `StepExecutionResult`   `execute​(ExecutionContext context)`           
          `String`                `getDescription​(ExecutionContext context)`    
          `String`                `getShortName()`                              

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

        []{#SHORT_NAME}

        -   #### SHORT_NAME

                public static final String SHORT_NAME

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../constant-values.html#com.facebook.buck.android.ConcatStep.SHORT_NAME)
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.io.filesystem.ProjectFilesystem,com.google.common.collect.ImmutableList,java.nio.file.Path)}

        -   #### ConcatStep

                public ConcatStep​(ProjectFilesystem filesystem,
                                  com.google.common.collect.ImmutableList<Path> inputs,
                                  Path outputPath)

            ::: block
            Use this constructor if the files to concatenate are known
            at the time of step creation.
            :::

            [Parameters:]{.paramLabel}
            :   `inputs` - The files to be concatenated
            :   `outputPath` - The desired output path.

        []{#<init>(com.facebook.buck.io.filesystem.ProjectFilesystem,com.google.common.collect.ImmutableList.Builder,java.nio.file.Path)}

        -   #### ConcatStep

                public ConcatStep​(ProjectFilesystem filesystem,
                                  com.google.common.collect.ImmutableList.Builder<Path> inputsBuilder,
                                  Path outputPath)

            ::: block
            Use this constructor if the files to concatenate are not
            known at the time of step creation.
            :::

            [Parameters:]{.paramLabel}
            :   `inputsBuilder` - The files to be concatenated, in
                builder form
            :   `outputPath` - The desired output path.
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#execute(com.facebook.buck.core.build.execution.context.ExecutionContext)}

        -   #### execute

            ``` methodSignature
            public StepExecutionResult execute​(ExecutionContext context)
                                        throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `execute` in interface `Step`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#getShortName()}

        -   #### getShortName

            ``` methodSignature
            public String getShortName()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getShortName` in interface `Step`

            [Returns:]{.returnLabel}
            :   a short name/description for the command, such as
                \"javac\". Should fit on one line.

        []{#getDescription(com.facebook.buck.core.build.execution.context.ExecutionContext)}

        -   #### getDescription

            ``` methodSignature
            public String getDescription​(ExecutionContext context)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getDescription` in interface `Step`
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

-   [Overview](../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../deprecated-list.html)
-   [Index](../../../../index-all.html)
-   [Help](../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../allclasses.html)

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
