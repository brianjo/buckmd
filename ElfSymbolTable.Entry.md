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

## Class ElfSymbolTable.Entry {#class-elfsymboltable.entry .title title="Class ElfSymbolTable.Entry"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.cxx.toolchain.elf.ElfSymbolTable.Entry

::: description
-   

    Enclosing class:
    :   [ElfSymbolTable](ElfSymbolTable.html "class in com.facebook.buck.cxx.toolchain.elf")

    ------------------------------------------------------------------------

        public static class ElfSymbolTable.Entry
        extends Object

    ::: block
    Encapsulate the data in an ELF section header.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type   Class                         Description
          ------------------- ----------------------------- -------------
          `static class `     `ElfSymbolTable.Entry.Info`    

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type             Field        Description
          ----------------------------- ------------ -------------
          `ElfSymbolTable.Entry.Info`   `st_info`     
          `long`                        `st_name`     
          `int`                         `st_other`    
          `int`                         `st_shndx`    
          `long`                        `st_size`     
          `long`                        `st_value`    

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                  Description
          -------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `Entry​(long st_name,      ElfSymbolTable.Entry.Info st_info,      int st_other,      int st_shndx,      long st_value,      long st_size)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type        Method                  Description
          ------------------------ ----------------------- -------------
          `ElfSymbolTable.Entry`   `withSize​(long size)`    

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

        []{#st_name}

        -   #### st_name

                public final long st_name

        []{#st_info}

        -   #### st_info

                public final ElfSymbolTable.Entry.Info st_info

        []{#st_other}

        -   #### st_other

                public final int st_other

        []{#st_shndx}

        -   #### st_shndx

                public final int st_shndx

        []{#st_value}

        -   #### st_value

                public final long st_value

        []{#st_size}

        -   #### st_size

                public final long st_size
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(long,com.facebook.buck.cxx.toolchain.elf.ElfSymbolTable.Entry.Info,int,int,long,long)}

        -   #### Entry

                public Entry​(long st_name,
                             ElfSymbolTable.Entry.Info st_info,
                             int st_other,
                             int st_shndx,
                             long st_value,
                             long st_size)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#withSize(long)}

        -   #### withSize

            ``` methodSignature
            public ElfSymbolTable.Entry withSize​(long size)
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
