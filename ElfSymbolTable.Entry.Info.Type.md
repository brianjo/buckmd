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

## Enum ElfSymbolTable.Entry.Info.Type {#enum-elfsymboltable.entry.info.type .title title="Enum ElfSymbolTable.Entry.Info.Type"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [java.lang.Enum](http://docs.oracle.com/javase/7/docs/api/java/lang/Enum.html?is-external=true "class or interface in java.lang"){.externalLink}\<[ElfSymbolTable.Entry.Info.Type](ElfSymbolTable.Entry.Info.Type.html "enum in com.facebook.buck.cxx.toolchain.elf")\>

    -   -   com.facebook.buck.cxx.toolchain.elf.ElfSymbolTable.Entry.Info.Type

::: description
-   

    All Implemented Interfaces:
    :   `Serializable`, `Comparable<ElfSymbolTable.Entry.Info.Type>`

    ```{=html}
    <!-- -->
    ```

    Enclosing class:
    :   [ElfSymbolTable.Entry.Info](ElfSymbolTable.Entry.Info.html "class in com.facebook.buck.cxx.toolchain.elf")

    ------------------------------------------------------------------------

        public static enum ElfSymbolTable.Entry.Info.Type
        extends Enum<ElfSymbolTable.Entry.Info.Type>
:::

::: summary
-   ::: {.section role="region"}
    -   []{#enum.constant.summary}

        ### Enum Constant Summary

          Enum Constant   Description
          --------------- -------------
          `STT_COMMON`     
          `STT_FILE`       
          `STT_FUNC`       
          `STT_NOTYPE`     
          `STT_OBJECT`     
          `STT_SECTION`    
          `STT_TLS`        

          : Enum Constants[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static ElfSymbolT    | `ofIntValue​(int val)` |                       |
        | able.Entry.Info.Type` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static ElfSymbolT    | `                     | ::: block             |
        | able.Entry.Info.Type` | valueOf​(String name)` | Returns the enum      |
        |                       |                       | constant of this type |
        |                       |                       | with the specified    |
        |                       |                       | name.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static ElfSymbolTab  | `values()`            | ::: block             |
        | le.Entry.Info.Type[]` |                       | Returns an array      |
        |                       |                       | containing the        |
        |                       |                       | constants of this     |
        |                       |                       | enum type, in the     |
        |                       |                       | order they are        |
        |                       |                       | declared.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
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

        []{#STT_NOTYPE}

        -   #### STT_NOTYPE

                public static final ElfSymbolTable.Entry.Info.Type STT_NOTYPE

        []{#STT_OBJECT}

        -   #### STT_OBJECT

                public static final ElfSymbolTable.Entry.Info.Type STT_OBJECT

        []{#STT_FUNC}

        -   #### STT_FUNC

                public static final ElfSymbolTable.Entry.Info.Type STT_FUNC

        []{#STT_SECTION}

        -   #### STT_SECTION

                public static final ElfSymbolTable.Entry.Info.Type STT_SECTION

        []{#STT_FILE}

        -   #### STT_FILE

                public static final ElfSymbolTable.Entry.Info.Type STT_FILE

        []{#STT_COMMON}

        -   #### STT_COMMON

                public static final ElfSymbolTable.Entry.Info.Type STT_COMMON

        []{#STT_TLS}

        -   #### STT_TLS

                public static final ElfSymbolTable.Entry.Info.Type STT_TLS
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#values()}

        -   #### values

            ``` methodSignature
            public static ElfSymbolTable.Entry.Info.Type[] values()
            ```

            ::: block
            Returns an array containing the constants of this enum type,
            in the order they are declared. This method may be used to
            iterate over the constants as follows:
                for (ElfSymbolTable.Entry.Info.Type c : ElfSymbolTable.Entry.Info.Type.values())
                    System.out.println(c);
            :::

            [Returns:]{.returnLabel}
            :   an array containing the constants of this enum type, in
                the order they are declared

        []{#valueOf(java.lang.String)}

        -   #### valueOf

            ``` methodSignature
            public static ElfSymbolTable.Entry.Info.Type valueOf​(String name)
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

        []{#ofIntValue(int)}

        -   #### ofIntValue

            ``` methodSignature
            public static ElfSymbolTable.Entry.Info.Type ofIntValue​(int val)
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
