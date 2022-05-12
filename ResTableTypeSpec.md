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
[Package]{.packageLabelInType} [com.facebook.buck.android.resources](package-summary.html)
:::

## Class ResTableTypeSpec {#class-restabletypespec .title title="Class ResTableTypeSpec"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.android.resources.ResChunk](ResChunk.html "class in com.facebook.buck.android.resources")

    -   -   com.facebook.buck.android.resources.ResTableTypeSpec

::: description
-   

    ------------------------------------------------------------------------

        public class ResTableTypeSpec
        extends ResChunk

    ::: block
    ResTableTypeSpec is a ResChunk specifying the flags for each
    resource of a given type. These flags specify which types of
    configuration contain multiple values for a given resource. A
    ResTableTypeSpec consists of: ResChunk_header u16 type u16
    header_size u32 chunk_size u8 id u8 0x00 u16 0x0000 u32 entry_count
    This is then followed by entry_count u32s giving the flags for each
    resource of this type.

    In practice, this is then followed by a ResTableType for each
    configuration that has resources of this type. For convenience,
    those are considered to be part of the ResTableTypeSpec.
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

        -   []{#fields.inherited.from.class.com.facebook.buck.android.resources.ResChunk}

            ### Fields inherited from class com.facebook.buck.android.resources.[ResChunk](ResChunk.html "class in com.facebook.buck.android.resources")

            `CHUNK_RES_TABLE_PACKAGE, CHUNK_RES_TABLE_TYPE, CHUNK_RES_TABLE_TYPE_SPEC, CHUNK_RESOURCE_TABLE, CHUNK_STRING_POOL, CHUNK_XML_REF_MAP, CHUNK_XML_TREE`
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `void`                | `dump​(StringPool      |                       |
        |                       |  strings,     ResTabl |                       |
        |                       | ePackage resPackage,  |                       |
        |                       |     PrintStream out)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `sta                  | `get​(ByteBuffer buf)` |                       |
        | tic ResTableTypeSpec` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `List<ResTableType>`  | `getConfigs()`        |                       |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `getEntryCount()`     |                       |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `getResourceType()`   |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getRes               |                       |
        |                       | ourceTypeName​(ResTabl |                       |
        |                       | ePackage resPackage)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `getTotalSize()`      | ::: block             |
        |                       |                       | For most chunk\'s     |
        |                       |                       | totalSize ==          |
        |                       |                       | chunkSize.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `pu                   |                       |
        |                       | t​(ByteBuffer output)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `reassignIds​(Referen  |                       |
        |                       | ceMapper refMapping)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `sta                  | `sli                  |                       |
        | tic ResTableTypeSpec` | ce​(ResTableTypeSpec s |                       |
        |                       | pec,      int count)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `transformKeyRe       |                       |
        |                       | ferences​(ResChunk.Ref |                       |
        |                       | Transformer visitor)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `transformStringRe    |                       |
        |                       | ferences​(ResChunk.Ref |                       |
        |                       | Transformer visitor)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `visitK               |                       |
        |                       | eyReferences​(ResChunk |                       |
        |                       | .RefVisitor visitor)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `visitRef             |                       |
        |                       | erences​(int[] ids,    |                       |
        |                       |              ResChunk |                       |
        |                       | .RefVisitor visitor)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `visitStringReference |                       |
        |                       | s​(int[] ids,          |                       |
        |                       |              ResChunk |                       |
        |                       | .RefVisitor visitor)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `visitStri            |                       |
        |                       | ngReferences​(ResChunk |                       |
        |                       | .RefVisitor visitor)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.android.resources.ResChunk}

            ### Methods inherited from class com.facebook.buck.android.resources.[ResChunk](ResChunk.html "class in com.facebook.buck.android.resources")

            `getChunkSize, getHeaderSize, getType, serialize, slice, slice, wrap`

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
    -   []{#method.detail}

        ### Method Detail

        []{#slice(com.facebook.buck.android.resources.ResTableTypeSpec,int)}

        -   #### slice

            ``` methodSignature
            public static ResTableTypeSpec slice​(ResTableTypeSpec spec,
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
            public static ResTableTypeSpec get​(ByteBuffer buf)
            ```

        []{#getTotalSize()}

        -   #### getTotalSize

            ``` methodSignature
            public int getTotalSize()
            ```

            ::: block
            [Description copied from
            class: `ResChunk`]{.descfrmTypeLabel}
            :::

            ::: block
            For most chunk\'s totalSize == chunkSize. For some types,
            the type logically consists of multiple chunks. In these
            cases, totalSize is the sum of all the chunks. This is the
            full size written/read from a buffer for get/put.
            :::

            [Overrides:]{.overrideSpecifyLabel}
            :   `getTotalSize` in class `ResChunk`

        []{#getResourceTypeName(com.facebook.buck.android.resources.ResTablePackage)}

        -   #### getResourceTypeName

            ``` methodSignature
            public String getResourceTypeName​(ResTablePackage resPackage)
            ```

        []{#dump(com.facebook.buck.android.resources.StringPool,com.facebook.buck.android.resources.ResTablePackage,java.io.PrintStream)}

        -   #### dump

            ``` methodSignature
            public void dump​(StringPool strings,
                             ResTablePackage resPackage,
                             PrintStream out)
            ```

        []{#getResourceType()}

        -   #### getResourceType

            ``` methodSignature
            public int getResourceType()
            ```

        []{#getConfigs()}

        -   #### getConfigs

            ``` methodSignature
            public List<ResTableType> getConfigs()
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

        []{#visitStringReferences(com.facebook.buck.android.resources.ResChunk.RefVisitor)}

        -   #### visitStringReferences

            ``` methodSignature
            public void visitStringReferences​(ResChunk.RefVisitor visitor)
            ```

        []{#visitStringReferences(int[],com.facebook.buck.android.resources.ResChunk.RefVisitor)}

        -   #### visitStringReferences

            ``` methodSignature
            public void visitStringReferences​(int[] ids,
                                              ResChunk.RefVisitor visitor)
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

        []{#getEntryCount()}

        -   #### getEntryCount

            ``` methodSignature
            public int getEntryCount()
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
-   Field \| 
-   Constr \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
