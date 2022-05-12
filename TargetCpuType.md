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
[Package]{.packageLabelInType} [com.facebook.buck.android.toolchain.ndk](package-summary.html)
:::

## Enum TargetCpuType {#enum-targetcputype .title title="Enum TargetCpuType"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [java.lang.Enum](http://docs.oracle.com/javase/7/docs/api/java/lang/Enum.html?is-external=true "class or interface in java.lang"){.externalLink}\<[TargetCpuType](TargetCpuType.html "enum in com.facebook.buck.android.toolchain.ndk")\>

    -   -   com.facebook.buck.android.toolchain.ndk.TargetCpuType

::: description
-   

    All Implemented Interfaces:
    :   `Serializable`, `Comparable<TargetCpuType>`

    ------------------------------------------------------------------------

        public enum TargetCpuType
        extends Enum<TargetCpuType>

    ::: block
    The CPU architectures to target.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#enum.constant.summary}

        ### Enum Constant Summary

          Enum Constant   Description
          --------------- -------------
          `ARM`            
          `ARM64`          
          `ARMV7`          
          `MIPS`           
          `X86`            
          `X86_64`         

          : Enum Constants[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `abstract com.go      | `ge                   |                       |
        | ogle.common.collect.I | tAssemblerFlags​(NdkCo |                       |
        | mmutableList<String>` | mpilerType compiler)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract com.go      | `g                    |                       |
        | ogle.common.collect.I | etCompilerFlags​(NdkCo |                       |
        | mmutableList<String>` | mpilerType compiler)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract com.go      | `getLinkerFlags​(NdkCo |                       |
        | ogle.common.collect.I | mpilerType compiler)` |                       |
        | mmutableList<String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `ab                   | `getTargetArch()`     |                       |
        | stract NdkTargetArch` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstr                | `getTargetArchAbi()`  |                       |
        | act NdkTargetArchAbi` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `a                    | `getToolchain()`      |                       |
        | bstract NdkToolchain` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstrac              | `                     |                       |
        | t NdkToolchainTarget` | getToolchainTarget()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `                     | ::: block             |
        | static TargetCpuType` | valueOf​(String name)` | Returns the enum      |
        |                       |                       | constant of this type |
        |                       |                       | with the specified    |
        |                       |                       | name.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `st                   | `values()`            | ::: block             |
        | atic TargetCpuType[]` |                       | Returns an array      |
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
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
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

        []{#ARM}

        -   #### ARM

                public static final TargetCpuType ARM

        []{#ARMV7}

        -   #### ARMV7

                public static final TargetCpuType ARMV7

        []{#ARM64}

        -   #### ARM64

                public static final TargetCpuType ARM64

        []{#X86}

        -   #### X86

                public static final TargetCpuType X86

        []{#X86_64}

        -   #### X86_64

                public static final TargetCpuType X86_64

        []{#MIPS}

        -   #### MIPS

                public static final TargetCpuType MIPS
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#values()}

        -   #### values

            ``` methodSignature
            public static TargetCpuType[] values()
            ```

            ::: block
            Returns an array containing the constants of this enum type,
            in the order they are declared. This method may be used to
            iterate over the constants as follows:
                for (TargetCpuType c : TargetCpuType.values())
                    System.out.println(c);
            :::

            [Returns:]{.returnLabel}
            :   an array containing the constants of this enum type, in
                the order they are declared

        []{#valueOf(java.lang.String)}

        -   #### valueOf

            ``` methodSignature
            public static TargetCpuType valueOf​(String name)
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

        []{#getTargetArch()}

        -   #### getTargetArch

            ``` methodSignature
            public abstract NdkTargetArch getTargetArch()
            ```

        []{#getTargetArchAbi()}

        -   #### getTargetArchAbi

            ``` methodSignature
            public abstract NdkTargetArchAbi getTargetArchAbi()
            ```

        []{#getToolchain()}

        -   #### getToolchain

            ``` methodSignature
            public abstract NdkToolchain getToolchain()
            ```

        []{#getToolchainTarget()}

        -   #### getToolchainTarget

            ``` methodSignature
            public abstract NdkToolchainTarget getToolchainTarget()
            ```

        []{#getAssemblerFlags(com.facebook.buck.android.toolchain.ndk.NdkCompilerType)}

        -   #### getAssemblerFlags

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableList<String> getAssemblerFlags​(NdkCompilerType compiler)
            ```

        []{#getCompilerFlags(com.facebook.buck.android.toolchain.ndk.NdkCompilerType)}

        -   #### getCompilerFlags

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableList<String> getCompilerFlags​(NdkCompilerType compiler)
            ```

        []{#getLinkerFlags(com.facebook.buck.android.toolchain.ndk.NdkCompilerType)}

        -   #### getLinkerFlags

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableList<String> getLinkerFlags​(NdkCompilerType compiler)
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
