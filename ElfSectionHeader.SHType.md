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
-   [Enum Constants](#enum.constant.summary) \| 
-   Field \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Enum Constants](#enum.constant.detail) \| 
-   Field \| 
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

## Enum ElfSectionHeader.SHType {#enum-elfsectionheader.shtype .title title="Enum ElfSectionHeader.SHType"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [java.lang.Enum](http://docs.oracle.com/javase/7/docs/api/java/lang/Enum.html?is-external=true "class or interface in java.lang"){.externalLink}\<[ElfSectionHeader.SHType](ElfSectionHeader.SHType.html "enum in com.facebook.buck.cxx.toolchain.elf")\>

    -   -   com.facebook.buck.cxx.toolchain.elf.ElfSectionHeader.SHType

::: description
-   

    All Implemented Interfaces:
    :   `Serializable`, `Comparable<ElfSectionHeader.SHType>`

    ```{=html}
    <!-- -->
    ```

    Enclosing class:
    :   [ElfSectionHeader](ElfSectionHeader.html "class in com.facebook.buck.cxx.toolchain.elf")

    ------------------------------------------------------------------------

        public static enum ElfSectionHeader.SHType
        extends Enum<ElfSectionHeader.SHType>
:::

::: summary
-   ::: {.section role="region"}
    -   []{#enum.constant.summary}

        ### Enum Constant Summary

          Enum Constant       Description
          ------------------- -------------
          `SHT_DYNAMIC`        
          `SHT_DYNSYM`         
          `SHT_GNU_VERDEF`     
          `SHT_GNU_VERNEED`    
          `SHT_GNU_VERSYM`     
          `SHT_HASH`           
          `SHT_NOBITS`         
          `SHT_NOTE`           
          `SHT_NULL`           
          `SHT_PROGBITS`       
          `SHT_REL`            
          `SHT_RELA`           
          `SHT_SHLIB`          
          `SHT_STRTAB`         
          `SHT_SYMTAB`         
          `SHT_UNKNOWN`        

          : Enum Constants[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `int`                 | `getValue()`          |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static Elf           | `                     | ::: block             |
        | SectionHeader.SHType` | valueOf​(String name)` | Returns the enum      |
        |                       |                       | constant of this type |
        |                       |                       | with the specified    |
        |                       |                       | name.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static ElfSe         | `values()`            | ::: block             |
        | ctionHeader.SHType[]` |                       | Returns an array      |
        |                       |                       | containing the        |
        |                       |                       | constants of this     |
        |                       |                       | enum type, in the     |
        |                       |                       | order they are        |
        |                       |                       | declared.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Enum}

            ### Methods inherited from class java.lang.[Enum](http://docs.oracle.com/javase/7/docs/api/java/lang/Enum.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, compareTo, equals, finalize, getDeclaringClass, hashCode, name, ordinal, toString, valueOf`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `getClass, notify, notifyAll, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#enum.constant.detail}

        ### Enum Constant Detail

        []{#SHT_NULL}

        -   #### SHT_NULL

                public static final ElfSectionHeader.SHType SHT_NULL

        []{#SHT_PROGBITS}

        -   #### SHT_PROGBITS

                public static final ElfSectionHeader.SHType SHT_PROGBITS

        []{#SHT_SYMTAB}

        -   #### SHT_SYMTAB

                public static final ElfSectionHeader.SHType SHT_SYMTAB

        []{#SHT_STRTAB}

        -   #### SHT_STRTAB

                public static final ElfSectionHeader.SHType SHT_STRTAB

        []{#SHT_RELA}

        -   #### SHT_RELA

                public static final ElfSectionHeader.SHType SHT_RELA

        []{#SHT_HASH}

        -   #### SHT_HASH

                public static final ElfSectionHeader.SHType SHT_HASH

        []{#SHT_DYNAMIC}

        -   #### SHT_DYNAMIC

                public static final ElfSectionHeader.SHType SHT_DYNAMIC

        []{#SHT_NOTE}

        -   #### SHT_NOTE

                public static final ElfSectionHeader.SHType SHT_NOTE

        []{#SHT_NOBITS}

        -   #### SHT_NOBITS

                public static final ElfSectionHeader.SHType SHT_NOBITS

        []{#SHT_REL}

        -   #### SHT_REL

                public static final ElfSectionHeader.SHType SHT_REL

        []{#SHT_SHLIB}

        -   #### SHT_SHLIB

                public static final ElfSectionHeader.SHType SHT_SHLIB

        []{#SHT_DYNSYM}

        -   #### SHT_DYNSYM

                public static final ElfSectionHeader.SHType SHT_DYNSYM

        []{#SHT_GNU_VERNEED}

        -   #### SHT_GNU_VERNEED

                public static final ElfSectionHeader.SHType SHT_GNU_VERNEED

        []{#SHT_GNU_VERDEF}

        -   #### SHT_GNU_VERDEF

                public static final ElfSectionHeader.SHType SHT_GNU_VERDEF

        []{#SHT_GNU_VERSYM}

        -   #### SHT_GNU_VERSYM

                public static final ElfSectionHeader.SHType SHT_GNU_VERSYM

        []{#SHT_UNKNOWN}

        -   #### SHT_UNKNOWN

                public static final ElfSectionHeader.SHType SHT_UNKNOWN
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#values()}

        -   #### values

            ``` methodSignature
            public static ElfSectionHeader.SHType[] values()
            ```

            ::: block
            Returns an array containing the constants of this enum type,
            in the order they are declared. This method may be used to
            iterate over the constants as follows:
                for (ElfSectionHeader.SHType c : ElfSectionHeader.SHType.values())
                    System.out.println(c);
            :::

            [Returns:]{.returnLabel}
            :   an array containing the constants of this enum type, in
                the order they are declared

        []{#valueOf(java.lang.String)}

        -   #### valueOf

            ``` methodSignature
            public static ElfSectionHeader.SHType valueOf​(String name)
            ```

            ::: block
            Returns the enum constant of this type with the specified
            name. The string must match *exactly* an identifier used to
            declare an enum constant in this type. (Extraneous
            whitespace characters are not permitted.)
            :::

            [Parameters:]{.paramLabel}
            :   `name` - the name of the enum constant to be returned.

            [Returns:]{.returnLabel}
            :   the enum constant with the specified name

            [Throws:]{.throwsLabel}
            :   `IllegalArgumentException` - if this enum type has no
                constant with the specified name
            :   `NullPointerException` - if the argument is null

        []{#getValue()}

        -   #### getValue

            ``` methodSignature
            public int getValue()
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
-   Nested \| 
-   [Enum Constants](#enum.constant.summary) \| 
-   Field \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Enum Constants](#enum.constant.detail) \| 
-   Field \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
