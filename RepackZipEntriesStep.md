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
[Package]{.packageLabelInType} [com.facebook.buck.zip](package-summary.html)
:::

## Class RepackZipEntriesStep {#class-repackzipentriesstep .title title="Class RepackZipEntriesStep"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.zip.RepackZipEntriesStep

::: description
-   

    All Implemented Interfaces:
    :   `Step`

    ------------------------------------------------------------------------

        public class RepackZipEntriesStep
        extends Object
        implements Step

    ::: block
    A command that creates a copy of a ZIP archive, making sure that
    certain user-specified entries are packed with a certain compression
    level.
    Can be used, for instance, to force the resources.arsc file in an
    Android .apk to be compressed.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

        +-----------------------------------+-----------------------------------+
        | Constructor                       | Description                       |
        +===================================+===================================+
        | `Re                               | ::: block                         |
        | packZipEntriesStep​(ProjectFilesys | Creates a                         |
        | tem filesystem,                   | [`RepackZipEntriesS               |
        |    Path inputPath,                | tep`](RepackZipEntriesStep.html " |
        |       Path outputPath,            | class in com.facebook.buck.zip"). |
        |           com.google.common.colle | :::                               |
        | ct.ImmutableSet<String> entries)` |                                   |
        +-----------------------------------+-----------------------------------+
        | `RepackZipEntriesStep​(Projec      | ::: block                         |
        | tFilesystem filesystem,           | Creates a                         |
        |            Path inputPath,        | [`RepackZipEntriesS               |
        |               Path outputPath,    | tep`](RepackZipEntriesStep.html " |
        |                   com.google.comm | class in com.facebook.buck.zip"). |
        | on.collect.ImmutableSet<String> e | :::                               |
        | ntries,                     ZipCo |                                   |
        | mpressionLevel compressionLevel)` |                                   |
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
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.io.filesystem.ProjectFilesystem,java.nio.file.Path,java.nio.file.Path,com.google.common.collect.ImmutableSet)}

        -   #### RepackZipEntriesStep

                public RepackZipEntriesStep​(ProjectFilesystem filesystem,
                                            Path inputPath,
                                            Path outputPath,
                                            com.google.common.collect.ImmutableSet<String> entries)

            ::: block
            Creates a
            [`RepackZipEntriesStep`](RepackZipEntriesStep.html "class in com.facebook.buck.zip").
            A temporary directory will be created and used to extract
            entries. Entries will be packed with the maximum compression
            level.
            :::

            [Parameters:]{.paramLabel}
            :   `inputPath` - input archive
            :   `outputPath` - destination archive
            :   `entries` - files to repack (e.g.
                `ImmutableSet.of("resources.arsc")`)

        []{#<init>(com.facebook.buck.io.filesystem.ProjectFilesystem,java.nio.file.Path,java.nio.file.Path,com.google.common.collect.ImmutableSet,com.facebook.buck.util.zip.ZipCompressionLevel)}

        -   #### RepackZipEntriesStep

                public RepackZipEntriesStep​(ProjectFilesystem filesystem,
                                            Path inputPath,
                                            Path outputPath,
                                            com.google.common.collect.ImmutableSet<String> entries,
                                            ZipCompressionLevel compressionLevel)

            ::: block
            Creates a
            [`RepackZipEntriesStep`](RepackZipEntriesStep.html "class in com.facebook.buck.zip").
            :::

            [Parameters:]{.paramLabel}
            :   `inputPath` - input archive
            :   `outputPath` - destination archive
            :   `entries` - files to repack (e.g.
                `ImmutableSet.of("resources.arsc")`)
            :   `compressionLevel` - the level of compression to use
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
