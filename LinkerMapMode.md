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
-   [Field](#field.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Enum Constants](#enum.constant.detail) \| 
-   [Field](#field.detail) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.cxx.toolchain](package-summary.html)
:::

## Enum LinkerMapMode {#enum-linkermapmode .title title="Enum LinkerMapMode"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [java.lang.Enum](http://docs.oracle.com/javase/7/docs/api/java/lang/Enum.html?is-external=true "class or interface in java.lang"){.externalLink}\<[LinkerMapMode](LinkerMapMode.html "enum in com.facebook.buck.cxx.toolchain")\>

    -   -   com.facebook.buck.cxx.toolchain.LinkerMapMode

::: description
-   

    All Implemented Interfaces:
    :   `FlavorConvertible`, `Serializable`, `Comparable<LinkerMapMode>`

    ------------------------------------------------------------------------

        public enum LinkerMapMode
        extends Enum<LinkerMapMode>
        implements FlavorConvertible

    ::: block
    Defines if linker map should be generated or not.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#enum.constant.summary}

        ### Enum Constant Summary

          Enum Constant     Description
          ----------------- -------------
          `NO_LINKER_MAP`    

          : Enum Constants[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type                      Field             Description
          -------------------------------------- ----------------- -------------
          `static FlavorDomain<LinkerMapMode>`   `FLAVOR_DOMAIN`    

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `Flavor`              | `getFlavor()`         |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static boolean`      | `isLinkerMapEnabl     |                       |
        |                       | edForBuildTarget​(Buil |                       |
        |                       | dTarget buildTarget)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static BuildTarget`  | `removeLinkerM        |                       |
        |                       | apModeFlavorInTarget​( |                       |
        |                       | BuildTarget buildTarg |                       |
        |                       | et,                   |                       |
        |                       |                 Optio |                       |
        |                       | nal<LinkerMapMode> fl |                       |
        |                       | avoredLinkerMapMode)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static BuildTarget`  | `restoreLinkerMa      |                       |
        |                       | pModeFlavorInTarget​(B |                       |
        |                       | uildTarget buildTarge |                       |
        |                       | t,                    |                       |
        |                       |                 Optio |                       |
        |                       | nal<LinkerMapMode> fl |                       |
        |                       | avoredLinkerMapMode)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `                     | ::: block             |
        | static LinkerMapMode` | valueOf​(String name)` | Returns the enum      |
        |                       |                       | constant of this type |
        |                       |                       | with the specified    |
        |                       |                       | name.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `st                   | `values()`            | ::: block             |
        | atic LinkerMapMode[]` |                       | Returns an array      |
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

        []{#NO_LINKER_MAP}

        -   #### NO_LINKER_MAP

                public static final LinkerMapMode NO_LINKER_MAP
    :::

    ::: {.section role="region"}
    -   []{#field.detail}

        ### Field Detail

        []{#FLAVOR_DOMAIN}

        -   #### FLAVOR_DOMAIN

                public static final FlavorDomain<LinkerMapMode> FLAVOR_DOMAIN
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#values()}

        -   #### values

            ``` methodSignature
            public static LinkerMapMode[] values()
            ```

            ::: block
            Returns an array containing the constants of this enum type,
            in the order they are declared. This method may be used to
            iterate over the constants as follows:
                for (LinkerMapMode c : LinkerMapMode.values())
                    System.out.println(c);
            :::

            [Returns:]{.returnLabel}
            :   an array containing the constants of this enum type, in
                the order they are declared

        []{#valueOf(java.lang.String)}

        -   #### valueOf

            ``` methodSignature
            public static LinkerMapMode valueOf​(String name)
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

        []{#getFlavor()}

        -   #### getFlavor

            ``` methodSignature
            public Flavor getFlavor()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getFlavor` in interface `FlavorConvertible`

        []{#isLinkerMapEnabledForBuildTarget(com.facebook.buck.core.model.BuildTarget)}

        -   #### isLinkerMapEnabledForBuildTarget

            ``` methodSignature
            public static boolean isLinkerMapEnabledForBuildTarget​(BuildTarget buildTarget)
            ```

        []{#removeLinkerMapModeFlavorInTarget(com.facebook.buck.core.model.BuildTarget,java.util.Optional)}

        -   #### removeLinkerMapModeFlavorInTarget

            ``` methodSignature
            public static BuildTarget removeLinkerMapModeFlavorInTarget​(BuildTarget buildTarget,
                                                                        Optional<LinkerMapMode> flavoredLinkerMapMode)
            ```

        []{#restoreLinkerMapModeFlavorInTarget(com.facebook.buck.core.model.BuildTarget,java.util.Optional)}

        -   #### restoreLinkerMapModeFlavorInTarget

            ``` methodSignature
            public static BuildTarget restoreLinkerMapModeFlavorInTarget​(BuildTarget buildTarget,
                                                                         Optional<LinkerMapMode> flavoredLinkerMapMode)
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
-   [Field](#field.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Enum Constants](#enum.constant.detail) \| 
-   [Field](#field.detail) \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
