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
[Package]{.packageLabelInType} [com.facebook.buck.util.zip.collect](package-summary.html)
:::

## Class ZipEntrySourceCollectionBuilder {#class-zipentrysourcecollectionbuilder .title title="Class ZipEntrySourceCollectionBuilder"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.util.zip.collect.ZipEntrySourceCollectionBuilder

::: description
-   

    ------------------------------------------------------------------------

        public class ZipEntrySourceCollectionBuilder
        extends Object

    ::: block
    A builder for
    [`ZipEntrySourceCollection`](ZipEntrySourceCollection.html "interface in com.facebook.buck.util.zip.collect")
    that allows to build a collection using provided source files as
    well as source zip files.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                   Description
          ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `ZipEntrySourceCollectionBuilder​(com.google.common.collect.ImmutableSet<Pattern> entriesToExclude,                                OnDuplicateEntry onDuplicateEntryAction)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `void`                | `addFile​(Stri         | ::: block             |
        |                       | ng entryName,         | Add the given file as |
        |                       | Path sourceFilePath)` | a source for an entry |
        |                       |                       | with the provided     |
        |                       |                       | name.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `addZipFi             | ::: block             |
        |                       | le​(Path zipFilePath)` | Add all entries of a  |
        |                       |                       | given zip file to the |
        |                       |                       | collection (excluding |
        |                       |                       | entries that match    |
        |                       |                       | [`excluded            |
        |                       |                       | EntriesMatcher`](#exc |
        |                       |                       | ludedEntriesMatcher). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ZipE                 | `build()`             |                       |
        | ntrySourceCollection` |                       |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
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

        []{#<init>(com.google.common.collect.ImmutableSet,com.facebook.buck.util.zip.collect.OnDuplicateEntry)}

        -   #### ZipEntrySourceCollectionBuilder

                public ZipEntrySourceCollectionBuilder​(com.google.common.collect.ImmutableSet<Pattern> entriesToExclude,
                                                       OnDuplicateEntry onDuplicateEntryAction)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#addFile(java.lang.String,java.nio.file.Path)}

        -   #### addFile

            ``` methodSignature
            public void addFile​(String entryName,
                                Path sourceFilePath)
            ```

            ::: block
            Add the given file as a source for an entry with the
            provided name.
            :::

        []{#addZipFile(java.nio.file.Path)}

        -   #### addZipFile

            ``` methodSignature
            public void addZipFile​(Path zipFilePath)
                            throws IOException
            ```

            ::: block
            Add all entries of a given zip file to the collection
            (excluding entries that match
            [`excludedEntriesMatcher`](#excludedEntriesMatcher).
            :::

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#build()}

        -   #### build

            ``` methodSignature
            public ZipEntrySourceCollection build()
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
