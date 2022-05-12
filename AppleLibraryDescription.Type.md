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
[Package]{.packageLabelInType} [com.facebook.buck.apple](package-summary.html)
:::

## Enum AppleLibraryDescription.Type {#enum-applelibrarydescription.type .title title="Enum AppleLibraryDescription.Type"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [java.lang.Enum](http://docs.oracle.com/javase/7/docs/api/java/lang/Enum.html?is-external=true "class or interface in java.lang"){.externalLink}\<[AppleLibraryDescription.Type](AppleLibraryDescription.Type.html "enum in com.facebook.buck.apple")\>

    -   -   com.facebook.buck.apple.AppleLibraryDescription.Type

::: description
-   

    All Implemented Interfaces:
    :   `FlavorConvertible`, `Serializable`,
        `Comparable<AppleLibraryDescription.Type>`

    ```{=html}
    <!-- -->
    ```

    Enclosing class:
    :   [AppleLibraryDescription](AppleLibraryDescription.html "class in com.facebook.buck.apple")

    ------------------------------------------------------------------------

        public static enum AppleLibraryDescription.Type
        extends Enum<AppleLibraryDescription.Type>
        implements FlavorConvertible
:::

::: summary
-   ::: {.section role="region"}
    -   []{#enum.constant.summary}

        ### Enum Constant Summary

          Enum Constant                            Description
          ---------------------------------------- -------------
          `EXPORTED_HEADERS`                        
          `FRAMEWORK`                               
          `HEADERS`                                 
          `MACH_O_BUNDLE`                           
          `SHARED`                                  
          `STATIC`                                  
          `STATIC_PIC`                              
          `SWIFT_COMPILE`                           
          `SWIFT_EXPORTED_OBJC_GENERATED_HEADER`    
          `SWIFT_OBJC_GENERATED_HEADER`             
          `SWIFT_UNDERLYING_MODULE`                 

          : Enum Constants[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `Flavor`              | `getFlavor()`         |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static AppleLib      | `                     | ::: block             |
        | raryDescription.Type` | valueOf​(String name)` | Returns the enum      |
        |                       |                       | constant of this type |
        |                       |                       | with the specified    |
        |                       |                       | name.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static AppleLibra    | `values()`            | ::: block             |
        | ryDescription.Type[]` |                       | Returns an array      |
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

        []{#HEADERS}

        -   #### HEADERS

                public static final AppleLibraryDescription.Type HEADERS

        []{#EXPORTED_HEADERS}

        -   #### EXPORTED_HEADERS

                public static final AppleLibraryDescription.Type EXPORTED_HEADERS

        []{#SHARED}

        -   #### SHARED

                public static final AppleLibraryDescription.Type SHARED

        []{#STATIC_PIC}

        -   #### STATIC_PIC

                public static final AppleLibraryDescription.Type STATIC_PIC

        []{#STATIC}

        -   #### STATIC

                public static final AppleLibraryDescription.Type STATIC

        []{#MACH_O_BUNDLE}

        -   #### MACH_O\_BUNDLE

                public static final AppleLibraryDescription.Type MACH_O_BUNDLE

        []{#FRAMEWORK}

        -   #### FRAMEWORK

                public static final AppleLibraryDescription.Type FRAMEWORK

        []{#SWIFT_COMPILE}

        -   #### SWIFT_COMPILE

                public static final AppleLibraryDescription.Type SWIFT_COMPILE

        []{#SWIFT_OBJC_GENERATED_HEADER}

        -   #### SWIFT_OBJC_GENERATED_HEADER

                public static final AppleLibraryDescription.Type SWIFT_OBJC_GENERATED_HEADER

        []{#SWIFT_EXPORTED_OBJC_GENERATED_HEADER}

        -   #### SWIFT_EXPORTED_OBJC_GENERATED_HEADER

                public static final AppleLibraryDescription.Type SWIFT_EXPORTED_OBJC_GENERATED_HEADER

        []{#SWIFT_UNDERLYING_MODULE}

        -   #### SWIFT_UNDERLYING_MODULE

                public static final AppleLibraryDescription.Type SWIFT_UNDERLYING_MODULE
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#values()}

        -   #### values

            ``` methodSignature
            public static AppleLibraryDescription.Type[] values()
            ```

            ::: block
            Returns an array containing the constants of this enum type,
            in the order they are declared. This method may be used to
            iterate over the constants as follows:
                for (AppleLibraryDescription.Type c : AppleLibraryDescription.Type.values())
                    System.out.println(c);
            :::

            [Returns:]{.returnLabel}
            :   an array containing the constants of this enum type, in
                the order they are declared

        []{#valueOf(java.lang.String)}

        -   #### valueOf

            ``` methodSignature
            public static AppleLibraryDescription.Type valueOf​(String name)
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
