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
[Package]{.packageLabelInType} [com.facebook.buck.support.fix](package-summary.html)
:::

## Enum BuckFixSpecParser.FixSpecFailure {#enum-buckfixspecparser.fixspecfailure .title title="Enum BuckFixSpecParser.FixSpecFailure"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [java.lang.Enum](http://docs.oracle.com/javase/7/docs/api/java/lang/Enum.html?is-external=true "class or interface in java.lang"){.externalLink}\<[BuckFixSpecParser.FixSpecFailure](BuckFixSpecParser.FixSpecFailure.html "enum in com.facebook.buck.support.fix")\>

    -   -   com.facebook.buck.support.fix.BuckFixSpecParser.FixSpecFailure

::: description
-   

    All Implemented Interfaces:
    :   `Serializable`, `Comparable<BuckFixSpecParser.FixSpecFailure>`

    ```{=html}
    <!-- -->
    ```

    Enclosing class:
    :   [BuckFixSpecParser](BuckFixSpecParser.html "class in com.facebook.buck.support.fix")

    ------------------------------------------------------------------------

        public static enum BuckFixSpecParser.FixSpecFailure
        extends Enum<BuckFixSpecParser.FixSpecFailure>

    ::: block
    The various ways that trying to parse a FixSpec can fail
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#enum.constant.summary}

        ### Enum Constant Summary

          Enum Constant                     Description
          --------------------------------- -------------
          `MISSING`                          
          `MISSING_BUILD_ID`                 
          `MISSING_COMMAND_ARGS`             
          `MISSING_EXIT_CODE`                
          `MISSING_EXPANDED_COMMAND_ARGS`    
          `MISSING_FIX_SPEC_FILE_IN_LOGS`    

          : Enum Constants[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `String`              | `                     | ::: block             |
        |                       | humanReadableError()` | Get a human readable  |
        |                       |                       | error message for     |
        |                       |                       | this failure          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static BuckFixSpecP  | `                     | ::: block             |
        | arser.FixSpecFailure` | valueOf​(String name)` | Returns the enum      |
        |                       |                       | constant of this type |
        |                       |                       | with the specified    |
        |                       |                       | name.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `values()`            | ::: block             |
        | static BuckFixSpecPar |                       | Returns an array      |
        | ser.FixSpecFailure[]` |                       | containing the        |
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

        []{#MISSING}

        -   #### MISSING

                public static final BuckFixSpecParser.FixSpecFailure MISSING

        []{#MISSING_BUILD_ID}

        -   #### MISSING_BUILD_ID

                public static final BuckFixSpecParser.FixSpecFailure MISSING_BUILD_ID

        []{#MISSING_EXIT_CODE}

        -   #### MISSING_EXIT_CODE

                public static final BuckFixSpecParser.FixSpecFailure MISSING_EXIT_CODE

        []{#MISSING_COMMAND_ARGS}

        -   #### MISSING_COMMAND_ARGS

                public static final BuckFixSpecParser.FixSpecFailure MISSING_COMMAND_ARGS

        []{#MISSING_EXPANDED_COMMAND_ARGS}

        -   #### MISSING_EXPANDED_COMMAND_ARGS

                public static final BuckFixSpecParser.FixSpecFailure MISSING_EXPANDED_COMMAND_ARGS

        []{#MISSING_FIX_SPEC_FILE_IN_LOGS}

        -   #### MISSING_FIX_SPEC_FILE_IN_LOGS

                public static final BuckFixSpecParser.FixSpecFailure MISSING_FIX_SPEC_FILE_IN_LOGS
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#values()}

        -   #### values

            ``` methodSignature
            public static BuckFixSpecParser.FixSpecFailure[] values()
            ```

            ::: block
            Returns an array containing the constants of this enum type,
            in the order they are declared. This method may be used to
            iterate over the constants as follows:
                for (BuckFixSpecParser.FixSpecFailure c : BuckFixSpecParser.FixSpecFailure.values())
                    System.out.println(c);
            :::

            [Returns:]{.returnLabel}
            :   an array containing the constants of this enum type, in
                the order they are declared

        []{#valueOf(java.lang.String)}

        -   #### valueOf

            ``` methodSignature
            public static BuckFixSpecParser.FixSpecFailure valueOf​(String name)
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

        []{#humanReadableError()}

        -   #### humanReadableError

            ``` methodSignature
            public String humanReadableError()
            ```

            ::: block
            Get a human readable error message for this failure
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
