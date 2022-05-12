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
[Package]{.packageLabelInType} [com.facebook.buck.slb](package-summary.html)
:::

## Class ThriftUtil {#class-thriftutil .title title="Class ThriftUtil"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.slb.ThriftUtil

::: description
-   

    ------------------------------------------------------------------------

        public final class ThriftUtil
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static void`         | `dese                 |                       |
        |                       | rialize​(ThriftProtoco |                       |
        |                       | l protocol,           |                       |
        |                       |   byte[] source,      |                       |
        |                       |        org.apache.thr |                       |
        |                       | ift.TBase<?,​?> dest)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static void`         | `deseriali            |                       |
        |                       | ze​(ThriftProtocol pro |                       |
        |                       | tocol,            Inp |                       |
        |                       | utStream source,      |                       |
        |                       |        org.apache.thr |                       |
        |                       | ift.TBase<?,​?> dest)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static void`         | `deserial             | ::: block             |
        |                       | ize​(ThriftProtocol pr | Deserialize a message |
        |                       | otocol,            By | from a ByteBuffer.    |
        |                       | teBuffer source,      | :::                   |
        |                       |        org.apache.thr |                       |
        |                       | ift.TBase<?,​?> dest)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static or            | `ge                   |                       |
        | g.apache.thrift.proto | tProtocolFactory​(Thri |                       |
        | col.TProtocolFactory` | ftProtocol protocol)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `st                   | `newProtoc            |                       |
        | atic org.apache.thrif | olInstance​(ThriftProt |                       |
        | t.protocol.TProtocol` | ocol protocol,        |                       |
        |                       |              org.apac |                       |
        |                       | he.thrift.transport.T |                       |
        |                       | Transport transport)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static byte[]`       | `serialize​(ThriftPr   |                       |
        |                       | otocol protocol,      |                       |
        |                       |      org.apache.thrif |                       |
        |                       | t.TBase<?,​?> source)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static void`         | `serial               |                       |
        |                       | ize​(ThriftProtocol pr |                       |
        |                       | otocol,          org. |                       |
        |                       | apache.thrift.TBase<? |                       |
        |                       | ,​?> source,           |                       |
        |                       | OutputStream stream)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static ByteBuffer`   | `                     |                       |
        |                       | serializeToByteBuffer |                       |
        |                       | ​(ThriftProtocol proto |                       |
        |                       | col,                  |                       |
        |                       |      org.apache.thrif |                       |
        |                       | t.TBase<?,​?> source)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static String`       | `thriftToDebugJson​(o  |                       |
        |                       | rg.apache.thrift.TBas |                       |
        |                       | e<?,​?> thriftObject)` |                       |
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

        []{#getProtocolFactory(com.facebook.buck.slb.ThriftProtocol)}

        -   #### getProtocolFactory

            ``` methodSignature
            public static org.apache.thrift.protocol.TProtocolFactory getProtocolFactory​(ThriftProtocol protocol)
            ```

        []{#newProtocolInstance(com.facebook.buck.slb.ThriftProtocol,org.apache.thrift.transport.TTransport)}

        -   #### newProtocolInstance

            ``` methodSignature
            public static org.apache.thrift.protocol.TProtocol newProtocolInstance​(ThriftProtocol protocol,
                                                                                   org.apache.thrift.transport.TTransport transport)
            ```

        []{#serialize(com.facebook.buck.slb.ThriftProtocol,org.apache.thrift.TBase,java.io.OutputStream)}

        -   #### serialize

            ``` methodSignature
            public static void serialize​(ThriftProtocol protocol,
                                         org.apache.thrift.TBase<?,​?> source,
                                         OutputStream stream)
                                  throws ThriftException
            ```

            [Throws:]{.throwsLabel}
            :   `ThriftException`

        []{#serialize(com.facebook.buck.slb.ThriftProtocol,org.apache.thrift.TBase)}

        -   #### serialize

            ``` methodSignature
            public static byte[] serialize​(ThriftProtocol protocol,
                                           org.apache.thrift.TBase<?,​?> source)
                                    throws ThriftException
            ```

            [Throws:]{.throwsLabel}
            :   `ThriftException`

        []{#serializeToByteBuffer(com.facebook.buck.slb.ThriftProtocol,org.apache.thrift.TBase)}

        -   #### serializeToByteBuffer

            ``` methodSignature
            public static ByteBuffer serializeToByteBuffer​(ThriftProtocol protocol,
                                                           org.apache.thrift.TBase<?,​?> source)
                                                    throws ThriftException
            ```

            [Throws:]{.throwsLabel}
            :   `ThriftException`

        []{#deserialize(com.facebook.buck.slb.ThriftProtocol,byte[],org.apache.thrift.TBase)}

        -   #### deserialize

            ``` methodSignature
            public static void deserialize​(ThriftProtocol protocol,
                                           byte[] source,
                                           org.apache.thrift.TBase<?,​?> dest)
                                    throws ThriftException
            ```

            [Throws:]{.throwsLabel}
            :   `ThriftException`

        []{#deserialize(com.facebook.buck.slb.ThriftProtocol,java.io.InputStream,org.apache.thrift.TBase)}

        -   #### deserialize

            ``` methodSignature
            public static void deserialize​(ThriftProtocol protocol,
                                           InputStream source,
                                           org.apache.thrift.TBase<?,​?> dest)
                                    throws ThriftException
            ```

            [Throws:]{.throwsLabel}
            :   `ThriftException`

        []{#deserialize(com.facebook.buck.slb.ThriftProtocol,java.nio.ByteBuffer,org.apache.thrift.TBase)}

        -   #### deserialize

            ``` methodSignature
            public static void deserialize​(ThriftProtocol protocol,
                                           ByteBuffer source,
                                           org.apache.thrift.TBase<?,​?> dest)
                                    throws ThriftException
            ```

            ::: block
            Deserialize a message from a ByteBuffer.
            :::

            [Throws:]{.throwsLabel}
            :   `ThriftException`

        []{#thriftToDebugJson(org.apache.thrift.TBase)}

        -   #### thriftToDebugJson

            ``` methodSignature
            public static String thriftToDebugJson​(org.apache.thrift.TBase<?,​?> thriftObject)
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
