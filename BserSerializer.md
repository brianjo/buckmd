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
[Package]{.packageLabelInType} [com.facebook.buck.util.bser](package-summary.html)
:::

## Class BserSerializer {#class-bserserializer .title title="Class BserSerializer"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.util.bser.BserSerializer

::: description
-   

    ------------------------------------------------------------------------

        public class BserSerializer
        extends Object

    ::: block
    Encoder for the BSER binary JSON format used by the Watchman
    service:
    https://facebook.github.io/watchman/docs/bser.html
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor          Description
          -------------------- -------------
          `BserSerializer()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `ByteBuffer`          | `seria                | ::: block             |
        |                       | lizeToBuffer​(Object v | Serializes an object  |
        |                       | alue,                 | using BSER encoding.  |
        |                       |   ByteBuffer buffer)` | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `serializeToSt        | ::: block             |
        |                       | ream​(Object value,    | Serializes an object  |
        |                       |                Output | using BSER encoding   |
        |                       | Stream outputStream)` | to the stream.        |
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

        []{#<init>()}

        -   #### BserSerializer

                public BserSerializer()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#serializeToStream(java.lang.Object,java.io.OutputStream)}

        -   #### serializeToStream

            ``` methodSignature
            public void serializeToStream​(Object value,
                                          OutputStream outputStream)
                                   throws IOException
            ```

            ::: block
            Serializes an object using BSER encoding to the stream.
            :::

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#serializeToBuffer(java.lang.Object,java.nio.ByteBuffer)}

        -   #### serializeToBuffer

            ``` methodSignature
            public ByteBuffer serializeToBuffer​(Object value,
                                                ByteBuffer buffer)
                                         throws IOException
            ```

            ::: block
            Serializes an object using BSER encoding. If possible,
            writes the object to the provided byte buffer and returns
            it. If the buffer is not big enough to hold the object,
            returns a new buffer.
            After returning, buffer.position() is advanced past the last
            encoded byte.
            :::

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
