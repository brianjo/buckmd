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

## Class Elf {#class-elf .title title="Class Elf"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.cxx.toolchain.elf.Elf

::: description
-   

    ------------------------------------------------------------------------

        public class Elf
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static class `       | `Elf.Elf32`           |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static class `       | `Elf.Elf64`           |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static interface `   | `Elf.El               | ::: block             |
        |                       | fSectionLookupResult` | A tuple of section    |
        |                       |                       | index and             |
        |                       |                       | [`ElfSection`](       |
        |                       |                       | ElfSection.html "clas |
        |                       |                       | s in com.facebook.buc |
        |                       |                       | k.cxx.toolchain.elf") |
        |                       |                       | object returned from  |
        |                       |                       | lookup functions in   |
        |                       |                       | this class.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type   Field      Description
          ------------------- ---------- -------------
          `ElfHeader`         `header`    

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                Description
          -------------------------- -------------
          `Elf​(ByteBuffer buffer)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                        Method                                                                                      Description
          ---------------------------------------- ------------------------------------------------------------------------------------------- -------------
          `Elf.ElfSectionLookupResult`             `getMandatorySectionByName​(Object fileName,                          String sectionName)`    
          `int`                                    `getNumberOfSections()`                                                                      
          `ElfSection`                             `getSectionByIndex​(int index)`                                                               
          `Optional<Elf.ElfSectionLookupResult>`   `getSectionByName​(String name)`                                                              
          `String`                                 `getSectionName​(ElfSectionHeader sectionHeader)`                                             
          `static boolean`                         `isElf​(ByteBuffer buffer)`                                                                   

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

        []{#header}

        -   #### header

                public final ElfHeader header
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(java.nio.ByteBuffer)}

        -   #### Elf

                public Elf​(ByteBuffer buffer)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getNumberOfSections()}

        -   #### getNumberOfSections

            ``` methodSignature
            public int getNumberOfSections()
            ```

        []{#getSectionByIndex(int)}

        -   #### getSectionByIndex

            ``` methodSignature
            public ElfSection getSectionByIndex​(int index)
            ```

            [Returns:]{.returnLabel}
            :   the parsed section header for the section at the given
                index.

        []{#getSectionName(com.facebook.buck.cxx.toolchain.elf.ElfSectionHeader)}

        -   #### getSectionName

            ``` methodSignature
            public String getSectionName​(ElfSectionHeader sectionHeader)
            ```

            [Returns:]{.returnLabel}
            :   the name of the section found in the section header
                string table.

        []{#getSectionByName(java.lang.String)}

        -   #### getSectionByName

            ``` methodSignature
            public Optional<Elf.ElfSectionLookupResult> getSectionByName​(String name)
            ```

            [Returns:]{.returnLabel}
            :   the parsed section header for the section of the given
                name.

        []{#getMandatorySectionByName(java.lang.Object,java.lang.String)}

        -   #### getMandatorySectionByName

            ``` methodSignature
            public Elf.ElfSectionLookupResult getMandatorySectionByName​(Object fileName,
                                                                        String sectionName)
                                                                 throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#isElf(java.nio.ByteBuffer)}

        -   #### isElf

            ``` methodSignature
            public static boolean isElf​(ByteBuffer buffer)
            ```

            [Returns:]{.returnLabel}
            :   whether the data this buffer points to is most likely
                ELF.
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
