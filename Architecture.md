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
[Package]{.packageLabelInType} [com.facebook.buck.util.environment](package-summary.html)
:::

## Enum Architecture {#enum-architecture .title title="Enum Architecture"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [java.lang.Enum](http://docs.oracle.com/javase/7/docs/api/java/lang/Enum.html?is-external=true "class or interface in java.lang"){.externalLink}\<[Architecture](Architecture.html "enum in com.facebook.buck.util.environment")\>

    -   -   com.facebook.buck.util.environment.Architecture

::: description
-   

    All Implemented Interfaces:
    :   `Serializable`, `Comparable<Architecture>`

    ------------------------------------------------------------------------

        public enum Architecture
        extends Enum<Architecture>

    ::: block
    Represents the CPU architecture of a system.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#enum.constant.summary}

        ### Enum Constant Summary

          Enum Constant   Description
          --------------- -------------
          `AARCH64`        
          `ARM`            
          `ARMEB`          
          `MIPS`           
          `MIPS64`         
          `MIPSEL`         
          `MIPSEL64`       
          `POWERPC`        
          `PPC64`          
          `UNKNOWN`        
          `X86_32`         
          `X86_64`         

          : Enum Constants[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static Architecture` | `detect()`            |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static Architecture` | `detect​(Pr            | ::: block             |
        |                       | operties properties)` | Detect the host       |
        |                       |                       | architecture from the |
        |                       |                       | given Java properties |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static Architecture` | `f                    |                       |
        |                       | romName​(String name)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `toString()`          |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static Architecture` | `                     | ::: block             |
        |                       | valueOf​(String name)` | Returns the enum      |
        |                       |                       | constant of this type |
        |                       |                       | with the specified    |
        |                       |                       | name.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `s                    | `values()`            | ::: block             |
        | tatic Architecture[]` |                       | Returns an array      |
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

            `clone, compareTo, equals, finalize, getDeclaringClass, hashCode, name, ordinal, valueOf`

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

        []{#AARCH64}

        -   #### AARCH64

                public static final Architecture AARCH64

        []{#ARM}

        -   #### ARM

                public static final Architecture ARM

        []{#ARMEB}

        -   #### ARMEB

                public static final Architecture ARMEB

        []{#MIPS}

        -   #### MIPS

                public static final Architecture MIPS

        []{#MIPS64}

        -   #### MIPS64

                public static final Architecture MIPS64

        []{#MIPSEL}

        -   #### MIPSEL

                public static final Architecture MIPSEL

        []{#MIPSEL64}

        -   #### MIPSEL64

                public static final Architecture MIPSEL64

        []{#POWERPC}

        -   #### POWERPC

                public static final Architecture POWERPC

        []{#PPC64}

        -   #### PPC64

                public static final Architecture PPC64

        []{#UNKNOWN}

        -   #### UNKNOWN

                public static final Architecture UNKNOWN

        []{#X86_32}

        -   #### X86_32

                public static final Architecture X86_32

        []{#X86_64}

        -   #### X86_64

                public static final Architecture X86_64
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#values()}

        -   #### values

            ``` methodSignature
            public static Architecture[] values()
            ```

            ::: block
            Returns an array containing the constants of this enum type,
            in the order they are declared. This method may be used to
            iterate over the constants as follows:
                for (Architecture c : Architecture.values())
                    System.out.println(c);
            :::

            [Returns:]{.returnLabel}
            :   an array containing the constants of this enum type, in
                the order they are declared

        []{#valueOf(java.lang.String)}

        -   #### valueOf

            ``` methodSignature
            public static Architecture valueOf​(String name)
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

        []{#detect(java.util.Properties)}

        -   #### detect

            ``` methodSignature
            public static Architecture detect​(Properties properties)
            ```

            ::: block
            Detect the host architecture from the given Java properties
            :::

        []{#detect()}

        -   #### detect

            ``` methodSignature
            public static Architecture detect()
            ```

            [Returns:]{.returnLabel}
            :   CPU architecture of the currently running OS.

        []{#fromName(java.lang.String)}

        -   #### fromName

            ``` methodSignature
            public static Architecture fromName​(String name)
            ```

        []{#toString()}

        -   #### toString

            ``` methodSignature
            public String toString()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `toString` in class `Enum<Architecture>`
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
