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
[Package]{.packageLabelInType} [com.facebook.buck.android](package-summary.html)
:::

## Class AndroidBinaryGraphEnhancer {#class-androidbinarygraphenhancer .title title="Class AndroidBinaryGraphEnhancer"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.android.AndroidBinaryGraphEnhancer

::: description
-   

    ------------------------------------------------------------------------

        public class AndroidBinaryGraphEnhancer
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `st                   | `add                  | ::: block             |
        | atic com.google.commo | BuildConfigDeps​(Build | If the user specified |
        | n.collect.ImmutableSo | Target originalBuildT | any                   |
        | rtedSet<JavaLibrary>` | arget,                | a                     |
        |                       |     ProjectFilesystem | ndroid_build_config() |
        |                       |  projectFilesystem,   | rules, then we must   |
        |                       |                  com. | add some build rules  |
        |                       | facebook.buck.android | to generate the       |
        |                       | .PackageType packageT | production            |
        |                       | ype,                  | `BuildConfig.class`   |
        |                       |   EnumSet<ExopackageM | files and ensure that |
        |                       | ode> exopackageModes, | they are included in  |
        |                       |                    Bu | the list of           |
        |                       | ildConfigFields build | [`Androi              |
        |                       | ConfigValues,         | dPackageableCollectio |
        |                       |            Optional<S | n.getClasspathEntries |
        |                       | ourcePath> buildConfi | ToDex()`](packageable |
        |                       | gValuesFile,          | /AndroidPackageableCo |
        |                       |           ActionGraph | llection.html#getClas |
        |                       | Builder graphBuilder, | spathEntriesToDex()). |
        |                       |                    Ja | :::                   |
        |                       | vac javac,            |                       |
        |                       |         JavacOptions  |                       |
        |                       | javacOptions,         |                       |
        |                       |            AndroidPac |                       |
        |                       | kageableCollection pa |                       |
        |                       | ckageableCollection)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.facebook.buck.an | `getReso              |                       |
        | droid.AndroidBinaryRe | urcesGraphEnhancer()` |                       |
        | sourcesGraphEnhancer` |                       |                       |
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

        []{#getResourcesGraphEnhancer()}

        -   #### getResourcesGraphEnhancer

            ``` methodSignature
            public com.facebook.buck.android.AndroidBinaryResourcesGraphEnhancer getResourcesGraphEnhancer()
            ```

        []{#addBuildConfigDeps(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.android.PackageType,java.util.EnumSet,com.facebook.buck.rules.coercer.BuildConfigFields,java.util.Optional,com.facebook.buck.core.rules.ActionGraphBuilder,com.facebook.buck.jvm.java.Javac,com.facebook.buck.jvm.java.JavacOptions,com.facebook.buck.android.packageable.AndroidPackageableCollection)}

        -   #### addBuildConfigDeps

            ``` methodSignature
            public static com.google.common.collect.ImmutableSortedSet<JavaLibrary> addBuildConfigDeps​(BuildTarget originalBuildTarget,
                                                                                                       ProjectFilesystem projectFilesystem,
                                                                                                       com.facebook.buck.android.PackageType packageType,
                                                                                                       EnumSet<ExopackageMode> exopackageModes,
                                                                                                       BuildConfigFields buildConfigValues,
                                                                                                       Optional<SourcePath> buildConfigValuesFile,
                                                                                                       ActionGraphBuilder graphBuilder,
                                                                                                       Javac javac,
                                                                                                       JavacOptions javacOptions,
                                                                                                       AndroidPackageableCollection packageableCollection)
            ```

            ::: block
            If the user specified any android_build_config() rules, then
            we must add some build rules to generate the production
            `BuildConfig.class` files and ensure that they are included
            in the list of
            [`AndroidPackageableCollection.getClasspathEntriesToDex()`](packageable/AndroidPackageableCollection.html#getClasspathEntriesToDex()).
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
