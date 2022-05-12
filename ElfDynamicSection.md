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

## Class ElfDynamicSection {#class-elfdynamicsection .title title="Class ElfDynamicSection"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.cxx.toolchain.elf.ElfDynamicSection

::: description
-   

    ------------------------------------------------------------------------

        public class ElfDynamicSection
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type   Class                       Description
          ------------------- --------------------------- -------------
          `static class `     `ElfDynamicSection.DTag`     
          `static class `     `ElfDynamicSection.Entry`    

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type                                                    Field       Description
          -------------------------------------------------------------------- ----------- -------------
          `com.google.common.collect.ImmutableList<ElfDynamicSection.Entry>`   `entries`    

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                     Description
          ----------------------------------------------------------------------------------------------- -------------
          `ElfDynamicSection​(com.google.common.collect.ImmutableList<ElfDynamicSection.Entry> entries)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type            Method                                                       Description
          ---------------------------- ------------------------------------------------------------ -------------
          `Optional<Long>`             `lookup​(ElfDynamicSection.DTag dTag)`                         
          `static ElfDynamicSection`   `parse​(ElfHeader.EIClass eiClass,      ByteBuffer buffer)`    
          `void`                       `write​(ElfHeader.EIClass eiClass,      ByteBuffer buffer)`    

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

        []{#entries}

        -   #### entries

                public final com.google.common.collect.ImmutableList<ElfDynamicSection.Entry> entries
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.google.common.collect.ImmutableList)}

        -   #### ElfDynamicSection

                public ElfDynamicSection​(com.google.common.collect.ImmutableList<ElfDynamicSection.Entry> entries)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#parse(com.facebook.buck.cxx.toolchain.elf.ElfHeader.EIClass,java.nio.ByteBuffer)}

        -   #### parse

            ``` methodSignature
            public static ElfDynamicSection parse​(ElfHeader.EIClass eiClass,
                                                  ByteBuffer buffer)
            ```

        []{#write(com.facebook.buck.cxx.toolchain.elf.ElfHeader.EIClass,java.nio.ByteBuffer)}

        -   #### write

            ``` methodSignature
            public void write​(ElfHeader.EIClass eiClass,
                              ByteBuffer buffer)
            ```

        []{#lookup(com.facebook.buck.cxx.toolchain.elf.ElfDynamicSection.DTag)}

        -   #### lookup

            ``` methodSignature
            public Optional<Long> lookup​(ElfDynamicSection.DTag dTag)
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
