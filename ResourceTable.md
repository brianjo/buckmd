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

## Class ResourceTable {#class-resourcetable .title title="Class ResourceTable"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.android.resources.ResChunk](ResChunk.html "class in com.facebook.buck.android.resources")

    -   -   com.facebook.buck.android.resources.ResourceTable

::: description
-   

    ------------------------------------------------------------------------

        public class ResourceTable
        extends ResChunk

    ::: block
    A ResourceTable is the top-level representation of resources.arsc.
    It consists of a header: ResTable_header u32 chunk_type u32
    header_size u32 chunk_size u32 package_count
    The header is followed by a StringPool and then package_count
    packages.

    In practice, aapt always generates .arsc files with package_count ==
    1.
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

          Modifier and Type   Field           Description
          ------------------- --------------- -------------
          `static int`        `HEADER_SIZE`    

          : Fields[ ]{.tabEnd}

        -   []{#fields.inherited.from.class.com.facebook.buck.android.resources.ResChunk}

            ### Fields inherited from class com.facebook.buck.android.resources.[ResChunk](ResChunk.html "class in com.facebook.buck.android.resources")

            `CHUNK_RES_TABLE_PACKAGE, CHUNK_RES_TABLE_TYPE, CHUNK_RES_TABLE_TYPE_SPEC, CHUNK_RESOURCE_TABLE, CHUNK_STRING_POOL, CHUNK_XML_REF_MAP, CHUNK_XML_TREE`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                    Description
          ------------------------------------------------------------------------------ -------------
          `ResourceTable​(StringPool strings,              ResTablePackage resPackage)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type        Method                                                                    Description
          ------------------------ ------------------------------------------------------------------------- -------------
          `void`                   `dump​(PrintStream out)`                                                    
          `void`                   `dumpStrings​(PrintStream out)`                                             
          `static ResourceTable`   `get​(ByteBuffer buf)`                                                      
          `ResTablePackage`        `getPackage()`                                                             
          `StringPool`             `getStrings()`                                                             
          `void`                   `put​(ByteBuffer buf)`                                                      
          `void`                   `reassignIds​(ReferenceMapper refMapping)`                                  
          `static ResourceTable`   `slice​(ResourceTable table,      Map<Integer,​Integer> countsToExtract)`    

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
                Values](../../../../../constant-values.html#com.facebook.buck.android.resources.ResourceTable.HEADER_SIZE)
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.android.resources.StringPool,com.facebook.buck.android.resources.ResTablePackage)}

        -   #### ResourceTable

                public ResourceTable​(StringPool strings,
                                     ResTablePackage resPackage)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#get(java.nio.ByteBuffer)}

        -   #### get

            ``` methodSignature
            public static ResourceTable get​(ByteBuffer buf)
            ```

        []{#put(java.nio.ByteBuffer)}

        -   #### put

            ``` methodSignature
            public void put​(ByteBuffer buf)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `put` in class `ResChunk`

        []{#reassignIds(com.facebook.buck.android.resources.ReferenceMapper)}

        -   #### reassignIds

            ``` methodSignature
            public void reassignIds​(ReferenceMapper refMapping)
            ```

        []{#slice(com.facebook.buck.android.resources.ResourceTable,java.util.Map)}

        -   #### slice

            ``` methodSignature
            public static ResourceTable slice​(ResourceTable table,
                                              Map<Integer,​Integer> countsToExtract)
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

        []{#getPackage()}

        -   #### getPackage

            ``` methodSignature
            public ResTablePackage getPackage()
            ```

        []{#dumpStrings(java.io.PrintStream)}

        -   #### dumpStrings

            ``` methodSignature
            public void dumpStrings​(PrintStream out)
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
