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

## Interface Arg {#interface-arg .title title="Interface Arg"}
:::

::: contentContainer
::: description
-   

    All Superinterfaces:
    :   `AddsToRuleKey`

    ```{=html}
    <!-- -->
    ```

    All Known Subinterfaces:
    :   `ToolArg`

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `CompositeArg`, `CxxThinLTOIndexArg`,
        `FileListableLinkerInputArg`, `FormatArg`, `ProxyArg`,
        `RelativeLinkArg`, `RustLibraryArg`, `SanitizedArg`,
        `SourcePathArg`, `StringArg`, `WorkerMacroArg`, `WriteToFileArg`

    ------------------------------------------------------------------------

        public interface Arg
        extends AddsToRuleKey

    ::: block
    An abstraction for modeling the arguments that contribute to a
    command run by a
    [`BuildRule`](../../core/rules/BuildRule.html "interface in com.facebook.buck.core.rules"),
    and also carry information for computing a rule key.
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
        | `boolean`             | `                     |                       |
        |                       | equals​(Object other)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `sta                  | `flattenToSpac        |                       |
        | tic Optional<String>` | eSeparatedString​(Opti |                       |
        |                       | onal<Arg> arg,        |                       |
        |                       |                       |                       |
        |                       |   SourcePathResolverA |                       |
        |                       | dapter pathResolver)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `hashCode()`          |                       |
        +-----------------------+-----------------------+-----------------------+
        | `default String`      | `singl                | ::: block             |
        |                       | eCommandLineArg​(Sourc | Resolve this argument |
        |                       | ePathResolverAdapter  | to single string,     |
        |                       | pathResolverAdapter)` | fail if this arg      |
        |                       |                       | corresponds to none   |
        |                       |                       | or more than one      |
        |                       |                       | argument.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static String`       | `strin                | ::: block             |
        |                       | gify​(Arg arg,         | Converts an Arg to a  |
        |                       |   SourcePathResolverA | String by concatting  |
        |                       | dapter pathResolver)` | all the command-line  |
        |                       |                       | appended strings.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static <K> com.goo   | `stringify​(com.goog   |                       |
        | gle.common.collect.Im | le.common.collect.Imm |                       |
        | mutableMap<K,​String>` | utableMap<K,​? extends |                       |
        |                       |  Arg> argMap,         |                       |
        |                       |   SourcePathResolverA |                       |
        |                       | dapter pathResolver)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static com.go        | `strin                |                       |
        | ogle.common.collect.I | gify​(Iterable<? exten |                       |
        | mmutableList<String>` | ds Arg> args,         |                       |
        |                       |   SourcePathResolverA |                       |
        |                       | dapter pathResolver)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static com.go        | `stringifyList​(A      |                       |
        | ogle.common.collect.I | rg input,             |                       |
        | mmutableList<String>` |   SourcePathResolverA |                       |
        |                       | dapter pathResolver)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `toString()`          |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
        .tableTab}[[Default
        Methods](javascript:show(16);)[ ]{.tabEnd}]{#t5 .tableTab}
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#flattenToSpaceSeparatedString(java.util.Optional,com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter)}

        -   #### flattenToSpaceSeparatedString

            ``` methodSignature
            static Optional<String> flattenToSpaceSeparatedString​(Optional<Arg> arg,
                                                                  SourcePathResolverAdapter pathResolver)
            ```

        []{#appendToCommandLine(java.util.function.Consumer,com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter)}

        -   #### appendToCommandLine

            ``` methodSignature
            void appendToCommandLine​(java.util.function.Consumer<String> consumer,
                                     SourcePathResolverAdapter pathResolver)
            ```

            ::: block
            Feed the contents of the Arg to the supplied consumer. This
            call may feed any number of elements (including zero) into
            the consumer. This is only ever safe to call when the rule
            is running, as it may do things like resolving source paths.
            :::

        []{#singleCommandLineArg(com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter)}

        -   #### singleCommandLineArg

            ``` methodSignature
            default String singleCommandLineArg​(SourcePathResolverAdapter pathResolverAdapter)
            ```

            ::: block
            Resolve this argument to single string, fail if this arg
            corresponds to none or more than one argument.
            :::

        []{#toString()}

        -   #### toString

            ``` methodSignature
            String toString()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `toString` in class `Object`

            [Returns:]{.returnLabel}
            :   a
                [`String`](http://docs.oracle.com/javase/7/docs/api/java/lang/String.html?is-external=true "class or interface in java.lang"){.externalLink}
                representation suitable to use for debugging.

        []{#equals(java.lang.Object)}

        -   #### equals

            ``` methodSignature
            boolean equals​(Object other)
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `equals` in class `Object`

        []{#hashCode()}

        -   #### hashCode

            ``` methodSignature
            int hashCode()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `hashCode` in class `Object`

        []{#stringifyList(com.facebook.buck.rules.args.Arg,com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter)}

        -   #### stringifyList

            ``` methodSignature
            static com.google.common.collect.ImmutableList<String> stringifyList​(Arg input,
                                                                                 SourcePathResolverAdapter pathResolver)
            ```

        []{#stringify(java.lang.Iterable,com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter)}

        -   #### stringify

            ``` methodSignature
            static com.google.common.collect.ImmutableList<String> stringify​(Iterable<? extends Arg> args,
                                                                             SourcePathResolverAdapter pathResolver)
            ```

        []{#stringify(com.facebook.buck.rules.args.Arg,com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter)}

        -   #### stringify

            ``` methodSignature
            static String stringify​(Arg arg,
                                    SourcePathResolverAdapter pathResolver)
            ```

            ::: block
            Converts an Arg to a String by concatting all the
            command-line appended strings.
            :::

        []{#stringify(com.google.common.collect.ImmutableMap,com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter)}

        -   #### stringify

            ``` methodSignature
            static <K> com.google.common.collect.ImmutableMap<K,​String> stringify​(com.google.common.collect.ImmutableMap<K,​? extends Arg> argMap,
                                                                                        SourcePathResolverAdapter pathResolver)
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
