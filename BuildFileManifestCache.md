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
[Package]{.packageLabelInType} [com.facebook.buck.parser.manifest](package-summary.html)
:::

## Class BuildFileManifestCache {#class-buildfilemanifestcache .title title="Class BuildFileManifestCache"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.parser.manifest.BuildFileManifestCache

::: description
-   

    All Implemented Interfaces:
    :   `GraphEngineCache<BuildPackagePathToBuildFileManifestKey,​BuildFileManifest>`

    ------------------------------------------------------------------------

        public class BuildFileManifestCache
        extends Object
        implements GraphEngineCache<BuildPackagePathToBuildFileManifestKey,​BuildFileManifest>

    ::: block
    Stores
    [`BuildFileManifest`](../api/BuildFileManifest.html "class in com.facebook.buck.parser.api")
    for each parsed build file
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static class `       | `BuildFileManif       | ::: block             |
        |                       | estCache.Invalidator` | Subscribes to         |
        |                       |                       | watchman event and    |
        |                       |                       | invalidates internal  |
        |                       |                       | state of a provided   |
        |                       |                       | [`BuildFileManif      |
        |                       |                       | estCache`](BuildFileM |
        |                       |                       | anifestCache.html "cl |
        |                       |                       | ass in com.facebook.b |
        |                       |                       | uck.parser.manifest") |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `Optiona              | `get​(Bu               | ::: block             |
        | l<BuildFileManifest>` | ildPackagePathToBuild | Optionally returns    |
        |                       | FileManifestKey key)` | the cached result     |
        |                       |                       | given the key         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `BuildFileManif       | `getInvalidator()`    |                       |
        | estCache.Invalidator` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static Bu            | `of​(Path superRootP   | ::: block             |
        | ildFileManifestCache` | ath,   Path rootPath, | Create a new instance |
        |                       |    Path buildFileName | of                    |
        |                       | ,   ProjectFilesystem | [`BuildFileManif      |
        |                       | View fileSystemView)` | estCache`](BuildFileM |
        |                       |                       | anifestCache.html "cl |
        |                       |                       | ass in com.facebook.b |
        |                       |                       | uck.parser.manifest") |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `put​(                 | ::: block             |
        |                       | BuildPackagePathToBui | Offers the given key  |
        |                       | ldFileManifestKey key | and value for caching |
        |                       | ,    BuildFileManifes | :::                   |
        |                       | t buildFileManifest)` |                       |
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
    -   []{#method.detail}

        ### Method Detail

        []{#of(java.nio.file.Path,java.nio.file.Path,java.nio.file.Path,com.facebook.buck.io.filesystem.ProjectFilesystemView)}

        -   #### of

            ``` methodSignature
            public static BuildFileManifestCache of​(Path superRootPath,
                                                    Path rootPath,
                                                    Path buildFileName,
                                                    ProjectFilesystemView fileSystemView)
            ```

            ::: block
            Create a new instance of
            [`BuildFileManifestCache`](BuildFileManifestCache.html "class in com.facebook.buck.parser.manifest")
            :::

            [Parameters:]{.paramLabel}
            :   `superRootPath` - Absolute path to the cell root folder
                which contains all other cells. All files and includes
                should be descendants of this path.
            :   `rootPath` - Absolute path to the root folder for which
                files and subfolders are cached, this is usually the
                root path of the cell. It may be the same path as
                `superRootPath` or a subfolder of it.
            :   `buildFileName` - File name of the build file (for
                example, BUCK) in a form of a
                [`Path`](http://docs.oracle.com/javase/7/docs/api/java/nio/file/Path.html?is-external=true "class or interface in java.nio.file"){.externalLink}
            :   `fileSystemView` -
                [`ProjectFilesystemView`](../../io/filesystem/ProjectFilesystemView.html "interface in com.facebook.buck.io.filesystem")
                that is used to physically access files, used for
                invalidations

        []{#get(com.facebook.buck.parser.manifest.BuildPackagePathToBuildFileManifestKey)}

        -   #### get

            ``` methodSignature
            public Optional<BuildFileManifest> get​(BuildPackagePathToBuildFileManifestKey key)
            ```

            ::: block
            [Description copied from
            interface: `GraphEngineCache`]{.descfrmTypeLabel}
            :::

            ::: block
            Optionally returns the cached result given the key
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `get` in
                interface `GraphEngineCache<BuildPackagePathToBuildFileManifestKey,​BuildFileManifest>`

            [Parameters:]{.paramLabel}
            :   `key` - The desired key

            [Returns:]{.returnLabel}
            :   the result if cached, otherwise an empty Optional

        []{#put(com.facebook.buck.parser.manifest.BuildPackagePathToBuildFileManifestKey,com.facebook.buck.parser.api.BuildFileManifest)}

        -   #### put

            ``` methodSignature
            public void put​(BuildPackagePathToBuildFileManifestKey key,
                            BuildFileManifest buildFileManifest)
            ```

            ::: block
            [Description copied from
            interface: `GraphEngineCache`]{.descfrmTypeLabel}
            :::

            ::: block
            Offers the given key and value for caching
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `put` in
                interface `GraphEngineCache<BuildPackagePathToBuildFileManifestKey,​BuildFileManifest>`

            [Parameters:]{.paramLabel}
            :   `key` - the key to cache
            :   `buildFileManifest` - the value to cache

        []{#getInvalidator()}

        -   #### getInvalidator

            ``` methodSignature
            public BuildFileManifestCache.Invalidator getInvalidator()
            ```

            [Returns:]{.returnLabel}
            :   class that listens to watchman events and invalidates
                internal cache state
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
