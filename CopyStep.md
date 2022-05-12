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
-   Field \| 
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.step.fs](package-summary.html)
:::

## Class CopyStep {#class-copystep .title title="Class CopyStep"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.step.fs.CopyStep

::: description
-   

    All Implemented Interfaces:
    :   `Step`

    ------------------------------------------------------------------------

        public class CopyStep
        extends Object
        implements Step
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static class `       | `Co                   | ::: block             |
        |                       | pyStep.DirectoryMode` | When copying a        |
        |                       |                       | directory, this       |
        |                       |                       | specifies whether     |
        |                       |                       | only the contents of  |
        |                       |                       | the directory should  |
        |                       |                       | be copied, or if the  |
        |                       |                       | directory itself      |
        |                       |                       | should be included.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `StepExecutionResult` | `execute​(Execu        |                       |
        |                       | tionContext context)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static CopyStep`     | `f                    | ::: block             |
        |                       | orDirectory​(ProjectFi | Creates a CopyStep    |
        |                       | lesystem filesystem,  | which recursively     |
        |                       |             Path sour | copies a directory    |
        |                       | ce,             Path  | from \'source\' to    |
        |                       | destination,          | \'destination\'.      |
        |                       |     CopyStep.Director | :::                   |
        |                       | yMode directoryMode)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static CopyStep`     | `forFile​(ProjectFiles | ::: block             |
        |                       | ystem filesystem,     | Creates a CopyStep    |
        |                       |     Path source,      | which copies a single |
        |                       |    Path destination)` | file from \'source\'  |
        |                       |                       | to \'destination\'.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getDescription​(Execu |                       |
        |                       | tionContext context)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getShortName()`      |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isRecursive()`       |                       |
        +-----------------------+-----------------------+-----------------------+

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
    -   []{#method.detail}

        ### Method Detail

        []{#forFile(com.facebook.buck.io.filesystem.ProjectFilesystem,java.nio.file.Path,java.nio.file.Path)}

        -   #### forFile

            ``` methodSignature
            public static CopyStep forFile​(ProjectFilesystem filesystem,
                                           Path source,
                                           Path destination)
            ```

            ::: block
            Creates a CopyStep which copies a single file from
            \'source\' to \'destination\'.
            :::

        []{#forDirectory(com.facebook.buck.io.filesystem.ProjectFilesystem,java.nio.file.Path,java.nio.file.Path,com.facebook.buck.step.fs.CopyStep.DirectoryMode)}

        -   #### forDirectory

            ``` methodSignature
            public static CopyStep forDirectory​(ProjectFilesystem filesystem,
                                                Path source,
                                                Path destination,
                                                CopyStep.DirectoryMode directoryMode)
            ```

            ::: block
            Creates a CopyStep which recursively copies a directory from
            \'source\' to \'destination\'. See
            [`CopyStep.DirectoryMode`](CopyStep.DirectoryMode.html "enum in com.facebook.buck.step.fs")
            for options to control the copy.
            :::

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

        []{#isRecursive()}

        -   #### isRecursive

            ``` methodSignature
            public boolean isRecursive()
            ```

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
-   Field \| 
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   Constr \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
