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

-   [Overview](../../../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../../index-all.html)
-   [Help](../../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.core.rules.actions.lib.args](package-summary.html)
:::

## Class CommandLineArgsFactory {#class-commandlineargsfactory .title title="Class CommandLineArgsFactory"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.rules.actions.lib.args.CommandLineArgsFactory

::: description
-   

    ------------------------------------------------------------------------

        public class CommandLineArgsFactory
        extends Object

    ::: block
    Factory class that returns more efficient implementations of
    [`CommandLineArgs`](CommandLineArgs.html "interface in com.facebook.buck.core.rules.actions.lib.args")
    depending on what type of arguments are available (e.g. a list of
    args may return a different concrete class than a single arg)
    This should be the public way to construct
    [`CommandLineArgs`](CommandLineArgs.html "interface in com.facebook.buck.core.rules.actions.lib.args")
    objects.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                  Description
          ---------------------------- -------------
          `CommandLineArgsFactory()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `st                   | `from​(com.google.c    | ::: block             |
        | atic CommandLineArgs` | ommon.collect.Immutab | Create a              |
        |                       | leList<Object> args)` | [`CommandLineArgs`    |
        |                       |                       | ](CommandLineArgs.htm |
        |                       |                       | l "interface in com.f |
        |                       |                       | acebook.buck.core.rul |
        |                       |                       | es.actions.lib.args") |
        |                       |                       | instance for a list   |
        |                       |                       | of arguments          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `st                   | `                     | ::: block             |
        | atic CommandLineArgs` | from​(com.google.commo | Create a              |
        |                       | n.collect.ImmutableLi | [`CommandLineArgs`    |
        |                       | st<Object> args,      | ](CommandLineArgs.htm |
        |                       | String formatString)` | l "interface in com.f |
        |                       |                       | acebook.buck.core.rul |
        |                       |                       | es.actions.lib.args") |
        |                       |                       | instance for a list   |
        |                       |                       | of arguments          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static String`       | `                     | ::: block             |
        |                       | validateFormatString​( | Throws an exception   |
        |                       | String formatString)` | if the `formatString` |
        |                       |                       | is not a valid        |
        |                       |                       | stringification       |
        |                       |                       | format string         |
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

        -   #### CommandLineArgsFactory

                public CommandLineArgsFactory()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#validateFormatString(java.lang.String)}

        -   #### validateFormatString

            ``` methodSignature
            public static String validateFormatString​(String formatString)
                                               throws CommandLineArgException
            ```

            ::: block
            Throws an exception if the `formatString` is not a valid
            stringification format string
            :::

            [Throws:]{.throwsLabel}
            :   `CommandLineArgException`

        []{#from(com.google.common.collect.ImmutableList)}

        -   #### from

            ``` methodSignature
            public static CommandLineArgs from​(com.google.common.collect.ImmutableList<Object> args)
                                        throws CommandLineArgException
            ```

            ::: block
            Create a
            [`CommandLineArgs`](CommandLineArgs.html "interface in com.facebook.buck.core.rules.actions.lib.args")
            instance for a list of arguments
            :::

            [Parameters:]{.paramLabel}
            :   `args` - the list of primitive command line args

            [Returns:]{.returnLabel}
            :   A
                [`CommandLineArgs`](CommandLineArgs.html "interface in com.facebook.buck.core.rules.actions.lib.args")
                object for this collection of args

            [Throws:]{.throwsLabel}
            :   `CommandLineArgException` - if `args` contains an arg
                with an invalid type

        []{#from(com.google.common.collect.ImmutableList,java.lang.String)}

        -   #### from

            ``` methodSignature
            public static CommandLineArgs from​(com.google.common.collect.ImmutableList<Object> args,
                                               String formatString)
                                        throws CommandLineArgException
            ```

            ::: block
            Create a
            [`CommandLineArgs`](CommandLineArgs.html "interface in com.facebook.buck.core.rules.actions.lib.args")
            instance for a list of arguments
            :::

            [Parameters:]{.paramLabel}
            :   `args` - the list of primitive command line args
            :   `formatString` - the format string to apply after
                stringifying arguments

            [Returns:]{.returnLabel}
            :   A
                [`CommandLineArgs`](CommandLineArgs.html "interface in com.facebook.buck.core.rules.actions.lib.args")
                object for this collection of args

            [Throws:]{.throwsLabel}
            :   `CommandLineArgException` - if `args` contains an arg
                with an invalid type
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

-   [Overview](../../../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../../index-all.html)
-   [Help](../../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../../allclasses.html)

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
