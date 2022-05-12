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

## Enum PBXCopyFilesBuildPhase.Destination {#enum-pbxcopyfilesbuildphase.destination .title title="Enum PBXCopyFilesBuildPhase.Destination"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [java.lang.Enum](http://docs.oracle.com/javase/7/docs/api/java/lang/Enum.html?is-external=true "class or interface in java.lang"){.externalLink}\<[PBXCopyFilesBuildPhase.Destination](PBXCopyFilesBuildPhase.Destination.html "enum in com.facebook.buck.apple.xcode.xcodeproj")\>

    -   -   com.facebook.buck.apple.xcode.xcodeproj.PBXCopyFilesBuildPhase.Destination

::: description
-   

    All Implemented Interfaces:
    :   `Serializable`, `Comparable<PBXCopyFilesBuildPhase.Destination>`

    ```{=html}
    <!-- -->
    ```

    Enclosing class:
    :   [PBXCopyFilesBuildPhase](PBXCopyFilesBuildPhase.html "class in com.facebook.buck.apple.xcode.xcodeproj")

    ------------------------------------------------------------------------

        public static enum PBXCopyFilesBuildPhase.Destination
        extends Enum<PBXCopyFilesBuildPhase.Destination>

    ::: block
    The prefix path, this does not use SourceTreePath and build
    variables but rather some sort of enum.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#enum.constant.summary}

        ### Enum Constant Summary

          Enum Constant         Description
          --------------------- -------------
          `ABSOLUTE`             
          `APPCLIPS`             
          `EXECUTABLES`          
          `FRAMEWORKS`           
          `JAVA_RESOURCES`       
          `PLUGINS`              
          `PRODUCTS`             
          `QLGENERATOR`          
          `RESOURCES`            
          `SHARED_FRAMEWORKS`    
          `SHARED_SUPPORT`       
          `WRAPPER`              
          `XPC`                  

          : Enum Constants[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `int`                 | `getValue()`          |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `                     | ::: block             |
        | static PBXCopyFilesBu | valueOf​(String name)` | Returns the enum      |
        | ildPhase.Destination` |                       | constant of this type |
        |                       |                       | with the specified    |
        |                       |                       | name.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `st                   | `values()`            | ::: block             |
        | atic PBXCopyFilesBuil |                       | Returns an array      |
        | dPhase.Destination[]` |                       | containing the        |
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

        []{#ABSOLUTE}

        -   #### ABSOLUTE

                public static final PBXCopyFilesBuildPhase.Destination ABSOLUTE

        []{#WRAPPER}

        -   #### WRAPPER

                public static final PBXCopyFilesBuildPhase.Destination WRAPPER

        []{#EXECUTABLES}

        -   #### EXECUTABLES

                public static final PBXCopyFilesBuildPhase.Destination EXECUTABLES

        []{#RESOURCES}

        -   #### RESOURCES

                public static final PBXCopyFilesBuildPhase.Destination RESOURCES

        []{#APPCLIPS}

        -   #### APPCLIPS

                public static final PBXCopyFilesBuildPhase.Destination APPCLIPS

        []{#FRAMEWORKS}

        -   #### FRAMEWORKS

                public static final PBXCopyFilesBuildPhase.Destination FRAMEWORKS

        []{#SHARED_FRAMEWORKS}

        -   #### SHARED_FRAMEWORKS

                public static final PBXCopyFilesBuildPhase.Destination SHARED_FRAMEWORKS

        []{#SHARED_SUPPORT}

        -   #### SHARED_SUPPORT

                public static final PBXCopyFilesBuildPhase.Destination SHARED_SUPPORT

        []{#PLUGINS}

        -   #### PLUGINS

                public static final PBXCopyFilesBuildPhase.Destination PLUGINS

        []{#JAVA_RESOURCES}

        -   #### JAVA_RESOURCES

                public static final PBXCopyFilesBuildPhase.Destination JAVA_RESOURCES

        []{#PRODUCTS}

        -   #### PRODUCTS

                public static final PBXCopyFilesBuildPhase.Destination PRODUCTS

        []{#XPC}

        -   #### XPC

                public static final PBXCopyFilesBuildPhase.Destination XPC

        []{#QLGENERATOR}

        -   #### QLGENERATOR

                public static final PBXCopyFilesBuildPhase.Destination QLGENERATOR
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#values()}

        -   #### values

            ``` methodSignature
            public static PBXCopyFilesBuildPhase.Destination[] values()
            ```

            ::: block
            Returns an array containing the constants of this enum type,
            in the order they are declared. This method may be used to
            iterate over the constants as follows:
                for (PBXCopyFilesBuildPhase.Destination c : PBXCopyFilesBuildPhase.Destination.values())
                    System.out.println(c);
            :::

            [Returns:]{.returnLabel}
            :   an array containing the constants of this enum type, in
                the order they are declared

        []{#valueOf(java.lang.String)}

        -   #### valueOf

            ``` methodSignature
            public static PBXCopyFilesBuildPhase.Destination valueOf​(String name)
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

        []{#getValue()}

        -   #### getValue

            ``` methodSignature
            public int getValue()
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
