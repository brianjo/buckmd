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
[Package]{.packageLabelInType} [com.facebook.buck.android.aapt](package-summary.html)
:::

## Class MiniAapt {#class-miniaapt .title title="Class MiniAapt"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.android.aapt.MiniAapt

::: description
-   

    All Implemented Interfaces:
    :   `Step`

    ------------------------------------------------------------------------

        public class MiniAapt
        extends Object
        implements Step

    ::: block
    Step which parses resources in an android `res` directory and
    compiles them into a `  R.txt` file, following the exact same format
    as the Android build tool `aapt`.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type   Class                               Description
          ------------------- ----------------------------------- -------------
          `static class `     `MiniAapt.ResourceCollectionType`    

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Field                 | Description           |
        +=======================+=======================+=======================+
        | `static com.go        | `IGN                  | ::: block             |
        | ogle.common.collect.I | ORED_FILE_EXTENSIONS` | See                   |
        | mmutableList<String>` |                       | [`Aa                  |
        |                       |                       | ptStep`](../AaptStep. |
        |                       |                       | html "class in com.fa |
        |                       |                       | cebook.buck.android") |
        |                       |                       | for a list of files   |
        |                       |                       | that we ignore.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                                                                                          Description
          ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `MiniAapt​(SourcePathResolverAdapter resolver,         ProjectFilesystem filesystem,         SourcePath resDirectory,         Path pathToTextSymbolsFile,         com.google.common.collect.ImmutableSet<Path> pathsToSymbolsOfDeps)`                                                                                                                  
          `MiniAapt​(SourcePathResolverAdapter resolver,         ProjectFilesystem filesystem,         SourcePath resDirectory,         Path pathToOutputFile,         com.google.common.collect.ImmutableSet<Path> pathsToSymbolsOfDeps,         boolean isGrayscaleImageProcessingEnabled,         MiniAapt.ResourceCollectionType resourceCollectionType)`    

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

        []{#IGNORED_FILE_EXTENSIONS}

        -   #### IGNORED_FILE_EXTENSIONS

                public static final com.google.common.collect.ImmutableList<String> IGNORED_FILE_EXTENSIONS

            ::: block
            See
            [`AaptStep`](../AaptStep.html "class in com.facebook.buck.android")
            for a list of files that we ignore.
            :::
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.sourcepath.SourcePath,java.nio.file.Path,com.google.common.collect.ImmutableSet)}

        -   #### MiniAapt

                public MiniAapt​(SourcePathResolverAdapter resolver,
                                ProjectFilesystem filesystem,
                                SourcePath resDirectory,
                                Path pathToTextSymbolsFile,
                                com.google.common.collect.ImmutableSet<Path> pathsToSymbolsOfDeps)

        []{#<init>(com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.sourcepath.SourcePath,java.nio.file.Path,com.google.common.collect.ImmutableSet,boolean,com.facebook.buck.android.aapt.MiniAapt.ResourceCollectionType)}

        -   #### MiniAapt

                public MiniAapt​(SourcePathResolverAdapter resolver,
                                ProjectFilesystem filesystem,
                                SourcePath resDirectory,
                                Path pathToOutputFile,
                                com.google.common.collect.ImmutableSet<Path> pathsToSymbolsOfDeps,
                                boolean isGrayscaleImageProcessingEnabled,
                                MiniAapt.ResourceCollectionType resourceCollectionType)
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
