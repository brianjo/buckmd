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
[Package]{.packageLabelInType} [com.facebook.buck.rules.keys](package-summary.html)
:::

## Class DependencyFileEntry {#class-dependencyfileentry .title title="Class DependencyFileEntry"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.rules.keys.DependencyFileEntry

::: description
-   

    ------------------------------------------------------------------------

        public abstract class DependencyFileEntry
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor               Description
          ------------------------- -------------
          `DependencyFileEntry()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `protected void`      | `check()`             |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static               | `from                 |                       |
        |  DependencyFileEntry` | SourcePath​(SourcePath |                       |
        |                       |  sourcePath,          |                       |
        |                       |       SourcePathResol |                       |
        |                       | verAdapter resolver)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static Path`         | `ge                   | ::: block             |
        |                       | tPathToFile​(SourcePat | Gets the path to the  |
        |                       | hResolverAdapter reso | file.                 |
        |                       | lver,              So | :::                   |
        |                       | urcePath sourcePath)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static               | `of​(Path pathToFile)` |                       |
        |  DependencyFileEntry` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static               | `of​(                  |                       |
        |  DependencyFileEntry` | Path pathToFile,   Op |                       |
        |                       | tional<? extends Path |                       |
        |                       | > pathWithinArchive)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract Path`       | `pathToFile()`        |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abs                  | `pathWithinArchive()` |                       |
        | tract Optional<Path>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
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

        []{#<init>()}

        -   #### DependencyFileEntry

                public DependencyFileEntry()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#pathToFile()}

        -   #### pathToFile

            ``` methodSignature
            public abstract Path pathToFile()
            ```

        []{#pathWithinArchive()}

        -   #### pathWithinArchive

            ``` methodSignature
            public abstract Optional<Path> pathWithinArchive()
            ```

        []{#check()}

        -   #### check

            ``` methodSignature
            @Check
            protected void check()
            ```

        []{#getPathToFile(com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter,com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### getPathToFile

            ``` methodSignature
            public static Path getPathToFile​(SourcePathResolverAdapter resolver,
                                             SourcePath sourcePath)
            ```

            ::: block
            Gets the path to the file. This would be the value of
            DependencyFileEntry.pathToFile() if the SourcePath is
            converted to a DependencyFileEntry.
            :::

        []{#fromSourcePath(com.facebook.buck.core.sourcepath.SourcePath,com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter)}

        -   #### fromSourcePath

            ``` methodSignature
            public static DependencyFileEntry fromSourcePath​(SourcePath sourcePath,
                                                             SourcePathResolverAdapter resolver)
            ```

        []{#of(java.nio.file.Path,java.util.Optional)}

        -   #### of

            ``` methodSignature
            public static DependencyFileEntry of​(Path pathToFile,
                                                 Optional<? extends Path> pathWithinArchive)
            ```

        []{#of(java.nio.file.Path)}

        -   #### of

            ``` methodSignature
            public static DependencyFileEntry of​(Path pathToFile)
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
