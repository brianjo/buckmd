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
[Package]{.packageLabelInType} [com.facebook.buck.cxx.toolchain.elf](package-summary.html)
:::

## Class ElfHeader {#class-elfheader .title title="Class ElfHeader"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.cxx.toolchain.elf.ElfHeader

::: description
-   

    ------------------------------------------------------------------------

        public class ElfHeader
        extends Object

    ::: block
    Encapsulate the data found in an ELF header.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type   Class                 Description
          ------------------- --------------------- -------------
          `static class `     `ElfHeader.EIClass`    
          `static class `     `ElfHeader.EIData`     

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type     Field           Description
          --------------------- --------------- -------------
          `int`                 `e_ehsize`       
          `long`                `e_entry`        
          `long`                `e_flags`        
          `byte[]`              `e_ident`        
          `int`                 `e_machine`      
          `int`                 `e_phentsize`    
          `int`                 `e_phnum`        
          `long`                `e_phoff`        
          `int`                 `e_shentsize`    
          `int`                 `e_shnum`        
          `long`                `e_shoff`        
          `int`                 `e_shstrndx`     
          `int`                 `e_type`         
          `long`                `e_version`      
          `ElfHeader.EIClass`   `ei_class`       
          `static int`          `EI_CLASS`       
          `ElfHeader.EIData`    `ei_data`        
          `static int`          `EI_DATA`        
          `static int`          `EI_MAG0`        
          `static int`          `EI_MAG1`        
          `static int`          `EI_MAG2`        
          `static int`          `EI_MAG3`        
          `static int`          `EI_NIDENT`      
          `static int`          `EI_PAD`         
          `static int`          `EI_VERSION`     
          `static byte`         `ELFMAG0`        
          `static byte`         `ELFMAG1`        
          `static byte`         `ELFMAG2`        
          `static byte`         `ELFMAG3`        

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                       Description
          ------------------- ---------------------------- -------------
          `ElfHeader`         `withEntry​(long e_entry)`     
          `void`              `write​(ByteBuffer buffer)`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
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

        []{#EI_MAG0}

        -   #### EI_MAG0

                public static final int EI_MAG0

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../constant-values.html#com.facebook.buck.cxx.toolchain.elf.ElfHeader.EI_MAG0)

        []{#EI_MAG1}

        -   #### EI_MAG1

                public static final int EI_MAG1

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../constant-values.html#com.facebook.buck.cxx.toolchain.elf.ElfHeader.EI_MAG1)

        []{#EI_MAG2}

        -   #### EI_MAG2

                public static final int EI_MAG2

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../constant-values.html#com.facebook.buck.cxx.toolchain.elf.ElfHeader.EI_MAG2)

        []{#EI_MAG3}

        -   #### EI_MAG3

                public static final int EI_MAG3

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../constant-values.html#com.facebook.buck.cxx.toolchain.elf.ElfHeader.EI_MAG3)

        []{#EI_CLASS}

        -   #### EI_CLASS

                public static final int EI_CLASS

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../constant-values.html#com.facebook.buck.cxx.toolchain.elf.ElfHeader.EI_CLASS)

        []{#EI_DATA}

        -   #### EI_DATA

                public static final int EI_DATA

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../constant-values.html#com.facebook.buck.cxx.toolchain.elf.ElfHeader.EI_DATA)

        []{#EI_VERSION}

        -   #### EI_VERSION

                public static final int EI_VERSION

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../constant-values.html#com.facebook.buck.cxx.toolchain.elf.ElfHeader.EI_VERSION)

        []{#EI_PAD}

        -   #### EI_PAD

                public static final int EI_PAD

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../constant-values.html#com.facebook.buck.cxx.toolchain.elf.ElfHeader.EI_PAD)

        []{#EI_NIDENT}

        -   #### EI_NIDENT

                public static final int EI_NIDENT

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../constant-values.html#com.facebook.buck.cxx.toolchain.elf.ElfHeader.EI_NIDENT)

        []{#ELFMAG0}

        -   #### ELFMAG0

                public static final byte ELFMAG0

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../constant-values.html#com.facebook.buck.cxx.toolchain.elf.ElfHeader.ELFMAG0)

        []{#ELFMAG1}

        -   #### ELFMAG1

                public static final byte ELFMAG1

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../constant-values.html#com.facebook.buck.cxx.toolchain.elf.ElfHeader.ELFMAG1)

        []{#ELFMAG2}

        -   #### ELFMAG2

                public static final byte ELFMAG2

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../constant-values.html#com.facebook.buck.cxx.toolchain.elf.ElfHeader.ELFMAG2)

        []{#ELFMAG3}

        -   #### ELFMAG3

                public static final byte ELFMAG3

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../constant-values.html#com.facebook.buck.cxx.toolchain.elf.ElfHeader.ELFMAG3)

        []{#ei_class}

        -   #### ei_class

                public final ElfHeader.EIClass ei_class

        []{#ei_data}

        -   #### ei_data

                public final ElfHeader.EIData ei_data

        []{#e_ident}

        -   #### e_ident

                public final byte[] e_ident

        []{#e_type}

        -   #### e_type

                public final int e_type

        []{#e_machine}

        -   #### e_machine

                public final int e_machine

        []{#e_version}

        -   #### e_version

                public final long e_version

        []{#e_entry}

        -   #### e_entry

                public final long e_entry

        []{#e_phoff}

        -   #### e_phoff

                public final long e_phoff

        []{#e_shoff}

        -   #### e_shoff

                public final long e_shoff

        []{#e_flags}

        -   #### e_flags

                public final long e_flags

        []{#e_ehsize}

        -   #### e_ehsize

                public final int e_ehsize

        []{#e_phentsize}

        -   #### e_phentsize

                public final int e_phentsize

        []{#e_phnum}

        -   #### e_phnum

                public final int e_phnum

        []{#e_shentsize}

        -   #### e_shentsize

                public final int e_shentsize

        []{#e_shnum}

        -   #### e_shnum

                public final int e_shnum

        []{#e_shstrndx}

        -   #### e_shstrndx

                public final int e_shstrndx
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#write(java.nio.ByteBuffer)}

        -   #### write

            ``` methodSignature
            public void write​(ByteBuffer buffer)
            ```

        []{#withEntry(long)}

        -   #### withEntry

            ``` methodSignature
            public ElfHeader withEntry​(long e_entry)
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
