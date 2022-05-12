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
[Package]{.packageLabelInType} [com.facebook.buck.unarchive](package-summary.html)
:::

## Class UnarchiveStep {#class-unarchivestep .title title="Class UnarchiveStep"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.unarchive.UnarchiveStep

::: description
-   

    All Implemented Interfaces:
    :   `Step`

    ```{=html}
    <!-- -->
    ```

    Direct Known Subclasses:
    :   `UntarStep`, `UnzipStep`

    ------------------------------------------------------------------------

        public abstract class UnarchiveStep
        extends Object
        implements Step

    ::: block
    A step that extracts arbitrary archives
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type               Field                    Description
          ------------------------------- ------------------------ -------------
          `protected Path`                `archiveFile`             
          `protected Path`                `destinationDirectory`    
          `protected PatternsMatcher`     `entriesToExclude`        
          `protected ProjectFilesystem`   `filesystem`              

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

        +-----------------------------------+-----------------------------------+
        | Constructor                       | Description                       |
        +===================================+===================================+
        | `Unarchi                          | ::: block                         |
        | veStep​(ArchiveFormat format,      | Create an instance of             |
        |          ProjectFilesystem filesy | UnarchiveStep                     |
        | stem,              Path archiveFi | :::                               |
        | le,              Path destination |                                   |
        | Directory,              Optional< |                                   |
        | Path> stripPrefix,              P |                                   |
        | atternsMatcher entriesToExclude)` |                                   |
        +-----------------------------------+-----------------------------------+

        : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type       Method                                Description
          ----------------------- ------------------------------------- -------------
          `StepExecutionResult`   `execute​(ExecutionContext context)`    

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
        -   []{#methods.inherited.from.class.com.facebook.buck.step.Step}

            ### Methods inherited from interface com.facebook.buck.step.[Step](../step/Step.html "interface in com.facebook.buck.step")

            `getDescription, getShortName`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#field.detail}

        ### Field Detail

        []{#filesystem}

        -   #### filesystem

                protected final ProjectFilesystem filesystem

        []{#archiveFile}

        -   #### archiveFile

                protected final Path archiveFile

        []{#destinationDirectory}

        -   #### destinationDirectory

                protected final Path destinationDirectory

        []{#entriesToExclude}

        -   #### entriesToExclude

                protected final PatternsMatcher entriesToExclude
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.util.unarchive.ArchiveFormat,com.facebook.buck.io.filesystem.ProjectFilesystem,java.nio.file.Path,java.nio.file.Path,java.util.Optional,com.facebook.buck.util.PatternsMatcher)}

        -   #### UnarchiveStep

                public UnarchiveStep​(ArchiveFormat format,
                                     ProjectFilesystem filesystem,
                                     Path archiveFile,
                                     Path destinationDirectory,
                                     Optional<Path> stripPrefix,
                                     PatternsMatcher entriesToExclude)

            ::: block
            Create an instance of UnarchiveStep
            :::

            [Parameters:]{.paramLabel}
            :   `format` - The type of file that will be extracted
            :   `filesystem` - The filesystem that the archive will be
                extracted into
            :   `archiveFile` - The path to the file to extract
            :   `destinationDirectory` - The directory to extract files
                into
            :   `stripPrefix` - If present, strip this prefix from paths
                inside of the archive
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#execute(com.facebook.buck.core.build.execution.context.ExecutionContext)}

        -   #### execute

            ``` methodSignature
            public StepExecutionResult execute​(ExecutionContext context)
                                        throws IOException,
                                               InterruptedException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `execute` in interface `Step`

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
