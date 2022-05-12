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
[Package]{.packageLabelInType} [com.facebook.buck.android](package-summary.html)
:::

## Enum ResourceFilters.Density {#enum-resourcefilters.density .title title="Enum ResourceFilters.Density"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [java.lang.Enum](http://docs.oracle.com/javase/7/docs/api/java/lang/Enum.html?is-external=true "class or interface in java.lang"){.externalLink}\<[ResourceFilters.Density](ResourceFilters.Density.html "enum in com.facebook.buck.android")\>

    -   -   com.facebook.buck.android.ResourceFilters.Density

::: description
-   

    All Implemented Interfaces:
    :   `Serializable`, `Comparable<ResourceFilters.Density>`

    ```{=html}
    <!-- -->
    ```

    Enclosing class:
    :   [ResourceFilters](ResourceFilters.html "class in com.facebook.buck.android")

    ------------------------------------------------------------------------

        public static enum ResourceFilters.Density
        extends Enum<ResourceFilters.Density>

    ::: block
    Represents the names and values of valid densities for resources as
    defined in
    http://developer.android.com/guide/topics/resources/providing-resources.html#DensityQualifier
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#enum.constant.summary}

        ### Enum Constant Summary

          Enum Constant    Description
          ---------------- -------------
          `HDPI`            
          `LDPI`            
          `MDPI`            
          `NO_QUALIFIER`    
          `TVDPI`           
          `XHDPI`           
          `XXHDPI`          
          `XXXHDPI`         

          : Enum Constants[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type                                                      Field        Description
          ---------------------------------------------------------------------- ------------ -------------
          `static com.google.common.collect.Ordering<ResourceFilters.Density>`   `ORDERING`    

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static Res           | `from​(String s)`      |                       |
        | ourceFilters.Density` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static boolean`      | `isDensity​(String s)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `toString()`          |                       |
        +-----------------------+-----------------------+-----------------------+
        | `double`              | `value()`             |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static Res           | `                     | ::: block             |
        | ourceFilters.Density` | valueOf​(String name)` | Returns the enum      |
        |                       |                       | constant of this type |
        |                       |                       | with the specified    |
        |                       |                       | name.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static Resou         | `values()`            | ::: block             |
        | rceFilters.Density[]` |                       | Returns an array      |
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

        []{#LDPI}

        -   #### LDPI

                public static final ResourceFilters.Density LDPI

        []{#NO_QUALIFIER}

        -   #### NO_QUALIFIER

                public static final ResourceFilters.Density NO_QUALIFIER

        []{#MDPI}

        -   #### MDPI

                public static final ResourceFilters.Density MDPI

        []{#TVDPI}

        -   #### TVDPI

                public static final ResourceFilters.Density TVDPI

        []{#HDPI}

        -   #### HDPI

                public static final ResourceFilters.Density HDPI

        []{#XHDPI}

        -   #### XHDPI

                public static final ResourceFilters.Density XHDPI

        []{#XXHDPI}

        -   #### XXHDPI

                public static final ResourceFilters.Density XXHDPI

        []{#XXXHDPI}

        -   #### XXXHDPI

                public static final ResourceFilters.Density XXXHDPI
    :::

    ::: {.section role="region"}
    -   []{#field.detail}

        ### Field Detail

        []{#ORDERING}

        -   #### ORDERING

                public static final com.google.common.collect.Ordering<ResourceFilters.Density> ORDERING
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#values()}

        -   #### values

            ``` methodSignature
            public static ResourceFilters.Density[] values()
            ```

            ::: block
            Returns an array containing the constants of this enum type,
            in the order they are declared. This method may be used to
            iterate over the constants as follows:
                for (ResourceFilters.Density c : ResourceFilters.Density.values())
                    System.out.println(c);
            :::

            [Returns:]{.returnLabel}
            :   an array containing the constants of this enum type, in
                the order they are declared

        []{#valueOf(java.lang.String)}

        -   #### valueOf

            ``` methodSignature
            public static ResourceFilters.Density valueOf​(String name)
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

        []{#value()}

        -   #### value

            ``` methodSignature
            public double value()
            ```

        []{#toString()}

        -   #### toString

            ``` methodSignature
            public String toString()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `toString` in class `Enum<ResourceFilters.Density>`

        []{#from(java.lang.String)}

        -   #### from

            ``` methodSignature
            public static ResourceFilters.Density from​(String s)
            ```

        []{#isDensity(java.lang.String)}

        -   #### isDensity

            ``` methodSignature
            public static boolean isDensity​(String s)
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
