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
[Package]{.packageLabelInType} [com.facebook.buck.parser.api](package-summary.html)
:::

## Class BuildFileManifestPojoizer {#class-buildfilemanifestpojoizer .title title="Class BuildFileManifestPojoizer"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.parser.api.BuildFileManifestPojoizer

::: description
-   

    ------------------------------------------------------------------------

        public class BuildFileManifestPojoizer
        extends Object

    ::: block
    Utility class to convert parser-created objects to equivalent
    POJO-typed objects
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static class `       | `                     | ::: block             |
        |                       | BuildFileManifestPojo | Container to hold     |
        |                       | izer.PojoTransformer` | transformation        |
        |                       |                       | function for classes  |
        |                       |                       | assignable to a       |
        |                       |                       | provided class.       |
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
        | `Build                | `addPojoTransforme    | ::: block             |
        | FileManifestPojoizer` | r​(BuildFileManifestPo | Add a custom          |
        |                       | joizer.PojoTransforme | transformer to        |
        |                       | r customTransformer)` | [`BuildFileManifes    |
        |                       |                       | tPojoizer`](BuildFile |
        |                       |                       | ManifestPojoizer.html |
        |                       |                       |  "class in com.facebo |
        |                       |                       | ok.buck.parser.api"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Object`              | `convertToPo          | ::: block             |
        |                       | jo​(Object parserObj)` | Recursively convert   |
        |                       |                       | parser-created        |
        |                       |                       | objects into          |
        |                       |                       | equivalent POJO       |
        |                       |                       | objects.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static Build         | `of()`                | ::: block             |
        | FileManifestPojoizer` |                       | Create an instance of |
        |                       |                       | [`BuildFileManife     |
        |                       |                       | stPojoizer`](BuildFil |
        |                       |                       | eManifestPojoizer.htm |
        |                       |                       | l "class in com.faceb |
        |                       |                       | ook.buck.parser.api") |
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
    -   []{#method.detail}

        ### Method Detail

        []{#of()}

        -   #### of

            ``` methodSignature
            public static BuildFileManifestPojoizer of()
            ```

            ::: block
            Create an instance of
            [`BuildFileManifestPojoizer`](BuildFileManifestPojoizer.html "class in com.facebook.buck.parser.api")
            :::

        []{#addPojoTransformer(com.facebook.buck.parser.api.BuildFileManifestPojoizer.PojoTransformer)}

        -   #### addPojoTransformer

            ``` methodSignature
            public BuildFileManifestPojoizer addPojoTransformer​(BuildFileManifestPojoizer.PojoTransformer customTransformer)
            ```

            ::: block
            Add a custom transformer to
            [`BuildFileManifestPojoizer`](BuildFileManifestPojoizer.html "class in com.facebook.buck.parser.api").
            If a type specified in this transfomer matches the type of
            parser object, the transformation function is invoked. It is
            expected for transformation function to return POJO-type
            accepted by `BuildFileManifest`.
            This utility exists mainly to decouple some specific types
            known to some parser only, from generic parser API

            This method effectively makes
            [`BuildFileManifestPojoizer`](BuildFileManifestPojoizer.html "class in com.facebook.buck.parser.api")
            mutable. This is only because the implementation of the
            transformer may want to recursively call
            [`convertToPojo(java.lang.Object)`](#convertToPojo(java.lang.Object))
            so
            [`BuildFileManifestPojoizer`](BuildFileManifestPojoizer.html "class in com.facebook.buck.parser.api")
            should be constructed beforehand.
            :::

        []{#convertToPojo(java.lang.Object)}

        -   #### convertToPojo

            ``` methodSignature
            public Object convertToPojo​(Object parserObj)
            ```

            ::: block
            Recursively convert parser-created objects into equivalent
            POJO objects. All collections are replaced with Immutable
            collections. So, by contract, only the following collections
            are allowed to be in converted objects: ImmutableList,
            ImmutableSet, ImmutableSortedSet, ImmutableMap,
            ImmutableSortedMap. Any of concrete implementation of those
            abstract immutable collections is allowed.
            Other allowed types are primitive Java types, Optional, and
            classes from com.facebook.buck.parser.api package.

            This function is allowed to be called from transformer
            function for full recursion

            Examples: SkylarkDict is replaced with ImmutableMap,
            SkylarkList is replaced with ImmutableList recursively
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
