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

-   [Overview](../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../deprecated-list.html)
-   [Index](../../../../../index-all.html)
-   [Help](../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.android.aapt](package-summary.html)
:::

## Class RDotTxtEntry {#class-rdottxtentry .title title="Class RDotTxtEntry"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.android.aapt.RDotTxtEntry

::: description
-   

    All Implemented Interfaces:
    :   `Comparable<RDotTxtEntry>`

    ```{=html}
    <!-- -->
    ```

    Direct Known Subclasses:
    :   `FakeRDotTxtEntry`

    ------------------------------------------------------------------------

        public class RDotTxtEntry
        extends Object
        implements Comparable<RDotTxtEntry>

    ::: block
    Represents a row from a symbols file generated by `aapt`.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type   Class                               Description
          ------------------- ----------------------------------- -------------
          `static class `     `RDotTxtEntry.CustomDrawableType`    
          `static class `     `RDotTxtEntry.IdType`                
          `static class `     `RDotTxtEntry.RType`                 

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type                                           Field                   Description
          ----------------------------------------------------------- ----------------------- -------------
          `RDotTxtEntry.CustomDrawableType`                           `customType`             
          `RDotTxtEntry.IdType`                                       `idType`                 
          `String`                                                    `idValue`                
          `static String`                                             `INT_ARRAY_SEPARATOR`    
          `String`                                                    `name`                   
          `String`                                                    `parent`                 
          `static java.util.function.Function<String,​RDotTxtEntry>`   `TO_ENTRY`               
          `RDotTxtEntry.RType`                                        `type`                   

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                               Description
          ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `RDotTxtEntry​(RDotTxtEntry.IdType idType,             RDotTxtEntry.RType type,             String name,             String idValue)`                                                                                       
          `RDotTxtEntry​(RDotTxtEntry.IdType idType,             RDotTxtEntry.RType type,             String name,             String idValue,             RDotTxtEntry.CustomDrawableType customType)`                               
          `RDotTxtEntry​(RDotTxtEntry.IdType idType,             RDotTxtEntry.RType type,             String name,             String idValue,             RDotTxtEntry.CustomDrawableType customType,             String parent)`    
          `RDotTxtEntry​(RDotTxtEntry.IdType idType,             RDotTxtEntry.RType type,             String name,             String idValue,             String parent)`                                                            

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `int`                 | `compareT             | ::: block             |
        |                       | o​(RDotTxtEntry that)` | A collection of       |
        |                       |                       | Resources should be   |
        |                       |                       | sorted such that      |
        |                       |                       | Resources of the same |
        |                       |                       | type should be        |
        |                       |                       | grouped together, and |
        |                       |                       | should be             |
        |                       |                       | alphabetized within   |
        |                       |                       | that group.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RDotTxtEntry`        | `copyWithNewIdValu    |                       |
        |                       | e​(String newIdValue)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `RDotTxtEntry`        | `copyWithNewP         |                       |
        |                       | arent​(String parent)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `equals​(Object obj)`  |                       |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `hashCode()`          |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static Op            | `parse                |                       |
        | tional<RDotTxtEntry>` | ​(String rDotTxtLine)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `stati                | `readResources​(       | ::: block             |
        | c List<RDotTxtEntry>` | ProjectFilesystem own | Read resource IDs     |
        |                       | ingFilesystem,        | from a R.txt file and |
        |                       |        Path rDotTxt)` | add them to a list of |
        |                       |                       | entries               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `toString()`          |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, finalize, getClass, notify, notifyAll, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#field.detail}

        ### Field Detail

        []{#TO_ENTRY}

        -   #### TO_ENTRY

                public static final java.util.function.Function<String,​RDotTxtEntry> TO_ENTRY

        []{#INT_ARRAY_SEPARATOR}

        -   #### INT_ARRAY_SEPARATOR

                public static final String INT_ARRAY_SEPARATOR

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.android.aapt.RDotTxtEntry.INT_ARRAY_SEPARATOR)

        []{#idType}

        -   #### idType

                public final RDotTxtEntry.IdType idType

        []{#type}

        -   #### type

                public final RDotTxtEntry.RType type

        []{#name}

        -   #### name

                public final String name

        []{#idValue}

        -   #### idValue

                public final String idValue

        []{#parent}

        -   #### parent

                public final String parent

        []{#customType}

        -   #### customType

                public final RDotTxtEntry.CustomDrawableType customType
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.android.aapt.RDotTxtEntry.IdType,com.facebook.buck.android.aapt.RDotTxtEntry.RType,java.lang.String,java.lang.String)}

        -   #### RDotTxtEntry

                public RDotTxtEntry​(RDotTxtEntry.IdType idType,
                                    RDotTxtEntry.RType type,
                                    String name,
                                    String idValue)

        []{#<init>(com.facebook.buck.android.aapt.RDotTxtEntry.IdType,com.facebook.buck.android.aapt.RDotTxtEntry.RType,java.lang.String,java.lang.String,java.lang.String)}

        -   #### RDotTxtEntry

                public RDotTxtEntry​(RDotTxtEntry.IdType idType,
                                    RDotTxtEntry.RType type,
                                    String name,
                                    String idValue,
                                    @Nullable
                                    String parent)

        []{#<init>(com.facebook.buck.android.aapt.RDotTxtEntry.IdType,com.facebook.buck.android.aapt.RDotTxtEntry.RType,java.lang.String,java.lang.String,com.facebook.buck.android.aapt.RDotTxtEntry.CustomDrawableType)}

        -   #### RDotTxtEntry

                public RDotTxtEntry​(RDotTxtEntry.IdType idType,
                                    RDotTxtEntry.RType type,
                                    String name,
                                    String idValue,
                                    RDotTxtEntry.CustomDrawableType customType)

        []{#<init>(com.facebook.buck.android.aapt.RDotTxtEntry.IdType,com.facebook.buck.android.aapt.RDotTxtEntry.RType,java.lang.String,java.lang.String,com.facebook.buck.android.aapt.RDotTxtEntry.CustomDrawableType,java.lang.String)}

        -   #### RDotTxtEntry

                public RDotTxtEntry​(RDotTxtEntry.IdType idType,
                                    RDotTxtEntry.RType type,
                                    String name,
                                    String idValue,
                                    RDotTxtEntry.CustomDrawableType customType,
                                    @Nullable
                                    String parent)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#copyWithNewIdValue(java.lang.String)}

        -   #### copyWithNewIdValue

            ``` methodSignature
            public RDotTxtEntry copyWithNewIdValue​(String newIdValue)
            ```

        []{#copyWithNewParent(java.lang.String)}

        -   #### copyWithNewParent

            ``` methodSignature
            public RDotTxtEntry copyWithNewParent​(String parent)
            ```

        []{#parse(java.lang.String)}

        -   #### parse

            ``` methodSignature
            public static Optional<RDotTxtEntry> parse​(String rDotTxtLine)
            ```

        []{#readResources(com.facebook.buck.io.filesystem.ProjectFilesystem,java.nio.file.Path)}

        -   #### readResources

            ``` methodSignature
            public static List<RDotTxtEntry> readResources​(ProjectFilesystem owningFilesystem,
                                                           Path rDotTxt)
                                                    throws IOException
            ```

            ::: block
            Read resource IDs from a R.txt file and add them to a list
            of entries
            :::

            [Parameters:]{.paramLabel}
            :   `owningFilesystem` - The project filesystem to use
            :   `rDotTxt` - the path to the R.txt file to read

            [Returns:]{.returnLabel}
            :   a list of RDotTxtEntry objects read from the file

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#compareTo(com.facebook.buck.android.aapt.RDotTxtEntry)}

        -   #### compareTo

            ``` methodSignature
            public int compareTo​(RDotTxtEntry that)
            ```

            ::: block
            A collection of Resources should be sorted such that
            Resources of the same type should be grouped together, and
            should be alphabetized within that group.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `compareTo` in interface `Comparable<RDotTxtEntry>`

        []{#equals(java.lang.Object)}

        -   #### equals

            ``` methodSignature
            public boolean equals​(Object obj)
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `equals` in class `Object`

        []{#hashCode()}

        -   #### hashCode

            ``` methodSignature
            public int hashCode()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `hashCode` in class `Object`

        []{#toString()}

        -   #### toString

            ``` methodSignature
            public String toString()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `toString` in class `Object`
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

-   [Overview](../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../deprecated-list.html)
-   [Index](../../../../../index-all.html)
-   [Help](../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../allclasses.html)

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