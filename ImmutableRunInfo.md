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

-   [Overview](../../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../index-all.html)
-   [Help](../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.core.rules.providers.lib](package-summary.html)
:::

## Class ImmutableRunInfo {#class-immutableruninfo .title title="Class ImmutableRunInfo"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.core.starlark.compatible.BuckStarlarkStructObject](../../../starlark/compatible/BuckStarlarkStructObject.html "class in com.facebook.buck.core.starlark.compatible")

    -   -   [com.facebook.buck.core.rules.providers.impl.BuiltInProviderInfo](../impl/BuiltInProviderInfo.html "class in com.facebook.buck.core.rules.providers.impl")\<[RunInfo](RunInfo.html "class in com.facebook.buck.core.rules.providers.lib")\>

        -   -   [com.facebook.buck.core.rules.providers.lib.RunInfo](RunInfo.html "class in com.facebook.buck.core.rules.providers.lib")

            -   -   com.facebook.buck.core.rules.providers.lib.ImmutableRunInfo

::: description
-   

    All Implemented Interfaces:
    :   `AddsToRuleKey`, `CommandLineArgs`, `CommandLineArgsApi`,
        `ProviderInfo<RunInfo>`, `SkylarkProviderInfo`,
        `com.google.devtools.build.lib.skylarkinterface.SkylarkPrintable`,
        `com.google.devtools.build.lib.skylarkinterface.SkylarkValue`,
        `com.google.devtools.build.lib.syntax.ClassObject`

    ------------------------------------------------------------------------

        @ParametersAreNonnullByDefault
        @Generated("org.immutables.processor.ProxyProcessor")
        @Immutable
        @CheckReturnValue
        public final class ImmutableRunInfo
        extends RunInfo

    ::: block
    Immutable implementation of
    [`RunInfo`](RunInfo.html "class in com.facebook.buck.core.rules.providers.lib").
    Use the static factory method to create immutable instances:
    `new ImmutableRunInfo()`.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        -   []{#nested.classes.inherited.from.class.com.facebook.buck.core.rules.actions.lib.args.CommandLineArgs}

            ### Nested classes/interfaces inherited from interface com.facebook.buck.core.rules.actions.lib.args.[CommandLineArgs](../../actions/lib/args/CommandLineArgs.html "interface in com.facebook.buck.core.rules.actions.lib.args")

            `CommandLineArgs.ArgAndFormatString`
    :::

    ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        -   []{#fields.inherited.from.class.com.facebook.buck.core.rules.providers.lib.RunInfo}

            ### Fields inherited from class com.facebook.buck.core.rules.providers.lib.[RunInfo](RunInfo.html "class in com.facebook.buck.core.rules.providers.lib")

            `PROVIDER`

        ```{=html}
        <!-- -->
        ```
        -   []{#fields.inherited.from.class.com.facebook.buck.core.rules.actions.lib.args.CommandLineArgs}

            ### Fields inherited from interface com.facebook.buck.core.rules.actions.lib.args.[CommandLineArgs](../../actions/lib/args/CommandLineArgs.html "interface in com.facebook.buck.core.rules.actions.lib.args")

            `DEFAULT_FORMAT_STRING`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

        +-----------------------------------+-----------------------------------+
        | Constructor                       | Description                       |
        +===================================+===================================+
        | `ImmutableRunInfo​(Map<St          | ::: block                         |
        | ring,​? extends String> env,       | Construct a new immutable         |
        |            CommandLineArgs args)` | `RunInfo` instance.               |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+

        : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `CommandLineArgs`     | `args()`              |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.c         | `env()`               |                       |
        | ommon.collect.Immutab |                       |                       |
        | leMap<String,​String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `eq                   | ::: block             |
        |                       | uals​(Object another)` | This instance is      |
        |                       |                       | equal to all          |
        |                       |                       | instances of          |
        |                       |                       | `ImmutableRunInfo`    |
        |                       |                       | that have equal       |
        |                       |                       | attribute values.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `hashCode()`          | ::: block             |
        |                       |                       | Computes a hash code  |
        |                       |                       | from attributes:      |
        |                       |                       | `env`, `args`.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `toString()`          | ::: block             |
        |                       |                       | Prints the immutable  |
        |                       |                       | value `RunInfo` with  |
        |                       |                       | attribute values.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.providers.lib.RunInfo}

            ### Methods inherited from class com.facebook.buck.core.rules.providers.lib.[RunInfo](RunInfo.html "class in com.facebook.buck.core.rules.providers.lib")

            `getArgsAndFormatStrings, getEnvironmentVariables, getEstimatedArgsCount, instantiateFromSkylark, visitInputsAndOutputs`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.providers.impl.BuiltInProviderInfo}

            ### Methods inherited from class com.facebook.buck.core.rules.providers.impl.[BuiltInProviderInfo](../impl/BuiltInProviderInfo.html "class in com.facebook.buck.core.rules.providers.impl")

            `getDeclaredClass, getProvider, getProviderInfo, isImmutable`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.starlark.compatible.BuckStarlarkStructObject}

            ### Methods inherited from class com.facebook.buck.core.starlark.compatible.[BuckStarlarkStructObject](../../../starlark/compatible/BuckStarlarkStructObject.html "class in com.facebook.buck.core.starlark.compatible")

            `getErrorMessageForUnknownField, getFieldNames, getMethods, getValue, repr`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, finalize, getClass, notify, notifyAll, wait, wait, wait`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.actions.lib.args.CommandLineArgsApi}

            ### Methods inherited from interface com.facebook.buck.core.rules.actions.lib.args.[CommandLineArgsApi](../../actions/lib/args/CommandLineArgsApi.html "interface in com.facebook.buck.core.rules.actions.lib.args")

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
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(java.util.Map,com.facebook.buck.core.rules.actions.lib.args.CommandLineArgs)}

        -   #### ImmutableRunInfo

                public ImmutableRunInfo​(Map<String,​? extends String> env,
                                        CommandLineArgs args)

            ::: block
            Construct a new immutable `RunInfo` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `env` - The value for the `env` attribute
            :   `args` - The value for the `args` attribute
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#env()}

        -   #### env

            ``` methodSignature
            public com.google.common.collect.ImmutableMap<String,​String> env()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `env` in class `RunInfo`

            [Returns:]{.returnLabel}
            :   any additional environment variables that should be used
                when executing

        []{#args()}

        -   #### args

            ``` methodSignature
            public CommandLineArgs args()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `args` in class `RunInfo`

            [Returns:]{.returnLabel}
            :   the command line arguments to use when executing

        []{#equals(java.lang.Object)}

        -   #### equals

            ``` methodSignature
            public boolean equals​(@Nullable
                                  Object another)
            ```

            ::: block
            This instance is equal to all instances of
            `ImmutableRunInfo` that have equal attribute values.
            :::

            [Overrides:]{.overrideSpecifyLabel}
            :   `equals` in class `Object`

            [Returns:]{.returnLabel}
            :   `true` if `this` is equal to `another` instance

        []{#hashCode()}

        -   #### hashCode

            ``` methodSignature
            public int hashCode()
            ```

            ::: block
            Computes a hash code from attributes: `env`, `args`.
            :::

            [Overrides:]{.overrideSpecifyLabel}
            :   `hashCode` in class `Object`

            [Returns:]{.returnLabel}
            :   hashCode value

        []{#toString()}

        -   #### toString

            ``` methodSignature
            public String toString()
            ```

            ::: block
            Prints the immutable value `RunInfo` with attribute values.
            :::

            [Overrides:]{.overrideSpecifyLabel}
            :   `toString` in class `Object`

            [Returns:]{.returnLabel}
            :   A string representation of the value
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

-   [Overview](../../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../index-all.html)
-   [Help](../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../allclasses.html)

<div>

<div>

JavaScript is disabled on your browser.

</div>

</div>

<div>

-   Summary: 
-   [Nested](#nested.class.summary) \| 
-   [Field](#field.summary) \| 
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
