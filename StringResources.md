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

-   [Overview](../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../deprecated-list.html)
-   [Index](../../../../index-all.html)
-   [Help](../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.android](package-summary.html)
:::

## Class StringResources {#class-stringresources .title title="Class StringResources"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.android.StringResources

::: description
-   

    ------------------------------------------------------------------------

        public class StringResources
        extends Object

    ::: block
    Represents string resources of types string, plural and array for a
    locale. Also responsible for generating a custom format binary file
    for the resources.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type                                                                                                                      Field       Description
          -------------------------------------------------------------------------------------------------------------------------------------- ----------- -------------
          `SortedMap<Integer,​EnumMap<com.facebook.buck.android.StringResources.Gender,​com.google.common.collect.ImmutableList<String>>>`         `arrays`     
          `SortedMap<Integer,​EnumMap<com.facebook.buck.android.StringResources.Gender,​com.google.common.collect.ImmutableMap<String,​String>>>`   `plurals`    
          `SortedMap<Integer,​EnumMap<com.facebook.buck.android.StringResources.Gender,​String>>`                                                  `strings`    

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                                                                                                                                                                     Description
          ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `StringResources​(SortedMap<Integer,​EnumMap<com.facebook.buck.android.StringResources.Gender,​String>> strings,                SortedMap<Integer,​EnumMap<com.facebook.buck.android.StringResources.Gender,​com.google.common.collect.ImmutableMap<String,​String>>> plurals,                SortedMap<Integer,​EnumMap<com.facebook.buck.android.StringResources.Gender,​com.google.common.collect.ImmutableList<String>>> arrays)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `byte[]`              | `ge                   | ::: block             |
        |                       | tBinaryFileContent()` | Returns a byte array  |
        |                       |                       | that represents the   |
        |                       |                       | entire set of         |
        |                       |                       | strings, plurals and  |
        |                       |                       | string arrays in the  |
        |                       |                       | following binary file |
        |                       |                       | format:               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `StringResources`     | `getMerged            |                       |
        |                       | Resources​(StringResou |                       |
        |                       | rces otherResources)` |                       |
        +-----------------------+-----------------------+-----------------------+

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

        []{#strings}

        -   #### strings

                public final SortedMap<Integer,​EnumMap<com.facebook.buck.android.StringResources.Gender,​String>> strings

        []{#plurals}

        -   #### plurals

                public final SortedMap<Integer,​EnumMap<com.facebook.buck.android.StringResources.Gender,​com.google.common.collect.ImmutableMap<String,​String>>> plurals

        []{#arrays}

        -   #### arrays

                public final SortedMap<Integer,​EnumMap<com.facebook.buck.android.StringResources.Gender,​com.google.common.collect.ImmutableList<String>>> arrays
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(java.util.SortedMap,java.util.SortedMap,java.util.SortedMap)}

        -   #### StringResources

                public StringResources​(SortedMap<Integer,​EnumMap<com.facebook.buck.android.StringResources.Gender,​String>> strings,
                                       SortedMap<Integer,​EnumMap<com.facebook.buck.android.StringResources.Gender,​com.google.common.collect.ImmutableMap<String,​String>>> plurals,
                                       SortedMap<Integer,​EnumMap<com.facebook.buck.android.StringResources.Gender,​com.google.common.collect.ImmutableList<String>>> arrays)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getMergedResources(com.facebook.buck.android.StringResources)}

        -   #### getMergedResources

            ``` methodSignature
            public StringResources getMergedResources​(StringResources otherResources)
            ```

        []{#getBinaryFileContent()}

        -   #### getBinaryFileContent

            ``` methodSignature
            public byte[] getBinaryFileContent()
            ```

            ::: block
            Returns a byte array that represents the entire set of
            strings, plurals and string arrays in the following binary
            file format:
                   [Int: Version]

                   [Int: # of strings]
                   [Int: Smallest resource id among strings]
                   [[Short: resource id delta] [Byte: #genders] [[Byte: gender enum ordinal] [Short: length of
                    the string]] x #genders] x # of strings
                   [Byte array of the string value] x # summation of genders over # of strings

                   [Int: # of plurals]
                   [Int: Smallest resource id among plurals]
                   [[Short: resource id delta] [Byte: #genders] [[Byte: gender enum ordinal] [Byte: #categories]
                    [[Byte: category] [Short: length of plural value]] x #categories] x # of genders]
                    x # of plurals
                   [Byte array of plural value] x Summation of genders over plural categories over # of plurals

                   [Int: # of arrays]
                   [Int: Smallest resource id among arrays]
                   [[Short: resource id delta] [Byte: #genders] [[Byte: gender enum ordinal] [Int: #elements]
                    [Short: length of element] x # phaof elements] x # of genders] x # of arrays
                   [Byte array of string value] x Summation of genders over array elements over # of arrays
                 
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

-   [Overview](../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../deprecated-list.html)
-   [Index](../../../../index-all.html)
-   [Help](../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../allclasses.html)

<div>

<div>

JavaScript is disabled on your browser.

</div>

</div>

<div>

-   Summary: 
-   Nested \| 
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
