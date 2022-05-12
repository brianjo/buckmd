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
[Package]{.packageLabelInType} [com.facebook.buck.util.unarchive](package-summary.html)
:::

## Class Unzip {#class-unzip .title title="Class Unzip"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.util.unarchive.Unarchiver](Unarchiver.html "class in com.facebook.buck.util.unarchive")

    -   -   com.facebook.buck.util.unarchive.Unzip

::: description
-   

    ------------------------------------------------------------------------

        public class Unzip
        extends Unarchiver

    ::: block
    A simple utility class that extracts zip files
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor   Description
          ------------- -------------
          `Unzip()`      

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `com                  | `extractArchive​(Pat   | ::: block             |
        | .google.common.collec | h archiveFile,        | Unzips a file to a    |
        | t.ImmutableSet<Path>` |         ProjectFilesy | destination and       |
        |                       | stem filesystem,      | returns the paths of  |
        |                       |           Path relati | the written files.    |
        |                       | vePath,               | :::                   |
        |                       |  Optional<Path> strip |                       |
        |                       | Prefix,               |                       |
        |                       |  PatternsMatcher entr |                       |
        |                       | iesToExclude,         |                       |
        |                       |        ExistingFileMo |                       |
        |                       | de existingFileMode)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static com           | `getZipMembers​(Path   | ::: block             |
        | .google.common.collec | archiveAbsolutePath)` | Gets a set of files   |
        | t.ImmutableSet<Path>` |                       | that are contained in |
        |                       |                       | an archive            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.util.unarchive.Unarchiver}

            ### Methods inherited from class com.facebook.buck.util.unarchive.[Unarchiver](Unarchiver.html "class in com.facebook.buck.util.unarchive")

            `extractArchive, extractArchive, extractArchive, extractArchive`

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

        []{#<init>()}

        -   #### Unzip

                public Unzip()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#extractArchive(java.nio.file.Path,com.facebook.buck.io.filesystem.ProjectFilesystem,java.nio.file.Path,java.util.Optional,com.facebook.buck.util.PatternsMatcher,com.facebook.buck.util.unarchive.ExistingFileMode)}

        -   #### extractArchive

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<Path> extractArchive​(Path archiveFile,
                                                                               ProjectFilesystem filesystem,
                                                                               Path relativePath,
                                                                               Optional<Path> stripPrefix,
                                                                               PatternsMatcher entriesToExclude,
                                                                               ExistingFileMode existingFileMode)
                                                                        throws IOException
            ```

            ::: block
            Unzips a file to a destination and returns the paths of the
            written files.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `extractArchive` in class `Unarchiver`

            [Parameters:]{.paramLabel}
            :   `archiveFile` - The path to the archive
            :   `filesystem` - The filesystem that will be extracted
                into
            :   `relativePath` - The path relative to the filesystem to
                extract files into
            :   `stripPrefix` - If provided, only files under this
                prefix will be extracted. This prefix prefix will also
                be removed from the destination path. e.g.
                foo.tar.gz/foo/bar/baz with a prefix of foo will extract
                bar/baz into the destination directory. If not provided,
                no stripping is done.
            :   `entriesToExclude` - Entries that match this matcher
                will not be extracted
            :   `existingFileMode` - How to handle existing files

            [Returns:]{.returnLabel}
            :   A list of paths to files that were created (not
                directories)

            [Throws:]{.throwsLabel}
            :   `IOException` - If the archive could not be extracted
                for any reason

        []{#getZipMembers(java.nio.file.Path)}

        -   #### getZipMembers

            ``` methodSignature
            public static com.google.common.collect.ImmutableSet<Path> getZipMembers​(Path archiveAbsolutePath)
                                                                              throws IOException
            ```

            ::: block
            Gets a set of files that are contained in an archive
            :::

            [Parameters:]{.paramLabel}
            :   `archiveAbsolutePath` - The absolute path to the archive

            [Returns:]{.returnLabel}
            :   A set of files (not directories) that are contained in
                the zip file

            [Throws:]{.throwsLabel}
            :   `IOException` - If there is an error reading the archive
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
