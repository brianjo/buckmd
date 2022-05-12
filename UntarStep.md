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
[Package]{.packageLabelInType} [com.facebook.buck.unarchive](package-summary.html)
:::

## Class UntarStep {#class-untarstep .title title="Class UntarStep"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.unarchive.UnarchiveStep](UnarchiveStep.html "class in com.facebook.buck.unarchive")

    -   -   com.facebook.buck.unarchive.UntarStep

::: description
-   

    All Implemented Interfaces:
    :   `Step`

    ------------------------------------------------------------------------

        public class UntarStep
        extends UnarchiveStep

    ::: block
    A step that extracts tar archives
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        -   []{#fields.inherited.from.class.com.facebook.buck.unarchive.UnarchiveStep}

            ### Fields inherited from class com.facebook.buck.unarchive.[UnarchiveStep](UnarchiveStep.html "class in com.facebook.buck.unarchive")

            `archiveFile, destinationDirectory, entriesToExclude, filesystem`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

        +-----------------------------------+-----------------------------------+
        | Constructor                       | Description                       |
        +===================================+===================================+
        | `UntarS                           | ::: block                         |
        | tep​(ProjectFilesystem filesystem, | Create an instance of UntarStep   |
        |           Path archiveFile,       | :::                               |
        |     Path destinationDirectory,    |                                   |
        |        Optional<Path> stripPrefix |                                   |
        | ,          ArchiveFormat format)` |                                   |
        +-----------------------------------+-----------------------------------+

        : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                                       Description
          ------------------- -------------------------------------------- -------------
          `String`            `getDescription​(ExecutionContext context)`    
          `String`            `getShortName()`                              

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.unarchive.UnarchiveStep}

            ### Methods inherited from class com.facebook.buck.unarchive.[UnarchiveStep](UnarchiveStep.html "class in com.facebook.buck.unarchive")

            `execute`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.io.filesystem.ProjectFilesystem,java.nio.file.Path,java.nio.file.Path,java.util.Optional,com.facebook.buck.util.unarchive.ArchiveFormat)}

        -   #### UntarStep

                public UntarStep​(ProjectFilesystem filesystem,
                                 Path archiveFile,
                                 Path destinationDirectory,
                                 Optional<Path> stripPrefix,
                                 ArchiveFormat format)

            ::: block
            Create an instance of UntarStep
            :::

            [Parameters:]{.paramLabel}
            :   `filesystem` - The filesystem that the archive will be
                extracted into
            :   `archiveFile` - The path to the file to extract
            :   `destinationDirectory` - The directory to extract files
                into
            :   `stripPrefix` - If present, strip this prefix from paths
                inside of the archive
            :   `format` - The format to extract

            [Throws:]{.throwsLabel}
            :   `RuntimeException` - if a non-tar format is provided
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getShortName()}

        -   #### getShortName

            ``` methodSignature
            public String getShortName()
            ```

            [Returns:]{.returnLabel}
            :   a short name/description for the command, such as
                \"javac\". Should fit on one line.

        []{#getDescription(com.facebook.buck.core.build.execution.context.ExecutionContext)}

        -   #### getDescription

            ``` methodSignature
            public String getDescription​(ExecutionContext context)
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
-   Field \| 
-   [Constr](#constructor.detail) \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
