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
[Package]{.packageLabelInType} [com.facebook.buck.util.charset](package-summary.html)
:::

## Class NulTerminatedCharsetDecoder {#class-nulterminatedcharsetdecoder .title title="Class NulTerminatedCharsetDecoder"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.util.charset.NulTerminatedCharsetDecoder

::: description
-   

    ------------------------------------------------------------------------

        @NotThreadSafe
        public class NulTerminatedCharsetDecoder
        extends Object

    ::: block
    Wrapper for
    [`CharsetDecoder`](http://docs.oracle.com/javase/7/docs/api/java/nio/charset/CharsetDecoder.html?is-external=true "class or interface in java.nio.charset"){.externalLink}
    to provide decoding of NUL-terminated bytestrings to Unicode
    Strings.
    Instances of this object are not thread-safe. If you want to re-use
    this object, make sure to synchronize access and invoke
    [`reset()`](#reset()) between uses.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type   Class                                  Description
          ------------------- -------------------------------------- -------------
          `static class `     `NulTerminatedCharsetDecoder.Result`    

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type   Field                                    Description
          ------------------- ---------------------------------------- -------------
          `static int`        `DEFAULT_INITIAL_CHAR_BUFFER_CAPACITY`    

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                             Description
          ------------------------------------------------------------------------------------------------------- -------------
          `NulTerminatedCharsetDecoder​(CharsetDecoder decoder)`                                                    
          `NulTerminatedCharsetDecoder​(CharsetDecoder decoder,                            int initialCapacity)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                      Method                                                                    Description
          -------------------------------------- ------------------------------------------------------------------------- -------------
          `NulTerminatedCharsetDecoder.Result`   `decode​(ByteBuffer in,       CharBuffer out,       boolean endOfInput)`    
          `String`                               `decodeString​(ByteBuffer in)`                                              
          `static String`                        `decodeUTF8String​(ByteBuffer in)`                                          
          `void`                                 `reset()`                                                                  

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
    -   []{#field.detail}

        ### Field Detail

        []{#DEFAULT_INITIAL_CHAR_BUFFER_CAPACITY}

        -   #### DEFAULT_INITIAL_CHAR_BUFFER_CAPACITY

                public static final int DEFAULT_INITIAL_CHAR_BUFFER_CAPACITY

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.util.charset.NulTerminatedCharsetDecoder.DEFAULT_INITIAL_CHAR_BUFFER_CAPACITY)
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(java.nio.charset.CharsetDecoder)}

        -   #### NulTerminatedCharsetDecoder

                public NulTerminatedCharsetDecoder​(CharsetDecoder decoder)

        []{#<init>(java.nio.charset.CharsetDecoder,int)}

        -   #### NulTerminatedCharsetDecoder

                public NulTerminatedCharsetDecoder​(CharsetDecoder decoder,
                                                   int initialCapacity)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#decodeUTF8String(java.nio.ByteBuffer)}

        -   #### decodeUTF8String

            ``` methodSignature
            public static String decodeUTF8String​(ByteBuffer in)
                                           throws CharacterCodingException
            ```

            [Throws:]{.throwsLabel}
            :   `CharacterCodingException`

        []{#decodeString(java.nio.ByteBuffer)}

        -   #### decodeString

            ``` methodSignature
            public String decodeString​(ByteBuffer in)
                                throws CharacterCodingException
            ```

            [Throws:]{.throwsLabel}
            :   `CharacterCodingException`

        []{#decode(java.nio.ByteBuffer,java.nio.CharBuffer,boolean)}

        -   #### decode

            ``` methodSignature
            public NulTerminatedCharsetDecoder.Result decode​(ByteBuffer in,
                                                             CharBuffer out,
                                                             boolean endOfInput)
            ```

        []{#reset()}

        -   #### reset

            ``` methodSignature
            public void reset()
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
