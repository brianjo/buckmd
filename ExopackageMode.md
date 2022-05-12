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
[Package]{.packageLabelInType} [com.facebook.buck.android.exopackage](package-summary.html)
:::

## Enum ExopackageMode {#enum-exopackagemode .title title="Enum ExopackageMode"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [java.lang.Enum](http://docs.oracle.com/javase/7/docs/api/java/lang/Enum.html?is-external=true "class or interface in java.lang"){.externalLink}\<[ExopackageMode](ExopackageMode.html "enum in com.facebook.buck.android.exopackage")\>

    -   -   com.facebook.buck.android.exopackage.ExopackageMode

::: description
-   

    All Implemented Interfaces:
    :   `Serializable`, `Comparable<ExopackageMode>`

    ------------------------------------------------------------------------

        public enum ExopackageMode
        extends Enum<ExopackageMode>
:::

::: summary
-   ::: {.section role="region"}
    -   []{#enum.constant.summary}

        ### Enum Constant Summary

          Enum Constant      Description
          ------------------ -------------
          `ARCH64`            
          `MODULES`           
          `NATIVE_LIBRARY`    
          `RESOURCES`         
          `SECONDARY_DEX`     

          : Enum Constants[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static boolean`      | `enable               |                       |
        |                       | dForArch64​(EnumSet<Ex |                       |
        |                       | opackageMode> modes)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static boolean`      | `enabled              |                       |
        |                       | ForModules​(EnumSet<Ex |                       |
        |                       | opackageMode> modes)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static boolean`      | `enabledForNativ      |                       |
        |                       | eLibraries​(EnumSet<Ex |                       |
        |                       | opackageMode> modes)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static boolean`      | `enabledFo            |                       |
        |                       | rResources​(EnumSet<Ex |                       |
        |                       | opackageMode> modes)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static boolean`      | `enabledForSeco       |                       |
        |                       | ndaryDexes​(EnumSet<Ex |                       |
        |                       | opackageMode> modes)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static int`          | `toBitmask​(EnumSet<Ex |                       |
        |                       | opackageMode> modes)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `s                    | `                     | ::: block             |
        | tatic ExopackageMode` | valueOf​(String name)` | Returns the enum      |
        |                       |                       | constant of this type |
        |                       |                       | with the specified    |
        |                       |                       | name.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `sta                  | `values()`            | ::: block             |
        | tic ExopackageMode[]` |                       | Returns an array      |
        |                       |                       | containing the        |
        |                       |                       | constants of this     |
        |                       |                       | enum type, in the     |
        |                       |                       | order they are        |
        |                       |                       | declared.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
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

        []{#SECONDARY_DEX}

        -   #### SECONDARY_DEX

                public static final ExopackageMode SECONDARY_DEX

        []{#NATIVE_LIBRARY}

        -   #### NATIVE_LIBRARY

                public static final ExopackageMode NATIVE_LIBRARY

        []{#RESOURCES}

        -   #### RESOURCES

                public static final ExopackageMode RESOURCES

        []{#MODULES}

        -   #### MODULES

                public static final ExopackageMode MODULES

        []{#ARCH64}

        -   #### ARCH64

                public static final ExopackageMode ARCH64
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#values()}

        -   #### values

            ``` methodSignature
            public static ExopackageMode[] values()
            ```

            ::: block
            Returns an array containing the constants of this enum type,
            in the order they are declared. This method may be used to
            iterate over the constants as follows:
                for (ExopackageMode c : ExopackageMode.values())
                    System.out.println(c);
            :::

            [Returns:]{.returnLabel}
            :   an array containing the constants of this enum type, in
                the order they are declared

        []{#valueOf(java.lang.String)}

        -   #### valueOf

            ``` methodSignature
            public static ExopackageMode valueOf​(String name)
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

        []{#enabledForSecondaryDexes(java.util.EnumSet)}

        -   #### enabledForSecondaryDexes

            ``` methodSignature
            public static boolean enabledForSecondaryDexes​(EnumSet<ExopackageMode> modes)
            ```

        []{#enabledForNativeLibraries(java.util.EnumSet)}

        -   #### enabledForNativeLibraries

            ``` methodSignature
            public static boolean enabledForNativeLibraries​(EnumSet<ExopackageMode> modes)
            ```

        []{#enabledForResources(java.util.EnumSet)}

        -   #### enabledForResources

            ``` methodSignature
            public static boolean enabledForResources​(EnumSet<ExopackageMode> modes)
            ```

        []{#enabledForModules(java.util.EnumSet)}

        -   #### enabledForModules

            ``` methodSignature
            public static boolean enabledForModules​(EnumSet<ExopackageMode> modes)
            ```

        []{#enabledForArch64(java.util.EnumSet)}

        -   #### enabledForArch64

            ``` methodSignature
            public static boolean enabledForArch64​(EnumSet<ExopackageMode> modes)
            ```

        []{#toBitmask(java.util.EnumSet)}

        -   #### toBitmask

            ``` methodSignature
            public static int toBitmask​(EnumSet<ExopackageMode> modes)
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
