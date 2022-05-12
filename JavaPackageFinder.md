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
[Package]{.packageLabelInType} [com.facebook.buck.jvm.core](package-summary.html)
:::

## Interface JavaPackageFinder {#interface-javapackagefinder .title title="Interface JavaPackageFinder"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `DefaultJavaPackageFinder`, `ResourcesRootPackageFinder`

    ------------------------------------------------------------------------

        public interface JavaPackageFinder
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
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

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#findJavaPackageFolder(java.nio.file.Path)}

        -   #### findJavaPackageFolder

            ``` methodSignature
            Path findJavaPackageFolder​(Path pathRelativeToProjectRoot)
            ```

            ::: block
            Given the relative path to a file under the project root,
            return the Java package with which the file is associated.
            For .java files, this is generally obvious, as they contain
            an explicit \"package\" statement. For other files, such as
            resources, other heuristics must be used.
            :::

            [Parameters:]{.paramLabel}
            :   `pathRelativeToProjectRoot` - may be a path to either a
                file or a directory. If a directory, then it must end in
                a slash.

            [Returns:]{.returnLabel}
            :   a path that always ends with a slash, or the empty
                string, indicating the root directory.

        []{#findJavaPackage(java.nio.file.Path)}

        -   #### findJavaPackage

            ``` methodSignature
            String findJavaPackage​(Path pathRelativeToProjectRoot)
            ```

        []{#findJavaPackage(com.facebook.buck.core.model.BuildTarget)}

        -   #### findJavaPackage

            ``` methodSignature
            String findJavaPackage​(BuildTarget buildTarget)
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
