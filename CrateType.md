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
[Package]{.packageLabelInType} [com.facebook.buck.features.rust](package-summary.html)
:::

## Enum CrateType {#enum-cratetype .title title="Enum CrateType"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [java.lang.Enum](http://docs.oracle.com/javase/7/docs/api/java/lang/Enum.html?is-external=true "class or interface in java.lang"){.externalLink}\<[CrateType](CrateType.html "enum in com.facebook.buck.features.rust")\>

    -   -   com.facebook.buck.features.rust.CrateType

::: description
-   

    All Implemented Interfaces:
    :   `Serializable`, `Comparable<CrateType>`

    ------------------------------------------------------------------------

        public enum CrateType
        extends Enum<CrateType>

    ::: block
    Describe the kinds of crates rustc can generate.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#enum.constant.summary}

        ### Enum Constant Summary

          Enum Constant       Description
          ------------------- -------------
          `BIN`                
          `CDYLIB`             
          `CHECK`              
          `CHECKBIN`           
          `DYLIB`              
          `LIB`                
          `PROC_MACRO`         
          `RLIB`               
          `RLIB_PIC`           
          `SAVEANALYSIS`       
          `SAVEANALYSISBIN`    
          `STATIC`             
          `STATIC_PIC`         

          : Enum Constants[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `String`              | `filename             | ::: block             |
        |                       | For​(BuildTarget targe | Return an appropriate |
        |                       | t,            String  | filename for this     |
        |                       | name,            CxxP | crate, given its type |
        |                       | latform cxxPlatform)` | and the platform.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Flavor`              | `getFlavor()`         |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isCheck()`           | ::: block             |
        |                       |                       | We\'re just checking  |
        |                       |                       | the code, and         |
        |                       |                       | generating metadata   |
        |                       |                       | to allow dependents   |
        |                       |                       | to check.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isDynamic()`         | ::: block             |
        |                       |                       | Crate dynamically     |
        |                       |                       | links with its        |
        |                       |                       | dependents.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isExecutable()`      | ::: block             |
        |                       |                       | Create generates an   |
        |                       |                       | executable            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isNative()`          | ::: block             |
        |                       |                       | Return true if this   |
        |                       |                       | crate type is         |
        |                       |                       | intended to be a      |
        |                       |                       | native output (ie,    |
        |                       |                       | not intended for      |
        |                       |                       | further processing by |
        |                       |                       | the Rust toolchain).  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isPic()`             | ::: block             |
        |                       |                       | Crate needs to be     |
        |                       |                       | compiled with         |
        |                       |                       | relocation-model=pic. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isProcMacro()`       | ::: block             |
        |                       |                       | Return true if this   |
        |                       |                       | is generating a       |
        |                       |                       | compiler plugin - ie, |
        |                       |                       | it should be linked   |
        |                       |                       | with a different      |
        |                       |                       | linker and linker     |
        |                       |                       | flags.                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isSaveAnalysis()`    | ::: block             |
        |                       |                       | Save-analysis is a    |
        |                       |                       | more detailed version |
        |                       |                       | of check, which saves |
        |                       |                       | full type and other   |
        |                       |                       | information in a json |
        |                       |                       | file for consumption  |
        |                       |                       | by other tools        |
        |                       |                       | (namely RLS).         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `needAllDeps()`       | ::: block             |
        |                       |                       | Linking this crate    |
        |                       |                       | needs all the         |
        |                       |                       | dependencies          |
        |                       |                       | available.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `toString()`          |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static CrateType`    | `                     | ::: block             |
        |                       | valueOf​(String name)` | Returns the enum      |
        |                       |                       | constant of this type |
        |                       |                       | with the specified    |
        |                       |                       | name.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static CrateType[]`  | `values()`            | ::: block             |
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

        []{#BIN}

        -   #### BIN

                public static final CrateType BIN

        []{#CHECK}

        -   #### CHECK

                public static final CrateType CHECK

        []{#CHECKBIN}

        -   #### CHECKBIN

                public static final CrateType CHECKBIN

        []{#SAVEANALYSIS}

        -   #### SAVEANALYSIS

                public static final CrateType SAVEANALYSIS

        []{#SAVEANALYSISBIN}

        -   #### SAVEANALYSISBIN

                public static final CrateType SAVEANALYSISBIN

        []{#LIB}

        -   #### LIB

                public static final CrateType LIB

        []{#RLIB}

        -   #### RLIB

                public static final CrateType RLIB

        []{#RLIB_PIC}

        -   #### RLIB_PIC

                public static final CrateType RLIB_PIC

        []{#DYLIB}

        -   #### DYLIB

                public static final CrateType DYLIB

        []{#CDYLIB}

        -   #### CDYLIB

                public static final CrateType CDYLIB

        []{#STATIC}

        -   #### STATIC

                public static final CrateType STATIC

        []{#STATIC_PIC}

        -   #### STATIC_PIC

                public static final CrateType STATIC_PIC

        []{#PROC_MACRO}

        -   #### PROC_MACRO

                public static final CrateType PROC_MACRO
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#values()}

        -   #### values

            ``` methodSignature
            public static CrateType[] values()
            ```

            ::: block
            Returns an array containing the constants of this enum type,
            in the order they are declared. This method may be used to
            iterate over the constants as follows:
                for (CrateType c : CrateType.values())
                    System.out.println(c);
            :::

            [Returns:]{.returnLabel}
            :   an array containing the constants of this enum type, in
                the order they are declared

        []{#valueOf(java.lang.String)}

        -   #### valueOf

            ``` methodSignature
            public static CrateType valueOf​(String name)
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

        []{#toString()}

        -   #### toString

            ``` methodSignature
            public String toString()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `toString` in class `Enum<CrateType>`

        []{#getFlavor()}

        -   #### getFlavor

            ``` methodSignature
            public Flavor getFlavor()
            ```

        []{#isNative()}

        -   #### isNative

            ``` methodSignature
            public boolean isNative()
            ```

            ::: block
            Return true if this crate type is intended to be a native
            output (ie, not intended for further processing by the Rust
            toolchain). In other words, a binary, or a native-linkable
            shared or static object.
            :::

            [Returns:]{.returnLabel}
            :   Is natively usable.

        []{#needAllDeps()}

        -   #### needAllDeps

            ``` methodSignature
            public boolean needAllDeps()
            ```

            ::: block
            Linking this crate needs all the dependencies available.
            :::

            [Returns:]{.returnLabel}
            :   Need all deps.

        []{#isDynamic()}

        -   #### isDynamic

            ``` methodSignature
            public boolean isDynamic()
            ```

            ::: block
            Crate dynamically links with its dependents.
            :::

            [Returns:]{.returnLabel}
            :   Is dynamic.

        []{#isPic()}

        -   #### isPic

            ``` methodSignature
            public boolean isPic()
            ```

            ::: block
            Crate needs to be compiled with relocation-model=pic.
            Executables are currently always compiled with -pie, and so
            are also PIC.
            :::

            [Returns:]{.returnLabel}
            :   Needs PIC.

        []{#isExecutable()}

        -   #### isExecutable

            ``` methodSignature
            public boolean isExecutable()
            ```

            ::: block
            Create generates an executable
            :::

        []{#isCheck()}

        -   #### isCheck

            ``` methodSignature
            public boolean isCheck()
            ```

            ::: block
            We\'re just checking the code, and generating metadata to
            allow dependents to check. For libraries this means we emit
            a metadata file, and binaries produce no output (they just
            consume library metadata). \"save-analysis\" also builds in
            check mode, but we\'re only concerned about the analysis
            output.
            :::

        []{#isSaveAnalysis()}

        -   #### isSaveAnalysis

            ``` methodSignature
            public boolean isSaveAnalysis()
            ```

            ::: block
            Save-analysis is a more detailed version of check, which
            saves full type and other information in a json file for
            consumption by other tools (namely RLS).
            :::

        []{#isProcMacro()}

        -   #### isProcMacro

            ``` methodSignature
            public boolean isProcMacro()
            ```

            ::: block
            Return true if this is generating a compiler plugin - ie, it
            should be linked with a different linker and linker flags.
            :::

        []{#filenameFor(com.facebook.buck.core.model.BuildTarget,java.lang.String,com.facebook.buck.cxx.toolchain.CxxPlatform)}

        -   #### filenameFor

            ``` methodSignature
            public String filenameFor​(BuildTarget target,
                                      String name,
                                      CxxPlatform cxxPlatform)
            ```

            ::: block
            Return an appropriate filename for this crate, given its
            type and the platform.
            :::

            [Parameters:]{.paramLabel}
            :   `name` - Base filename
            :   `cxxPlatform` - Platform we\'re building for

            [Returns:]{.returnLabel}
            :   Path component
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
