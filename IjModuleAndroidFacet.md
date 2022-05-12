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

-   [Overview](../../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../index-all.html)
-   [Help](../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.features.project.intellij.model](package-summary.html)
:::

## Class IjModuleAndroidFacet {#class-ijmoduleandroidfacet .title title="Class IjModuleAndroidFacet"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.features.project.intellij.model.IjModuleAndroidFacet

::: description
-   

    ------------------------------------------------------------------------

        public abstract class IjModuleAndroidFacet
        extends Object

    ::: block
    The information necessary to add the Android facet to the module.
    This essentially means the Java code in the given module is written
    against the Android SDK.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type   Class                            Description
          ------------------- -------------------------------- -------------
          `static class `     `IjModuleAndroidFacet.Builder`    

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                Description
          -------------------------- -------------
          `IjModuleAndroidFacet()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `abstract boolean`    | `a                    |                       |
        |                       | utogenerateSources()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static IjModule      | `builder()`           |                       |
        | AndroidFacet.Builder` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `di                   |                       |
        |                       | scoverPackageName​(And |                       |
        |                       | roidManifestParser an |                       |
        |                       | droidManifestParser)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Path`                | `getA                 |                       |
        |                       | ndroidManifestPath()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstrac              | `get                  |                       |
        | t AndroidProjectType` | AndroidProjectType()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract com         | `getAssetPaths()`     |                       |
        | .google.common.collec |                       |                       |
        | t.ImmutableSet<Path>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Path>`      | `ge                   |                       |
        |                       | tFirstManifestPath()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract Path`       | `getG                 |                       |
        |                       | eneratedSourcePath()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract com         | `getManifestPaths()`  |                       |
        | .google.common.collec |                       |                       |
        | t.ImmutableSet<Path>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `getMinSdkVersion()`  |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract com.g       | `getMinSdkVersions()` |                       |
        | oogle.common.collect. |                       |                       |
        | ImmutableSet<String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstr                | `getPackageName()`    |                       |
        | act Optional<String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abs                  | `get                  |                       |
        | tract Optional<Path>` | ProguardConfigPath()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract com         | `getResourcePaths()`  |                       |
        | .google.common.collec |                       |                       |
        | t.ImmutableSet<Path>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `hasVa                | ::: block             |
        |                       | lidAndroidManifest()` | AndroidManifest.xml   |
        |                       |                       | can be generated when |
        |                       |                       | package name is       |
        |                       |                       | known.                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isAndroidLibrary()`  |                       |
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

        -   #### IjModuleAndroidFacet

                public IjModuleAndroidFacet()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getManifestPaths()}

        -   #### getManifestPaths

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableSet<Path> getManifestPaths()
            ```

            [Returns:]{.returnLabel}
            :   set of paths to all AndroidManifest.xml files.

        []{#getResourcePaths()}

        -   #### getResourcePaths

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableSet<Path> getResourcePaths()
            ```

            [Returns:]{.returnLabel}
            :   paths to resources (usually stuff under the res/
                folder).

        []{#getAssetPaths()}

        -   #### getAssetPaths

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableSet<Path> getAssetPaths()
            ```

            [Returns:]{.returnLabel}
            :   paths to assets (usually stuff under the assets/
                folder).

        []{#getProguardConfigPath()}

        -   #### getProguardConfigPath

            ``` methodSignature
            public abstract Optional<Path> getProguardConfigPath()
            ```

            [Returns:]{.returnLabel}
            :   paths to the proguard configuration.

        []{#isAndroidLibrary()}

        -   #### isAndroidLibrary

            ``` methodSignature
            public boolean isAndroidLibrary()
            ```

            [Returns:]{.returnLabel}
            :   whether or not this is an Android Library. IntelliJ
                identifies libraries using a is_android_library_project
                setting in the module iml to allow other modules which
                depend on it to inherit assets, resources, etc.

        []{#getAndroidProjectType()}

        -   #### getAndroidProjectType

            ``` methodSignature
            public abstract AndroidProjectType getAndroidProjectType()
            ```

        []{#getPackageName()}

        -   #### getPackageName

            ``` methodSignature
            public abstract Optional<String> getPackageName()
            ```

            [Returns:]{.returnLabel}
            :   The package that the R file should be located in. This
                is used by android_resources targets to specify the
                package their resources should referenced via.

        []{#autogenerateSources()}

        -   #### autogenerateSources

            ``` methodSignature
            public abstract boolean autogenerateSources()
            ```

        []{#getMinSdkVersion()}

        -   #### getMinSdkVersion

            ``` methodSignature
            @Lazy
            public Optional<String> getMinSdkVersion()
            ```

            [Returns:]{.returnLabel}
            :   The minimum Android SDK version supported.

        []{#discoverPackageName(com.facebook.buck.features.project.intellij.lang.android.AndroidManifestParser)}

        -   #### discoverPackageName

            ``` methodSignature
            @Lazy
            public Optional<String> discoverPackageName​(AndroidManifestParser androidManifestParser)
            ```

            [Returns:]{.returnLabel}
            :   either the package name from facet or package name from
                the first manifest

        []{#getFirstManifestPath()}

        -   #### getFirstManifestPath

            ``` methodSignature
            public Optional<Path> getFirstManifestPath()
            ```

        []{#getMinSdkVersions()}

        -   #### getMinSdkVersions

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableSet<String> getMinSdkVersions()
            ```

        []{#getGeneratedSourcePath()}

        -   #### getGeneratedSourcePath

            ``` methodSignature
            public abstract Path getGeneratedSourcePath()
            ```

        []{#hasValidAndroidManifest()}

        -   #### hasValidAndroidManifest

            ``` methodSignature
            @Lazy
            public boolean hasValidAndroidManifest()
            ```

            ::: block
            AndroidManifest.xml can be generated when package name is
            known. Also, it\'s not generated when there is exactly one
            manifest from targets (this manifest will be used in
            IntelliJ project).
            :::

        []{#getAndroidManifestPath()}

        -   #### getAndroidManifestPath

            ``` methodSignature
            @Lazy
            public Path getAndroidManifestPath()
            ```

        []{#builder()}

        -   #### builder

            ``` methodSignature
            public static IjModuleAndroidFacet.Builder builder()
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

-   [Overview](../../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../index-all.html)
-   [Help](../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../allclasses.html)

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
