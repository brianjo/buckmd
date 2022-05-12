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
[Package]{.packageLabelInType} [com.facebook.buck.util](package-summary.html)
:::

## Class ByteBufferReplacer {#class-bytebufferreplacer .title title="Class ByteBufferReplacer"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.util.ByteBufferReplacer

::: description
-   

    ------------------------------------------------------------------------

        public class ByteBufferReplacer
        extends Object

    ::: block
    Performs an in-place find-and-replace on
    [`ByteBuffer`](http://docs.oracle.com/javase/7/docs/api/java/nio/ByteBuffer.html?is-external=true "class or interface in java.nio"){.externalLink}
    objects, where the replacements are of equal length to what they\'re
    replacing.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                Description
          ------------------------------------------------------------------------------------------ -------------
          `ByteBufferReplacer​(com.google.common.collect.ImmutableMap<byte[],​byte[]> replacements)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `stati                | `fromPaths​(com        | ::: block             |
        | c ByteBufferReplacer` | .google.common.collec | Build a replacer      |
        |                       | t.ImmutableMap<Path,​P | using the given map   |
        |                       | ath> paths,           | of paths to           |
        |                       | char separator,       | replacement paths,    |
        |                       |     Charset charset)` | using `charset` to    |
        |                       |                       | convert to underlying |
        |                       |                       | byte arrays.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `replac               |                       |
        |                       | e​(ByteBuffer buffer)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `replace​(ByteB        | ::: block             |
        |                       | uffer buffer,         | Perform an in-place   |
        |                       | int maxReplacements)` | replacement pass over |
        |                       |                       | the given buffer      |
        |                       |                       | (bounded by           |
        |                       |                       | [`Buffer.             |
        |                       |                       | position`](http://doc |
        |                       |                       | s.oracle.com/javase/7 |
        |                       |                       | /docs/api/java/nio/Bu |
        |                       |                       | ffer.html?is-external |
        |                       |                       | =true#position "class |
        |                       |                       |  or interface in java |
        |                       |                       | .nio"){.externalLink} |
        |                       |                       | and                   |
        |                       |                       | [`Buf                 |
        |                       |                       | fer.limit`](http://do |
        |                       |                       | cs.oracle.com/javase/ |
        |                       |                       | 7/docs/api/java/nio/B |
        |                       |                       | uffer.html?is-externa |
        |                       |                       | l=true#limit "class o |
        |                       |                       | r interface in java.n |
        |                       |                       | io"){.externalLink}). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
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

        []{#<init>(com.google.common.collect.ImmutableMap)}

        -   #### ByteBufferReplacer

                public ByteBufferReplacer​(com.google.common.collect.ImmutableMap<byte[],​byte[]> replacements)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#fromPaths(com.google.common.collect.ImmutableMap,char,java.nio.charset.Charset)}

        -   #### fromPaths

            ``` methodSignature
            public static ByteBufferReplacer fromPaths​(com.google.common.collect.ImmutableMap<Path,​Path> paths,
                                                       char separator,
                                                       Charset charset)
            ```

            ::: block
            Build a replacer using the given map of paths to replacement
            paths, using `charset` to convert to underlying byte arrays.
            If the replacement paths are not long enough, use the given
            path separator to fill.
            :::

        []{#replace(java.nio.ByteBuffer,int)}

        -   #### replace

            ``` methodSignature
            public int replace​(ByteBuffer buffer,
                               int maxReplacements)
            ```

            ::: block
            Perform an in-place replacement pass over the given buffer
            (bounded by
            [`Buffer.position`](http://docs.oracle.com/javase/7/docs/api/java/nio/Buffer.html?is-external=true#position "class or interface in java.nio"){.externalLink}
            and
            [`Buffer.limit`](http://docs.oracle.com/javase/7/docs/api/java/nio/Buffer.html?is-external=true#limit "class or interface in java.nio"){.externalLink}).
            :::

            [Parameters:]{.paramLabel}
            :   `buffer` - the buffer on which to perform replacements.
            :   `maxReplacements` - the maximum number of replacements
                to perform (-1 means unlimited).

            [Returns:]{.returnLabel}
            :   the number of replacements that happened.

        []{#replace(java.nio.ByteBuffer)}

        -   #### replace

            ``` methodSignature
            public int replace​(ByteBuffer buffer)
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
