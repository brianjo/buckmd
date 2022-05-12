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

## Enum AndroidBuckConfig.NdkSearchOrderEntry {#enum-androidbuckconfig.ndksearchorderentry .title title="Enum AndroidBuckConfig.NdkSearchOrderEntry"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [java.lang.Enum](http://docs.oracle.com/javase/7/docs/api/java/lang/Enum.html?is-external=true "class or interface in java.lang"){.externalLink}\<[AndroidBuckConfig.NdkSearchOrderEntry](AndroidBuckConfig.NdkSearchOrderEntry.html "enum in com.facebook.buck.android")\>

    -   -   com.facebook.buck.android.AndroidBuckConfig.NdkSearchOrderEntry

::: description
-   

    All Implemented Interfaces:
    :   `Serializable`,
        `Comparable<AndroidBuckConfig.NdkSearchOrderEntry>`

    ```{=html}
    <!-- -->
    ```

    Enclosing class:
    :   [AndroidBuckConfig](AndroidBuckConfig.html "class in com.facebook.buck.android")

    ------------------------------------------------------------------------

        public static enum AndroidBuckConfig.NdkSearchOrderEntry
        extends Enum<AndroidBuckConfig.NdkSearchOrderEntry>

    ::: block
    Values acceptable for ndk.ndk_search_order.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#enum.constant.summary}

        ### Enum Constant Summary

          Enum Constant                  Description
          ------------------------------ -------------
          `ANDROID_NDK_ENV`               
          `ANDROID_NDK_HOME_ENV`          
          `ANDROID_NDK_REPOSITORY_ENV`    
          `NDK_DIRECTORY_CONFIG`          
          `NDK_HOME_ENV`                  
          `NDK_REPOSITORY_CONFIG`         

          : Enum Constants[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type   Field          Description
          ------------------- -------------- -------------
          `String`            `entryValue`    

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `sta                  | `                     | ::: block             |
        | tic AndroidBuckConfig | valueOf​(String name)` | Returns the enum      |
        | .NdkSearchOrderEntry` |                       | constant of this type |
        |                       |                       | with the specified    |
        |                       |                       | name.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `stati                | `values()`            | ::: block             |
        | c AndroidBuckConfig.N |                       | Returns an array      |
        | dkSearchOrderEntry[]` |                       | containing the        |
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

        []{#ANDROID_NDK_REPOSITORY_ENV}

        -   #### ANDROID_NDK_REPOSITORY_ENV

                public static final AndroidBuckConfig.NdkSearchOrderEntry ANDROID_NDK_REPOSITORY_ENV

        []{#ANDROID_NDK_ENV}

        -   #### ANDROID_NDK_ENV

                public static final AndroidBuckConfig.NdkSearchOrderEntry ANDROID_NDK_ENV

        []{#NDK_HOME_ENV}

        -   #### NDK_HOME_ENV

                public static final AndroidBuckConfig.NdkSearchOrderEntry NDK_HOME_ENV

        []{#ANDROID_NDK_HOME_ENV}

        -   #### ANDROID_NDK_HOME_ENV

                public static final AndroidBuckConfig.NdkSearchOrderEntry ANDROID_NDK_HOME_ENV

        []{#NDK_REPOSITORY_CONFIG}

        -   #### NDK_REPOSITORY_CONFIG

                public static final AndroidBuckConfig.NdkSearchOrderEntry NDK_REPOSITORY_CONFIG

        []{#NDK_DIRECTORY_CONFIG}

        -   #### NDK_DIRECTORY_CONFIG

                public static final AndroidBuckConfig.NdkSearchOrderEntry NDK_DIRECTORY_CONFIG
    :::

    ::: {.section role="region"}
    -   []{#field.detail}

        ### Field Detail

        []{#entryValue}

        -   #### entryValue

                public final String entryValue
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#values()}

        -   #### values

            ``` methodSignature
            public static AndroidBuckConfig.NdkSearchOrderEntry[] values()
            ```

            ::: block
            Returns an array containing the constants of this enum type,
            in the order they are declared. This method may be used to
            iterate over the constants as follows:
                for (AndroidBuckConfig.NdkSearchOrderEntry c : AndroidBuckConfig.NdkSearchOrderEntry.values())
                    System.out.println(c);
            :::

            [Returns:]{.returnLabel}
            :   an array containing the constants of this enum type, in
                the order they are declared

        []{#valueOf(java.lang.String)}

        -   #### valueOf

            ``` methodSignature
            public static AndroidBuckConfig.NdkSearchOrderEntry valueOf​(String name)
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
