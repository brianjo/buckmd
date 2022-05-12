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
[Package]{.packageLabelInType} [com.facebook.buck.cxx.toolchain.objectfile](package-summary.html)
:::

## Class Machos {#class-machos .title title="Class Machos"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.cxx.toolchain.objectfile.Machos

::: description
-   

    ------------------------------------------------------------------------

        public class Machos
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type   Class                     Description
          ------------------- ------------------------- -------------
          `static class `     `Machos.MachoException`    

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type   Field                 Description
          ------------------- --------------------- -------------
          `static int`        `LC_DYLD_INFO_ONLY`    
          `static int`        `LC_SYMTAB`            

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `stati                | `gener                | ::: block             |
        | c Map<byte[],​byte[]>` | ateReplacementMap​(Map | Prepares a            |
        |                       | <Path,​Path> pathMap)` | replacement map for   |
        |                       |                       | prefixes.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `protected            | `getHeader​(M          | ::: block             |
        |  static com.facebook. | appedByteBuffer map)` | Returns the Mach-O    |
        | buck.cxx.toolchain.ob |                       | header provided the   |
        | jectfile.MachoHeader` |                       | file is Mach-O,       |
        |                       |                       | otherwise throws an   |
        |                       |                       | exception.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static               | `tryRewritingMatching | ::: block             |
        | Optional<ByteBuffer>` | Path​(byte[] stringByt | Checks whether a      |
        |                       | es,                   | string matches a      |
        |                       |        int stringOffs | prefix and returns a  |
        |                       | et,                   | rewritten copy if     |
        |                       |        Map<byte[],​byt | that\'s the case.     |
        |                       | e[]> replacementMap)` | :::                   |
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
    -   []{#field.detail}

        ### Field Detail

        []{#LC_SYMTAB}

        -   #### LC_SYMTAB

                public static final int LC_SYMTAB

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../constant-values.html#com.facebook.buck.cxx.toolchain.objectfile.Machos.LC_SYMTAB)

        []{#LC_DYLD_INFO_ONLY}

        -   #### LC_DYLD_INFO_ONLY

                public static final int LC_DYLD_INFO_ONLY

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../constant-values.html#com.facebook.buck.cxx.toolchain.objectfile.Machos.LC_DYLD_INFO_ONLY)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getHeader(java.nio.MappedByteBuffer)}

        -   #### getHeader

            ``` methodSignature
            protected static com.facebook.buck.cxx.toolchain.objectfile.MachoHeader getHeader​(MappedByteBuffer map)
                                                                                       throws Machos.MachoException
            ```

            ::: block
            Returns the Mach-O header provided the file is Mach-O,
            otherwise throws an exception.
            :::

            [Throws:]{.throwsLabel}
            :   `Machos.MachoException`

        []{#generateReplacementMap(java.util.Map)}

        -   #### generateReplacementMap

            ``` methodSignature
            public static Map<byte[],​byte[]> generateReplacementMap​(Map<Path,​Path> pathMap)
            ```

            ::: block
            Prepares a replacement map for prefixes. For example, if had
            two entries: 1. \"/path/to/repo\" -\> \"\", 2.
            \"/path/to/repo/cell\" -\> \"cell\"
            The resulting map would contain: 1. \"/path/to/repo/\" -\>
            \"./\" 2. \"/path/to/repo/cell/\" -\> \"cell/\"

            The above means we can do very simple (and fast!) search &
            replace.
            :::

        []{#tryRewritingMatchingPath(byte[],int,java.util.Map)}

        -   #### tryRewritingMatchingPath

            ``` methodSignature
            public static Optional<ByteBuffer> tryRewritingMatchingPath​(byte[] stringBytes,
                                                                        int stringOffset,
                                                                        Map<byte[],​byte[]> replacementMap)
            ```

            ::: block
            Checks whether a string matches a prefix and returns a
            rewritten copy if that\'s the case. For example, given a
            string \"/Users/fb/repo/cell\" and a replacement map
            containing \"/Users/fb/repo/\" -\> \"./\", it will return a
            ByteBuffer wrapping \"./cell\".
            NB: This is a perf sensitive method.
            :::
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
