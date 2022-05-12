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
-   Field \| 
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.support.cli.args](package-summary.html)
:::

## Class BuckArgsMethods {#class-buckargsmethods .title title="Class BuckArgsMethods"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.support.cli.args.BuckArgsMethods

::: description
-   

    ------------------------------------------------------------------------

        public class BuckArgsMethods
        extends Object

    ::: block
    Utility class for methods related to args handling.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static com.go        | `expandAtFiles​(I      | ::: block             |
        | ogle.common.collect.I | terable<String> args, | Expand AT-file syntax |
        | mmutableList<String>` |               com.goo | in a way that matches |
        |                       | gle.common.collect.Im | what args4j does.     |
        |                       | mutableMap<CellName,​A | :::                   |
        |                       | bsPath> cellMapping)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static com.go        | `filterArgs​(List<St   | ::: block             |
        | ogle.common.collect.I | ring> args,           | Drops options from    |
        | mmutableList<String>` |  com.google.common.co | the args array.       |
        |                       | llect.ImmutableSet<St | :::                   |
        |                       | ring> optionsToSkip)` |                       |
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
    -   []{#method.detail}

        ### Method Detail

        []{#expandAtFiles(java.lang.Iterable,com.google.common.collect.ImmutableMap)}

        -   #### expandAtFiles

            ``` methodSignature
            public static com.google.common.collect.ImmutableList<String> expandAtFiles​(Iterable<String> args,
                                                                                        com.google.common.collect.ImmutableMap<CellName,​AbsPath> cellMapping)
            ```

            ::: block
            Expand AT-file syntax in a way that matches what args4j
            does. We have this because we\'d like to correctly log the
            arguments coming from the AT-files and there is no way to
            get the expanded args array from args4j.
            In addition to files passed using a regular `@` syntax, this
            method also extracts command line arguments from AT-file
            syntax files passed via `--flagfile` command line option.
            :::

            [Parameters:]{.paramLabel}
            :   `args` - original args array
            :   `cellMapping` - a map from cell names to their roots

            [Returns:]{.returnLabel}
            :   args array with AT-files expanded.

        []{#filterArgs(java.util.List,com.google.common.collect.ImmutableSet)}

        -   #### filterArgs

            ``` methodSignature
            public static com.google.common.collect.ImmutableList<String> filterArgs​(List<String> args,
                                                                                     com.google.common.collect.ImmutableSet<String> optionsToSkip)
            ```

            ::: block
            Drops options from the args array.
            :::

            [Parameters:]{.paramLabel}
            :   `args` - args array.
            :   `optionsToSkip` - if args contains an element from this
                array skip the element and the element immediately after
                it.

            [Returns:]{.returnLabel}
            :   filtered args array
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
-   Field \| 
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   Constr \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
