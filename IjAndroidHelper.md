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

-   [Overview](../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../deprecated-list.html)
-   [Index](../../../../../../index-all.html)
-   [Help](../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.features.project.intellij](package-summary.html)
:::

## Class IjAndroidHelper {#class-ijandroidhelper .title title="Class IjAndroidHelper"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.features.project.intellij.IjAndroidHelper

::: description
-   

    ------------------------------------------------------------------------

        public final class IjAndroidHelper
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static Path`         | `cre                  |                       |
        |                       | ateAndroidGenPath​(Pro |                       |
        |                       | jectFilesystem projec |                       |
        |                       | tFilesystem,          |                       |
        |                       |             IjProject |                       |
        |                       | Config projectConfig, |                       |
        |                       |                       |                       |
        |                       | Path moduleBasePath)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static String`       | `getAn                |                       |
        |                       | droidApkDir​(ProjectFi |                       |
        |                       | lesystem filesystem)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static String`       | `getAndroid           | ::: block             |
        |                       | GenDir​(ProjectFilesys | This directory is     |
        |                       | tem filesystem,       | analogous to the gen/ |
        |                       |            IjProjectC | directory that        |
        |                       | onfig projectConfig)` | IntelliJ would        |
        |                       |                       | produce when building |
        |                       |                       | an Android module.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
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

        []{#getAndroidGenDir(com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.features.project.intellij.model.IjProjectConfig)}

        -   #### getAndroidGenDir

            ``` methodSignature
            public static String getAndroidGenDir​(ProjectFilesystem filesystem,
                                                  IjProjectConfig projectConfig)
            ```

            ::: block
            This directory is analogous to the gen/ directory that
            IntelliJ would produce when building an Android module. It
            contains files such as R.java, BuildConfig.java, and
            Manifest.java.
            By default, IntelliJ generates its gen/ directories in our
            source tree, which would likely mess with the user\'s use of
            `glob(['**&#x2f;*.java'])`. For this reason, we encourage
            users to target
            :::

        []{#getAndroidApkDir(com.facebook.buck.io.filesystem.ProjectFilesystem)}

        -   #### getAndroidApkDir

            ``` methodSignature
            public static String getAndroidApkDir​(ProjectFilesystem filesystem)
            ```

        []{#createAndroidGenPath(com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.features.project.intellij.model.IjProjectConfig,java.nio.file.Path)}

        -   #### createAndroidGenPath

            ``` methodSignature
            public static Path createAndroidGenPath​(ProjectFilesystem projectFilesystem,
                                                    IjProjectConfig projectConfig,
                                                    Path moduleBasePath)
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

-   [Overview](../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../deprecated-list.html)
-   [Index](../../../../../../index-all.html)
-   [Help](../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../allclasses.html)

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
