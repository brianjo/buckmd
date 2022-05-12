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
[Package]{.packageLabelInType} [com.facebook.buck.step.fs](package-summary.html)
:::

## Class XzStep {#class-xzstep .title title="Class XzStep"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.step.fs.XzStep

::: description
-   

    All Implemented Interfaces:
    :   `Step`

    ------------------------------------------------------------------------

        public class XzStep
        extends Object
        implements Step

    ::: block
    A [`Step`](../Step.html "interface in com.facebook.buck.step") to
    compress a file with XZ / LZMA2.
    :::

    [See Also:]{.seeLabel}
    :   [XZ](http://tukaani.org/xz/), [XZ for
        Java](http://tukaani.org/xz/java.html), [XZ
        Embedded](http://tukaani.org/xz/embedded.html)
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type   Field                         Description
          ------------------- ----------------------------- -------------
          `static int`        `DEFAULT_COMPRESSION_LEVEL`    

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

        +-----------------------------------+-----------------------------------+
        | Constructor                       | Description                       |
        +===================================+===================================+
        | `XzStep​(ProjectFilesyst           | ::: block                         |
        | em filesystem,       Path sourceF | Creates an XzStep to compress a   |
        | ile,       int compressionLevel)` | file with XZ at a user supplied   |
        |                                   | compression level .               |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+
        | `XzStep​(Proje                     | ::: block                         |
        | ctFilesystem filesystem,       Pa | Creates an XzStep to compress a   |
        | th sourceFile,       Path outputP | file with the given XZ            |
        | ath,       int compressionLevel)` | compression level and output      |
        |                                   | path.                             |
        |                                   | :::                               |
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
          `Path`                  `getDestinationFile()`                        
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

        []{#DEFAULT_COMPRESSION_LEVEL}

        -   #### DEFAULT_COMPRESSION_LEVEL

                public static final int DEFAULT_COMPRESSION_LEVEL

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.step.fs.XzStep.DEFAULT_COMPRESSION_LEVEL)
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.io.filesystem.ProjectFilesystem,java.nio.file.Path,java.nio.file.Path,int)}

        -   #### XzStep

                public XzStep​(ProjectFilesystem filesystem,
                              Path sourceFile,
                              Path outputPath,
                              int compressionLevel)

            ::: block
            Creates an XzStep to compress a file with the given XZ
            compression level and output path.
            Decompression will require up to 64MiB of RAM.
            :::

            [Parameters:]{.paramLabel}
            :   `sourceFile` - file to compress
            :   `outputPath` - the desired output path.
            :   `compressionLevel` - level of compression (from 0-9)

        []{#<init>(com.facebook.buck.io.filesystem.ProjectFilesystem,java.nio.file.Path,int)}

        -   #### XzStep

                public XzStep​(ProjectFilesystem filesystem,
                              Path sourceFile,
                              int compressionLevel)

            ::: block
            Creates an XzStep to compress a file with XZ at a user
            supplied compression level .
            The destination file will be `sourceFile` with the added
            `.xz` extension.

            Decompression will require up to 64MiB of RAM.
            :::

            [Parameters:]{.paramLabel}
            :   `sourceFile` - file to compress
            :   `compressionLevel` - value from 0 to 9. Higher values
                result in better compression, but also need more time to
                compress and will need more RAM to decompress.
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

        []{#getDestinationFile()}

        -   #### getDestinationFile

            ``` methodSignature
            public Path getDestinationFile()
            ```

        []{#getDescription(com.facebook.buck.core.build.execution.context.ExecutionContext)}

        -   #### getDescription

            ``` methodSignature
            public String getDescription​(ExecutionContext context)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getDescription` in interface `Step`

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