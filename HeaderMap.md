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
[Package]{.packageLabelInType} [com.facebook.buck.apple.clang](package-summary.html)
:::

## Class HeaderMap {#class-headermap .title title="Class HeaderMap"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.apple.clang.HeaderMap

::: description
-   

    ------------------------------------------------------------------------

        public class HeaderMap
        extends Object

    ::: block
    Header maps are essentially hash maps from strings to paths (coded
    as two strings: a prefix and a suffix).
    This class provides support for reading and generating clang header
    maps. No spec is available but we conform to the [reader class
    defined in the Clang
    documentation](http://clang.llvm.org/doxygen/HeaderMap_8h_source.html).

    Note: currently we don\'t support offsets greater than
    MAX_SIGNED_INT.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static class `       | `HeaderMap.Builder`   | ::: block             |
        |                       |                       | Build a header map    |
        |                       |                       | from individual       |
        |                       |                       | mappings.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static interface `   | `Header               | ::: block             |
        |                       | Map.HeaderMapVisitor` | Visitor function for  |
        |                       |                       | [`visit(He            |
        |                       |                       | aderMapVisitor)`](#vi |
        |                       |                       | sit(com.facebook.buck |
        |                       |                       | .apple.clang.HeaderMa |
        |                       |                       | p.HeaderMapVisitor)). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type            Method                                        Description
          ---------------------------- --------------------------------------------- -------------
          `static HeaderMap.Builder`   `builder()`                                    
          `static HeaderMap`           `deserialize​(byte[] bytes)`                    
          `static HeaderMap`           `deserialize​(ByteBuffer buffer)`               
          `byte[]`                     `getBytes()`                                   
          `byte[]`                     `getBytes​(ByteOrder bo)`                       
          `int`                        `getMaxValueLength()`                          
          `int`                        `getNumBuckets()`                              
          `int`                        `getNumEntries()`                              
          `int`                        `getRequiredBufferCapacity()`                  
          `static HeaderMap`           `loadFromFile​(File hmapFile)`                  
          `String`                     `lookup​(String str)`                           
          `void`                       `print​(Appendable stream)`                     
          `void`                       `serialize​(ByteBuffer buffer)`                 
          `String`                     `toString()`                                   
          `void`                       `visit​(HeaderMap.HeaderMapVisitor visitor)`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
          Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
          .tableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getNumEntries()}

        -   #### getNumEntries

            ``` methodSignature
            public int getNumEntries()
            ```

        []{#getNumBuckets()}

        -   #### getNumBuckets

            ``` methodSignature
            public int getNumBuckets()
            ```

        []{#getMaxValueLength()}

        -   #### getMaxValueLength

            ``` methodSignature
            public int getMaxValueLength()
            ```

        []{#visit(com.facebook.buck.apple.clang.HeaderMap.HeaderMapVisitor)}

        -   #### visit

            ``` methodSignature
            public void visit​(HeaderMap.HeaderMapVisitor visitor)
            ```

        []{#toString()}

        -   #### toString

            ``` methodSignature
            public String toString()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `toString` in class `Object`

        []{#print(java.lang.Appendable)}

        -   #### print

            ``` methodSignature
            public void print​(Appendable stream)
            ```

        []{#lookup(java.lang.String)}

        -   #### lookup

            ``` methodSignature
            @Nullable
            public String lookup​(String str)
            ```

        []{#deserialize(byte[])}

        -   #### deserialize

            ``` methodSignature
            @Nullable
            public static HeaderMap deserialize​(byte[] bytes)
            ```

        []{#deserialize(java.nio.ByteBuffer)}

        -   #### deserialize

            ``` methodSignature
            @Nullable
            public static HeaderMap deserialize​(ByteBuffer buffer)
            ```

        []{#loadFromFile(java.io.File)}

        -   #### loadFromFile

            ``` methodSignature
            public static HeaderMap loadFromFile​(File hmapFile)
                                          throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#getRequiredBufferCapacity()}

        -   #### getRequiredBufferCapacity

            ``` methodSignature
            public int getRequiredBufferCapacity()
            ```

        []{#getBytes()}

        -   #### getBytes

            ``` methodSignature
            public byte[] getBytes()
            ```

        []{#getBytes(java.nio.ByteOrder)}

        -   #### getBytes

            ``` methodSignature
            public byte[] getBytes​(ByteOrder bo)
            ```

        []{#serialize(java.nio.ByteBuffer)}

        -   #### serialize

            ``` methodSignature
            public void serialize​(ByteBuffer buffer)
            ```

        []{#builder()}

        -   #### builder

            ``` methodSignature
            public static HeaderMap.Builder builder()
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
