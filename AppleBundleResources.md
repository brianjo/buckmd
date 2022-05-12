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
[Package]{.packageLabelInType} [com.facebook.buck.apple](package-summary.html)
:::

## Class AppleBundleResources {#class-applebundleresources .title title="Class AppleBundleResources"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.apple.AppleBundleResources

::: description
-   

    All Implemented Interfaces:
    :   `AddsToRuleKey`

    ------------------------------------------------------------------------

        public abstract class AppleBundleResources
        extends Object
        implements AddsToRuleKey

    ::: block
    Resources to be bundled into a bundle.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type   Class                            Description
          ------------------- -------------------------------- -------------
          `static class `     `AppleBundleResources.Builder`    

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                Description
          -------------------------- -------------
          `AppleBundleResources()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static AppleBun      | `builder()`           |                       |
        | dleResources.Builder` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getAll()`            | ::: block             |
        | Iterable<SourcePath>` |                       | Returns all the       |
        |                       |                       | SourcePaths from the  |
        |                       |                       | different types of    |
        |                       |                       | resources.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `SortedSet<App        | `                     | ::: block             |
        | leBundleDestination>` | getAllDestinations()` | All kinds of          |
        |                       |                       | destinations that are |
        |                       |                       | used by paths in this |
        |                       |                       | object.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ab                   | `getDirsCont          | ::: block             |
        | stract com.google.com | ainingResourceDirs()` | Directories whose     |
        | mon.collect.Immutable |                       | contents should be    |
        | Set<SourcePathWithApp |                       | copied into the root  |
        | leBundleDestination>` |                       | of the resources      |
        |                       |                       | subdirectory.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ab                   | `getResourceDirs()`   | ::: block             |
        | stract com.google.com |                       | Directories that      |
        | mon.collect.Immutable |                       | should be copied into |
        | Set<SourcePathWithApp |                       | the bundle as         |
        | leBundleDestination>` |                       | directories of files  |
        |                       |                       | with the same name.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Set<SourcePath>`     | `get                  |                       |
        |                       | ResourceDirsForDestin |                       |
        |                       | ation​(AppleBundleDest |                       |
        |                       | ination destination)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `ab                   | `getResourceFiles()`  | ::: block             |
        | stract com.google.com |                       | Files that are copied |
        | mon.collect.Immutable |                       | to the root of the    |
        | Set<SourcePathWithApp |                       | resources             |
        | leBundleDestination>` |                       | subdirectory.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Set<SourcePath>`     | `getR                 |                       |
        |                       | esourceFilesForDestin |                       |
        |                       | ation​(AppleBundleDest |                       |
        |                       | ination destination)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract com.googl   | `getRe                | ::: block             |
        | e.common.collect.Immu | sourceVariantFiles()` | Resource files with   |
        | tableSet<SourcePath>` |                       | localization          |
        |                       |                       | variants.             |
        |                       |                       | :::                   |
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

        -   #### AppleBundleResources

                public AppleBundleResources()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getResourceDirs()}

        -   #### getResourceDirs

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableSet<SourcePathWithAppleBundleDestination> getResourceDirs()
            ```

            ::: block
            Directories that should be copied into the bundle as
            directories of files with the same name.
            :::

        []{#getDirsContainingResourceDirs()}

        -   #### getDirsContainingResourceDirs

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableSet<SourcePathWithAppleBundleDestination> getDirsContainingResourceDirs()
            ```

            ::: block
            Directories whose contents should be copied into the root of
            the resources subdirectory.
            This is useful when the directory contents are not known
            beforehand, such as when a rule generates a directory of
            files.
            :::

        []{#getResourceFiles()}

        -   #### getResourceFiles

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableSet<SourcePathWithAppleBundleDestination> getResourceFiles()
            ```

            ::: block
            Files that are copied to the root of the resources
            subdirectory.
            :::

        []{#getResourceVariantFiles()}

        -   #### getResourceVariantFiles

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableSet<SourcePath> getResourceVariantFiles()
            ```

            ::: block
            Resource files with localization variants.
            :::

        []{#getResourceDirsForDestination(com.facebook.buck.apple.AppleBundleDestination)}

        -   #### getResourceDirsForDestination

            ``` methodSignature
            public Set<SourcePath> getResourceDirsForDestination​(AppleBundleDestination destination)
            ```

        []{#getResourceFilesForDestination(com.facebook.buck.apple.AppleBundleDestination)}

        -   #### getResourceFilesForDestination

            ``` methodSignature
            public Set<SourcePath> getResourceFilesForDestination​(AppleBundleDestination destination)
            ```

        []{#getAllDestinations()}

        -   #### getAllDestinations

            ``` methodSignature
            public SortedSet<AppleBundleDestination> getAllDestinations()
            ```

            ::: block
            All kinds of destinations that are used by paths in this
            object.
            :::

        []{#getAll()}

        -   #### getAll

            ``` methodSignature
            public Iterable<SourcePath> getAll()
            ```

            ::: block
            Returns all the SourcePaths from the different types of
            resources.
            :::

        []{#builder()}

        -   #### builder

            ``` methodSignature
            public static AppleBundleResources.Builder builder()
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
