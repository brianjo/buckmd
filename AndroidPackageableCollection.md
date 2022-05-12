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
[Package]{.packageLabelInType} [com.facebook.buck.android.packageable](package-summary.html)
:::

## Interface AndroidPackageableCollection {#interface-androidpackageablecollection .title title="Interface AndroidPackageableCollection"}
:::

::: contentContainer
::: description
-   

    ------------------------------------------------------------------------

        @Enclosing
        public interface AndroidPackageableCollection

    ::: block
    A collection of Android content that should be included in an
    Android package (apk or aar).
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type   Interface                                        Description
          ------------------- ------------------------------------------------ -------------
          `static class `     `AndroidPackageableCollection.ResourceDetails`    

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `com                  | `getAnd               | ::: block             |
        | .google.common.collec | roidManifestPieces()` | Android manifests to  |
        | t.ImmutableMultimap<A |                       | merge with the        |
        | PKModule,​SourcePath>` |                       | manifest skeleton.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com                  | `ge                   | ::: block             |
        | .google.common.collec | tAssetsDirectories()` | Directories           |
        | t.ImmutableMultimap<A |                       | containing assets to  |
        | PKModule,​SourcePath>` |                       | be included directly  |
        |                       |                       | in the apk, under the |
        |                       |                       | \"assets\" directory. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `co                   | `getBuildConfigs()`   |                       |
        | m.google.common.colle |                       |                       |
        | ct.ImmutableMap<Strin |                       |                       |
        | g,​BuildConfigFields>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `jav                  | `getClassNam          | ::: block             |
        | a.util.function.Suppl | esToHashesSupplier()` | See                   |
        | ier<com.google.common |                       | [`Has                 |
        | .collect.ImmutableMap |                       | JavaClassHashes.getCl |
        | <String,​com.google.co |                       | assNamesToHashes()`]( |
        | mmon.hash.HashCode>>` |                       | ../../jvm/core/HasJav |
        |                       |                       | aClassHashes.html#get |
        |                       |                       | ClassNamesToHashes()) |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.googl            | `getCla               | ::: block             |
        | e.common.collect.Immu | sspathEntriesToDex()` | Java classes (jars)   |
        | tableSet<SourcePath>` |                       | to include in the     |
        |                       |                       | package.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Set<BuildTarget>`    | `get                  | ::: block             |
        |                       | JavaLibrariesToDex()` | [`Java                |
        |                       |                       | Library`](../../jvm/c |
        |                       |                       | ore/JavaLibrary.html  |
        |                       |                       | "interface in com.fac |
        |                       |                       | ebook.buck.jvm.core") |
        |                       |                       | rules whose output    |
        |                       |                       | will be dexed and     |
        |                       |                       | included in the       |
        |                       |                       | package.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com                  | `getModuleMappedCla   | ::: block             |
        | .google.common.collec | sspathEntriesToDex()` | Java classes to       |
        | t.ImmutableMultimap<A |                       | include in the        |
        | PKModule,​SourcePath>` |                       | package sorted into   |
        |                       |                       | modules               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com                  | `getNativeLi          | ::: block             |
        | .google.common.collec | bAssetsDirectories()` | Directories           |
        | t.ImmutableMultimap<A |                       | containing native     |
        | PKModule,​SourcePath>` |                       | libraries to be used  |
        |                       |                       | as assets.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com                  | `getNat               | ::: block             |
        | .google.common.collec | iveLibsDirectories()` | Directories           |
        | t.ImmutableMultimap<A |                       | containing native     |
        | PKModule,​SourcePath>` |                       | libraries.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.google           | `                     | ::: block             |
        | .common.collect.Immut | getNativeLibsDirector | Directories           |
        | ableList<SourcePath>` | iesForSystemLoader()` | containing native     |
        |                       |                       | libraries which must  |
        |                       |                       | be loadable by the    |
        |                       |                       | system loader.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.c         | `                     | ::: block             |
        | ommon.collect.Immutab | getNativeLinkables()` | Native libraries      |
        | leMultimap<APKModule, |                       | mapped from modules.  |
        | ​NativeLinkableGroup>` |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.c         | `getNat               | ::: block             |
        | ommon.collect.Immutab | iveLinkablesAssets()` | Native libraries to   |
        | leMultimap<APKModule, |                       | be packaged as        |
        | ​NativeLinkableGroup>` |                       | assets.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.googl            | `getNo                | ::: block             |
        | e.common.collect.Immu | DxClasspathEntries()` | Java classes that     |
        | tableSet<SourcePath>` |                       | were used during      |
        |                       |                       | compilation, but      |
        |                       |                       | don\'t got into the   |
        |                       |                       | package.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com                  | `getPat               | ::: block             |
        | .google.common.collec | hsToThirdPartyJars()` | Prebuilt/third-party  |
        | t.ImmutableMultimap<A |                       | jars to be included   |
        | PKModule,​SourcePath>` |                       | in the package.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.googl            | `                     | ::: block             |
        | e.common.collect.Immu | getProguardConfigs()` | Proguard              |
        | tableSet<SourcePath>` |                       | configurations to     |
        |                       |                       | include when running  |
        |                       |                       | release builds.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.          | `                     |                       |
        | common.collect.Immuta | getResourceDetails()` |                       |
        | bleMap<APKModule,​Andr |                       |                       |
        | oidPackageableCollect |                       |                       |
        | ion.ResourceDetails>` |                       |                       |
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

        []{#getResourceDetails()}

        -   #### getResourceDetails

            ``` methodSignature
            com.google.common.collect.ImmutableMap<APKModule,​AndroidPackageableCollection.ResourceDetails> getResourceDetails()
            ```

        []{#getNativeLinkables()}

        -   #### getNativeLinkables

            ``` methodSignature
            com.google.common.collect.ImmutableMultimap<APKModule,​NativeLinkableGroup> getNativeLinkables()
            ```

            ::: block
            Native libraries mapped from modules.
            :::

        []{#getNativeLinkablesAssets()}

        -   #### getNativeLinkablesAssets

            ``` methodSignature
            com.google.common.collect.ImmutableMultimap<APKModule,​NativeLinkableGroup> getNativeLinkablesAssets()
            ```

            ::: block
            Native libraries to be packaged as assets.
            :::

        []{#getNativeLibsDirectories()}

        -   #### getNativeLibsDirectories

            ``` methodSignature
            com.google.common.collect.ImmutableMultimap<APKModule,​SourcePath> getNativeLibsDirectories()
            ```

            ::: block
            Directories containing native libraries.
            :::

        []{#getNativeLibAssetsDirectories()}

        -   #### getNativeLibAssetsDirectories

            ``` methodSignature
            com.google.common.collect.ImmutableMultimap<APKModule,​SourcePath> getNativeLibAssetsDirectories()
            ```

            ::: block
            Directories containing native libraries to be used as
            assets.
            :::

        []{#getNativeLibsDirectoriesForSystemLoader()}

        -   #### getNativeLibsDirectoriesForSystemLoader

            ``` methodSignature
            com.google.common.collect.ImmutableList<SourcePath> getNativeLibsDirectoriesForSystemLoader()
            ```

            ::: block
            Directories containing native libraries which must be
            loadable by the system loader. Since these cannot be in a
            separate module, we use a list instead of a map
            :::

        []{#getAssetsDirectories()}

        -   #### getAssetsDirectories

            ``` methodSignature
            com.google.common.collect.ImmutableMultimap<APKModule,​SourcePath> getAssetsDirectories()
            ```

            ::: block
            Directories containing assets to be included directly in the
            apk, under the \"assets\" directory.
            :::

        []{#getProguardConfigs()}

        -   #### getProguardConfigs

            ``` methodSignature
            com.google.common.collect.ImmutableSet<SourcePath> getProguardConfigs()
            ```

            ::: block
            Proguard configurations to include when running release
            builds.
            :::

        []{#getClasspathEntriesToDex()}

        -   #### getClasspathEntriesToDex

            ``` methodSignature
            com.google.common.collect.ImmutableSet<SourcePath> getClasspathEntriesToDex()
            ```

            ::: block
            Java classes (jars) to include in the package.
            :::

        []{#getAndroidManifestPieces()}

        -   #### getAndroidManifestPieces

            ``` methodSignature
            com.google.common.collect.ImmutableMultimap<APKModule,​SourcePath> getAndroidManifestPieces()
            ```

            ::: block
            Android manifests to merge with the manifest skeleton.
            :::

        []{#getModuleMappedClasspathEntriesToDex()}

        -   #### getModuleMappedClasspathEntriesToDex

            ``` methodSignature
            com.google.common.collect.ImmutableMultimap<APKModule,​SourcePath> getModuleMappedClasspathEntriesToDex()
            ```

            ::: block
            Java classes to include in the package sorted into modules
            :::

        []{#getNoDxClasspathEntries()}

        -   #### getNoDxClasspathEntries

            ``` methodSignature
            com.google.common.collect.ImmutableSet<SourcePath> getNoDxClasspathEntries()
            ```

            ::: block
            Java classes that were used during compilation, but don\'t
            got into the package. This is only used by \"buck project\".
            (It\'s existence is kind of contrary to the purpose of this
            class, but we make exceptions for \"buck project\".)
            :::

        []{#getBuildConfigs()}

        -   #### getBuildConfigs

            ``` methodSignature
            com.google.common.collect.ImmutableMap<String,​BuildConfigFields> getBuildConfigs()
            ```

        []{#getPathsToThirdPartyJars()}

        -   #### getPathsToThirdPartyJars

            ``` methodSignature
            com.google.common.collect.ImmutableMultimap<APKModule,​SourcePath> getPathsToThirdPartyJars()
            ```

            ::: block
            Prebuilt/third-party jars to be included in the package. For
            apks, their resources will be placed directly in the apk.
            :::

        []{#getJavaLibrariesToDex()}

        -   #### getJavaLibrariesToDex

            ``` methodSignature
            Set<BuildTarget> getJavaLibrariesToDex()
            ```

            ::: block
            [`JavaLibrary`](../../jvm/core/JavaLibrary.html "interface in com.facebook.buck.jvm.core")
            rules whose output will be dexed and included in the
            package.
            :::

        []{#getClassNamesToHashesSupplier()}

        -   #### getClassNamesToHashesSupplier

            ``` methodSignature
            java.util.function.Supplier<com.google.common.collect.ImmutableMap<String,​com.google.common.hash.HashCode>> getClassNamesToHashesSupplier()
            ```

            ::: block
            See
            [`HasJavaClassHashes.getClassNamesToHashes()`](../../jvm/core/HasJavaClassHashes.html#getClassNamesToHashes())
            :::
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
