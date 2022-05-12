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
[Package]{.packageLabelInType} [com.facebook.buck.edenfs](package-summary.html)
:::

## Class EdenProjectFilesystemDelegate {#class-edenprojectfilesystemdelegate .title title="Class EdenProjectFilesystemDelegate"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.edenfs.EdenProjectFilesystemDelegate

::: description
-   

    All Implemented Interfaces:
    :   `ProjectFilesystemDelegate`

    ------------------------------------------------------------------------

        public final class EdenProjectFilesystemDelegate
        extends Object
        implements ProjectFilesystemDelegate
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                     Description
          --------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `EdenProjectFilesystemDelegate​(EdenMount mount,                              ProjectFilesystemDelegate delegate,                              Config config)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                   Method                                                                   Description
          ------------------------------------------------------------------- ------------------------------------------------------------------------ -------------
          `Sha1HashCode`                                                      `computeSha1​(Path pathRelativeToProjectRootOrJustAbsolute)`               
          `boolean`                                                           `exists​(Path pathRelativeToProjectRoot,       LinkOption... options)`     
          `com.google.common.collect.ImmutableMap<String,​? extends Object>`   `getDetailsForLogging()`                                                  
          `Path`                                                              `getPathForRelativePath​(Path pathRelativeToProjectRootOrJustAbsolute)`    
          `boolean`                                                           `isExecutable​(Path child)`                                                
          `boolean`                                                           `isSymlink​(Path path)`                                                    

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

        []{#<init>(com.facebook.buck.edenfs.EdenMount,com.facebook.buck.io.filesystem.ProjectFilesystemDelegate,com.facebook.buck.util.config.Config)}

        -   #### EdenProjectFilesystemDelegate

                public EdenProjectFilesystemDelegate​(EdenMount mount,
                                                     ProjectFilesystemDelegate delegate,
                                                     Config config)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getDetailsForLogging()}

        -   #### getDetailsForLogging

            ``` methodSignature
            public com.google.common.collect.ImmutableMap<String,​? extends Object> getDetailsForLogging()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getDetailsForLogging` in
                interface `ProjectFilesystemDelegate`

            [Returns:]{.returnLabel}
            :   details about the delegate suitable for writing to a
                logger. It is recommended that the keys of this map are
                unique in namespace of the things a logger may want to
                log. Values must be
                [`String`](http://docs.oracle.com/javase/7/docs/api/java/lang/String.html?is-external=true "class or interface in java.lang"){.externalLink},
                `int`, or `boolean`.

        []{#computeSha1(java.nio.file.Path)}

        -   #### computeSha1

            ``` methodSignature
            public Sha1HashCode computeSha1​(Path pathRelativeToProjectRootOrJustAbsolute)
                                     throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `computeSha1` in interface `ProjectFilesystemDelegate`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#getPathForRelativePath(java.nio.file.Path)}

        -   #### getPathForRelativePath

            ``` methodSignature
            public Path getPathForRelativePath​(Path pathRelativeToProjectRootOrJustAbsolute)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getPathForRelativePath` in
                interface `ProjectFilesystemDelegate`

        []{#isExecutable(java.nio.file.Path)}

        -   #### isExecutable

            ``` methodSignature
            public boolean isExecutable​(Path child)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `isExecutable` in interface `ProjectFilesystemDelegate`

        []{#isSymlink(java.nio.file.Path)}

        -   #### isSymlink

            ``` methodSignature
            public boolean isSymlink​(Path path)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `isSymlink` in interface `ProjectFilesystemDelegate`

        []{#exists(java.nio.file.Path,java.nio.file.LinkOption...)}

        -   #### exists

            ``` methodSignature
            public boolean exists​(Path pathRelativeToProjectRoot,
                                  LinkOption... options)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `exists` in interface `ProjectFilesystemDelegate`
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
