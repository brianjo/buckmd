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
[Package]{.packageLabelInType} [com.facebook.buck.io.filesystem](package-summary.html)
:::

## Interface ProjectFilesystemDelegate {#interface-projectfilesystemdelegate .title title="Interface ProjectFilesystemDelegate"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `DefaultProjectFilesystemDelegate`,
        `EdenProjectFilesystemDelegate`

    ------------------------------------------------------------------------

        public interface ProjectFilesystemDelegate

    ::: block
    Delegate that a
    [`ProjectFilesystem`](ProjectFilesystem.html "interface in com.facebook.buck.io.filesystem")
    can use to leverage a specialized implementation of certain
    filesystem operations, tailored to the underlying filesystem. Use of
    the delegate is often motivated by performance reasons.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                   Method                                                                  Description
          ------------------------------------------------------------------- ----------------------------------------------------------------------- -------------
          `Sha1HashCode`                                                      `computeSha1​(Path pathRelativeToProjectRootOrJustAbsolute)`              
          `boolean`                                                           `exists​(Path pathRelativeToProjectRoot,       LinkOption... options)`    
          `com.google.common.collect.ImmutableMap<String,​? extends Object>`   `getDetailsForLogging()`                                                 
          `Path`                                                              `getPathForRelativePath​(Path pathRelativeToProjectRoot)`                 
          `boolean`                                                           `isExecutable​(Path child)`                                               
          `boolean`                                                           `isSymlink​(Path path)`                                                   

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

        []{#computeSha1(java.nio.file.Path)}

        -   #### computeSha1

            ``` methodSignature
            Sha1HashCode computeSha1​(Path pathRelativeToProjectRootOrJustAbsolute)
                              throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#getPathForRelativePath(java.nio.file.Path)}

        -   #### getPathForRelativePath

            ``` methodSignature
            Path getPathForRelativePath​(Path pathRelativeToProjectRoot)
            ```

        []{#isExecutable(java.nio.file.Path)}

        -   #### isExecutable

            ``` methodSignature
            boolean isExecutable​(Path child)
            ```

        []{#isSymlink(java.nio.file.Path)}

        -   #### isSymlink

            ``` methodSignature
            boolean isSymlink​(Path path)
            ```

        []{#exists(java.nio.file.Path,java.nio.file.LinkOption...)}

        -   #### exists

            ``` methodSignature
            boolean exists​(Path pathRelativeToProjectRoot,
                           LinkOption... options)
            ```

        []{#getDetailsForLogging()}

        -   #### getDetailsForLogging

            ``` methodSignature
            com.google.common.collect.ImmutableMap<String,​? extends Object> getDetailsForLogging()
            ```

            [Returns:]{.returnLabel}
            :   details about the delegate suitable for writing to a
                logger. It is recommended that the keys of this map are
                unique in namespace of the things a logger may want to
                log. Values must be
                [`String`](http://docs.oracle.com/javase/7/docs/api/java/lang/String.html?is-external=true "class or interface in java.lang"){.externalLink},
                `int`, or `boolean`.
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
