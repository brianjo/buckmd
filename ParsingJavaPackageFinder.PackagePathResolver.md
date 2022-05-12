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

-   [Overview](../../../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../../index-all.html)
-   [Help](../../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.features.project.intellij.lang.java](package-summary.html)
:::

## Class ParsingJavaPackageFinder.PackagePathResolver {#class-parsingjavapackagefinder.packagepathresolver .title title="Class ParsingJavaPackageFinder.PackagePathResolver"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.features.project.intellij.lang.java.ParsingJavaPackageFinder.PackagePathResolver

::: description
-   

    Enclosing class:
    :   [ParsingJavaPackageFinder](ParsingJavaPackageFinder.html "class in com.facebook.buck.features.project.intellij.lang.java")

    ------------------------------------------------------------------------

        public static class ParsingJavaPackageFinder.PackagePathResolver
        extends Object

    ::: block
    Convenience class containing logic for dealing with Java package
    directory structures and package paths.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                    Description
          -------------------------------------------------------------------------------------------------------------- -------------
          `PackagePathResolver​(JavaFileParser javaFileParser,                    ProjectFilesystem projectFilesystem)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `Optional<Path>`      | `                     | ::: block             |
        |                       | getPackagePathFromSou | Tries to return the   |
        |                       | rce​(Path sourcePath)` | package path from a   |
        |                       |                       | Java source file.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Path>`      | `getSourceRootFromSou | ::: block             |
        |                       | rce​(Path sourcePath)` | Given a file at       |
        |                       |                       | \`a/b/c/D.java\`, and |
        |                       |                       | full name of the      |
        |                       |                       | class is \`b.c.D\`,   |
        |                       |                       | the source root for   |
        |                       |                       | that file is \`a\`.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

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

        []{#<init>(com.facebook.buck.jvm.java.JavaFileParser,com.facebook.buck.io.filesystem.ProjectFilesystem)}

        -   #### PackagePathResolver

                public PackagePathResolver​(JavaFileParser javaFileParser,
                                           ProjectFilesystem projectFilesystem)

            [Parameters:]{.paramLabel}
            :   `javaFileParser` - parser to read Java sources with.
            :   `projectFilesystem` - filesystem.
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getPackagePathFromSource(java.nio.file.Path)}

        -   #### getPackagePathFromSource

            ``` methodSignature
            public Optional<Path> getPackagePathFromSource​(Path sourcePath)
            ```

            ::: block
            Tries to return the package path from a Java source file.
            Returns empty if the file could not be parsed.
            :::

            [Parameters:]{.paramLabel}
            :   `sourcePath` - path to the java source file.

            [Returns:]{.returnLabel}
            :   the parsed path.

        []{#getSourceRootFromSource(java.nio.file.Path)}

        -   #### getSourceRootFromSource

            ``` methodSignature
            public Optional<Path> getSourceRootFromSource​(Path sourcePath)
            ```

            ::: block
            Given a file at \`a/b/c/D.java\`, and full name of the class
            is \`b.c.D\`, the source root for that file is \`a\`.
            Returns empty if either the file could not be parsed or the
            directory structure does not match the package.
            :::

            [Parameters:]{.paramLabel}
            :   `sourcePath` - path to the java source file.

            [Returns:]{.returnLabel}
            :   the path to source root.
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

-   [Overview](../../../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../../index-all.html)
-   [Help](../../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../../allclasses.html)

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
