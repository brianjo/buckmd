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
[Package]{.packageLabelInType} [com.facebook.buck.core.macros](package-summary.html)
:::

## Class MacroFinder {#class-macrofinder .title title="Class MacroFinder"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.macros.MacroFinder

::: description
-   

    ------------------------------------------------------------------------

        public final class MacroFinder
        extends Object

    ::: block
    Replace and extracts macros from input strings.
    Examples: \$(exe //foo:bar) \$(location :bar) \$(platform)
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `st                   | `findAll​(com.google.c |                       |
        | atic com.google.commo | ommon.collect.Immutab |                       |
        | n.collect.ImmutableLi | leSet<String> macros, |                       |
        | st<MacroMatchResult>` |         String blob)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static Option        | `match​(com.google     |                       |
        | al<MacroMatchResult>` | .common.collect.Immut |                       |
        |                       | ableSet<String> macro |                       |
        |                       | s,      String blob)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static <T> T`        | `r                    | ::: block             |
        |                       | eplace​(com.google.com | Expand macros         |
        |                       | mon.collect.Immutable | embedded in a string. |
        |                       | Map<String,​MacroRepla | :::                   |
        |                       | cer<T>> replacers,    |                       |
        |                       |      String blob,     |                       |
        |                       |     boolean resolveEs |                       |
        |                       | caping,        MacroC |                       |
        |                       | ombiner<T> combiner)` |                       |
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

        []{#match(com.google.common.collect.ImmutableSet,java.lang.String)}

        -   #### match

            ``` methodSignature
            public static Optional<MacroMatchResult> match​(com.google.common.collect.ImmutableSet<String> macros,
                                                           String blob)
                                                    throws MacroException
            ```

            [Throws:]{.throwsLabel}
            :   `MacroException`

        []{#replace(com.google.common.collect.ImmutableMap,java.lang.String,boolean,com.facebook.buck.core.macros.MacroCombiner)}

        -   #### replace

            ``` methodSignature
            public static <T> T replace​(com.google.common.collect.ImmutableMap<String,​MacroReplacer<T>> replacers,
                                        String blob,
                                        boolean resolveEscaping,
                                        MacroCombiner<T> combiner)
                                 throws MacroException
            ```

            ::: block
            Expand macros embedded in a string.
            :::

            [Parameters:]{.paramLabel}
            :   `replacers` - a map of macro names to
                [`MacroReplacer`](MacroReplacer.html "interface in com.facebook.buck.core.macros")
                objects used to expand them.
            :   `blob` - the input string containing macros to be
                expanded
            :   `resolveEscaping` - whether to drop characters used to
                escape literal uses of \`\$(\...)\`

            [Returns:]{.returnLabel}
            :   a copy of the input string with all macros expanded

            [Throws:]{.throwsLabel}
            :   `MacroException`

        []{#findAll(com.google.common.collect.ImmutableSet,java.lang.String)}

        -   #### findAll

            ``` methodSignature
            public static com.google.common.collect.ImmutableList<MacroMatchResult> findAll​(com.google.common.collect.ImmutableSet<String> macros,
                                                                                            String blob)
                                                                                     throws MacroException
            ```

            [Throws:]{.throwsLabel}
            :   `MacroException`
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
