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

-   [Overview](../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../deprecated-list.html)
-   [Index](../../../../../../index-all.html)
-   [Help](../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.features.apple.projectV2](package-summary.html)
:::

## Class CoreDataResource {#class-coredataresource .title title="Class CoreDataResource"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.features.apple.projectV2.CoreDataResource

::: description
-   

    ------------------------------------------------------------------------

        public class CoreDataResource
        extends Object

    ::: block
    Represents a core data resource from disk.
    A Core Data Resource can be a directory in the event that it
    contains version information. In that case, the path will be the
    root name of the directory and it will contain a nonnull version
    info object which contains all file paths for each versioned file as
    well as a .xccurrentversion file which is an XML file pointing to
    the name of the current file.

    In the event that it is not versioned, the versionInfo will be empty
    and the path itself will simply be the path to the core data model
    object file.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static class `       | `CoreDataResourc      | ::: block             |
        |                       | e.VersionInformation` | Details the version   |
        |                       |                       | information for a     |
        |                       |                       | core data file.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                Description
          ---------------------------------------------------------------------------------------------------------- -------------
          `CoreDataResource​(Path path,                 Optional<CoreDataResource.VersionInformation> versionInfo)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `sta                  | `                     | ::: block             |
        | tic CoreDataResource` | fromResourceArgs​(Appl | Creates a             |
        |                       | eWrapperResourceArg d | CoreDataResource      |
        |                       | ataModel,             | object from an        |
        |                       |      ProjectFilesyste | Ap                    |
        |                       | m projectFilesystem)` | pleWrapperResourceArg |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Path`                | `getPath()`           |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Opti                 | `versionInfo()`       |                       |
        | onal<CoreDataResource |                       |                       |
        | .VersionInformation>` |                       |                       |
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
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(java.nio.file.Path,java.util.Optional)}

        -   #### CoreDataResource

                public CoreDataResource​(Path path,
                                        Optional<CoreDataResource.VersionInformation> versionInfo)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getPath()}

        -   #### getPath

            ``` methodSignature
            public Path getPath()
            ```

        []{#versionInfo()}

        -   #### versionInfo

            ``` methodSignature
            public Optional<CoreDataResource.VersionInformation> versionInfo()
            ```

        []{#fromResourceArgs(com.facebook.buck.apple.AppleWrapperResourceArg,com.facebook.buck.io.filesystem.ProjectFilesystem)}

        -   #### fromResourceArgs

            ``` methodSignature
            public static CoreDataResource fromResourceArgs​(AppleWrapperResourceArg dataModel,
                                                            ProjectFilesystem projectFilesystem)
                                                     throws IOException
            ```

            ::: block
            Creates a CoreDataResource object from an
            AppleWrapperResourceArg
            :::

            [Parameters:]{.paramLabel}
            :   `dataModel` - The resource to convert.
            :   `projectFilesystem` - The file system to use for
                verifying version information.

            [Returns:]{.returnLabel}
            :   A new CoreDataResource with its compiled verison
                information.

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

-   [Overview](../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../deprecated-list.html)
-   [Index](../../../../../../index-all.html)
-   [Help](../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../allclasses.html)

<div>

<div>

JavaScript is disabled on your browser.

</div>

</div>

<div>

-   Summary: 
-   [Nested](#nested.class.summary) \| 
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
