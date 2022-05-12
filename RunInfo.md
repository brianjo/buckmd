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
-   [Field](#field.detail) \| 
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

## Class RunInfo {#class-runinfo .title title="Class RunInfo"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.core.starlark.compatible.BuckStarlarkStructObject](../../../starlark/compatible/BuckStarlarkStructObject.html "class in com.facebook.buck.core.starlark.compatible")

    -   -   [com.facebook.buck.core.rules.providers.impl.BuiltInProviderInfo](../impl/BuiltInProviderInfo.html "class in com.facebook.buck.core.rules.providers.impl")\<[RunInfo](RunInfo.html "class in com.facebook.buck.core.rules.providers.lib")\>

        -   -   com.facebook.buck.core.rules.providers.lib.RunInfo

::: description
-   

    All Implemented Interfaces:
    :   `AddsToRuleKey`, `CommandLineArgs`, `CommandLineArgsApi`,
        `ProviderInfo<RunInfo>`, `SkylarkProviderInfo`,
        `com.google.devtools.build.lib.skylarkinterface.SkylarkPrintable`,
        `com.google.devtools.build.lib.skylarkinterface.SkylarkValue`,
        `com.google.devtools.build.lib.syntax.ClassObject`

    ```{=html}
    <!-- -->
    ```

    Direct Known Subclasses:
    :   `ImmutableRunInfo`

    ------------------------------------------------------------------------

        public abstract class RunInfo
        extends BuiltInProviderInfo<RunInfo>
        implements CommandLineArgs

    ::: block
    The standard
    [`Provider`](../Provider.html "interface in com.facebook.buck.core.rules.providers")
    that describes how to run a given build rule\'s outputs.
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

          Modifier and Type                   Field        Description
          ----------------------------------- ------------ -------------
          `static BuiltInProvider<RunInfo>`   `PROVIDER`    

          : Fields[ ]{.tabEnd}

        -   []{#fields.inherited.from.class.com.facebook.buck.core.rules.actions.lib.args.CommandLineArgs}

            ### Fields inherited from interface com.facebook.buck.core.rules.actions.lib.args.[CommandLineArgs](../../actions/lib/args/CommandLineArgs.html "interface in com.facebook.buck.core.rules.actions.lib.args")

            `DEFAULT_FORMAT_STRING`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor   Description
          ------------- -------------
          `RunInfo()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `abst                 | `args()`              |                       |
        | ract CommandLineArgs` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `env()`               |                       |
        | abstract com.google.c |                       |                       |
        | ommon.collect.Immutab |                       |                       |
        | leMap<String,​String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
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
        |                       |                       | [`CommandLi           |
        |                       |                       | neArgs.getArgsAndForm |
        |                       |                       | atStrings()`](../../a |
        |                       |                       | ctions/lib/args/Comma |
        |                       |                       | ndLineArgs.html#getAr |
        |                       |                       | gsAndFormatStrings()) |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static RunInfo`      | `i                    | ::: block             |
        |                       | nstantiateFromSkylark | Create an instance of |
        |                       | ​(com.google.devtools. | RunInfo from skylark  |
        |                       | build.lib.syntax.Skyl | arguments.            |
        |                       | arkDict<String,​String | :::                   |
        |                       | > env,                |                       |
        |                       |         Object args)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `visitInputsAndOu     | ::: block             |
        |                       | tputs​(java.util.funct | Add any artifacts     |
        |                       | ion.Consumer<Artifact | from                  |
        |                       | > inputs,             | [`CommandLi           |
        |                       |           java.util.f | neArgs.getArgsAndForm |
        |                       | unction.Consumer<Outp | atStrings()`](../../a |
        |                       | utArtifact> outputs)` | ctions/lib/args/Comma |
        |                       |                       | ndLineArgs.html#getAr |
        |                       |                       | gsAndFormatStrings()) |
        |                       |                       | to `inputs` and       |
        |                       |                       | `  outputs`,          |
        |                       |                       | inferring based on    |
        |                       |                       | type                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

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

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`

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
    -   []{#field.detail}

        ### Field Detail

        []{#PROVIDER}

        -   #### PROVIDER

                public static final BuiltInProvider<RunInfo> PROVIDER
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### RunInfo

                public RunInfo()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#env()}

        -   #### env

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableMap<String,​String> env()
            ```

            [Returns:]{.returnLabel}
            :   any additional environment variables that should be used
                when executing

        []{#args()}

        -   #### args

            ``` methodSignature
            public abstract CommandLineArgs args()
            ```

            [Returns:]{.returnLabel}
            :   the command line arguments to use when executing

        []{#instantiateFromSkylark(com.google.devtools.build.lib.syntax.SkylarkDict,java.lang.Object)}

        -   #### instantiateFromSkylark

            ``` methodSignature
            public static RunInfo instantiateFromSkylark​(com.google.devtools.build.lib.syntax.SkylarkDict<String,​String> env,
                                                         Object args)
                                                  throws com.google.devtools.build.lib.syntax.EvalException
            ```

            ::: block
            Create an instance of RunInfo from skylark arguments.
            :::

            [Parameters:]{.paramLabel}
            :   `env` - environment variables to use when executing
            :   `args` - arguments used to execute this program. Must be
                one of
                [`CommandLineArgsBuilder`](../../../starlark/rule/args/CommandLineArgsBuilder.html "class in com.facebook.buck.core.starlark.rule.args"),
                [`CommandLineArgs`](../../actions/lib/args/CommandLineArgs.html "interface in com.facebook.buck.core.rules.actions.lib.args")
                or `SkylarkList`.

            [Returns:]{.returnLabel}
            :   An instance of
                [`RunInfo`](RunInfo.html "class in com.facebook.buck.core.rules.providers.lib")
                with immutable [`env()`](#env()) and [`args()`](#args())

            [Throws:]{.throwsLabel}
            :   `com.google.devtools.build.lib.syntax.EvalException` -
                the type passed in was incorrect

        []{#getEnvironmentVariables()}

        -   #### getEnvironmentVariables

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedMap<String,​String> getEnvironmentVariables()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getEnvironmentVariables` in interface `CommandLineArgs`

            [Returns:]{.returnLabel}
            :   Get a map of all environment variables that need to be
                added to execute this program.

        []{#getArgsAndFormatStrings()}

        -   #### getArgsAndFormatStrings

            ``` methodSignature
            public java.util.stream.Stream<CommandLineArgs.ArgAndFormatString> getArgsAndFormatStrings()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getArgsAndFormatStrings` in interface `CommandLineArgs`

            [Returns:]{.returnLabel}
            :   Get a stream of all raw argument objects that can be
                stringified with something like
                [`CommandLineArgStringifier.asString(ArtifactFilesystem, boolean, Object)`](../../actions/lib/args/CommandLineArgStringifier.html#asString(com.facebook.buck.core.artifact.ArtifactFilesystem,boolean,java.lang.Object))

        []{#getEstimatedArgsCount()}

        -   #### getEstimatedArgsCount

            ``` methodSignature
            public int getEstimatedArgsCount()
            ```

            ::: block
            [Description copied from
            interface: `CommandLineArgs`]{.descfrmTypeLabel}
            :::

            ::: block
            Get the approximate number of arguments that will be
            returned for
            [`CommandLineArgs.getArgsAndFormatStrings()`](../../actions/lib/args/CommandLineArgs.html#getArgsAndFormatStrings())
            This can be handy to pre-size destination collections
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getEstimatedArgsCount` in interface `CommandLineArgs`

            [Returns:]{.returnLabel}
            :   the approximate number of arguments. If retrieving the
                accurate count is efficient, a correct number is
                preferred. However if getting a correct number is
                impossible or expensive, an approximation is acceptable.

        []{#visitInputsAndOutputs(java.util.function.Consumer,java.util.function.Consumer)}

        -   #### visitInputsAndOutputs

            ``` methodSignature
            public void visitInputsAndOutputs​(java.util.function.Consumer<Artifact> inputs,
                                              java.util.function.Consumer<OutputArtifact> outputs)
            ```

            ::: block
            [Description copied from
            interface: `CommandLineArgs`]{.descfrmTypeLabel}
            :::

            ::: block
            Add any artifacts from
            [`CommandLineArgs.getArgsAndFormatStrings()`](../../actions/lib/args/CommandLineArgs.html#getArgsAndFormatStrings())
            to `inputs` and `  outputs`, inferring based on type
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `visitInputsAndOutputs` in interface `CommandLineArgs`
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
-   [Field](#field.detail) \| 
-   [Constr](#constructor.detail) \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
