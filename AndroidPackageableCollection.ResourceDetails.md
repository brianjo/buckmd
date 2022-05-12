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

## Class AndroidPackageableCollection.ResourceDetails {#class-androidpackageablecollection.resourcedetails .title title="Class AndroidPackageableCollection.ResourceDetails"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.android.packageable.AndroidPackageableCollection.ResourceDetails

::: description
-   

    Enclosing interface:
    :   [AndroidPackageableCollection](AndroidPackageableCollection.html "interface in com.facebook.buck.android.packageable")

    ------------------------------------------------------------------------

        public abstract static class AndroidPackageableCollection.ResourceDetails
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor           Description
          --------------------- -------------
          `ResourceDetails()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `abstract com.google  | `getR                 | ::: block             |
        | .common.collect.Immut | esourceDirectories()` | A list of \"res\"     |
        | ableList<SourcePath>` |                       | directories that      |
        |                       |                       | should be passed to   |
        |                       |                       | the aapt command to   |
        |                       |                       | build the APK, sorted |
        |                       |                       | topologically.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `abstr                | `getRe                | ::: block             |
        | act Set<BuildTarget>` | sourcesWithEmptyResBu | Unlike                |
        |                       | tNonEmptyAssetsDir()` | [`getReso             |
        |                       |                       | urcesWithNonEmptyResD |
        |                       |                       | ir()`](#getResourcesW |
        |                       |                       | ithNonEmptyResDir()), |
        |                       |                       | these resources only  |
        |                       |                       | contain \"assets\".   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `abstract com.google. | `getResources         | ::: block             |
        | common.collect.Immuta | WithNonEmptyResDir()` | A list of build       |
        | bleList<BuildTarget>` |                       | targets belonging to  |
        |                       |                       | [`AndroidResource`]   |
        |                       |                       | (../AndroidResource.h |
        |                       |                       | tml "class in com.fac |
        |                       |                       | ebook.buck.android")s |
        |                       |                       | with non-empty        |
        |                       |                       | \"res\" directory,    |
        |                       |                       | sorted topologically. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `abstract com.googl   | `getWhiteliste        | ::: block             |
        | e.common.collect.Immu | dStringDirectories()` | A set of \"res\"      |
        | tableSet<SourcePath>` |                       | directories that      |
        |                       |                       | contain               |
        |                       |                       | \"whitelisted\"       |
        |                       |                       | strings, i.e.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `hasResources()`      |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
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

        -   #### ResourceDetails

                public ResourceDetails()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getResourceDirectories()}

        -   #### getResourceDirectories

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableList<SourcePath> getResourceDirectories()
            ```

            ::: block
            A list of \"res\" directories that should be passed to the
            aapt command to build the APK, sorted topologically.
            :::

        []{#getWhitelistedStringDirectories()}

        -   #### getWhitelistedStringDirectories

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableSet<SourcePath> getWhitelistedStringDirectories()
            ```

            ::: block
            A set of \"res\" directories that contain \"whitelisted\"
            strings, i.e. the strings-as-assets resource filter does not
            affect these directories.
            :::

        []{#getResourcesWithNonEmptyResDir()}

        -   #### getResourcesWithNonEmptyResDir

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableList<BuildTarget> getResourcesWithNonEmptyResDir()
            ```

            ::: block
            A list of build targets belonging to
            [`AndroidResource`](../AndroidResource.html "class in com.facebook.buck.android")s
            with non-empty \"res\" directory, sorted topologically. Note
            that these are
            [`BuildTarget`](../../core/model/BuildTarget.html "class in com.facebook.buck.core.model")s
            to avoid introducing a circular dependency.
            :::

        []{#getResourcesWithEmptyResButNonEmptyAssetsDir()}

        -   #### getResourcesWithEmptyResButNonEmptyAssetsDir

            ``` methodSignature
            public abstract Set<BuildTarget> getResourcesWithEmptyResButNonEmptyAssetsDir()
            ```

            ::: block
            Unlike
            [`getResourcesWithNonEmptyResDir()`](#getResourcesWithNonEmptyResDir()),
            these resources only contain \"assets\".
            :::

        []{#hasResources()}

        -   #### hasResources

            ``` methodSignature
            @Derived
            public boolean hasResources()
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
