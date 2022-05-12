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
[Package]{.packageLabelInType} [com.facebook.buck.android.device](package-summary.html)
:::

## Enum TargetDevice.Type {#enum-targetdevice.type .title title="Enum TargetDevice.Type"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [java.lang.Enum](http://docs.oracle.com/javase/7/docs/api/java/lang/Enum.html?is-external=true "class or interface in java.lang"){.externalLink}\<[TargetDevice.Type](TargetDevice.Type.html "enum in com.facebook.buck.android.device")\>

    -   -   com.facebook.buck.android.device.TargetDevice.Type

::: description
-   

    All Implemented Interfaces:
    :   `Serializable`, `Comparable<TargetDevice.Type>`

    ```{=html}
    <!-- -->
    ```

    Enclosing class:
    :   [TargetDevice](TargetDevice.html "class in com.facebook.buck.android.device")

    ------------------------------------------------------------------------

        public static enum TargetDevice.Type
        extends Enum<TargetDevice.Type>
:::

::: summary
-   ::: {.section role="region"}
    -   []{#enum.constant.summary}

        ### Enum Constant Summary

          Enum Constant   Description
          --------------- -------------
          `BY_SERIAL`      
          `EMULATOR`       
          `REAL_DEVICE`    

          : Enum Constants[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `stat                 | `                     | ::: block             |
        | ic TargetDevice.Type` | valueOf​(String name)` | Returns the enum      |
        |                       |                       | constant of this type |
        |                       |                       | with the specified    |
        |                       |                       | name.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static               | `values()`            | ::: block             |
        |  TargetDevice.Type[]` |                       | Returns an array      |
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

        []{#REAL_DEVICE}

        -   #### REAL_DEVICE

                public static final TargetDevice.Type REAL_DEVICE

        []{#EMULATOR}

        -   #### EMULATOR

                public static final TargetDevice.Type EMULATOR

        []{#BY_SERIAL}

        -   #### BY_SERIAL

                public static final TargetDevice.Type BY_SERIAL
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#values()}

        -   #### values

            ``` methodSignature
            public static TargetDevice.Type[] values()
            ```

            ::: block
            Returns an array containing the constants of this enum type,
            in the order they are declared. This method may be used to
            iterate over the constants as follows:
                for (TargetDevice.Type c : TargetDevice.Type.values())
                    System.out.println(c);
            :::

            [Returns:]{.returnLabel}
            :   an array containing the constants of this enum type, in
                the order they are declared

        []{#valueOf(java.lang.String)}

        -   #### valueOf

            ``` methodSignature
            public static TargetDevice.Type valueOf​(String name)
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
