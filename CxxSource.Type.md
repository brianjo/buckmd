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
[Package]{.packageLabelInType} [com.facebook.buck.cxx](package-summary.html)
:::

## Enum CxxSource.Type {#enum-cxxsource.type .title title="Enum CxxSource.Type"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [java.lang.Enum](http://docs.oracle.com/javase/7/docs/api/java/lang/Enum.html?is-external=true "class or interface in java.lang"){.externalLink}\<[CxxSource.Type](CxxSource.Type.html "enum in com.facebook.buck.cxx")\>

    -   -   com.facebook.buck.cxx.CxxSource.Type

::: description
-   

    All Implemented Interfaces:
    :   `Serializable`, `Comparable<CxxSource.Type>`

    ```{=html}
    <!-- -->
    ```

    Enclosing class:
    :   [CxxSource](CxxSource.html "class in com.facebook.buck.cxx")

    ------------------------------------------------------------------------

        public static enum CxxSource.Type
        extends Enum<CxxSource.Type>
:::

::: summary
-   ::: {.section role="region"}
    -   []{#enum.constant.summary}

        ### Enum Constant Summary

          Enum Constant          Description
          ---------------------- -------------
          `ASM`                   
          `ASM_WITH_CPP`          
          `ASSEMBLER`             
          `ASSEMBLER_WITH_CPP`    
          `C`                     
          `C_CPP_OUTPUT`          
          `CUDA`                  
          `CUDA_CPP_OUTPUT`       
          `CXX`                   
          `CXX_CPP_OUTPUT`        
          `CXX_THINLINK`          
          `HIP`                   
          `HIP_CPP_OUTPUT`        
          `OBJC`                  
          `OBJC_CPP_OUTPUT`       
          `OBJCXX`                
          `OBJCXX_CPP_OUTPUT`     
          `PCM`                   

          : Enum Constants[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static Opti          | `fromExtensi          |                       |
        | onal<CxxSource.Type>` | on​(String extension)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static Opti          | `fromLangu            | ::: block             |
        | onal<CxxSource.Type>` | age​(String language)` | Returns existing type |
        |                       |                       | based on the language |
        |                       |                       | string                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.g                | `getExtensions()`     |                       |
        | oogle.common.collect. |                       |                       |
        | ImmutableSet<String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getLanguage()`       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `getPrecomp           | ::: block             |
        |                       | iledHeaderLanguage()` | \"Language\" type to  |
        |                       |                       | pass to the compiler  |
        |                       |                       | in order to generate  |
        |                       |                       | a precompiled header. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getPr                |                       |
        |                       | eprocessedLanguage()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isAssembly()`        |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isPreprocessable()`  |                       |
        +-----------------------+-----------------------+-----------------------+
        | `s                    | `                     | ::: block             |
        | tatic CxxSource.Type` | valueOf​(String name)` | Returns the enum      |
        |                       |                       | constant of this type |
        |                       |                       | with the specified    |
        |                       |                       | name.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `sta                  | `values()`            | ::: block             |
        | tic CxxSource.Type[]` |                       | Returns an array      |
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

        []{#C}

        -   #### C

                public static final CxxSource.Type C

        []{#CXX}

        -   #### CXX

                public static final CxxSource.Type CXX

        []{#CXX_THINLINK}

        -   #### CXX_THINLINK

                public static final CxxSource.Type CXX_THINLINK

        []{#OBJC}

        -   #### OBJC

                public static final CxxSource.Type OBJC

        []{#OBJCXX}

        -   #### OBJCXX

                public static final CxxSource.Type OBJCXX

        []{#CUDA}

        -   #### CUDA

                public static final CxxSource.Type CUDA

        []{#HIP}

        -   #### HIP

                public static final CxxSource.Type HIP

        []{#C_CPP_OUTPUT}

        -   #### C_CPP_OUTPUT

                public static final CxxSource.Type C_CPP_OUTPUT

        []{#CXX_CPP_OUTPUT}

        -   #### CXX_CPP_OUTPUT

                public static final CxxSource.Type CXX_CPP_OUTPUT

        []{#OBJC_CPP_OUTPUT}

        -   #### OBJC_CPP_OUTPUT

                public static final CxxSource.Type OBJC_CPP_OUTPUT

        []{#OBJCXX_CPP_OUTPUT}

        -   #### OBJCXX_CPP_OUTPUT

                public static final CxxSource.Type OBJCXX_CPP_OUTPUT

        []{#CUDA_CPP_OUTPUT}

        -   #### CUDA_CPP_OUTPUT

                public static final CxxSource.Type CUDA_CPP_OUTPUT

        []{#HIP_CPP_OUTPUT}

        -   #### HIP_CPP_OUTPUT

                public static final CxxSource.Type HIP_CPP_OUTPUT

        []{#ASSEMBLER_WITH_CPP}

        -   #### ASSEMBLER_WITH_CPP

                public static final CxxSource.Type ASSEMBLER_WITH_CPP

        []{#ASSEMBLER}

        -   #### ASSEMBLER

                public static final CxxSource.Type ASSEMBLER

        []{#ASM_WITH_CPP}

        -   #### ASM_WITH_CPP

                public static final CxxSource.Type ASM_WITH_CPP

        []{#ASM}

        -   #### ASM

                public static final CxxSource.Type ASM

        []{#PCM}

        -   #### PCM

                public static final CxxSource.Type PCM
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#values()}

        -   #### values

            ``` methodSignature
            public static CxxSource.Type[] values()
            ```

            ::: block
            Returns an array containing the constants of this enum type,
            in the order they are declared. This method may be used to
            iterate over the constants as follows:
                for (CxxSource.Type c : CxxSource.Type.values())
                    System.out.println(c);
            :::

            [Returns:]{.returnLabel}
            :   an array containing the constants of this enum type, in
                the order they are declared

        []{#valueOf(java.lang.String)}

        -   #### valueOf

            ``` methodSignature
            public static CxxSource.Type valueOf​(String name)
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

        []{#fromExtension(java.lang.String)}

        -   #### fromExtension

            ``` methodSignature
            public static Optional<CxxSource.Type> fromExtension​(String extension)
            ```

        []{#fromLanguage(java.lang.String)}

        -   #### fromLanguage

            ``` methodSignature
            public static Optional<CxxSource.Type> fromLanguage​(String language)
            ```

            ::: block
            Returns existing type based on the language string
            :::

            [Parameters:]{.paramLabel}
            :   `language` - the language string used to look up the
                Type

            [Returns:]{.returnLabel}
            :   Type if any type matches with the input string.
                Otherwise empty

        []{#getLanguage()}

        -   #### getLanguage

            ``` methodSignature
            public String getLanguage()
            ```

        []{#getPreprocessedLanguage()}

        -   #### getPreprocessedLanguage

            ``` methodSignature
            public String getPreprocessedLanguage()
            ```

        []{#getPrecompiledHeaderLanguage()}

        -   #### getPrecompiledHeaderLanguage

            ``` methodSignature
            public Optional<String> getPrecompiledHeaderLanguage()
            ```

            ::: block
            \"Language\" type to pass to the compiler in order to
            generate a precompiled header.
            Will be `absent` for source types which do not support
            precompiled headers.
            :::

        []{#isPreprocessable()}

        -   #### isPreprocessable

            ``` methodSignature
            public boolean isPreprocessable()
            ```

        []{#getExtensions()}

        -   #### getExtensions

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<String> getExtensions()
            ```

        []{#isAssembly()}

        -   #### isAssembly

            ``` methodSignature
            public boolean isAssembly()
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
