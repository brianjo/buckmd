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
[Package]{.packageLabelInType} [com.facebook.buck.apple.xcode.xcodeproj](package-summary.html)
:::

## Enum PBXReference.SourceTree {#enum-pbxreference.sourcetree .title title="Enum PBXReference.SourceTree"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [java.lang.Enum](http://docs.oracle.com/javase/7/docs/api/java/lang/Enum.html?is-external=true "class or interface in java.lang"){.externalLink}\<[PBXReference.SourceTree](PBXReference.SourceTree.html "enum in com.facebook.buck.apple.xcode.xcodeproj")\>

    -   -   com.facebook.buck.apple.xcode.xcodeproj.PBXReference.SourceTree

::: description
-   

    All Implemented Interfaces:
    :   `Serializable`, `Comparable<PBXReference.SourceTree>`

    ```{=html}
    <!-- -->
    ```

    Enclosing class:
    :   [PBXReference](PBXReference.html "class in com.facebook.buck.apple.xcode.xcodeproj")

    ------------------------------------------------------------------------

        public static enum PBXReference.SourceTree
        extends Enum<PBXReference.SourceTree>
:::

::: summary
-   ::: {.section role="region"}
    -   []{#enum.constant.summary}

        ### Enum Constant Summary

        +-----------------------------------+-----------------------------------+
        | Enum Constant                     | Description                       |
        +===================================+===================================+
        | `ABSOLUTE`                        | ::: block                         |
        |                                   | Absolute system path.             |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+
        | `BUILT_PRODUCTS_DIR`              | ::: block                         |
        |                                   | Relative to the build setting     |
        |                                   | `BUILT_PRODUCTS_DIR`.             |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+
        | `DEVELOPER_DIR`                   | ::: block                         |
        |                                   | Relative to the Developer content |
        |                                   | directory inside the Xcode        |
        |                                   | application (e.g.                 |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+
        | `GROUP`                           | ::: block                         |
        |                                   | Relative to the path of the group |
        |                                   | containing this.                  |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+
        | `PLATFORM_DIR`                    | ::: block                         |
        |                                   | Relative to the build setting     |
        |                                   | `PLATFORM_DIR`.                   |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+
        | `SDKROOT`                         | ::: block                         |
        |                                   | Relative to the build setting     |
        |                                   | `SDKROOT`.                        |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+
        | `SOURCE_ROOT`                     | ::: block                         |
        |                                   | Relative to the directory         |
        |                                   | containing the project file       |
        |                                   | `SOURCE_ROOT`.                    |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+

        : Enum Constants[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static Optional<PBXR | `fromBuildSetting​(    | ::: block             |
        | eference.SourceTree>` | String buildSetting)` | Return a sourceTree   |
        |                       |                       | given a build setting |
        |                       |                       | that is typically     |
        |                       |                       | used as a source tree |
        |                       |                       | prefix.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `toString()`          |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static PBX           | `                     | ::: block             |
        | Reference.SourceTree` | valueOf​(String name)` | Returns the enum      |
        |                       |                       | constant of this type |
        |                       |                       | with the specified    |
        |                       |                       | name.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static PBXRe         | `values()`            | ::: block             |
        | ference.SourceTree[]` |                       | Returns an array      |
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

        []{#GROUP}

        -   #### GROUP

                public static final PBXReference.SourceTree GROUP

            ::: block
            Relative to the path of the group containing this.
            :::

        []{#ABSOLUTE}

        -   #### ABSOLUTE

                public static final PBXReference.SourceTree ABSOLUTE

            ::: block
            Absolute system path.
            :::

        []{#BUILT_PRODUCTS_DIR}

        -   #### BUILT_PRODUCTS_DIR

                public static final PBXReference.SourceTree BUILT_PRODUCTS_DIR

            ::: block
            Relative to the build setting `BUILT_PRODUCTS_DIR`.
            :::

        []{#PLATFORM_DIR}

        -   #### PLATFORM_DIR

                public static final PBXReference.SourceTree PLATFORM_DIR

            ::: block
            Relative to the build setting `PLATFORM_DIR`.
            :::

        []{#SDKROOT}

        -   #### SDKROOT

                public static final PBXReference.SourceTree SDKROOT

            ::: block
            Relative to the build setting `SDKROOT`.
            :::

        []{#SOURCE_ROOT}

        -   #### SOURCE_ROOT

                public static final PBXReference.SourceTree SOURCE_ROOT

            ::: block
            Relative to the directory containing the project file
            `SOURCE_ROOT`.
            :::

        []{#DEVELOPER_DIR}

        -   #### DEVELOPER_DIR

                public static final PBXReference.SourceTree DEVELOPER_DIR

            ::: block
            Relative to the Developer content directory inside the Xcode
            application (e.g.
            `  /Applications/Xcode.app/Contents/Developer`).
            :::
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#values()}

        -   #### values

            ``` methodSignature
            public static PBXReference.SourceTree[] values()
            ```

            ::: block
            Returns an array containing the constants of this enum type,
            in the order they are declared. This method may be used to
            iterate over the constants as follows:
                for (PBXReference.SourceTree c : PBXReference.SourceTree.values())
                    System.out.println(c);
            :::

            [Returns:]{.returnLabel}
            :   an array containing the constants of this enum type, in
                the order they are declared

        []{#valueOf(java.lang.String)}

        -   #### valueOf

            ``` methodSignature
            public static PBXReference.SourceTree valueOf​(String name)
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
            :   `toString` in class `Enum<PBXReference.SourceTree>`

        []{#fromBuildSetting(java.lang.String)}

        -   #### fromBuildSetting

            ``` methodSignature
            public static Optional<PBXReference.SourceTree> fromBuildSetting​(String buildSetting)
            ```

            ::: block
            Return a sourceTree given a build setting that is typically
            used as a source tree prefix.
            The build setting may be optionally prefixed by \'\$\' which
            will be stripped.
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
