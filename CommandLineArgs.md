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
-   [Nested](#nested.class.summary) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.core.rules.actions.lib.args](package-summary.html)
:::

## Interface CommandLineArgs {#interface-commandlineargs .title title="Interface CommandLineArgs"}
:::

::: contentContainer
::: description
-   

    All Superinterfaces:
    :   `AddsToRuleKey`, `CommandLineArgsApi`,
        `com.google.devtools.build.lib.skylarkinterface.SkylarkPrintable`,
        `com.google.devtools.build.lib.skylarkinterface.SkylarkValue`

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `ImmutableRunInfo`, `RunInfo`

    ------------------------------------------------------------------------

        public interface CommandLineArgs
        extends AddsToRuleKey, CommandLineArgsApi

    ::: block
    Container for a list of objects that can be stringified into command
    line arguments for an action that executes a program.
    In the future this will also let us more efficiently concatenate
    command line arguments that are passed around as providers, as the
    [`CommandLineArgs`](CommandLineArgs.html "interface in com.facebook.buck.core.rules.actions.lib.args")
    objects may store the immutable objects more efficiently, and just
    construct a stream to interate over those internal collections.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Interface             | Description           |
        +=======================+=======================+=======================+
        | `static interface `   | `CommandLineArg       | ::: block             |
        |                       | s.ArgAndFormatString` | Simple container that |
        |                       |                       | holds a single        |
        |                       |                       | argument, and a       |
        |                       |                       | formatting string     |
        |                       |                       | that should be run    |
        |                       |                       | after                 |
        |                       |                       | [`CommandLineArgs.A   |
        |                       |                       | rgAndFormatString.get |
        |                       |                       | Object()`](CommandLin |
        |                       |                       | eArgs.ArgAndFormatStr |
        |                       |                       | ing.html#getObject()) |
        |                       |                       | has been stringified  |
        |                       |                       | (containing a single  |
        |                       |                       | %s).                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type   Field                     Description
          ------------------- ------------------------- -------------
          `static String`     `DEFAULT_FORMAT_STRING`    

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `java.util.stream.S   | `getAr                |                       |
        | tream<CommandLineArgs | gsAndFormatStrings()` |                       |
        | .ArgAndFormatString>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.common.   | `getEn                |                       |
        | collect.ImmutableSort | vironmentVariables()` |                       |
        | edMap<String,​String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `get                  | ::: block             |
        |                       | EstimatedArgsCount()` | Get the approximate   |
        |                       |                       | number of arguments   |
        |                       |                       | that will be returned |
        |                       |                       | for                   |
        |                       |                       | [`getArgsAndFor       |
        |                       |                       | matStrings()`](#getAr |
        |                       |                       | gsAndFormatStrings()) |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `visitInputsAndOu     | ::: block             |
        |                       | tputs​(java.util.funct | Add any artifacts     |
        |                       | ion.Consumer<Artifact | from                  |
        |                       | > inputs,             | [`getArgsAndFor       |
        |                       |           java.util.f | matStrings()`](#getAr |
        |                       | unction.Consumer<Outp | gsAndFormatStrings()) |
        |                       | utArtifact> outputs)` | to `inputs` and       |
        |                       |                       | `  outputs`,          |
        |                       |                       | inferring based on    |
        |                       |                       | type                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.actions.lib.args.CommandLineArgsApi}

            ### Methods inherited from interface com.facebook.buck.core.rules.actions.lib.args.[CommandLineArgsApi](CommandLineArgsApi.html "interface in com.facebook.buck.core.rules.actions.lib.args")

            `isImmutable, repr`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.google.devtools.build.lib.skylarkinterface.SkylarkPrintable}

            ### Methods inherited from interface com.google.devtools.build.lib.skylarkinterface.SkylarkPrintable

            `debugPrint, str`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.google.devtools.build.lib.skylarkinterface.SkylarkValue}

            ### Methods inherited from interface com.google.devtools.build.lib.skylarkinterface.SkylarkValue

            `isHashable`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#field.detail}

        ### Field Detail

        []{#DEFAULT_FORMAT_STRING}

        -   #### DEFAULT_FORMAT_STRING

                static final String DEFAULT_FORMAT_STRING

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../../../constant-values.html#com.facebook.buck.core.rules.actions.lib.args.CommandLineArgs.DEFAULT_FORMAT_STRING)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getEnvironmentVariables()}

        -   #### getEnvironmentVariables

            ``` methodSignature
            com.google.common.collect.ImmutableSortedMap<String,​String> getEnvironmentVariables()
            ```

            [Returns:]{.returnLabel}
            :   Get a map of all environment variables that need to be
                added to execute this program.

        []{#getArgsAndFormatStrings()}

        -   #### getArgsAndFormatStrings

            ``` methodSignature
            java.util.stream.Stream<CommandLineArgs.ArgAndFormatString> getArgsAndFormatStrings()
            ```

            [Returns:]{.returnLabel}
            :   Get a stream of all raw argument objects that can be
                stringified with something like
                [`CommandLineArgStringifier.asString(ArtifactFilesystem, boolean, Object)`](CommandLineArgStringifier.html#asString(com.facebook.buck.core.artifact.ArtifactFilesystem,boolean,java.lang.Object))

        []{#getEstimatedArgsCount()}

        -   #### getEstimatedArgsCount

            ``` methodSignature
            int getEstimatedArgsCount()
            ```

            ::: block
            Get the approximate number of arguments that will be
            returned for
            [`getArgsAndFormatStrings()`](#getArgsAndFormatStrings())
            This can be handy to pre-size destination collections
            :::

            [Returns:]{.returnLabel}
            :   the approximate number of arguments. If retrieving the
                accurate count is efficient, a correct number is
                preferred. However if getting a correct number is
                impossible or expensive, an approximation is acceptable.

        []{#visitInputsAndOutputs(java.util.function.Consumer,java.util.function.Consumer)}

        -   #### visitInputsAndOutputs

            ``` methodSignature
            void visitInputsAndOutputs​(java.util.function.Consumer<Artifact> inputs,
                                       java.util.function.Consumer<OutputArtifact> outputs)
            ```

            ::: block
            Add any artifacts from
            [`getArgsAndFormatStrings()`](#getArgsAndFormatStrings()) to
            `inputs` and `  outputs`, inferring based on type
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
-   [Nested](#nested.class.summary) \| 
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
