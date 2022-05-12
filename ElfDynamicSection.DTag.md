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

## Enum ElfDynamicSection.DTag {#enum-elfdynamicsection.dtag .title title="Enum ElfDynamicSection.DTag"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [java.lang.Enum](http://docs.oracle.com/javase/7/docs/api/java/lang/Enum.html?is-external=true "class or interface in java.lang"){.externalLink}\<[ElfDynamicSection.DTag](ElfDynamicSection.DTag.html "enum in com.facebook.buck.cxx.toolchain.elf")\>

    -   -   com.facebook.buck.cxx.toolchain.elf.ElfDynamicSection.DTag

::: description
-   

    All Implemented Interfaces:
    :   `Serializable`, `Comparable<ElfDynamicSection.DTag>`

    ```{=html}
    <!-- -->
    ```

    Enclosing class:
    :   [ElfDynamicSection](ElfDynamicSection.html "class in com.facebook.buck.cxx.toolchain.elf")

    ------------------------------------------------------------------------

        public static enum ElfDynamicSection.DTag
        extends Enum<ElfDynamicSection.DTag>
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type   Class                           Description
          ------------------- ------------------------------- -------------
          `static class `     `ElfDynamicSection.DTag.Type`    

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#enum.constant.summary}

        ### Enum Constant Summary

          Enum Constant          Description
          ---------------------- -------------
          `DT_BIND_NOW`           
          `DT_DEBUG`              
          `DT_FINI`               
          `DT_FINI_ARRAY`         
          `DT_FINI_ARRAYSZ`       
          `DT_FLAGS`              
          `DT_FLAGS_1`            
          `DT_GNU_HASH`           
          `DT_HASH`               
          `DT_INIT`               
          `DT_INIT_ARRAY`         
          `DT_INIT_ARRAYSZ`       
          `DT_JMPREL`             
          `DT_NEEDED`             
          `DT_NULL`               
          `DT_PLTGOT`             
          `DT_PLTREL`             
          `DT_PLTRELSZ`           
          `DT_PREINIT_ARRAY`      
          `DT_PREINIT_ARRAYSZ`    
          `DT_REL`                
          `DT_RELA`               
          `DT_RELACOUNT`          
          `DT_RELAENT`            
          `DT_RELASZ`             
          `DT_RELCOUNT`           
          `DT_RELENT`             
          `DT_RELSZ`              
          `DT_RPATH`              
          `DT_RUNPATH`            
          `DT_SONAME`             
          `DT_STRSZ`              
          `DT_STRTAB`             
          `DT_SYMBOLIC`           
          `DT_SYMENT`             
          `DT_SYMTAB`             
          `DT_TEXTREL`            
          `DT_TLSDESC_GOT`        
          `DT_TLSDESC_PLT`        
          `DT_VERDEF`             
          `DT_VERDEFNUM`          
          `DT_VERNEED`            
          `DT_VERNEEDNUM`         
          `DT_VERSYM`             

          : Enum Constants[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `ElfDyna              | `getType()`           |                       |
        | micSection.DTag.Type` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `getValue()`          |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static El            | `valueOf​(int val)`    | ::: block             |
        | fDynamicSection.DTag` |                       | Returns the enum      |
        |                       |                       | constant of this type |
        |                       |                       | with the specified    |
        |                       |                       | name.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static El            | `                     | ::: block             |
        | fDynamicSection.DTag` | valueOf​(String name)` | Returns the enum      |
        |                       |                       | constant of this type |
        |                       |                       | with the specified    |
        |                       |                       | name.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static ElfD          | `values()`            | ::: block             |
        | ynamicSection.DTag[]` |                       | Returns an array      |
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

        []{#DT_NULL}

        -   #### DT_NULL

                public static final ElfDynamicSection.DTag DT_NULL

        []{#DT_NEEDED}

        -   #### DT_NEEDED

                public static final ElfDynamicSection.DTag DT_NEEDED

        []{#DT_PLTRELSZ}

        -   #### DT_PLTRELSZ

                public static final ElfDynamicSection.DTag DT_PLTRELSZ

        []{#DT_PLTGOT}

        -   #### DT_PLTGOT

                public static final ElfDynamicSection.DTag DT_PLTGOT

        []{#DT_HASH}

        -   #### DT_HASH

                public static final ElfDynamicSection.DTag DT_HASH

        []{#DT_STRTAB}

        -   #### DT_STRTAB

                public static final ElfDynamicSection.DTag DT_STRTAB

        []{#DT_SYMTAB}

        -   #### DT_SYMTAB

                public static final ElfDynamicSection.DTag DT_SYMTAB

        []{#DT_RELA}

        -   #### DT_RELA

                public static final ElfDynamicSection.DTag DT_RELA

        []{#DT_RELASZ}

        -   #### DT_RELASZ

                public static final ElfDynamicSection.DTag DT_RELASZ

        []{#DT_RELAENT}

        -   #### DT_RELAENT

                public static final ElfDynamicSection.DTag DT_RELAENT

        []{#DT_STRSZ}

        -   #### DT_STRSZ

                public static final ElfDynamicSection.DTag DT_STRSZ

        []{#DT_SYMENT}

        -   #### DT_SYMENT

                public static final ElfDynamicSection.DTag DT_SYMENT

        []{#DT_INIT}

        -   #### DT_INIT

                public static final ElfDynamicSection.DTag DT_INIT

        []{#DT_FINI}

        -   #### DT_FINI

                public static final ElfDynamicSection.DTag DT_FINI

        []{#DT_SONAME}

        -   #### DT_SONAME

                public static final ElfDynamicSection.DTag DT_SONAME

        []{#DT_RPATH}

        -   #### DT_RPATH

                public static final ElfDynamicSection.DTag DT_RPATH

        []{#DT_SYMBOLIC}

        -   #### DT_SYMBOLIC

                public static final ElfDynamicSection.DTag DT_SYMBOLIC

        []{#DT_REL}

        -   #### DT_REL

                public static final ElfDynamicSection.DTag DT_REL

        []{#DT_RELSZ}

        -   #### DT_RELSZ

                public static final ElfDynamicSection.DTag DT_RELSZ

        []{#DT_RELENT}

        -   #### DT_RELENT

                public static final ElfDynamicSection.DTag DT_RELENT

        []{#DT_PLTREL}

        -   #### DT_PLTREL

                public static final ElfDynamicSection.DTag DT_PLTREL

        []{#DT_DEBUG}

        -   #### DT_DEBUG

                public static final ElfDynamicSection.DTag DT_DEBUG

        []{#DT_TEXTREL}

        -   #### DT_TEXTREL

                public static final ElfDynamicSection.DTag DT_TEXTREL

        []{#DT_JMPREL}

        -   #### DT_JMPREL

                public static final ElfDynamicSection.DTag DT_JMPREL

        []{#DT_BIND_NOW}

        -   #### DT_BIND_NOW

                public static final ElfDynamicSection.DTag DT_BIND_NOW

        []{#DT_INIT_ARRAY}

        -   #### DT_INIT_ARRAY

                public static final ElfDynamicSection.DTag DT_INIT_ARRAY

        []{#DT_FINI_ARRAY}

        -   #### DT_FINI_ARRAY

                public static final ElfDynamicSection.DTag DT_FINI_ARRAY

        []{#DT_INIT_ARRAYSZ}

        -   #### DT_INIT_ARRAYSZ

                public static final ElfDynamicSection.DTag DT_INIT_ARRAYSZ

        []{#DT_FINI_ARRAYSZ}

        -   #### DT_FINI_ARRAYSZ

                public static final ElfDynamicSection.DTag DT_FINI_ARRAYSZ

        []{#DT_RUNPATH}

        -   #### DT_RUNPATH

                public static final ElfDynamicSection.DTag DT_RUNPATH

        []{#DT_FLAGS}

        -   #### DT_FLAGS

                public static final ElfDynamicSection.DTag DT_FLAGS

        []{#DT_PREINIT_ARRAY}

        -   #### DT_PREINIT_ARRAY

                public static final ElfDynamicSection.DTag DT_PREINIT_ARRAY

        []{#DT_PREINIT_ARRAYSZ}

        -   #### DT_PREINIT_ARRAYSZ

                public static final ElfDynamicSection.DTag DT_PREINIT_ARRAYSZ

        []{#DT_GNU_HASH}

        -   #### DT_GNU_HASH

                public static final ElfDynamicSection.DTag DT_GNU_HASH

        []{#DT_TLSDESC_PLT}

        -   #### DT_TLSDESC_PLT

                public static final ElfDynamicSection.DTag DT_TLSDESC_PLT

        []{#DT_TLSDESC_GOT}

        -   #### DT_TLSDESC_GOT

                public static final ElfDynamicSection.DTag DT_TLSDESC_GOT

        []{#DT_VERSYM}

        -   #### DT_VERSYM

                public static final ElfDynamicSection.DTag DT_VERSYM

        []{#DT_RELACOUNT}

        -   #### DT_RELACOUNT

                public static final ElfDynamicSection.DTag DT_RELACOUNT

        []{#DT_RELCOUNT}

        -   #### DT_RELCOUNT

                public static final ElfDynamicSection.DTag DT_RELCOUNT

        []{#DT_FLAGS_1}

        -   #### DT_FLAGS_1

                public static final ElfDynamicSection.DTag DT_FLAGS_1

        []{#DT_VERDEF}

        -   #### DT_VERDEF

                public static final ElfDynamicSection.DTag DT_VERDEF

        []{#DT_VERDEFNUM}

        -   #### DT_VERDEFNUM

                public static final ElfDynamicSection.DTag DT_VERDEFNUM

        []{#DT_VERNEED}

        -   #### DT_VERNEED

                public static final ElfDynamicSection.DTag DT_VERNEED

        []{#DT_VERNEEDNUM}

        -   #### DT_VERNEEDNUM

                public static final ElfDynamicSection.DTag DT_VERNEEDNUM
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#values()}

        -   #### values

            ``` methodSignature
            public static ElfDynamicSection.DTag[] values()
            ```

            ::: block
            Returns an array containing the constants of this enum type,
            in the order they are declared. This method may be used to
            iterate over the constants as follows:
                for (ElfDynamicSection.DTag c : ElfDynamicSection.DTag.values())
                    System.out.println(c);
            :::

            [Returns:]{.returnLabel}
            :   an array containing the constants of this enum type, in
                the order they are declared

        []{#valueOf(java.lang.String)}

        -   #### valueOf

            ``` methodSignature
            public static ElfDynamicSection.DTag valueOf​(String name)
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

        []{#valueOf(int)}

        -   #### valueOf

            ``` methodSignature
            public static ElfDynamicSection.DTag valueOf​(int val)
            ```

            ::: block
            Returns the enum constant of this type with the specified
            name. The string must match *exactly* an identifier used to
            declare an enum constant in this type. (Extraneous
            whitespace characters are not permitted.)
            :::

            [Parameters:]{.paramLabel}
            :   `val` - the name of the enum constant to be returned.

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

        []{#getType()}

        -   #### getType

            ``` methodSignature
            public ElfDynamicSection.DTag.Type getType()
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
