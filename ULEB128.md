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
-   Nested \| 
-   Field \| 
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.cxx.toolchain.objectfile](package-summary.html)
:::

## Class ULEB128 {#class-uleb128 .title title="Class ULEB128"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.cxx.toolchain.objectfile.ULEB128

::: description
-   

    ------------------------------------------------------------------------

        public class ULEB128
        extends Object

    ::: block
    Utility for ULEB128 encoding as used by ld64.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor   Description
          ------------- -------------
          `ULEB128()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static long`         | `read​(By              | ::: block             |
        |                       | teBuffer byteBuffer)` | Reads a number        |
        |                       |                       | encoded as ULEB128.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static int`          | `size​(long value)`    | ::: block             |
        |                       |                       | Computes the size     |
        |                       |                       | when encoding values  |
        |                       |                       | using ULEB128.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static int`          | `writ                 | ::: block             |
        |                       | e​(ByteBuffer byteBuff | Encodes a value using |
        |                       | er,      long value)` | ULEB128 encoding.     |
        |                       |                       | :::                   |
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
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### ULEB128

                public ULEB128()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#size(long)}

        -   #### size

            ``` methodSignature
            public static int size​(long value)
            ```

            ::: block
            Computes the size when encoding values using ULEB128.
            :::

            [Parameters:]{.paramLabel}
            :   `value` - The value for which to return the size of in
                ULEB128.

            [Returns:]{.returnLabel}
            :   The number of bytes needed to encode {@param value}.

        []{#write(java.nio.ByteBuffer,long)}

        -   #### write

            ``` methodSignature
            public static int write​(ByteBuffer byteBuffer,
                                    long value)
            ```

            ::: block
            Encodes a value using ULEB128 encoding.
            :::

            [Parameters:]{.paramLabel}
            :   `byteBuffer` - The output destination used for encoding.
            :   `value` - The value to encode.

            [Returns:]{.returnLabel}
            :   Number of bytes written.

        []{#read(java.nio.ByteBuffer)}

        -   #### read

            ``` methodSignature
            public static long read​(ByteBuffer byteBuffer)
            ```

            ::: block
            Reads a number encoded as ULEB128. If the encoded number
            exceeds 64bits, then a `  java.lang.IllegalStateException`
            exception is thrown because `long` stores a maximum of
            64bits.
            :::

            [Parameters:]{.paramLabel}
            :   `byteBuffer` - The source which to read from.

            [Returns:]{.returnLabel}
            :   The value of the ULEB128 encoded number.
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
-   Nested \| 
-   Field \| 
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   [Constr](#constructor.detail) \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
