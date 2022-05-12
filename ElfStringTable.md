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
-   Field \| 
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
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

## Class ElfStringTable {#class-elfstringtable .title title="Class ElfStringTable"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.cxx.toolchain.elf.ElfStringTable

::: description
-   

    ------------------------------------------------------------------------

        public class ElfStringTable
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static com.goo       | `writeStringTableFr   | ::: block             |
        | gle.common.collect.Im | omStrings​(Iterable<St | Writes a string table |
        | mutableList<Integer>` | ring> strings,        | from the given        |
        |                       |                       | strings.              |
        |                       | OutputStream output)` | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static com.goo       | `writeStr             | ::: block             |
        | gle.common.collect.Im | ingTableFromStringTab | Writes a string table |
        | mutableList<Integer>` | le​(byte[] data,       | from null terminated  |
        |                       |                       | byte strings          |
        |                       |      Iterable<Integer | described by the byte |
        |                       | > indices,            | array and indices.    |
        |                       |                       | :::                   |
        |                       | OutputStream output)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#writeStringTableFromStringTable(byte[],java.lang.Iterable,java.io.OutputStream)}

        -   #### writeStringTableFromStringTable

            ``` methodSignature
            public static com.google.common.collect.ImmutableList<Integer> writeStringTableFromStringTable​(byte[] data,
                                                                                                           Iterable<Integer> indices,
                                                                                                           OutputStream output)
                                                                                                    throws IOException
            ```

            ::: block
            Writes a string table from null terminated byte strings
            described by the byte array and indices.
            :::

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#writeStringTableFromStrings(java.lang.Iterable,java.io.OutputStream)}

        -   #### writeStringTableFromStrings

            ``` methodSignature
            public static com.google.common.collect.ImmutableList<Integer> writeStringTableFromStrings​(Iterable<String> strings,
                                                                                                       OutputStream output)
                                                                                                throws IOException
            ```

            ::: block
            Writes a string table from the given strings.
            :::

            [Returns:]{.returnLabel}
            :   a list of offsets into the written string table for the
                input strings (where each offset positionally
                corresponds to a string in the input strings iterable).

            [Throws:]{.throwsLabel}
            :   `IOException`
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
-   Field \| 
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   Constr \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
