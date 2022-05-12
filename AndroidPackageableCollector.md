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
[Package]{.packageLabelInType} [com.facebook.buck.android.packageable](package-summary.html)
:::

## Class AndroidPackageableCollector {#class-androidpackageablecollector .title title="Class AndroidPackageableCollector"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.android.packageable.AndroidPackageableCollector

::: description
-   

    ------------------------------------------------------------------------

        public class AndroidPackageableCollector
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 Description
          ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `AndroidPackageableCollector​(BuildTarget collectionRoot)`                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    
          `AndroidPackageableCollector​(BuildTarget collectionRoot,                            com.google.common.collect.ImmutableSet<BuildTarget> buildTargetsToExcludeFromDex,                            APKModuleGraph apkModuleGraph)`                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             
          `AndroidPackageableCollector​(BuildTarget collectionRoot,                            com.google.common.collect.ImmutableSet<BuildTarget> buildTargetsToExcludeFromDex,                            APKModuleGraph apkModuleGraph,                            AndroidPackageableFilter androidPackageableFilter)`                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               
          `AndroidPackageableCollector​(BuildTarget collectionRoot,                            com.google.common.collect.ImmutableSet<BuildTarget> buildTargetsToExcludeFromDex,                            com.google.common.collect.ImmutableSet<BuildTarget> resourcesToExclude,                            com.google.common.collect.ImmutableCollection<SourcePath> nativeLibsToExclude,                            com.google.common.collect.ImmutableCollection<NativeLinkableGroup> nativeLinkablesToExcludeGroup,                            com.google.common.collect.ImmutableCollection<SourcePath> nativeLibAssetsToExclude,                            com.google.common.collect.ImmutableCollection<NativeLinkableGroup> nativeLinkableGroupAssetsToExclude,                            APKModuleGraph apkModuleGraph,                            AndroidPackageableFilter androidPackageableFilter)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `Android              | `                     |                       |
        | PackageableCollector` | addAssetsDirectory​(Bu |                       |
        |                       | ildTarget owner,      |                       |
        |                       |               SourceP |                       |
        |                       | ath assetsDirectory)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `addBui               |                       |
        |                       | ldConfig​(BuildTarget  |                       |
        |                       | owner,                |                       |
        |                       | String javaPackage,   |                       |
        |                       |              BuildCon |                       |
        |                       | figFields constants)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Android              | `addClasspathEntry    |                       |
        | PackageableCollector` | ​(HasJavaClassHashes h |                       |
        |                       | asJavaClassHashes,    |                       |
        |                       |                Source |                       |
        |                       | Path classpathEntry)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Android              | `addManifes           | ::: block             |
        | PackageableCollector` | tPiece​(BuildTarget ow | add a manifest piece  |
        |                       | ner,                  | associated with the   |
        |                       | SourcePath manifest)` | target owner.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Android              | `addNativeLib         |                       |
        | PackageableCollector` | AssetsDirectory​(Build |                       |
        |                       | Target owner,         |                       |
        |                       |                     S |                       |
        |                       | ourcePath assetsDir)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Android              | `addNa                |                       |
        | PackageableCollector` | tiveLibsDirectory​(Bui |                       |
        |                       | ldTarget owner,       |                       |
        |                       |                  Sour |                       |
        |                       | cePath nativeLibDir)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Android              | `addNativeLibsD       | ::: block             |
        | PackageableCollector` | irectoryForSystemLoad | Add a directory       |
        |                       | er​(BuildTarget owner, | containing native     |
        |                       |                       | libraries that must   |
        |                       |                  Sour | be packaged in a      |
        |                       | cePath nativeLibDir)` | standard location so  |
        |                       |                       | that they are         |
        |                       |                       | accessible via the    |
        |                       |                       | system library        |
        |                       |                       | loader.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Android              | `addNativeLinkable    |                       |
        | PackageableCollector` | ​(NativeLinkableGroup  |                       |
        |                       | nativeLinkableGroup)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Android              | `a                    |                       |
        | PackageableCollector` | ddNativeLinkableAsset |                       |
        |                       | ​(NativeLinkableGroup  |                       |
        |                       | nativeLinkableGroup)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `a                    | ::: block             |
        |                       | ddPackageables​(Iterab | Add packageables      |
        |                       | le<AndroidPackageable | :::                   |
        |                       | > packageables,       |                       |
        |                       |           BuildRuleRe |                       |
        |                       | solver ruleResolver)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Android              | `addPathToThi         |                       |
        | PackageableCollector` | rdPartyJar​(BuildTarge |                       |
        |                       | t owner,              |                       |
        |                       |           SourcePath  |                       |
        |                       | pathToThirdPartyJar)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Android              | `addProguardConfig​(   |                       |
        | PackageableCollector` | BuildTarget owner,    |                       |
        |                       |                Source |                       |
        |                       | Path proguardConfig)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Android              | `                     |                       |
        | PackageableCollector` | addResourceDirectory​( |                       |
        |                       | BuildTarget owner,    |                       |
        |                       |                   Sou |                       |
        |                       | rcePath resourceDir)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Android              | `addStringWhit        |                       |
        | PackageableCollector` | elistedResourceDirect |                       |
        |                       | ory​(BuildTarget owner |                       |
        |                       | ,                     |                       |
        |                       |                   Sou |                       |
        |                       | rcePath resourceDir)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidP             | `build()`             |                       |
        | ackageableCollection` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static Iterable      | `getPa                | ::: block             |
        | <AndroidPackageable>` | ckageableRules​(Iterab | Returns all           |
        |                       | le<BuildRule> rules)` | [`Build               |
        |                       |                       | Rule`](../../core/rul |
        |                       |                       | es/BuildRule.html "in |
        |                       |                       | terface in com.facebo |
        |                       |                       | ok.buck.core.rules")s |
        |                       |                       | of the given rules    |
        |                       |                       | that are              |
        |                       |                       | [`AndroidPackagea     |
        |                       |                       | ble`](AndroidPackagea |
        |                       |                       | ble.html "interface i |
        |                       |                       | n com.facebook.buck.a |
        |                       |                       | ndroid.packageable"). |
        |                       |                       | :::                   |
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

        []{#<init>(com.facebook.buck.core.model.BuildTarget)}

        -   #### AndroidPackageableCollector

                public AndroidPackageableCollector​(BuildTarget collectionRoot)

        []{#<init>(com.facebook.buck.core.model.BuildTarget,com.google.common.collect.ImmutableSet,com.facebook.buck.android.apkmodule.APKModuleGraph)}

        -   #### AndroidPackageableCollector

                public AndroidPackageableCollector​(BuildTarget collectionRoot,
                                                   com.google.common.collect.ImmutableSet<BuildTarget> buildTargetsToExcludeFromDex,
                                                   APKModuleGraph apkModuleGraph)

        []{#<init>(com.facebook.buck.core.model.BuildTarget,com.google.common.collect.ImmutableSet,com.facebook.buck.android.apkmodule.APKModuleGraph,com.facebook.buck.android.packageable.AndroidPackageableFilter)}

        -   #### AndroidPackageableCollector

                public AndroidPackageableCollector​(BuildTarget collectionRoot,
                                                   com.google.common.collect.ImmutableSet<BuildTarget> buildTargetsToExcludeFromDex,
                                                   APKModuleGraph apkModuleGraph,
                                                   AndroidPackageableFilter androidPackageableFilter)

        []{#<init>(com.facebook.buck.core.model.BuildTarget,com.google.common.collect.ImmutableSet,com.google.common.collect.ImmutableSet,com.google.common.collect.ImmutableCollection,com.google.common.collect.ImmutableCollection,com.google.common.collect.ImmutableCollection,com.google.common.collect.ImmutableCollection,com.facebook.buck.android.apkmodule.APKModuleGraph,com.facebook.buck.android.packageable.AndroidPackageableFilter)}

        -   #### AndroidPackageableCollector

                public AndroidPackageableCollector​(BuildTarget collectionRoot,
                                                   com.google.common.collect.ImmutableSet<BuildTarget> buildTargetsToExcludeFromDex,
                                                   com.google.common.collect.ImmutableSet<BuildTarget> resourcesToExclude,
                                                   com.google.common.collect.ImmutableCollection<SourcePath> nativeLibsToExclude,
                                                   com.google.common.collect.ImmutableCollection<NativeLinkableGroup> nativeLinkablesToExcludeGroup,
                                                   com.google.common.collect.ImmutableCollection<SourcePath> nativeLibAssetsToExclude,
                                                   com.google.common.collect.ImmutableCollection<NativeLinkableGroup> nativeLinkableGroupAssetsToExclude,
                                                   APKModuleGraph apkModuleGraph,
                                                   AndroidPackageableFilter androidPackageableFilter)

            [Parameters:]{.paramLabel}
            :   `resourcesToExclude` - Only relevant to
                [`AndroidInstrumentationApk`](../AndroidInstrumentationApk.html "class in com.facebook.buck.android")
                which needs to remove resources that are already
                included in the
                com.facebook.buck.android.AndroidInstrumentationApkDescription.AbstractAndroidInstrumentationApkDescriptionArg#apk.
                The same goes for native libs and native linkables, and
                their asset counterparts.
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#addPackageables(java.lang.Iterable,com.facebook.buck.core.rules.BuildRuleResolver)}

        -   #### addPackageables

            ``` methodSignature
            public void addPackageables​(Iterable<AndroidPackageable> packageables,
                                        BuildRuleResolver ruleResolver)
            ```

            ::: block
            Add packageables
            :::

        []{#getPackageableRules(java.lang.Iterable)}

        -   #### getPackageableRules

            ``` methodSignature
            public static Iterable<AndroidPackageable> getPackageableRules​(Iterable<BuildRule> rules)
            ```

            ::: block
            Returns all
            [`BuildRule`](../../core/rules/BuildRule.html "interface in com.facebook.buck.core.rules")s
            of the given rules that are
            [`AndroidPackageable`](AndroidPackageable.html "interface in com.facebook.buck.android.packageable").
            Helper for implementations of AndroidPackageable that just
            want to return all of their packagable dependencies.
            :::

        []{#addStringWhitelistedResourceDirectory(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### addStringWhitelistedResourceDirectory

            ``` methodSignature
            public AndroidPackageableCollector addStringWhitelistedResourceDirectory​(BuildTarget owner,
                                                                                     SourcePath resourceDir)
            ```

        []{#addResourceDirectory(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### addResourceDirectory

            ``` methodSignature
            public AndroidPackageableCollector addResourceDirectory​(BuildTarget owner,
                                                                    SourcePath resourceDir)
            ```

        []{#addNativeLibsDirectory(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### addNativeLibsDirectory

            ``` methodSignature
            public AndroidPackageableCollector addNativeLibsDirectory​(BuildTarget owner,
                                                                      SourcePath nativeLibDir)
            ```

        []{#addNativeLibsDirectoryForSystemLoader(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### addNativeLibsDirectoryForSystemLoader

            ``` methodSignature
            public AndroidPackageableCollector addNativeLibsDirectoryForSystemLoader​(BuildTarget owner,
                                                                                     SourcePath nativeLibDir)
            ```

            ::: block
            Add a directory containing native libraries that must be
            packaged in a standard location so that they are accessible
            via the system library loader.
            :::

        []{#addNativeLinkable(com.facebook.buck.cxx.toolchain.nativelink.NativeLinkableGroup)}

        -   #### addNativeLinkable

            ``` methodSignature
            public AndroidPackageableCollector addNativeLinkable​(NativeLinkableGroup nativeLinkableGroup)
            ```

        []{#addNativeLinkableAsset(com.facebook.buck.cxx.toolchain.nativelink.NativeLinkableGroup)}

        -   #### addNativeLinkableAsset

            ``` methodSignature
            public AndroidPackageableCollector addNativeLinkableAsset​(NativeLinkableGroup nativeLinkableGroup)
            ```

        []{#addNativeLibAssetsDirectory(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### addNativeLibAssetsDirectory

            ``` methodSignature
            public AndroidPackageableCollector addNativeLibAssetsDirectory​(BuildTarget owner,
                                                                           SourcePath assetsDir)
            ```

        []{#addAssetsDirectory(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### addAssetsDirectory

            ``` methodSignature
            public AndroidPackageableCollector addAssetsDirectory​(BuildTarget owner,
                                                                  SourcePath assetsDirectory)
            ```

        []{#addProguardConfig(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### addProguardConfig

            ``` methodSignature
            public AndroidPackageableCollector addProguardConfig​(BuildTarget owner,
                                                                 SourcePath proguardConfig)
            ```

        []{#addClasspathEntry(com.facebook.buck.jvm.core.HasJavaClassHashes,com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### addClasspathEntry

            ``` methodSignature
            public AndroidPackageableCollector addClasspathEntry​(HasJavaClassHashes hasJavaClassHashes,
                                                                 SourcePath classpathEntry)
            ```

        []{#addManifestPiece(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### addManifestPiece

            ``` methodSignature
            public AndroidPackageableCollector addManifestPiece​(BuildTarget owner,
                                                                SourcePath manifest)
            ```

            ::: block
            add a manifest piece associated with the target owner. If
            part of a module the manifest pieces will be included in
            both the module manifest and the base apk manifest
            :::

            [Parameters:]{.paramLabel}
            :   `owner` - target that owns the manifest piece
            :   `manifest` - the sourcepath to the manifest piece

            [Returns:]{.returnLabel}
            :   this

        []{#addPathToThirdPartyJar(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### addPathToThirdPartyJar

            ``` methodSignature
            public AndroidPackageableCollector addPathToThirdPartyJar​(BuildTarget owner,
                                                                      SourcePath pathToThirdPartyJar)
            ```

        []{#addBuildConfig(com.facebook.buck.core.model.BuildTarget,java.lang.String,com.facebook.buck.rules.coercer.BuildConfigFields)}

        -   #### addBuildConfig

            ``` methodSignature
            public void addBuildConfig​(BuildTarget owner,
                                       String javaPackage,
                                       BuildConfigFields constants)
            ```

        []{#build()}

        -   #### build

            ``` methodSignature
            public AndroidPackageableCollection build()
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
