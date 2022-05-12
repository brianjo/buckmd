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
[Package]{.packageLabelInType} [com.facebook.buck.jvm.java](package-summary.html)
:::

## Class AccumulateClassNamesStep {#class-accumulateclassnamesstep .title title="Class AccumulateClassNamesStep"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.jvm.java.AccumulateClassNamesStep

::: description
-   

    All Implemented Interfaces:
    :   `Step`

    ------------------------------------------------------------------------

        public class AccumulateClassNamesStep
        extends Object
        implements Step

    ::: block
    [`Step`](../../step/Step.html "interface in com.facebook.buck.step")
    that takes a directory or zip of `.class` files and traverses it to
    get the total set of `.class` files included by the directory or
    zip.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                 Description
          ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `AccumulateClassNamesStep​(ProjectFilesystem filesystem,                         Optional<Path> pathToJarOrClassesDirectory,                         Path whereClassNamesShouldBeWritten)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                                                         Method                                                                                                                              Description
          --------------------------------------------------------------------------------------------------------- ----------------------------------------------------------------------------------------------------------------------------------- -------------
          `static Optional<com.google.common.collect.ImmutableSortedMap<String,​com.google.common.hash.HashCode>>`   `calculateClassHashes​(ExecutionContext context,                     ProjectFilesystem filesystem,                     Path path)`    
          `StepExecutionResult`                                                                                     `execute​(ExecutionContext context)`                                                                                                  
          `String`                                                                                                  `getDescription​(ExecutionContext context)`                                                                                           
          `String`                                                                                                  `getShortName()`                                                                                                                     
          `static com.google.common.collect.ImmutableSortedMap<String,​com.google.common.hash.HashCode>`             `parseClassHashes​(List<String> lines)`                                                                                               

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
          Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
          .tableTab}[[Instance
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

        []{#<init>(com.facebook.buck.io.filesystem.ProjectFilesystem,java.util.Optional,java.nio.file.Path)}

        -   #### AccumulateClassNamesStep

                public AccumulateClassNamesStep​(ProjectFilesystem filesystem,
                                                Optional<Path> pathToJarOrClassesDirectory,
                                                Path whereClassNamesShouldBeWritten)

            [Parameters:]{.paramLabel}
            :   `pathToJarOrClassesDirectory` - Where to look for .class
                files. If absent, then an empty file will be written to
                `whereClassNamesShouldBeWritten`.
            :   `whereClassNamesShouldBeWritten` - Path to a file where
                an alphabetically sorted list of class files and
                corresponding SHA-1 hashes of their contents will be
                written.
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

        []{#calculateClassHashes(com.facebook.buck.core.build.execution.context.ExecutionContext,com.facebook.buck.io.filesystem.ProjectFilesystem,java.nio.file.Path)}

        -   #### calculateClassHashes

            ``` methodSignature
            public static Optional<com.google.common.collect.ImmutableSortedMap<String,​com.google.common.hash.HashCode>> calculateClassHashes​(ExecutionContext context,
                                                                                                                                                    ProjectFilesystem filesystem,
                                                                                                                                                    Path path)
            ```

            [Returns:]{.returnLabel}
            :   an Optional that will be absent if there was an error.

        []{#parseClassHashes(java.util.List)}

        -   #### parseClassHashes

            ``` methodSignature
            public static com.google.common.collect.ImmutableSortedMap<String,​com.google.common.hash.HashCode> parseClassHashes​(List<String> lines)
            ```

            [Parameters:]{.paramLabel}
            :   `lines` - that were written in the same format output by
                [`execute(ExecutionContext)`](#execute(com.facebook.buck.core.build.execution.context.ExecutionContext)).
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
