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
[Package]{.packageLabelInType} [com.facebook.buck.util.unit](package-summary.html)
:::

## Enum SizeUnit {#enum-sizeunit .title title="Enum SizeUnit"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [java.lang.Enum](http://docs.oracle.com/javase/7/docs/api/java/lang/Enum.html?is-external=true "class or interface in java.lang"){.externalLink}\<[SizeUnit](SizeUnit.html "enum in com.facebook.buck.util.unit")\>

    -   -   com.facebook.buck.util.unit.SizeUnit

::: description
-   

    All Implemented Interfaces:
    :   `Serializable`, `Comparable<SizeUnit>`

    ------------------------------------------------------------------------

        public enum SizeUnit
        extends Enum<SizeUnit>
:::

::: summary
-   ::: {.section role="region"}
    -   []{#enum.constant.summary}

        ### Enum Constant Summary

          Enum Constant   Description
          --------------- -------------
          `BYTES`          
          `GIGABYTES`      
          `KILOBYTES`      
          `MEGABYTES`      
          `TERABYTES`      

          : Enum Constants[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `String`              | `getAbbreviation()`   |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static P             | `getHum               |                       |
        | air<Double,​SizeUnit>` | anReadableSize​(double |                       |
        |                       |  size,                |                       |
        |                       |       SizeUnit unit)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `getOrdinal()`        |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static long`         | `pars                 | ::: block             |
        |                       | eBytes​(String input)` | Parses a string that  |
        |                       |                       | represents a size     |
        |                       |                       | into the number of    |
        |                       |                       | bytes represented by  |
        |                       |                       | that string.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `long`                | `                     |                       |
        |                       | toBytes​(double size)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `long`                | `toGi                 |                       |
        |                       | gabytes​(double size)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static String`       | `to                   |                       |
        |                       | HumanReadableString​(P |                       |
        |                       | air<Double,​SizeUnit>  |                       |
        |                       | size,                 |                       |
        |                       |       Locale locale)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `long`                | `toKi                 |                       |
        |                       | lobytes​(double size)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `long`                | `toMe                 |                       |
        |                       | gabytes​(double size)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `long`                | `toTe                 |                       |
        |                       | rabytes​(double size)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static SizeUnit`     | `                     | ::: block             |
        |                       | valueOf​(String name)` | Returns the enum      |
        |                       |                       | constant of this type |
        |                       |                       | with the specified    |
        |                       |                       | name.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static SizeUnit[]`   | `values()`            | ::: block             |
        |                       |                       | Returns an array      |
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

        []{#BYTES}

        -   #### BYTES

                public static final SizeUnit BYTES

        []{#KILOBYTES}

        -   #### KILOBYTES

                public static final SizeUnit KILOBYTES

        []{#MEGABYTES}

        -   #### MEGABYTES

                public static final SizeUnit MEGABYTES

        []{#GIGABYTES}

        -   #### GIGABYTES

                public static final SizeUnit GIGABYTES

        []{#TERABYTES}

        -   #### TERABYTES

                public static final SizeUnit TERABYTES
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#values()}

        -   #### values

            ``` methodSignature
            public static SizeUnit[] values()
            ```

            ::: block
            Returns an array containing the constants of this enum type,
            in the order they are declared. This method may be used to
            iterate over the constants as follows:
                for (SizeUnit c : SizeUnit.values())
                    System.out.println(c);
            :::

            [Returns:]{.returnLabel}
            :   an array containing the constants of this enum type, in
                the order they are declared

        []{#valueOf(java.lang.String)}

        -   #### valueOf

            ``` methodSignature
            public static SizeUnit valueOf​(String name)
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

        []{#getOrdinal()}

        -   #### getOrdinal

            ``` methodSignature
            public int getOrdinal()
            ```

        []{#getAbbreviation()}

        -   #### getAbbreviation

            ``` methodSignature
            public String getAbbreviation()
            ```

        []{#parseBytes(java.lang.String)}

        -   #### parseBytes

            ``` methodSignature
            public static long parseBytes​(String input)
                                   throws NumberFormatException
            ```

            ::: block
            Parses a string that represents a size into the number of
            bytes represented by that string.
            :::

            [Throws:]{.throwsLabel}
            :   `NumberFormatException`

        []{#toBytes(double)}

        -   #### toBytes

            ``` methodSignature
            public long toBytes​(double size)
            ```

        []{#toKilobytes(double)}

        -   #### toKilobytes

            ``` methodSignature
            public long toKilobytes​(double size)
            ```

        []{#toMegabytes(double)}

        -   #### toMegabytes

            ``` methodSignature
            public long toMegabytes​(double size)
            ```

        []{#toGigabytes(double)}

        -   #### toGigabytes

            ``` methodSignature
            public long toGigabytes​(double size)
            ```

        []{#toTerabytes(double)}

        -   #### toTerabytes

            ``` methodSignature
            public long toTerabytes​(double size)
            ```

        []{#getHumanReadableSize(double,com.facebook.buck.util.unit.SizeUnit)}

        -   #### getHumanReadableSize

            ``` methodSignature
            public static Pair<Double,​SizeUnit> getHumanReadableSize​(double size,
                                                                           SizeUnit unit)
            ```

        []{#toHumanReadableString(com.facebook.buck.util.types.Pair,java.util.Locale)}

        -   #### toHumanReadableString

            ``` methodSignature
            public static String toHumanReadableString​(Pair<Double,​SizeUnit> size,
                                                       Locale locale)
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
