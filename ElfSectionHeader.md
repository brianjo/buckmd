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
[Package]{.packageLabelInType} [com.facebook.buck.cxx.toolchain.elf](package-summary.html)
:::

## Class ElfSectionHeader {#class-elfsectionheader .title title="Class ElfSectionHeader"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.cxx.toolchain.elf.ElfSectionHeader

::: description
-   

    ------------------------------------------------------------------------

        public class ElfSectionHeader
        extends Object

    ::: block
    Encapsulate the data in an ELF section header.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type   Class                       Description
          ------------------- --------------------------- -------------
          `static class `     `ElfSectionHeader.SHType`    

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type           Field            Description
          --------------------------- ---------------- -------------
          `long`                      `sh_addr`         
          `long`                      `sh_addralign`    
          `long`                      `sh_entsize`      
          `long`                      `sh_flags`        
          `long`                      `sh_info`         
          `long`                      `sh_link`         
          `long`                      `sh_name`         
          `long`                      `sh_off`          
          `long`                      `sh_size`         
          `ElfSectionHeader.SHType`   `sh_type`         

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                                                                                 Description
          ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `ElfSectionHeader​(long sh_name,                 ElfSectionHeader.SHType sh_type,                 long sh_flags,                 long sh_addr,                 long sh_off,                 long sh_size,                 long sh_link,                 long sh_info,                 long sh_addralign,                 long sh_entsize)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type    Method                                                       Description
          -------------------- ------------------------------------------------------------ -------------
          `ElfSectionHeader`   `withInfo​(long info)`                                         
          `ElfSectionHeader`   `withSize​(long size)`                                         
          `void`               `write​(ElfHeader.EIClass eiClass,      ByteBuffer buffer)`    

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

        []{#sh_name}

        -   #### sh_name

                public final long sh_name

        []{#sh_type}

        -   #### sh_type

                public final ElfSectionHeader.SHType sh_type

        []{#sh_flags}

        -   #### sh_flags

                public final long sh_flags

        []{#sh_addr}

        -   #### sh_addr

                public final long sh_addr

        []{#sh_off}

        -   #### sh_off

                public final long sh_off

        []{#sh_size}

        -   #### sh_size

                public final long sh_size

        []{#sh_link}

        -   #### sh_link

                public final long sh_link

        []{#sh_info}

        -   #### sh_info

                public final long sh_info

        []{#sh_addralign}

        -   #### sh_addralign

                public final long sh_addralign

        []{#sh_entsize}

        -   #### sh_entsize

                public final long sh_entsize
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(long,com.facebook.buck.cxx.toolchain.elf.ElfSectionHeader.SHType,long,long,long,long,long,long,long,long)}

        -   #### ElfSectionHeader

                public ElfSectionHeader​(long sh_name,
                                        ElfSectionHeader.SHType sh_type,
                                        long sh_flags,
                                        long sh_addr,
                                        long sh_off,
                                        long sh_size,
                                        long sh_link,
                                        long sh_info,
                                        long sh_addralign,
                                        long sh_entsize)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#write(com.facebook.buck.cxx.toolchain.elf.ElfHeader.EIClass,java.nio.ByteBuffer)}

        -   #### write

            ``` methodSignature
            public void write​(ElfHeader.EIClass eiClass,
                              ByteBuffer buffer)
            ```

        []{#withSize(long)}

        -   #### withSize

            ``` methodSignature
            public ElfSectionHeader withSize​(long size)
            ```

        []{#withInfo(long)}

        -   #### withInfo

            ``` methodSignature
            public ElfSectionHeader withInfo​(long info)
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
