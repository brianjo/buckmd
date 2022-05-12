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
[Package]{.packageLabelInType} [com.facebook.buck.features.project.intellij.lang.java](package-summary.html)
:::

## Class ParsingJavaPackageFinder {#class-parsingjavapackagefinder .title title="Class ParsingJavaPackageFinder"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.features.project.intellij.lang.java.ParsingJavaPackageFinder

::: description
-   

    ------------------------------------------------------------------------

        public abstract class ParsingJavaPackageFinder
        extends Object

    ::: block
    Finds the package for a given file by looking at its contents first.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static class `       | `Par                  | ::: block             |
        |                       | singJavaPackageFinder | Convenience class     |
        |                       | .PackagePathResolver` | containing logic for  |
        |                       |                       | dealing with Java     |
        |                       |                       | package directory     |
        |                       |                       | structures and        |
        |                       |                       | package paths.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static class `       | `Parsing              |                       |
        |                       | JavaPackageFinder.Pat |                       |
        |                       | hComponentCountOrder` |                       |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                    Description
          ------------------------------ -------------
          `ParsingJavaPackageFinder()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `stat                 | `preparse​(Jav         | ::: block             |
        | ic JavaPackageFinder` | aFileParser javaFileP | Creates a hybrid      |
        |                       | arser,         Projec | [`Java                |
        |                       | tFilesystem projectFi | PackageFinder`](../.. |
        |                       | lesystem,         com | /../../../jvm/core/Ja |
        |                       | .google.common.collec | vaPackageFinder.html  |
        |                       | t.ImmutableSet<Path>  | "interface in com.fac |
        |                       | filesToParse,         | ebook.buck.jvm.core") |
        |                       |  JavaPackageFinder fa | which will resolve    |
        |                       | llbackPackageFinder)` | packages for the      |
        |                       |                       | selected paths based  |
        |                       |                       | on parsing the source |
        |                       |                       | files and use the     |
        |                       |                       | fallbackPackageFinder |
        |                       |                       | for everything else.  |
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
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### ParsingJavaPackageFinder

                public ParsingJavaPackageFinder()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#preparse(com.facebook.buck.jvm.java.JavaFileParser,com.facebook.buck.io.filesystem.ProjectFilesystem,com.google.common.collect.ImmutableSet,com.facebook.buck.jvm.core.JavaPackageFinder)}

        -   #### preparse

            ``` methodSignature
            public static JavaPackageFinder preparse​(JavaFileParser javaFileParser,
                                                     ProjectFilesystem projectFilesystem,
                                                     com.google.common.collect.ImmutableSet<Path> filesToParse,
                                                     JavaPackageFinder fallbackPackageFinder)
            ```

            ::: block
            Creates a hybrid
            [`JavaPackageFinder`](../../../../../jvm/core/JavaPackageFinder.html "interface in com.facebook.buck.jvm.core")
            which will resolve packages for the selected paths based on
            parsing the source files and use the fallbackPackageFinder
            for everything else.
            :::

            [Parameters:]{.paramLabel}
            :   `javaFileParser` - parser to read Java sources with.
            :   `projectFilesystem` - filesystem.
            :   `filesToParse` - set of files to parse.
            :   `fallbackPackageFinder` - package finder to use when the
                package can\'t be inferred from source.

            [Returns:]{.returnLabel}
            :   the described PackageFinder.
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
