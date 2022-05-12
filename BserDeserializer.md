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
[Package]{.packageLabelInType} [com.facebook.buck.util.bser](package-summary.html)
:::

## Class BserDeserializer {#class-bserdeserializer .title title="Class BserDeserializer"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.util.bser.BserDeserializer

::: description
-   

    ------------------------------------------------------------------------

        public class BserDeserializer
        extends Object

    ::: block
    Decoder for the BSER binary JSON format used by the Watchman
    service:
    https://facebook.github.io/watchman/docs/bser.html
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static class `       | `BserDeseriali        | ::: block             |
        |                       | zer.BserEofException` | Exception thrown when |
        |                       |                       | BSER parser           |
        |                       |                       | unexpectedly reaches  |
        |                       |                       | the end of the input  |
        |                       |                       | stream.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static class `       | `BserDese             |                       |
        |                       | rializer.KeyOrdering` |                       |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

        +-----------------------------------+-----------------------------------+
        | Constructor                       | Description                       |
        +===================================+===================================+
        | `BserDeserializer​(BserDeser       | ::: block                         |
        | ializer.KeyOrdering keyOrdering)` | If `keyOrdering` is `SORTED`, any |
        |                                   | `Map` objects in the resulting    |
        |                                   | value will have their keys sorted |
        |                                   | in natural order.                 |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+

        : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `Object`              | `dese                 | ::: block             |
        |                       | rializeBserValue​(Inpu | Deserializes the next |
        |                       | tStream inputStream)` | BSER-encoded value    |
        |                       |                       | from the stream.      |
        |                       |                       | :::                   |
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

        []{#<init>(com.facebook.buck.util.bser.BserDeserializer.KeyOrdering)}

        -   #### BserDeserializer

                public BserDeserializer​(BserDeserializer.KeyOrdering keyOrdering)

            ::: block
            If `keyOrdering` is `SORTED`, any `Map` objects in the
            resulting value will have their keys sorted in natural
            order. Otherwise, any `Map`s will have their keys in the
            same order with which they were encoded.
            :::
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#deserializeBserValue(java.io.InputStream)}

        -   #### deserializeBserValue

            ``` methodSignature
            @Nullable
            public Object deserializeBserValue​(InputStream inputStream)
                                        throws IOException
            ```

            ::: block
            Deserializes the next BSER-encoded value from the stream.
            :::

            [Returns:]{.returnLabel}
            :   either a
                [`String`](http://docs.oracle.com/javase/7/docs/api/java/lang/String.html?is-external=true "class or interface in java.lang"){.externalLink},
                [`Number`](http://docs.oracle.com/javase/7/docs/api/java/lang/Number.html?is-external=true "class or interface in java.lang"){.externalLink},
                [`List`](http://docs.oracle.com/javase/7/docs/api/java/util/List.html?is-external=true "class or interface in java.util"){.externalLink},
                [`Map`](http://docs.oracle.com/javase/7/docs/api/java/util/Map.html?is-external=true "class or interface in java.util"){.externalLink},
                or `null`, depending on the type of the top-level
                encoded object.

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
