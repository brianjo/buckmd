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
-   Field \| 
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   [Constr](#constructor.detail) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.core.exceptions](package-summary.html)
:::

## Class UserVerify {#class-userverify .title title="Class UserVerify"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.exceptions.UserVerify

::: description
-   

    ------------------------------------------------------------------------

        public class UserVerify
        extends Object

    ::: block
    Provides methods similar to `Verify` but throws
    [`HumanReadableException`](HumanReadableException.html "class in com.facebook.buck.core.exceptions")
    instead. Useful as a lightweight mechanism of verifying
    user-controlled args/state/etc.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor      Description
          ---------------- -------------
          `UserVerify()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static void`         | `checkArgument​(boole  | ::: block             |
        |                       | an argument,          | Verifies that         |
        |                       |      Object message)` | argument is true.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static void`         | `check                | ::: block             |
        |                       | Argument​(boolean argu | Verifies that         |
        |                       | ment,              St | argument is true.     |
        |                       | ring format,          | :::                   |
        |                       |      Object... args)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static void`         | `ve                   | ::: block             |
        |                       | rify​(boolean state,   | Verifies that state   |
        |                       |      Object message)` | is true.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static void`         | `ve                   | ::: block             |
        |                       | rify​(boolean state,   | Verifies that state   |
        |                       |      String format,   | is true.              |
        |                       |      Object... args)` | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static <T> T`        | `verifyNotN           | ::: block             |
        |                       | ull​(T value,          | Verifies that value   |
        |                       |      Object message)` | is not null, returns  |
        |                       |                       | the original object   |
        |                       |                       | if it is not null.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static <T> T`        | `verifyNotNull​(T v    | ::: block             |
        |                       | alue,              St | Verifies that value   |
        |                       | ring format,          | is not null, returns  |
        |                       |      Object... args)` | the original object   |
        |                       |                       | if it is not null     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### UserVerify

                public UserVerify()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#verifyNotNull(java.lang.Object,java.lang.Object)}
        []{#verifyNotNull(T,java.lang.Object)}

        -   #### verifyNotNull

            ``` methodSignature
            public static <T> T verifyNotNull​(@Nullable
                                              T value,
                                              Object message)
            ```

            ::: block
            Verifies that value is not null, returns the original object
            if it is not null.
            :::

        []{#verifyNotNull(java.lang.Object,java.lang.String,java.lang.Object[])}
        []{#verifyNotNull(T,java.lang.String,java.lang.Object...)}

        -   #### verifyNotNull

            ``` methodSignature
            public static <T> T verifyNotNull​(@Nullable
                                              T value,
                                              String format,
                                              Object... args)
            ```

            ::: block
            Verifies that value is not null, returns the original object
            if it is not null
            :::

        []{#verify(boolean,java.lang.Object)}

        -   #### verify

            ``` methodSignature
            public static void verify​(boolean state,
                                      Object message)
            ```

            ::: block
            Verifies that state is true.
            :::

        []{#verify(boolean,java.lang.String,java.lang.Object...)}

        -   #### verify

            ``` methodSignature
            public static void verify​(boolean state,
                                      String format,
                                      Object... args)
            ```

            ::: block
            Verifies that state is true.
            :::

        []{#checkArgument(boolean,java.lang.Object)}

        -   #### checkArgument

            ``` methodSignature
            public static void checkArgument​(boolean argument,
                                             Object message)
            ```

            ::: block
            Verifies that argument is true.
            :::

        []{#checkArgument(boolean,java.lang.String,java.lang.Object...)}

        -   #### checkArgument

            ``` methodSignature
            public static void checkArgument​(boolean argument,
                                             String format,
                                             Object... args)
            ```

            ::: block
            Verifies that argument is true.
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
-   Field \| 
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   [Constr](#constructor.detail) \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
