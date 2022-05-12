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
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.parser.manifest](package-summary.html)
:::

## Class BuildPackagePathToBuildFileManifestKey {#class-buildpackagepathtobuildfilemanifestkey .title title="Class BuildPackagePathToBuildFileManifestKey"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.parser.manifest.BuildPackagePathToBuildFileManifestKey

::: description
-   

    All Implemented Interfaces:
    :   `ComputeKey<BuildFileManifest>`

    ------------------------------------------------------------------------

        public abstract class BuildPackagePathToBuildFileManifestKey
        extends Object
        implements ComputeKey<BuildFileManifest>

    ::: block
    Transformation key containing path to a build file to parse
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type                                   Field          Description
          --------------------------------------------------- -------------- -------------
          `static ComputationIdentifier<BuildFileManifest>`   `IDENTIFIER`    

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                  Description
          -------------------------------------------- -------------
          `BuildPackagePathToBuildFileManifestKey()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `protected void`      | `check()`             |                       |
        +-----------------------+-----------------------+-----------------------+
        | `ComputationIdentifie | `getIdentifier()`     |                       |
        | r<BuildFileManifest>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract Path`       | `getPath()`           | ::: block             |
        |                       |                       | Path of the root of   |
        |                       |                       | the package to parse, |
        |                       |                       | relative to some root |
        |                       |                       | (usually cell root).  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `stat                 | `of​(Path path)`       |                       |
        | ic BuildPackagePathTo |                       |                       |
        | BuildFileManifestKey` |                       |                       |
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
    -   []{#field.detail}

        ### Field Detail

        []{#IDENTIFIER}

        -   #### IDENTIFIER

                public static final ComputationIdentifier<BuildFileManifest> IDENTIFIER
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### BuildPackagePathToBuildFileManifestKey

                public BuildPackagePathToBuildFileManifestKey()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getPath()}

        -   #### getPath

            ``` methodSignature
            public abstract Path getPath()
            ```

            ::: block
            Path of the root of the package to parse, relative to some
            root (usually cell root). The physical folder should contain
            build file.
            :::

        []{#check()}

        -   #### check

            ``` methodSignature
            @Check
            protected void check()
            ```

        []{#getIdentifier()}

        -   #### getIdentifier

            ``` methodSignature
            public ComputationIdentifier<BuildFileManifest> getIdentifier()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getIdentifier` in
                interface `ComputeKey<BuildFileManifest>`

            [Returns:]{.returnLabel}
            :   the identifier of this key. This identifier is used to
                map all keys of the same
                [`ComputationIdentifier`](../../core/graph/transformation/model/ComputationIdentifier.html "interface in com.facebook.buck.core.graph.transformation.model")
                to the same
                [`GraphComputation`](../../core/graph/transformation/GraphComputation.html "interface in com.facebook.buck.core.graph.transformation").

        []{#of(java.nio.file.Path)}

        -   #### of

            ``` methodSignature
            public static BuildPackagePathToBuildFileManifestKey of​(Path path)
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
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
-   [Constr](#constructor.detail) \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
