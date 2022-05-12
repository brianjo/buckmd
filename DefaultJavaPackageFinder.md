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

## Class DefaultJavaPackageFinder {#class-defaultjavapackagefinder .title title="Class DefaultJavaPackageFinder"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.jvm.java.DefaultJavaPackageFinder

::: description
-   

    All Implemented Interfaces:
    :   `JavaPackageFinder`

    ------------------------------------------------------------------------

        public class DefaultJavaPackageFinder
        extends Object
        implements JavaPackageFinder
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                        Description
          -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `DefaultJavaPackageFinder​(ProjectFilesystem projectFilesystem,                         com.google.common.collect.ImmutableSortedSet<String> pathsFromRoot,                         com.google.common.collect.ImmutableSet<String> pathElements)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static Defa          | `cre                  |                       |
        | ultJavaPackageFinder` | ateDefaultJavaPackage |                       |
        |                       | Finder​(ProjectFilesys |                       |
        |                       | tem projectFilesystem |                       |
        |                       | ,                     |                       |
        |                       |            Iterable<S |                       |
        |                       | tring> pathPatterns)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `findJavaPackage​(Buil |                       |
        |                       | dTarget buildTarget)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `findJa               |                       |
        |                       | vaPackage​(Path pathRe |                       |
        |                       | lativeToProjectRoot)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Path`                | `findJavaPack         | ::: block             |
        |                       | ageFolder​(Path pathRe | Given the relative    |
        |                       | lativeToProjectRoot)` | path to a file under  |
        |                       |                       | the project root,     |
        |                       |                       | return the Java       |
        |                       |                       | package with which    |
        |                       |                       | the file is           |
        |                       |                       | associated.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static String`       | `findJavaPac          |                       |
        |                       | kageWithPackageFolder |                       |
        |                       | ​(Path packageFolder)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.g                | `getPathElements()`   |                       |
        | oogle.common.collect. |                       |                       |
        | ImmutableSet<String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.          | `getPathsFromRoot()`  |                       |
        | common.collect.Immuta |                       |                       |
        | bleSortedSet<String>` |                       |                       |
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

        []{#<init>(com.facebook.buck.io.filesystem.ProjectFilesystem,com.google.common.collect.ImmutableSortedSet,com.google.common.collect.ImmutableSet)}

        -   #### DefaultJavaPackageFinder

                public DefaultJavaPackageFinder​(ProjectFilesystem projectFilesystem,
                                                com.google.common.collect.ImmutableSortedSet<String> pathsFromRoot,
                                                com.google.common.collect.ImmutableSet<String> pathElements)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#findJavaPackageFolder(java.nio.file.Path)}

        -   #### findJavaPackageFolder

            ``` methodSignature
            public Path findJavaPackageFolder​(Path pathRelativeToProjectRoot)
            ```

            ::: block
            [Description copied from
            interface: `JavaPackageFinder`]{.descfrmTypeLabel}
            :::

            ::: block
            Given the relative path to a file under the project root,
            return the Java package with which the file is associated.
            For .java files, this is generally obvious, as they contain
            an explicit \"package\" statement. For other files, such as
            resources, other heuristics must be used.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `findJavaPackageFolder` in interface `JavaPackageFinder`

            [Parameters:]{.paramLabel}
            :   `pathRelativeToProjectRoot` - may be a path to either a
                file or a directory. If a directory, then it must end in
                a slash.

            [Returns:]{.returnLabel}
            :   a path that always ends with a slash, or the empty
                string, indicating the root directory.

        []{#getPathsFromRoot()}

        -   #### getPathsFromRoot

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedSet<String> getPathsFromRoot()
            ```

        []{#getPathElements()}

        -   #### getPathElements

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<String> getPathElements()
            ```

        []{#createDefaultJavaPackageFinder(com.facebook.buck.io.filesystem.ProjectFilesystem,java.lang.Iterable)}

        -   #### createDefaultJavaPackageFinder

            ``` methodSignature
            public static DefaultJavaPackageFinder createDefaultJavaPackageFinder​(ProjectFilesystem projectFilesystem,
                                                                                  Iterable<String> pathPatterns)
            ```

            [Parameters:]{.paramLabel}
            :   `pathPatterns` - elements that start with a slash must
                be prefix patterns; all other elements indicate
                individual directory names (and therefore cannot contain
                slashes).

        []{#findJavaPackage(java.nio.file.Path)}

        -   #### findJavaPackage

            ``` methodSignature
            public String findJavaPackage​(Path pathRelativeToProjectRoot)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `findJavaPackage` in interface `JavaPackageFinder`

        []{#findJavaPackage(com.facebook.buck.core.model.BuildTarget)}

        -   #### findJavaPackage

            ``` methodSignature
            public String findJavaPackage​(BuildTarget buildTarget)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `findJavaPackage` in interface `JavaPackageFinder`

        []{#findJavaPackageWithPackageFolder(java.nio.file.Path)}

        -   #### findJavaPackageWithPackageFolder

            ``` methodSignature
            public static String findJavaPackageWithPackageFolder​(Path packageFolder)
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
