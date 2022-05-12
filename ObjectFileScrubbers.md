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
[Package]{.packageLabelInType} [com.facebook.buck.cxx.toolchain.objectfile](package-summary.html)
:::

## Class ObjectFileScrubbers {#class-objectfilescrubbers .title title="Class ObjectFileScrubbers"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.cxx.toolchain.objectfile.ObjectFileScrubbers

::: description
-   

    ------------------------------------------------------------------------

        public class ObjectFileScrubbers
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type   Class                                Description
          ------------------- ------------------------------------ -------------
          `static class `     `ObjectFileScrubbers.PaddingStyle`    

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type   Field                         Description
          ------------------- ----------------------------- -------------
          `static byte[]`     `END_OF_FILE_HEADER_MARKER`    
          `static byte[]`     `GLOBAL_HEADER`                
          `static byte[]`     `GLOBAL_THIN_HEADER`           

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static void`         | `checkArchive​(bo      |                       |
        |                       | olean expression,     |                       |
        |                       |          String msg)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static               | `createDat            |                       |
        | FileContentsScrubber` | eUidGidScrubber​(Objec |                       |
        |                       | tFileScrubbers.Paddin |                       |
        |                       | gStyle paddingStyle)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static byte[]`       | `get                  |                       |
        |                       | Bytes​(ByteBuffer buff |                       |
        |                       | er,         int len)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static ByteBuffer`   | `getCh                | ::: block             |
        |                       | arByteBuffer​(byte[] b | Returned buffer does  |
        |                       | ytes,                 | \_not\_ include       |
        |                       |   int startPosition)` | NULL-terminating      |
        |                       |                       | char.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static long`         | `getDecimal           |                       |
        |                       | StringAsLong​(ByteBuff |                       |
        |                       | er buffer,            |                       |
        |                       |             int len)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static int`          | `getLittleEndianIn    |                       |
        |                       | t​(ByteBuffer buffer)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static long`         | `getLittleEndianLon   |                       |
        |                       | g​(ByteBuffer buffer)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static short`        | `getLittleEndianShor  |                       |
        |                       | t​(ByteBuffer buffer)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static void`         | `putBytes             |                       |
        |                       | ​(ByteBuffer buffer,   |                       |
        |                       |        byte[] bytes)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static void`         | `putCh                | ::: block             |
        |                       | arByteBuffer​(ByteBuff | C string does \_not\_ |
        |                       | er dest,              | include               |
        |                       |      int position,    | NULL-terminating      |
        |                       |                ByteBu | char.                 |
        |                       | ffer charByteBuffer)` | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static void`         | `put                  |                       |
        |                       | IntAsDecimalString​(By |                       |
        |                       | teBuffer buffer,      |                       |
        |                       |                  int  |                       |
        |                       | len,                  |                       |
        |                       |      int value,       |                       |
        |                       |                 Objec |                       |
        |                       | tFileScrubbers.Paddin |                       |
        |                       | gStyle paddingStyle)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static void`         | `putIntAsOctalStr     |                       |
        |                       | ing​(ByteBuffer buffer |                       |
        |                       | ,                     |                       |
        |                       | int len,              |                       |
        |                       |        int value,     |                       |
        |                       |                 Objec |                       |
        |                       | tFileScrubbers.Paddin |                       |
        |                       | gStyle paddingStyle)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static void`         | `putL                 |                       |
        |                       | ittleEndianInt​(ByteBu |                       |
        |                       | ffer buffer,          |                       |
        |                       |           int value)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static void`         | `putLitt              |                       |
        |                       | leEndianLong​(ByteBuff |                       |
        |                       | er buffer,            |                       |
        |                       |          long value)` |                       |
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
    -   []{#field.detail}

        ### Field Detail

        []{#GLOBAL_HEADER}

        -   #### GLOBAL_HEADER

                public static final byte[] GLOBAL_HEADER

        []{#GLOBAL_THIN_HEADER}

        -   #### GLOBAL_THIN_HEADER

                public static final byte[] GLOBAL_THIN_HEADER

        []{#END_OF_FILE_HEADER_MARKER}

        -   #### END_OF_FILE_HEADER_MARKER

                public static final byte[] END_OF_FILE_HEADER_MARKER
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#createDateUidGidScrubber(com.facebook.buck.cxx.toolchain.objectfile.ObjectFileScrubbers.PaddingStyle)}

        -   #### createDateUidGidScrubber

            ``` methodSignature
            public static FileContentsScrubber createDateUidGidScrubber​(ObjectFileScrubbers.PaddingStyle paddingStyle)
            ```

        []{#getBytes(java.nio.ByteBuffer,int)}

        -   #### getBytes

            ``` methodSignature
            public static byte[] getBytes​(ByteBuffer buffer,
                                          int len)
            ```

        []{#getDecimalStringAsLong(java.nio.ByteBuffer,int)}

        -   #### getDecimalStringAsLong

            ``` methodSignature
            public static long getDecimalStringAsLong​(ByteBuffer buffer,
                                                      int len)
            ```

        []{#getLittleEndianLong(java.nio.ByteBuffer)}

        -   #### getLittleEndianLong

            ``` methodSignature
            public static long getLittleEndianLong​(ByteBuffer buffer)
            ```

        []{#getLittleEndianInt(java.nio.ByteBuffer)}

        -   #### getLittleEndianInt

            ``` methodSignature
            public static int getLittleEndianInt​(ByteBuffer buffer)
            ```

        []{#getLittleEndianShort(java.nio.ByteBuffer)}

        -   #### getLittleEndianShort

            ``` methodSignature
            public static short getLittleEndianShort​(ByteBuffer buffer)
            ```

        []{#getCharByteBuffer(byte[],int)}

        -   #### getCharByteBuffer

            ``` methodSignature
            public static ByteBuffer getCharByteBuffer​(byte[] bytes,
                                                       int startPosition)
            ```

            ::: block
            Returned buffer does \_not\_ include NULL-terminating char.
            :::

        []{#putCharByteBuffer(java.nio.ByteBuffer,int,java.nio.ByteBuffer)}

        -   #### putCharByteBuffer

            ``` methodSignature
            public static void putCharByteBuffer​(ByteBuffer dest,
                                                 int position,
                                                 ByteBuffer charByteBuffer)
            ```

            ::: block
            C string does \_not\_ include NULL-terminating char.
            :::

        []{#putBytes(java.nio.ByteBuffer,byte[])}

        -   #### putBytes

            ``` methodSignature
            public static void putBytes​(ByteBuffer buffer,
                                        byte[] bytes)
            ```

        []{#putIntAsOctalString(java.nio.ByteBuffer,int,int,com.facebook.buck.cxx.toolchain.objectfile.ObjectFileScrubbers.PaddingStyle)}

        -   #### putIntAsOctalString

            ``` methodSignature
            public static void putIntAsOctalString​(ByteBuffer buffer,
                                                   int len,
                                                   int value,
                                                   ObjectFileScrubbers.PaddingStyle paddingStyle)
            ```

        []{#putIntAsDecimalString(java.nio.ByteBuffer,int,int,com.facebook.buck.cxx.toolchain.objectfile.ObjectFileScrubbers.PaddingStyle)}

        -   #### putIntAsDecimalString

            ``` methodSignature
            public static void putIntAsDecimalString​(ByteBuffer buffer,
                                                     int len,
                                                     int value,
                                                     ObjectFileScrubbers.PaddingStyle paddingStyle)
            ```

        []{#putLittleEndianLong(java.nio.ByteBuffer,long)}

        -   #### putLittleEndianLong

            ``` methodSignature
            public static void putLittleEndianLong​(ByteBuffer buffer,
                                                   long value)
            ```

        []{#putLittleEndianInt(java.nio.ByteBuffer,int)}

        -   #### putLittleEndianInt

            ``` methodSignature
            public static void putLittleEndianInt​(ByteBuffer buffer,
                                                  int value)
            ```

        []{#checkArchive(boolean,java.lang.String)}

        -   #### checkArchive

            ``` methodSignature
            public static void checkArchive​(boolean expression,
                                            String msg)
                                     throws FileScrubber.ScrubException
            ```

            [Throws:]{.throwsLabel}
            :   `FileScrubber.ScrubException`
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
