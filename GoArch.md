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
[Package]{.packageLabelInType} [com.facebook.buck.features.go](package-summary.html)
:::

## Enum GoArch {#enum-goarch .title title="Enum GoArch"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [java.lang.Enum](http://docs.oracle.com/javase/7/docs/api/java/lang/Enum.html?is-external=true "class or interface in java.lang"){.externalLink}\<[GoArch](GoArch.html "enum in com.facebook.buck.features.go")\>

    -   -   com.facebook.buck.features.go.GoArch

::: description
-   

    All Implemented Interfaces:
    :   `Serializable`, `Comparable<GoArch>`

    ------------------------------------------------------------------------

        public enum GoArch
        extends Enum<GoArch>

    ::: block
    Represents the GOARCH values in Go found at:
    https://github.com/golang/go/blob/master/src/go/build/syslist.go
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#enum.constant.summary}

        ### Enum Constant Summary

          Enum Constant   Description
          --------------- -------------
          `AMD64`          
          `AMD64P32`       
          `ARM`            
          `ARM64`          
          `ARM64BE`        
          `ARMBE`          
          `ARMV5`          
          `ARMv6`          
          `ARMV7`          
          `I386`           
          `MIPS`           
          `MIPS64`         
          `MIPS64LE`       
          `MIPS64P32`      
          `MIPS64P32LE`    
          `MIPSLE`         
          `PPC`            
          `PPC64`          
          `PPC64LE`        
          `RISCV`          
          `RISCV64`        
          `S390`           
          `S390X`          
          `SPARC`          
          `SPARC64`        
          `WASM`           

          : Enum Constants[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static GoArch`       | `fromArchitectur      | ::: block             |
        |                       | e​(Architecture arch)` | returns the           |
        |                       |                       | corresponding GoOs    |
        |                       |                       | for a given           |
        |                       |                       | Architecture          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static GoArch`       | `fro                  | ::: block             |
        |                       | mString​(String name)` | Finds the GoArch from |
        |                       |                       | it\'s name.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getEnvVarValue()`    | ::: block             |
        |                       |                       | Returns the           |
        |                       |                       | environment variable  |
        |                       |                       | to be used for GOARCH |
        |                       |                       | to Go tools.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `ge                   | ::: block             |
        |                       | tEnvVarValueForArm()` | Returns the           |
        |                       |                       | environment variable  |
        |                       |                       | to be used for GOARM  |
        |                       |                       | to Go tools.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static GoArch`       | `                     | ::: block             |
        |                       | valueOf​(String name)` | Returns the enum      |
        |                       |                       | constant of this type |
        |                       |                       | with the specified    |
        |                       |                       | name.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static GoArch[]`     | `values()`            | ::: block             |
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

        []{#I386}

        -   #### I386

                public static final GoArch I386

        []{#AMD64}

        -   #### AMD64

                public static final GoArch AMD64

        []{#AMD64P32}

        -   #### AMD64P32

                public static final GoArch AMD64P32

        []{#ARM}

        -   #### ARM

                public static final GoArch ARM

        []{#ARMV5}

        -   #### ARMV5

                public static final GoArch ARMV5

        []{#ARMv6}

        -   #### ARMv6

                public static final GoArch ARMv6

        []{#ARMV7}

        -   #### ARMV7

                public static final GoArch ARMV7

        []{#ARMBE}

        -   #### ARMBE

                public static final GoArch ARMBE

        []{#ARM64}

        -   #### ARM64

                public static final GoArch ARM64

        []{#ARM64BE}

        -   #### ARM64BE

                public static final GoArch ARM64BE

        []{#PPC64}

        -   #### PPC64

                public static final GoArch PPC64

        []{#PPC64LE}

        -   #### PPC64LE

                public static final GoArch PPC64LE

        []{#MIPS}

        -   #### MIPS

                public static final GoArch MIPS

        []{#MIPSLE}

        -   #### MIPSLE

                public static final GoArch MIPSLE

        []{#MIPS64}

        -   #### MIPS64

                public static final GoArch MIPS64

        []{#MIPS64LE}

        -   #### MIPS64LE

                public static final GoArch MIPS64LE

        []{#MIPS64P32}

        -   #### MIPS64P32

                public static final GoArch MIPS64P32

        []{#MIPS64P32LE}

        -   #### MIPS64P32LE

                public static final GoArch MIPS64P32LE

        []{#PPC}

        -   #### PPC

                public static final GoArch PPC

        []{#RISCV}

        -   #### RISCV

                public static final GoArch RISCV

        []{#RISCV64}

        -   #### RISCV64

                public static final GoArch RISCV64

        []{#S390}

        -   #### S390

                public static final GoArch S390

        []{#S390X}

        -   #### S390X

                public static final GoArch S390X

        []{#SPARC}

        -   #### SPARC

                public static final GoArch SPARC

        []{#SPARC64}

        -   #### SPARC64

                public static final GoArch SPARC64

        []{#WASM}

        -   #### WASM

                public static final GoArch WASM
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#values()}

        -   #### values

            ``` methodSignature
            public static GoArch[] values()
            ```

            ::: block
            Returns an array containing the constants of this enum type,
            in the order they are declared. This method may be used to
            iterate over the constants as follows:
                for (GoArch c : GoArch.values())
                    System.out.println(c);
            :::

            [Returns:]{.returnLabel}
            :   an array containing the constants of this enum type, in
                the order they are declared

        []{#valueOf(java.lang.String)}

        -   #### valueOf

            ``` methodSignature
            public static GoArch valueOf​(String name)
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

        []{#getEnvVarValue()}

        -   #### getEnvVarValue

            ``` methodSignature
            public String getEnvVarValue()
            ```

            ::: block
            Returns the environment variable to be used for GOARCH to Go
            tools.
            :::

        []{#getEnvVarValueForArm()}

        -   #### getEnvVarValueForArm

            ``` methodSignature
            public String getEnvVarValueForArm()
            ```

            ::: block
            Returns the environment variable to be used for GOARM to Go
            tools.
            :::

        []{#fromString(java.lang.String)}

        -   #### fromString

            ``` methodSignature
            public static GoArch fromString​(String name)
            ```

            ::: block
            Finds the GoArch from it\'s name.
            :::

            [Parameters:]{.paramLabel}
            :   `name` - name of the GoArch as defined from Go itself

            [Returns:]{.returnLabel}
            :   GoArch for the matching name

            [Throws:]{.throwsLabel}
            :   `NoSuchElementException` - when a GoArch is not found
                for the name

        []{#fromArchitecture(com.facebook.buck.util.environment.Architecture)}

        -   #### fromArchitecture

            ``` methodSignature
            public static GoArch fromArchitecture​(Architecture arch)
                                           throws HumanReadableException
            ```

            ::: block
            returns the corresponding GoOs for a given Architecture
            :::

            [Parameters:]{.paramLabel}
            :   `arch` - the
                [`Architecture`](../../util/environment/Architecture.html "enum in com.facebook.buck.util.environment")
                to lookup

            [Returns:]{.returnLabel}
            :   GoArch for the matching platform

            [Throws:]{.throwsLabel}
            :   `HumanReadableException` - when a specific GoArch is not
                found for the Architecture
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
