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

## Class ResTableType {#class-restabletype .title title="Class ResTableType"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.android.resources.ResChunk](ResChunk.html "class in com.facebook.buck.android.resources")

    -   -   com.facebook.buck.android.resources.ResTableType

::: description
-   

    ------------------------------------------------------------------------

        public class ResTableType
        extends ResChunk

    ::: block
    ResTableType is a ResChunk holding the resource values for a given
    type and configuration. It consists of: ResChunk_header u32
    chunk_type u32 header_size u32 chunk_size u8 id u32 entry_count u32
    entry_start Config u32 config_size u8\[config_size - 4\] data
    This is followed by entry_count u32s containing offsets from
    entry_start to the data for each entry. If the offset for a resource
    is -1, that resource has no value in this configuration.

    After the offsets comes the entry data. Each entry is of the form:
    u16 size u16 flags StringRef key

    If \`(flags & FLAG_COMPLEX) == 0\` this data is then followed by:
    ResValue value

    Else it\'s followed by a map header: ResRef parent u32 count

    and \`count\` map entries of the form: ResRef name ResValue value
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

          Modifier and Type   Field                         Description
          ------------------- ----------------------------- -------------
          `static int`        `ATTRIBUTE_DATA_OFFSET`        
          `static int`        `ATTRIBUTE_NAME_REF_OFFSET`    
          `static int`        `ATTRIBUTE_SIZE_OFFSET`        
          `static int`        `ATTRIBUTE_TYPE_OFFSET`        

          : Fields[ ]{.tabEnd}

        -   []{#fields.inherited.from.class.com.facebook.buck.android.resources.ResChunk}

            ### Fields inherited from class com.facebook.buck.android.resources.[ResChunk](ResChunk.html "class in com.facebook.buck.android.resources")

            `CHUNK_RES_TABLE_PACKAGE, CHUNK_RES_TABLE_TYPE, CHUNK_RES_TABLE_TYPE_SPEC, CHUNK_RESOURCE_TABLE, CHUNK_STRING_POOL, CHUNK_XML_REF_MAP, CHUNK_XML_TREE`
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type       Method                                                                                                    Description
          ----------------------- --------------------------------------------------------------------------------------------------------- -------------
          `void`                  `dump​(StringPool strings,     ResTablePackage resPackage,     PrintStream out)`                            
          `static ResTableType`   `get​(ByteBuffer buf)`                                                                                      
          `int`                   `getEntryCount()`                                                                                          
          `int`                   `getEntryValueOffset​(int i)`                                                                               
          `int`                   `getResourceRef​(int id)`                                                                                   
          `void`                  `put​(ByteBuffer output)`                                                                                   
          `void`                  `reassignIds​(ReferenceMapper refMapping)`                                                                  
          `static ResTableType`   `slice​(ResTableType type,      int count)`                                                                 
          `void`                  `transformKeyReferences​(ResChunk.RefTransformer visitor)`                                                  
          `void`                  `transformReferences​(int[] ids,                    ResChunk.RefTransformer visitor)`                       
          `void`                  `transformReferences​(ResChunk.RefTransformer visitor)`                                                     
          `void`                  `transformStringReferences​(int[] idsToVisit,                          ResChunk.RefTransformer visitor)`    
          `void`                  `transformStringReferences​(ResChunk.RefTransformer visitor)`                                               
          `void`                  `visitKeyReferences​(ResChunk.RefVisitor visitor)`                                                          
          `void`                  `visitReferences​(int[] ids,                ResChunk.RefVisitor visitor)`                                   
          `void`                  `visitStringReferences​(int[] idsToVisit,                      ResChunk.RefVisitor visitor)`                
          `void`                  `visitStringReferences​(ResChunk.RefVisitor visitor)`                                                       

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

        []{#ATTRIBUTE_NAME_REF_OFFSET}

        -   #### ATTRIBUTE_NAME_REF_OFFSET

                public static final int ATTRIBUTE_NAME_REF_OFFSET

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.android.resources.ResTableType.ATTRIBUTE_NAME_REF_OFFSET)

        []{#ATTRIBUTE_SIZE_OFFSET}

        -   #### ATTRIBUTE_SIZE_OFFSET

                public static final int ATTRIBUTE_SIZE_OFFSET

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.android.resources.ResTableType.ATTRIBUTE_SIZE_OFFSET)

        []{#ATTRIBUTE_TYPE_OFFSET}

        -   #### ATTRIBUTE_TYPE_OFFSET

                public static final int ATTRIBUTE_TYPE_OFFSET

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.android.resources.ResTableType.ATTRIBUTE_TYPE_OFFSET)

        []{#ATTRIBUTE_DATA_OFFSET}

        -   #### ATTRIBUTE_DATA_OFFSET

                public static final int ATTRIBUTE_DATA_OFFSET

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.android.resources.ResTableType.ATTRIBUTE_DATA_OFFSET)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#slice(com.facebook.buck.android.resources.ResTableType,int)}

        -   #### slice

            ``` methodSignature
            @Nullable
            public static ResTableType slice​(ResTableType type,
                                             int count)
            ```

        []{#put(java.nio.ByteBuffer)}

        -   #### put

            ``` methodSignature
            public void put​(ByteBuffer output)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `put` in class `ResChunk`

        []{#get(java.nio.ByteBuffer)}

        -   #### get

            ``` methodSignature
            public static ResTableType get​(ByteBuffer buf)
            ```

        []{#dump(com.facebook.buck.android.resources.StringPool,com.facebook.buck.android.resources.ResTablePackage,java.io.PrintStream)}

        -   #### dump

            ``` methodSignature
            public void dump​(StringPool strings,
                             ResTablePackage resPackage,
                             PrintStream out)
            ```

        []{#getResourceRef(int)}

        -   #### getResourceRef

            ``` methodSignature
            public int getResourceRef​(int id)
            ```

        []{#getEntryValueOffset(int)}

        -   #### getEntryValueOffset

            ``` methodSignature
            public int getEntryValueOffset​(int i)
            ```

        []{#getEntryCount()}

        -   #### getEntryCount

            ``` methodSignature
            public int getEntryCount()
            ```

        []{#transformKeyReferences(com.facebook.buck.android.resources.ResChunk.RefTransformer)}

        -   #### transformKeyReferences

            ``` methodSignature
            public void transformKeyReferences​(ResChunk.RefTransformer visitor)
            ```

        []{#visitKeyReferences(com.facebook.buck.android.resources.ResChunk.RefVisitor)}

        -   #### visitKeyReferences

            ``` methodSignature
            public void visitKeyReferences​(ResChunk.RefVisitor visitor)
            ```

        []{#transformStringReferences(com.facebook.buck.android.resources.ResChunk.RefTransformer)}

        -   #### transformStringReferences

            ``` methodSignature
            public void transformStringReferences​(ResChunk.RefTransformer visitor)
            ```

        []{#transformStringReferences(int[],com.facebook.buck.android.resources.ResChunk.RefTransformer)}

        -   #### transformStringReferences

            ``` methodSignature
            public void transformStringReferences​(int[] idsToVisit,
                                                  ResChunk.RefTransformer visitor)
            ```

        []{#visitStringReferences(com.facebook.buck.android.resources.ResChunk.RefVisitor)}

        -   #### visitStringReferences

            ``` methodSignature
            public void visitStringReferences​(ResChunk.RefVisitor visitor)
            ```

        []{#visitStringReferences(int[],com.facebook.buck.android.resources.ResChunk.RefVisitor)}

        -   #### visitStringReferences

            ``` methodSignature
            public void visitStringReferences​(int[] idsToVisit,
                                              ResChunk.RefVisitor visitor)
            ```

        []{#transformReferences(com.facebook.buck.android.resources.ResChunk.RefTransformer)}

        -   #### transformReferences

            ``` methodSignature
            public void transformReferences​(ResChunk.RefTransformer visitor)
            ```

        []{#transformReferences(int[],com.facebook.buck.android.resources.ResChunk.RefTransformer)}

        -   #### transformReferences

            ``` methodSignature
            public void transformReferences​(int[] ids,
                                            ResChunk.RefTransformer visitor)
            ```

        []{#visitReferences(int[],com.facebook.buck.android.resources.ResChunk.RefVisitor)}

        -   #### visitReferences

            ``` methodSignature
            public void visitReferences​(int[] ids,
                                        ResChunk.RefVisitor visitor)
            ```

        []{#reassignIds(com.facebook.buck.android.resources.ReferenceMapper)}

        -   #### reassignIds

            ``` methodSignature
            public void reassignIds​(ReferenceMapper refMapping)
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
