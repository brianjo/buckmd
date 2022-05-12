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
-   [Field](#field.summary) \| 
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
-   Constr \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.util](package-summary.html)
:::

## Class AnsiEnvironmentChecking {#class-ansienvironmentchecking .title title="Class AnsiEnvironmentChecking"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.util.AnsiEnvironmentChecking

::: description
-   

    ------------------------------------------------------------------------

        public class AnsiEnvironmentChecking
        extends Object

    ::: block
    Utility class to check if the environment supports ANSI escape
    sequences.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type   Field                        Description
          ------------------- ---------------------------- -------------
          `static String`     `NAILGUN_STDERR_ISTTY_ENV`    
          `static String`     `NAILGUN_STDOUT_ISTTY_ENV`    

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static boolean`      | `environ              | ::: block             |
        |                       | mentSupportsAnsiEscap | Returns true if the   |
        |                       | es​(Platform platform, | environment supports  |
        |                       |                       | ANSI escape           |
        |                       |           Map<String, | sequences, false      |
        |                       | ​String> environment)` | otherwise.            |
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
    -   []{#field.detail}

        ### Field Detail

        []{#NAILGUN_STDOUT_ISTTY_ENV}

        -   #### NAILGUN_STDOUT_ISTTY_ENV

                public static final String NAILGUN_STDOUT_ISTTY_ENV

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../constant-values.html#com.facebook.buck.util.AnsiEnvironmentChecking.NAILGUN_STDOUT_ISTTY_ENV)

        []{#NAILGUN_STDERR_ISTTY_ENV}

        -   #### NAILGUN_STDERR_ISTTY_ENV

                public static final String NAILGUN_STDERR_ISTTY_ENV

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../constant-values.html#com.facebook.buck.util.AnsiEnvironmentChecking.NAILGUN_STDERR_ISTTY_ENV)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#environmentSupportsAnsiEscapes(com.facebook.buck.util.environment.Platform,java.util.Map)}

        -   #### environmentSupportsAnsiEscapes

            ``` methodSignature
            public static boolean environmentSupportsAnsiEscapes​(Platform platform,
                                                                 Map<String,​String> environment)
            ```

            ::: block
            Returns true if the environment supports ANSI escape
            sequences, false otherwise.
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
-   [Field](#field.summary) \| 
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
-   Constr \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
