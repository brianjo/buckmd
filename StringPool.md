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

## Class StringPool {#class-stringpool .title title="Class StringPool"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.android.resources.ResChunk](ResChunk.html "class in com.facebook.buck.android.resources")

    -   -   com.facebook.buck.android.resources.StringPool

::: description
-   

    ------------------------------------------------------------------------

        public class StringPool
        extends ResChunk

    ::: block
    A StringPool consists of a header: ResChunk_header u32 chunk_type
    u32 header_size u32 chunk_size u32 string_count u32 style_count u32
    flags - 0x1 sorted, 0x100 utf-8 encoded u32 strings_start - byte
    offset from the beginning to the style data u32 styles_start - byte
    offset from the beginning to the style data
    The header is followed by an u32\[string_count\] array of strings
    offsets (relative to strings_start) where the strings reside. This
    is then followed by a similar array for styles.

    In a utf-8 encoded string pool, a string data consists of: utf-16
    length, utf-8 length, string bytes, \\0.

    In a utf-16 encoded string pool, a string data consists of: utf-16
    length, string bytes, \\0\\0.

    A style is an array of tuples (u32 stringref, u32 start, u32 end). A
    stringref of 0xFFFFFFFF indicates the end of a style array (note
    that the next array may start at the immediately following word).
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

          Modifier and Type     Method                                  Description
          --------------------- --------------------------------------- -------------
          `StringPool`          `copy()`                                 
          `static StringPool`   `create​(Iterable<String> strings)`       
          `void`                `dump​(PrintStream out)`                  
          `static StringPool`   `get​(ByteBuffer buf)`                    
          `String`              `getOutputNormalizedString​(int data)`    
          `String`              `getString​(int id)`                      
          `int`                 `getStringCount()`                       
          `boolean`             `isUtf8()`                               
          `void`                `put​(ByteBuffer output)`                 

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
    -   []{#method.detail}

        ### Method Detail

        []{#create(java.lang.Iterable)}

        -   #### create

            ``` methodSignature
            public static StringPool create​(Iterable<String> strings)
            ```

        []{#get(java.nio.ByteBuffer)}

        -   #### get

            ``` methodSignature
            public static StringPool get​(ByteBuffer buf)
            ```

        []{#put(java.nio.ByteBuffer)}

        -   #### put

            ``` methodSignature
            public void put​(ByteBuffer output)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `put` in class `ResChunk`

        []{#getString(int)}

        -   #### getString

            ``` methodSignature
            public String getString​(int id)
            ```

        []{#dump(java.io.PrintStream)}

        -   #### dump

            ``` methodSignature
            public void dump​(PrintStream out)
            ```

        []{#getStringCount()}

        -   #### getStringCount

            ``` methodSignature
            public int getStringCount()
            ```

        []{#isUtf8()}

        -   #### isUtf8

            ``` methodSignature
            public boolean isUtf8()
            ```

        []{#getOutputNormalizedString(int)}

        -   #### getOutputNormalizedString

            ``` methodSignature
            public String getOutputNormalizedString​(int data)
            ```

        []{#copy()}

        -   #### copy

            ``` methodSignature
            public StringPool copy()
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
