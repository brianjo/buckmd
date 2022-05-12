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
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.io.file](package-summary.html)
:::

## Class MostFiles {#class-mostfiles .title title="Class MostFiles"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.io.file.MostFiles

::: description
-   

    ------------------------------------------------------------------------

        public final class MostFiles
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type   Class                                  Description
          ------------------- -------------------------------------- -------------
          `static class `     `MostFiles.DeleteRecursivelyOptions`    

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type   Field       Description
          ------------------- ----------- -------------
          `static long`       `S_IFDIR`    
          `static long`       `S_IFLNK`    
          `static long`       `S_IFREG`    

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static boolean`      | `concatenateFiles     | ::: block             |
        |                       | ​(Path dest,           | Concatenates the      |
        |                       |        Iterable<Path> | contents of one or    |
        |                       |  pathsToConcatenate)` | more files.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static void`         | `copyRecursively​(P    | ::: block             |
        |                       | ath fromPath,         | Recursively copies    |
        |                       |         Path toPath)` | all files under       |
        |                       |                       | `fromPath` to         |
        |                       |                       | `toPath`.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static void`         | `copyRecursively​(Pat  | ::: block             |
        |                       | h fromPath,           | Recursively copies    |
        |                       |       Path toPath,    | all files under       |
        |                       |              java.uti | `fromPath` to         |
        |                       | l.function.Function<P | `toPath`.             |
        |                       | ath,​Path> transform)` | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static void`         | `                     |                       |
        |                       | copyRecursively​(Path  |                       |
        |                       | fromPath,             |                       |
        |                       |     Path toPath,      |                       |
        |                       |            java.util. |                       |
        |                       | function.Function<Pat |                       |
        |                       | h,​Path> transform,    |                       |
        |                       |              java.uti |                       |
        |                       | l.function.Function<P |                       |
        |                       | ath,​Boolean> filter)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static void`         | `deleteRe             |                       |
        |                       | cursively​(Path path)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static void`         | `deleteRecursivel     |                       |
        |                       | yIfExists​(Path path)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static void`         | `deleteRecursivel     |                       |
        |                       | yWithOptions​(Path pat |                       |
        |                       | h,                    |                       |
        |                       |           EnumSet<Mos |                       |
        |                       | tFiles.DeleteRecursiv |                       |
        |                       | elyOptions> options)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static void`         | `makeE                | ::: block             |
        |                       | xecutable​(Path file)` | Tries to make the     |
        |                       |                       | specified file        |
        |                       |                       | executable.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static String`       | `s                    | ::: block             |
        |                       | anitize​(String name)` | Given a file name,    |
        |                       |                       | replace any illegal   |
        |                       |                       | characters from it.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static void`         | `sortFilesByAcce      | ::: block             |
        |                       | ssTime​(File[] files)` | Does an in-place sort |
        |                       |                       | of the specified      |
        |                       |                       | `files` array.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static void`         | `writeLin             | ::: block             |
        |                       | esToFile​(Iterable<Str | Writes the specified  |
        |                       | ing> lines,           | lines to the          |
        |                       |        AbsPath file)` | specified file,       |
        |                       |                       | encoded as UTF-8.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static void`         | `write                | ::: block             |
        |                       | LinesToFile​(Iterable< | Writes the specified  |
        |                       | String> lines,        | lines to the          |
        |                       |           Path file)` | specified file,       |
        |                       |                       | encoded as UTF-8.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
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

        []{#S_IFDIR}

        -   #### S_IFDIR

                public static final long S_IFDIR

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.io.file.MostFiles.S_IFDIR)

        []{#S_IFREG}

        -   #### S_IFREG

                public static final long S_IFREG

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.io.file.MostFiles.S_IFREG)

        []{#S_IFLNK}

        -   #### S_IFLNK

                public static final long S_IFLNK

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.io.file.MostFiles.S_IFLNK)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#deleteRecursivelyIfExists(java.nio.file.Path)}

        -   #### deleteRecursivelyIfExists

            ``` methodSignature
            public static void deleteRecursivelyIfExists​(Path path)
                                                  throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#copyRecursively(java.nio.file.Path,java.nio.file.Path)}

        -   #### copyRecursively

            ``` methodSignature
            public static void copyRecursively​(Path fromPath,
                                               Path toPath)
                                        throws IOException
            ```

            ::: block
            Recursively copies all files under `fromPath` to `toPath`.
            :::

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#copyRecursively(java.nio.file.Path,java.nio.file.Path,java.util.function.Function)}

        -   #### copyRecursively

            ``` methodSignature
            public static void copyRecursively​(Path fromPath,
                                               Path toPath,
                                               java.util.function.Function<Path,​Path> transform)
                                        throws IOException
            ```

            ::: block
            Recursively copies all files under `fromPath` to `toPath`.
            The `transform` will be applied after the destination path
            for a file has been relativized. This will remove any
            existing files in the toPath if there is a conflict.
            :::

            [Parameters:]{.paramLabel}
            :   `fromPath` - item to copy
            :   `toPath` - destination of copy
            :   `transform` - renaming function to apply when copying.
                If this function returns null, then the file is not
                copied.

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#copyRecursively(java.nio.file.Path,java.nio.file.Path,java.util.function.Function,java.util.function.Function)}

        -   #### copyRecursively

            ``` methodSignature
            public static void copyRecursively​(Path fromPath,
                                               Path toPath,
                                               java.util.function.Function<Path,​Path> transform,
                                               java.util.function.Function<Path,​Boolean> filter)
                                        throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#deleteRecursively(java.nio.file.Path)}

        -   #### deleteRecursively

            ``` methodSignature
            public static void deleteRecursively​(Path path)
                                          throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#deleteRecursivelyWithOptions(java.nio.file.Path,java.util.EnumSet)}

        -   #### deleteRecursivelyWithOptions

            ``` methodSignature
            public static void deleteRecursivelyWithOptions​(Path path,
                                                            EnumSet<MostFiles.DeleteRecursivelyOptions> options)
                                                     throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#writeLinesToFile(java.lang.Iterable,java.nio.file.Path)}

        -   #### writeLinesToFile

            ``` methodSignature
            public static void writeLinesToFile​(Iterable<String> lines,
                                                Path file)
                                         throws IOException
            ```

            ::: block
            Writes the specified lines to the specified file, encoded as
            UTF-8.
            :::

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#writeLinesToFile(java.lang.Iterable,com.facebook.buck.core.filesystems.AbsPath)}

        -   #### writeLinesToFile

            ``` methodSignature
            public static void writeLinesToFile​(Iterable<String> lines,
                                                AbsPath file)
                                         throws IOException
            ```

            ::: block
            Writes the specified lines to the specified file, encoded as
            UTF-8.
            :::

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#sortFilesByAccessTime(java.io.File[])}

        -   #### sortFilesByAccessTime

            ``` methodSignature
            public static void sortFilesByAccessTime​(File[] files)
            ```

            ::: block
            Does an in-place sort of the specified `files` array. Most
            recently accessed files will be at the front of the array
            when sorted.
            :::

        []{#makeExecutable(java.nio.file.Path)}

        -   #### makeExecutable

            ``` methodSignature
            public static void makeExecutable​(Path file)
                                       throws IOException
            ```

            ::: block
            Tries to make the specified file executable. For file
            systems that do support the POSIX-style permissions, the
            executable permission is set for each category of users that
            already has the read permission.
            If the file system does not support the executable
            permission or the operation fails, a `java.io.IOException`
            is thrown.
            :::

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#sanitize(java.lang.String)}

        -   #### sanitize

            ``` methodSignature
            public static String sanitize​(String name)
            ```

            ::: block
            Given a file name, replace any illegal characters from it.
            :::

            [Parameters:]{.paramLabel}
            :   `name` - The file name to sanitize

            [Returns:]{.returnLabel}
            :   a properly sanitized filename

        []{#concatenateFiles(java.nio.file.Path,java.lang.Iterable)}

        -   #### concatenateFiles

            ``` methodSignature
            public static boolean concatenateFiles​(Path dest,
                                                   Iterable<Path> pathsToConcatenate)
                                            throws IOException
            ```

            ::: block
            Concatenates the contents of one or more files.
            :::

            [Parameters:]{.paramLabel}
            :   `dest` - The path to which the concatenated files\'
                contents are written.
            :   `pathsToConcatenate` - The paths whose contents are
                concatenated to `dest`.

            [Returns:]{.returnLabel}
            :   `true` if any data was concatenated to `dest`, `false`
                otherwise.

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
-   [Field](#field.summary) \| 
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
-   Constr \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
