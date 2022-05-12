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
[Package]{.packageLabelInType} [com.facebook.buck.apple.xcode](package-summary.html)
:::

## Enum XCScheme.BuildActionEntry.BuildFor {#enum-xcscheme.buildactionentry.buildfor .title title="Enum XCScheme.BuildActionEntry.BuildFor"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [java.lang.Enum](http://docs.oracle.com/javase/7/docs/api/java/lang/Enum.html?is-external=true "class or interface in java.lang"){.externalLink}\<[XCScheme.BuildActionEntry.BuildFor](XCScheme.BuildActionEntry.BuildFor.html "enum in com.facebook.buck.apple.xcode")\>

    -   -   com.facebook.buck.apple.xcode.XCScheme.BuildActionEntry.BuildFor

::: description
-   

    All Implemented Interfaces:
    :   `Serializable`, `Comparable<XCScheme.BuildActionEntry.BuildFor>`

    ```{=html}
    <!-- -->
    ```

    Enclosing class:
    :   [XCScheme.BuildActionEntry](XCScheme.BuildActionEntry.html "class in com.facebook.buck.apple.xcode")

    ------------------------------------------------------------------------

        public static enum XCScheme.BuildActionEntry.BuildFor
        extends Enum<XCScheme.BuildActionEntry.BuildFor>
:::

::: summary
-   ::: {.section role="region"}
    -   []{#enum.constant.summary}

        ### Enum Constant Summary

          Enum Constant   Description
          --------------- -------------
          `ANALYZING`      
          `ARCHIVING`      
          `PROFILING`      
          `RUNNING`        
          `TESTING`        

          : Enum Constants[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type                                      Field               Description
          ------------------------------------------------------ ------------------- -------------
          `static EnumSet<XCScheme.BuildActionEntry.BuildFor>`   `DEFAULT`            
          `static EnumSet<XCScheme.BuildActionEntry.BuildFor>`   `INDEXING_ONLY`      
          `static EnumSet<XCScheme.BuildActionEntry.BuildFor>`   `MAIN_EXECUTABLE`    
          `static EnumSet<XCScheme.BuildActionEntry.BuildFor>`   `SCHEME_LIBRARY`     
          `static EnumSet<XCScheme.BuildActionEntry.BuildFor>`   `TEST_ONLY`          

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `                     | `                     | ::: block             |
        | static XCScheme.Build | valueOf​(String name)` | Returns the enum      |
        | ActionEntry.BuildFor` |                       | constant of this type |
        |                       |                       | with the specified    |
        |                       |                       | name.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `st                   | `values()`            | ::: block             |
        | atic XCScheme.BuildAc |                       | Returns an array      |
        | tionEntry.BuildFor[]` |                       | containing the        |
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

        []{#ANALYZING}

        -   #### ANALYZING

                public static final XCScheme.BuildActionEntry.BuildFor ANALYZING

        []{#TESTING}

        -   #### TESTING

                public static final XCScheme.BuildActionEntry.BuildFor TESTING

        []{#RUNNING}

        -   #### RUNNING

                public static final XCScheme.BuildActionEntry.BuildFor RUNNING

        []{#PROFILING}

        -   #### PROFILING

                public static final XCScheme.BuildActionEntry.BuildFor PROFILING

        []{#ARCHIVING}

        -   #### ARCHIVING

                public static final XCScheme.BuildActionEntry.BuildFor ARCHIVING
    :::

    ::: {.section role="region"}
    -   []{#field.detail}

        ### Field Detail

        []{#DEFAULT}

        -   #### DEFAULT

                public static final EnumSet<XCScheme.BuildActionEntry.BuildFor> DEFAULT

        []{#INDEXING_ONLY}

        -   #### INDEXING_ONLY

                public static final EnumSet<XCScheme.BuildActionEntry.BuildFor> INDEXING_ONLY

        []{#SCHEME_LIBRARY}

        -   #### SCHEME_LIBRARY

                public static final EnumSet<XCScheme.BuildActionEntry.BuildFor> SCHEME_LIBRARY

        []{#MAIN_EXECUTABLE}

        -   #### MAIN_EXECUTABLE

                public static final EnumSet<XCScheme.BuildActionEntry.BuildFor> MAIN_EXECUTABLE

        []{#TEST_ONLY}

        -   #### TEST_ONLY

                public static final EnumSet<XCScheme.BuildActionEntry.BuildFor> TEST_ONLY
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#values()}

        -   #### values

            ``` methodSignature
            public static XCScheme.BuildActionEntry.BuildFor[] values()
            ```

            ::: block
            Returns an array containing the constants of this enum type,
            in the order they are declared. This method may be used to
            iterate over the constants as follows:
                for (XCScheme.BuildActionEntry.BuildFor c : XCScheme.BuildActionEntry.BuildFor.values())
                    System.out.println(c);
            :::

            [Returns:]{.returnLabel}
            :   an array containing the constants of this enum type, in
                the order they are declared

        []{#valueOf(java.lang.String)}

        -   #### valueOf

            ``` methodSignature
            public static XCScheme.BuildActionEntry.BuildFor valueOf​(String name)
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
