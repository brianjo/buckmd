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

## Class ResourcesXml {#class-resourcesxml .title title="Class ResourcesXml"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.android.resources.ResChunk](ResChunk.html "class in com.facebook.buck.android.resources")

    -   -   com.facebook.buck.android.resources.ResourcesXml

::: description
-   

    ------------------------------------------------------------------------

        public class ResourcesXml
        extends ResChunk

    ::: block
    ResourcesXml handles Android\'s compiled xml format. It consists of:
    ResChunk_header u16 chunk_type u16 header_size u32 chunk_size
    The header is followed by a StringPool containing all the strings
    used in the xml. This is then followed by an optional RefMap. After
    the StringPool/RefMap comes a list of xml nodes of the form:
    ResChunk_header u16 chunk_type u16 header_size u32 chunk_size u32
    lineNumber StringRef comment

    Each node contains extra information depending on the type:

    XML_START_NS: StringRef prefix StringRef uri

    XML_END_NS: StringRef prefix StringRef uri

    XML_CDATA: StringRef data Res_value typedData

    XML_END_ELEMENT: StringRef namespace StringRef name

    XML_START_ELEMENT: StringRef namespace StringRef name u16 attrStart
    u16 attrSize u16 attrCount u16 idIndex u16 classIndex u16 styleIndex

    XML_START_ELEMENT is then followed by attrCount attributes of the
    form: StringRef namespace StringRef name StringRef rawValue
    Res_value typedValue
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        -   []{#nested.classes.inherited.from.class.com.facebook.buck.android.resources.ResChunk}

            ### Nested classes/interfaces inherited from class com.facebook.buck.android.resources.[ResChunk](ResChunk.html "class in com.facebook.buck.android.resources")

            `ResChunk.RefTransformer, ResChunk.RefVisitor`
    :::

    ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type   Field              Description
          ------------------- ------------------ -------------
          `static int`        `ATTRIBUTE_SIZE`    
          `static int`        `HEADER_SIZE`       

          : Fields[ ]{.tabEnd}

        -   []{#fields.inherited.from.class.com.facebook.buck.android.resources.ResChunk}

            ### Fields inherited from class com.facebook.buck.android.resources.[ResChunk](ResChunk.html "class in com.facebook.buck.android.resources")

            `CHUNK_RES_TABLE_PACKAGE, CHUNK_RES_TABLE_TYPE, CHUNK_RES_TABLE_TYPE_SPEC, CHUNK_RESOURCE_TABLE, CHUNK_STRING_POOL, CHUNK_XML_REF_MAP, CHUNK_XML_TREE`
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type       Method                                                   Description
          ----------------------- -------------------------------------------------------- -------------
          `void`                  `dump​(PrintStream out)`                                   
          `static ResourcesXml`   `get​(ByteBuffer buf)`                                     
          `StringPool`            `getStrings()`                                            
          `void`                  `put​(ByteBuffer buf)`                                     
          `void`                  `transformReferences​(ResChunk.RefTransformer visitor)`    
          `void`                  `visitReferences​(ResChunk.RefVisitor visitor)`            

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
          Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
          .tableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.android.resources.ResChunk}

            ### Methods inherited from class com.facebook.buck.android.resources.[ResChunk](ResChunk.html "class in com.facebook.buck.android.resources")

            `getChunkSize, getHeaderSize, getTotalSize, getType, serialize, slice, slice, wrap`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#field.detail}

        ### Field Detail

        []{#HEADER_SIZE}

        -   #### HEADER_SIZE

                public static final int HEADER_SIZE

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.android.resources.ResourcesXml.HEADER_SIZE)

        []{#ATTRIBUTE_SIZE}

        -   #### ATTRIBUTE_SIZE

                public static final int ATTRIBUTE_SIZE

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.android.resources.ResourcesXml.ATTRIBUTE_SIZE)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#get(java.nio.ByteBuffer)}

        -   #### get

            ``` methodSignature
            public static ResourcesXml get​(ByteBuffer buf)
            ```

        []{#put(java.nio.ByteBuffer)}

        -   #### put

            ``` methodSignature
            public void put​(ByteBuffer buf)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `put` in class `ResChunk`

        []{#transformReferences(com.facebook.buck.android.resources.ResChunk.RefTransformer)}

        -   #### transformReferences

            ``` methodSignature
            public void transformReferences​(ResChunk.RefTransformer visitor)
            ```

        []{#visitReferences(com.facebook.buck.android.resources.ResChunk.RefVisitor)}

        -   #### visitReferences

            ``` methodSignature
            public void visitReferences​(ResChunk.RefVisitor visitor)
            ```

        []{#dump(java.io.PrintStream)}

        -   #### dump

            ``` methodSignature
            public void dump​(PrintStream out)
            ```

        []{#getStrings()}

        -   #### getStrings

            ``` methodSignature
            public StringPool getStrings()
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
