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
[Package]{.packageLabelInType} [com.facebook.buck.rules.args](package-summary.html)
:::

## Class SanitizedArg {#class-sanitizedarg .title title="Class SanitizedArg"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.rules.args.SanitizedArg

::: description
-   

    All Implemented Interfaces:
    :   `AddsToRuleKey`, `Arg`

    ------------------------------------------------------------------------

        public class SanitizedArg
        extends Object
        implements Arg

    ::: block
    An [`Arg`](Arg.html "interface in com.facebook.buck.rules.args")
    which must be sanitized before contributing to a
    [`RuleKey`](../../core/rulekey/RuleKey.html "class in com.facebook.buck.core.rulekey").
         ImmutableMap<String, String> toolchainRoots =
             ImmutableMap.of("/opt/toolchain", "$TOOLCHAIN_ROOT");
         Path toolchainRoot = Paths.get("/opt/toolchain");
         Arg arg =
             new SanitizedArg(
                 Functions.forMap(toolchainRoots),
                 "/opt/toolchain/bin/tool");
         
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `void`                | `appendToCommandLine​( | ::: block             |
        |                       | java.util.function.Co | Feed the contents of  |
        |                       | nsumer<String> consum | the Arg to the        |
        |                       | er,                   | supplied consumer.    |
        |                       |   SourcePathResolverA | :::                   |
        |                       | dapter pathResolver)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static SanitizedArg` | `create​(java          | ::: block             |
        |                       | .util.function.Functi | Create a SanitizedArg |
        |                       | on<? super String,​Str | by applying the given |
        |                       | ing> sanitizer,       | sanitizer function to |
        |                       |  String unsanitized)` | an arg string.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `equals​(Object o)`    |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static com           | `from​(java.           | ::: block             |
        | .google.common.collec | util.function.Functio | Create a list of      |
        | t.ImmutableList<Arg>` | n<? super String,​Stri | SanitizedArgs by      |
        |                       | ng> sanitizer,     It | applying the given    |
        |                       | erable<String> args)` | sanitizer function to |
        |                       |                       | a list of arg strings |
        |                       |                       | and filtering empty   |
        |                       |                       | args                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static com           | `fromArgs​(java.u      | ::: block             |
        | .google.common.collec | til.function.Function | Create a list of      |
        | t.ImmutableList<Arg>` | <? super String,​Strin | SanitizedArg from     |
        |                       | g> sanitizer,         | list of Arg by        |
        |                       |  Iterable<Arg> args)` | applying the given    |
        |                       |                       | sanitizer StringArg   |
        |                       |                       | and filtering empty   |
        |                       |                       | StringArg.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `hashCode()`          |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `toString()`          |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, finalize, getClass, notify, notifyAll, wait, wait, wait`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.rules.args.Arg}

            ### Methods inherited from interface com.facebook.buck.rules.args.[Arg](Arg.html "interface in com.facebook.buck.rules.args")

            `singleCommandLineArg`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#appendToCommandLine(java.util.function.Consumer,com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter)}

        -   #### appendToCommandLine

            ``` methodSignature
            public void appendToCommandLine​(java.util.function.Consumer<String> consumer,
                                            SourcePathResolverAdapter pathResolver)
            ```

            ::: block
            [Description copied from
            interface: `Arg`]{.descfrmTypeLabel}
            :::

            ::: block
            Feed the contents of the Arg to the supplied consumer. This
            call may feed any number of elements (including zero) into
            the consumer. This is only ever safe to call when the rule
            is running, as it may do things like resolving source paths.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `appendToCommandLine` in interface `Arg`

        []{#toString()}

        -   #### toString

            ``` methodSignature
            public String toString()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `toString` in interface `Arg`

            [Overrides:]{.overrideSpecifyLabel}
            :   `toString` in class `Object`

            [Returns:]{.returnLabel}
            :   a
                [`String`](http://docs.oracle.com/javase/7/docs/api/java/lang/String.html?is-external=true "class or interface in java.lang"){.externalLink}
                representation suitable to use for debugging.

        []{#equals(java.lang.Object)}

        -   #### equals

            ``` methodSignature
            public boolean equals​(Object o)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `equals` in interface `Arg`

            [Overrides:]{.overrideSpecifyLabel}
            :   `equals` in class `Object`

        []{#hashCode()}

        -   #### hashCode

            ``` methodSignature
            public int hashCode()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `hashCode` in interface `Arg`

            [Overrides:]{.overrideSpecifyLabel}
            :   `hashCode` in class `Object`

        []{#create(java.util.function.Function,java.lang.String)}

        -   #### create

            ``` methodSignature
            public static SanitizedArg create​(java.util.function.Function<? super String,​String> sanitizer,
                                              String unsanitized)
            ```

            ::: block
            Create a SanitizedArg by applying the given sanitizer
            function to an arg string.
            :::

        []{#from(java.util.function.Function,java.lang.Iterable)}

        -   #### from

            ``` methodSignature
            public static com.google.common.collect.ImmutableList<Arg> from​(java.util.function.Function<? super String,​String> sanitizer,
                                                                            Iterable<String> args)
            ```

            ::: block
            Create a list of SanitizedArgs by applying the given
            sanitizer function to a list of arg strings and filtering
            empty args
            :::

        []{#fromArgs(java.util.function.Function,java.lang.Iterable)}

        -   #### fromArgs

            ``` methodSignature
            public static com.google.common.collect.ImmutableList<Arg> fromArgs​(java.util.function.Function<? super String,​String> sanitizer,
                                                                                Iterable<Arg> args)
            ```

            ::: block
            Create a list of SanitizedArg from list of Arg by applying
            the given sanitizer StringArg and filtering empty StringArg.
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
