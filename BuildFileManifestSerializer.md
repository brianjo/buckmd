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
[Package]{.packageLabelInType} [com.facebook.buck.parser.cache.json](package-summary.html)
:::

## Class BuildFileManifestSerializer {#class-buildfilemanifestserializer .title title="Class BuildFileManifestSerializer"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.parser.cache.json.BuildFileManifestSerializer

::: description
-   

    ------------------------------------------------------------------------

        public class BuildFileManifestSerializer
        extends Object

    ::: block
    This class serializes the
    [`BuildFileManifest`](../../api/BuildFileManifest.html "class in com.facebook.buck.parser.api")
    to a form that can be stored and read from disk.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `stat                 | `d                    | ::: block             |
        | ic BuildFileManifest` | eserialize​(byte[] bui | Deserializes an       |
        |                       | ldFileManifestBytes)` | instance of           |
        |                       |                       | [`BuildFile           |
        |                       |                       | Manifest`](../../api/ |
        |                       |                       | BuildFileManifest.htm |
        |                       |                       | l "class in com.faceb |
        |                       |                       | ook.buck.parser.api") |
        |                       |                       | from a byte array.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static byte[]`       | `seria                | ::: block             |
        |                       | lize​(BuildFileManifes | Serializes an         |
        |                       | t buildFileManifest)` | instance of           |
        |                       |                       | [`BuildFile           |
        |                       |                       | Manifest`](../../api/ |
        |                       |                       | BuildFileManifest.htm |
        |                       |                       | l "class in com.faceb |
        |                       |                       | ook.buck.parser.api") |
        |                       |                       | to a byte array.      |
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

        []{#serialize(com.facebook.buck.parser.api.BuildFileManifest)}

        -   #### serialize

            ``` methodSignature
            public static byte[] serialize​(BuildFileManifest buildFileManifest)
                                    throws IOException
            ```

            ::: block
            Serializes an instance of
            [`BuildFileManifest`](../../api/BuildFileManifest.html "class in com.facebook.buck.parser.api")
            to a byte array.
            :::

            [Parameters:]{.paramLabel}
            :   `buildFileManifest` - the instance of
                [`BuildFileManifest`](../../api/BuildFileManifest.html "class in com.facebook.buck.parser.api")
                to be serialized.

            [Returns:]{.returnLabel}
            :   a byte array with the serialized manifest.

            [Throws:]{.throwsLabel}
            :   `com.fasterxml.jackson.core.JsonProcessingException`
            :   `IOException`

        []{#deserialize(byte[])}

        -   #### deserialize

            ``` methodSignature
            public static BuildFileManifest deserialize​(byte[] buildFileManifestBytes)
                                                 throws IOException
            ```

            ::: block
            Deserializes an instance of
            [`BuildFileManifest`](../../api/BuildFileManifest.html "class in com.facebook.buck.parser.api")
            from a byte array.
            :::

            [Parameters:]{.paramLabel}
            :   `buildFileManifestBytes` - the bytes for the manifest to
                be deserialized.

            [Returns:]{.returnLabel}
            :   a new instance of
                [`BuildFileManifest`](../../api/BuildFileManifest.html "class in com.facebook.buck.parser.api")
                serialized from the `      buildFileManifestBytes`.

            [Throws:]{.throwsLabel}
            :   `IOException`
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
