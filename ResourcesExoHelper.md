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
[Package]{.packageLabelInType} [com.facebook.buck.android.exopackage](package-summary.html)
:::

## Class ResourcesExoHelper {#class-resourcesexohelper .title title="Class ResourcesExoHelper"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.android.exopackage.ResourcesExoHelper

::: description
-   

    ------------------------------------------------------------------------

        public class ResourcesExoHelper
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type   Field             Description
          ------------------- ----------------- -------------
          `static Path`       `RESOURCES_DIR`    

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `com.goog             | `getFilesToInstall()` |                       |
        | le.common.collect.Imm |                       |                       |
        | utableMap<Path,​Path>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static com.goog      | `getFilesToInstall​(co |                       |
        | le.common.collect.Imm | m.google.common.colle |                       |
        | utableMap<Path,​Path>` | ct.ImmutableMap<Strin |                       |
        |                       | g,​Path> filesByHash)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google           | `ge                   |                       |
        | .common.collect.Immut | tMetadataToInstall()` |                       |
        | ableMap<Path,​String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static com.google    | `getResourceFilesBy   | ::: block             |
        | .common.collect.Immut | Hash​(SourcePathResolv | Returns a map of hash |
        | ableMap<String,​Path>` | erAdapter pathResolve | to path for resource  |
        |                       | r,                    | files.                |
        |                       |     ProjectFilesystem | :::                   |
        |                       |  projectFilesystem,   |                       |
        |                       |                       |                       |
        |                       | java.util.stream.Stre |                       |
        |                       | am<ExopackagePathAndH |                       |
        |                       | ash> resourcesPaths)` |                       |
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
    -   []{#field.detail}

        ### Field Detail

        []{#RESOURCES_DIR}

        -   #### RESOURCES_DIR

                public static final Path RESOURCES_DIR
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getFilesToInstall(com.google.common.collect.ImmutableMap)}

        -   #### getFilesToInstall

            ``` methodSignature
            public static com.google.common.collect.ImmutableMap<Path,​Path> getFilesToInstall​(com.google.common.collect.ImmutableMap<String,​Path> filesByHash)
            ```

        []{#getResourceFilesByHash(com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter,com.facebook.buck.io.filesystem.ProjectFilesystem,java.util.stream.Stream)}

        -   #### getResourceFilesByHash

            ``` methodSignature
            public static com.google.common.collect.ImmutableMap<String,​Path> getResourceFilesByHash​(SourcePathResolverAdapter pathResolver,
                                                                                                           ProjectFilesystem projectFilesystem,
                                                                                                           java.util.stream.Stream<ExopackagePathAndHash> resourcesPaths)
            ```

            ::: block
            Returns a map of hash to path for resource files.
            :::

        []{#getFilesToInstall()}

        -   #### getFilesToInstall

            ``` methodSignature
            public com.google.common.collect.ImmutableMap<Path,​Path> getFilesToInstall()
            ```

        []{#getMetadataToInstall()}

        -   #### getMetadataToInstall

            ``` methodSignature
            public com.google.common.collect.ImmutableMap<Path,​String> getMetadataToInstall()
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
