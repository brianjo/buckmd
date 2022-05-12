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
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.android.resources](package-summary.html)
:::

## Class ResTablePackage {#class-restablepackage .title title="Class ResTablePackage"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.android.resources.ResChunk](ResChunk.html "class in com.facebook.buck.android.resources")

    -   -   com.facebook.buck.android.resources.ResTablePackage

::: description
-   

    ------------------------------------------------------------------------

        public class ResTablePackage
        extends ResChunk

    ::: block
    A Package consists of a header: ResTable_header u16 chunk_type u16
    header_size u32 chunk_size u32 package_id u16\[128\] name u32
    typeStringOffset u32 lastPublicTypeOffset u32 keyStringOffset u32
    lastPublicKeyOffset u32 typeIdOffset
    The header is followed by a types string pool (containing types like
    \"id\", \"attr\", \"drawable\", \...) and a keys string pool
    (containing the names of resources). Then follows a TypeSpec for
    each type (# of types can be derived from the size of the types
    stringpool).
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

          Modifier and Type   Field                Description
          ------------------- -------------------- -------------
          `static int`        `APP_PACKAGE_ID`      
          `static int`        `HEADER_SIZE`         
          `static int`        `NAME_DATA_LENGTH`    

          : Fields[ ]{.tabEnd}

        -   []{#fields.inherited.from.class.com.facebook.buck.android.resources.ResChunk}

            ### Fields inherited from class com.facebook.buck.android.resources.[ResChunk](ResChunk.html "class in com.facebook.buck.android.resources")

            `CHUNK_RES_TABLE_PACKAGE, CHUNK_RES_TABLE_TYPE, CHUNK_RES_TABLE_TYPE_SPEC, CHUNK_RESOURCE_TABLE, CHUNK_STRING_POOL, CHUNK_XML_REF_MAP, CHUNK_XML_TREE`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                        Description
          ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ -------------
          `ResTablePackage​(int chunkSize,                int packageId,                byte[] nameData,                StringPool types,                StringPool keys,                List<ResTableTypeSpec> typeSpecs)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type          Method                                                                         Description
          -------------------------- ------------------------------------------------------------------------------ -------------
          `void`                     `dump​(StringPool strings,     PrintStream out)`                                 
          `StringPool`               `getKeys()`                                                                     
          `byte[]`                   `getNameData()`                                                                 
          `String`                   `getRefName​(int i)`                                                             
          `StringPool`               `getTypes()`                                                                    
          `ResTableTypeSpec`         `getTypeSpec​(int type)`                                                         
          `List<ResTableTypeSpec>`   `getTypeSpecs()`                                                                
          `void`                     `put​(ByteBuffer output)`                                                        
          `void`                     `reassignIds​(ReferenceMapper refMapping)`                                       
          `static ResTablePackage`   `slice​(ResTablePackage resPackage,      Map<Integer,​Integer> countsToSlice)`    
          `void`                     `transformStringReferences​(ResChunk.RefTransformer visitor)`                    
          `void`                     `visitStringReferences​(ResChunk.RefVisitor visitor)`                            

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
                Values](../../../../../constant-values.html#com.facebook.buck.android.resources.ResTablePackage.HEADER_SIZE)

        []{#APP_PACKAGE_ID}

        -   #### APP_PACKAGE_ID

                public static final int APP_PACKAGE_ID

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.android.resources.ResTablePackage.APP_PACKAGE_ID)

        []{#NAME_DATA_LENGTH}

        -   #### NAME_DATA_LENGTH

                public static final int NAME_DATA_LENGTH

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.android.resources.ResTablePackage.NAME_DATA_LENGTH)
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(int,int,byte[],com.facebook.buck.android.resources.StringPool,com.facebook.buck.android.resources.StringPool,java.util.List)}

        -   #### ResTablePackage

                public ResTablePackage​(int chunkSize,
                                       int packageId,
                                       byte[] nameData,
                                       StringPool types,
                                       StringPool keys,
                                       List<ResTableTypeSpec> typeSpecs)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#reassignIds(com.facebook.buck.android.resources.ReferenceMapper)}

        -   #### reassignIds

            ``` methodSignature
            public void reassignIds​(ReferenceMapper refMapping)
            ```

        []{#slice(com.facebook.buck.android.resources.ResTablePackage,java.util.Map)}

        -   #### slice

            ``` methodSignature
            public static ResTablePackage slice​(ResTablePackage resPackage,
                                                Map<Integer,​Integer> countsToSlice)
            ```

        []{#put(java.nio.ByteBuffer)}

        -   #### put

            ``` methodSignature
            public void put​(ByteBuffer output)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `put` in class `ResChunk`

        []{#dump(com.facebook.buck.android.resources.StringPool,java.io.PrintStream)}

        -   #### dump

            ``` methodSignature
            public void dump​(StringPool strings,
                             PrintStream out)
            ```

        []{#getTypeSpecs()}

        -   #### getTypeSpecs

            ``` methodSignature
            public List<ResTableTypeSpec> getTypeSpecs()
            ```

        []{#getKeys()}

        -   #### getKeys

            ``` methodSignature
            public StringPool getKeys()
            ```

        []{#getTypeSpec(int)}

        -   #### getTypeSpec

            ``` methodSignature
            public ResTableTypeSpec getTypeSpec​(int type)
            ```

        []{#getTypes()}

        -   #### getTypes

            ``` methodSignature
            public StringPool getTypes()
            ```

        []{#getNameData()}

        -   #### getNameData

            ``` methodSignature
            public byte[] getNameData()
            ```

        []{#transformStringReferences(com.facebook.buck.android.resources.ResChunk.RefTransformer)}

        -   #### transformStringReferences

            ``` methodSignature
            public void transformStringReferences​(ResChunk.RefTransformer visitor)
            ```

        []{#visitStringReferences(com.facebook.buck.android.resources.ResChunk.RefVisitor)}

        -   #### visitStringReferences

            ``` methodSignature
            public void visitStringReferences​(ResChunk.RefVisitor visitor)
            ```

        []{#getRefName(int)}

        -   #### getRefName

            ``` methodSignature
            public String getRefName​(int i)
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
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
-   [Constr](#constructor.detail) \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
