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
-   [Field](#field.summary) \| 
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.android.resources](package-summary.html)
:::

## Class ResChunk {#class-reschunk .title title="Class ResChunk"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.android.resources.ResChunk

::: description
-   

    Direct Known Subclasses:
    :   `ResourcesXml`, `ResourceTable`, `ResTablePackage`,
        `ResTableType`, `ResTableTypeSpec`, `StringPool`

    ------------------------------------------------------------------------

        public abstract class ResChunk
        extends Object

    ::: block
    ResChunk is the base of most structures in Android\'s .arsc and
    compiled .xml files. It consists of: u16 chunkType u16 headerSize
    u32 chunkSize
    Some common types used by different chunks:

    StringRef is a u32 string id ResRef is a u32 resource id ResValue is
    a chunk of: u16 size u8 0x00 u8 dataType (one of
    ResChunk.RES_XXXXXXX) u32 data

    See
    https://android.googlesource.com/platform/frameworks/base/+/kitkat-release/include/androidfw/ResourceTypes.h
    for full specification.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type     Class                       Description
          --------------------- --------------------------- -------------
          `static interface `   `ResChunk.RefTransformer`    
          `static interface `   `ResChunk.RefVisitor`        

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type   Field                         Description
          ------------------- ----------------------------- -------------
          `static short`      `CHUNK_RES_TABLE_PACKAGE`      
          `static short`      `CHUNK_RES_TABLE_TYPE`         
          `static short`      `CHUNK_RES_TABLE_TYPE_SPEC`    
          `static short`      `CHUNK_RESOURCE_TABLE`         
          `static short`      `CHUNK_STRING_POOL`            
          `static short`      `CHUNK_XML_REF_MAP`            
          `static short`      `CHUNK_XML_TREE`               

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `int`                 | `getChunkSize()`      |                       |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `getHeaderSize()`     |                       |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `getTotalSize()`      | ::: block             |
        |                       |                       | For most chunk\'s     |
        |                       |                       | totalSize ==          |
        |                       |                       | chunkSize.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `getType()`           |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract void`       | `pu                   |                       |
        |                       | t​(ByteBuffer output)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `byte[]`              | `serialize()`         |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static ByteBuffer`   | `slice​(ByteBuffer m   |                       |
        |                       | ap,      int offset)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static ByteBuffer`   | `slice​(ByteBuff       |                       |
        |                       | er map,      int offs |                       |
        |                       | et,      int length)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static ByteBuffer`   | `wrap​(byte[] data)`   |                       |
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

        []{#CHUNK_STRING_POOL}

        -   #### CHUNK_STRING_POOL

                public static final short CHUNK_STRING_POOL

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.android.resources.ResChunk.CHUNK_STRING_POOL)

        []{#CHUNK_RESOURCE_TABLE}

        -   #### CHUNK_RESOURCE_TABLE

                public static final short CHUNK_RESOURCE_TABLE

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.android.resources.ResChunk.CHUNK_RESOURCE_TABLE)

        []{#CHUNK_XML_TREE}

        -   #### CHUNK_XML_TREE

                public static final short CHUNK_XML_TREE

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.android.resources.ResChunk.CHUNK_XML_TREE)

        []{#CHUNK_XML_REF_MAP}

        -   #### CHUNK_XML_REF_MAP

                public static final short CHUNK_XML_REF_MAP

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.android.resources.ResChunk.CHUNK_XML_REF_MAP)

        []{#CHUNK_RES_TABLE_PACKAGE}

        -   #### CHUNK_RES_TABLE_PACKAGE

                public static final short CHUNK_RES_TABLE_PACKAGE

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.android.resources.ResChunk.CHUNK_RES_TABLE_PACKAGE)

        []{#CHUNK_RES_TABLE_TYPE}

        -   #### CHUNK_RES_TABLE_TYPE

                public static final short CHUNK_RES_TABLE_TYPE

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.android.resources.ResChunk.CHUNK_RES_TABLE_TYPE)

        []{#CHUNK_RES_TABLE_TYPE_SPEC}

        -   #### CHUNK_RES_TABLE_TYPE_SPEC

                public static final short CHUNK_RES_TABLE_TYPE_SPEC

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.android.resources.ResChunk.CHUNK_RES_TABLE_TYPE_SPEC)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getType()}

        -   #### getType

            ``` methodSignature
            public final int getType()
            ```

        []{#getHeaderSize()}

        -   #### getHeaderSize

            ``` methodSignature
            public final int getHeaderSize()
            ```

        []{#getChunkSize()}

        -   #### getChunkSize

            ``` methodSignature
            public final int getChunkSize()
            ```

        []{#getTotalSize()}

        -   #### getTotalSize

            ``` methodSignature
            public int getTotalSize()
            ```

            ::: block
            For most chunk\'s totalSize == chunkSize. For some types,
            the type logically consists of multiple chunks. In these
            cases, totalSize is the sum of all the chunks. This is the
            full size written/read from a buffer for get/put.
            :::

        []{#serialize()}

        -   #### serialize

            ``` methodSignature
            public final byte[] serialize()
            ```

        []{#put(java.nio.ByteBuffer)}

        -   #### put

            ``` methodSignature
            public abstract void put​(ByteBuffer output)
            ```

        []{#wrap(byte[])}

        -   #### wrap

            ``` methodSignature
            public static ByteBuffer wrap​(byte[] data)
            ```

        []{#slice(java.nio.ByteBuffer,int)}

        -   #### slice

            ``` methodSignature
            public static ByteBuffer slice​(ByteBuffer map,
                                           int offset)
            ```

        []{#slice(java.nio.ByteBuffer,int,int)}

        -   #### slice

            ``` methodSignature
            public static ByteBuffer slice​(ByteBuffer map,
                                           int offset,
                                           int length)
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
-   [Nested](#nested.class.summary) \| 
-   [Field](#field.summary) \| 
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
-   Constr \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
