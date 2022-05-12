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
[Package]{.packageLabelInType} [com.facebook.buck.support.fix](package-summary.html)
:::

## Class FixBuckConfig {#class-fixbuckconfig .title title="Class FixBuckConfig"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.support.fix.FixBuckConfig

::: description
-   

    All Implemented Interfaces:
    :   `ConfigView<BuckConfig>`

    ------------------------------------------------------------------------

        public abstract class FixBuckConfig
        extends Object
        implements ConfigView<BuckConfig>

    ::: block
    Configuration that handles how \`buck fix\` and automatic
    invocations of fix scripts work
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor         Description
          ------------------- -------------
          `FixBuckConfig()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `List<String>`        | `                     | ::: block             |
        |                       | getAutofixCommands()` | List of commands that |
        |                       |                       | autofix is enabled    |
        |                       |                       | for                   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.facebook.buck    | `getAutofixEnabled()` | ::: block             |
        | .support.fix.FixBuckC |                       | When running \`buck   |
        | onfig.AutofixEnabled` |                       | fix\` automatically   |
        |                       |                       | on command failure is |
        |                       |                       | enabled               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.          | `getB                 | ::: block             |
        | common.collect.Immuta | uckProvidedScripts()` | Get a mapping of      |
        | bleMap<String,​com.goo |                       | short names to Paths  |
        | gle.common.collect.Im |                       | for buck provided fix |
        | mutableList<String>>` |                       | scripts               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `abstract BuckConfig` | `getDelegate()`       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<com.goo     | `getFixScript()`      | ::: block             |
        | gle.common.collect.Im |                       | Get the script to run |
        | mutableList<String>>` |                       | when buck fix is      |
        |                       |                       | invoked               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<String>`    | `g                    | ::: block             |
        |                       | etFixScriptContact()` | Get the contact to    |
        |                       |                       | use to tell users who |
        |                       |                       | to contact when       |
        |                       |                       | \`buck fix\` fails    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `g                    | ::: block             |
        |                       | etFixScriptMessage()` | Get the message to    |
        |                       |                       | show when invoking    |
        |                       |                       | \`buck fix\`          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.go               | `get                  | ::: block             |
        | ogle.common.collect.I | InterpolatedFixScript | Gets the full script  |
        | mmutableList<String>` | ​(com.google.common.co | to invoke in \`buck   |
        |                       | llect.ImmutableList<S | fix\`.                |
        |                       | tring> fixScript,     | :::                   |
        |                       |                       |                       |
        |                       | Path repositoryRoot,  |                       |
        |                       |                       |                       |
        |                       |    Path fixSpecPath)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getInterpola         | ::: block             |
        |                       | tedFixScriptMessage​(c | Gets the message to   |
        |                       | om.google.common.coll | print to users when   |
        |                       | ect.ImmutableList<Str | \`buck fix\` is       |
        |                       | ing> interpolatedFixS | invoked and performs  |
        |                       | cript,                | some substitutions    |
        |                       |                  Stri | :::                   |
        |                       | ng fixScriptContact)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<com.goo     | `                     | ::: block             |
        | gle.common.collect.Im | getLegacyFixScript()` | Get the previous      |
        | mutableList<String>>` |                       | script that JASABI    |
        |                       |                       | fixes                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `of​(                  |                       |
        | static FixBuckConfig` | BuckConfig delegate)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `shouldPri            | ::: block             |
        |                       | ntFixScriptMessage()` | Determine whether to  |
        |                       |                       | show a custom message |
        |                       |                       | when \`buck fix\` is  |
        |                       |                       | invoked               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `shouldRunAut         | ::: block             |
        |                       | ofix​(boolean isIntera | Whether or not to run |
        |                       | ctive,                | \`buck fix\`          |
        |                       |   String subcommand)` | automatically         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `should               | ::: block             |
        |                       | UseLegacyFixScript()` | Determine whether to  |
        |                       |                       | use the legacy        |
        |                       |                       | script, or the new    |
        |                       |                       | fix script system     |
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

        -   #### FixBuckConfig

                public FixBuckConfig()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getDelegate()}

        -   #### getDelegate

            ``` methodSignature
            public abstract BuckConfig getDelegate()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getDelegate` in interface `ConfigView<BuckConfig>`

        []{#of(com.facebook.buck.core.config.BuckConfig)}

        -   #### of

            ``` methodSignature
            public static FixBuckConfig of​(BuckConfig delegate)
            ```

        []{#getFixScript()}

        -   #### getFixScript

            ``` methodSignature
            @Lazy
            public Optional<com.google.common.collect.ImmutableList<String>> getFixScript()
            ```

            ::: block
            Get the script to run when buck fix is invoked
            :::

        []{#getLegacyFixScript()}

        -   #### getLegacyFixScript

            ``` methodSignature
            @Lazy
            public Optional<com.google.common.collect.ImmutableList<String>> getLegacyFixScript()
            ```

            ::: block
            Get the previous script that JASABI fixes
            :::

        []{#getFixScriptContact()}

        -   #### getFixScriptContact

            ``` methodSignature
            @Lazy
            public Optional<String> getFixScriptContact()
            ```

            ::: block
            Get the contact to use to tell users who to contact when
            \`buck fix\` fails
            :::

        []{#getFixScriptMessage()}

        -   #### getFixScriptMessage

            ``` methodSignature
            @Lazy
            public String getFixScriptMessage()
            ```

            ::: block
            Get the message to show when invoking \`buck fix\`
            :::

        []{#getAutofixEnabled()}

        -   #### getAutofixEnabled

            ``` methodSignature
            public com.facebook.buck.support.fix.FixBuckConfig.AutofixEnabled getAutofixEnabled()
            ```

            ::: block
            When running \`buck fix\` automatically on command failure
            is enabled
            :::

        []{#getAutofixCommands()}

        -   #### getAutofixCommands

            ``` methodSignature
            public List<String> getAutofixCommands()
            ```

            ::: block
            List of commands that autofix is enabled for
            :::

        []{#shouldRunAutofix(boolean,java.lang.String)}

        -   #### shouldRunAutofix

            ``` methodSignature
            public boolean shouldRunAutofix​(boolean isInteractive,
                                            String subcommand)
            ```

            ::: block
            Whether or not to run \`buck fix\` automatically
            :::

        []{#shouldPrintFixScriptMessage()}

        -   #### shouldPrintFixScriptMessage

            ``` methodSignature
            @Lazy
            public boolean shouldPrintFixScriptMessage()
            ```

            ::: block
            Determine whether to show a custom message when \`buck fix\`
            is invoked
            :::

        []{#shouldUseLegacyFixScript()}

        -   #### shouldUseLegacyFixScript

            ``` methodSignature
            @Lazy
            public boolean shouldUseLegacyFixScript()
            ```

            ::: block
            Determine whether to use the legacy script, or the new fix
            script system
            :::

        []{#getInterpolatedFixScript(com.google.common.collect.ImmutableList,java.nio.file.Path,java.nio.file.Path)}

        -   #### getInterpolatedFixScript

            ``` methodSignature
            public com.google.common.collect.ImmutableList<String> getInterpolatedFixScript​(com.google.common.collect.ImmutableList<String> fixScript,
                                                                                            Path repositoryRoot,
                                                                                            Path fixSpecPath)
            ```

            ::: block
            Gets the full script to invoke in \`buck fix\`.
            \`{fix_spec_path}\` is replaced with the path to the json
            file that contains details about the last run.
            \`{repository_root}\` is replaced with the absolute path to
            the repository root.
            :::

            [Parameters:]{.paramLabel}
            :   `fixScript` - The script to run (generally from the
                config file) that has not been interpolated
            :   `repositoryRoot` - The path to use for
                \`{repository_root}\`
            :   `fixSpecPath` - The path to use for \`{fix_spec_path}\`

            [Returns:]{.returnLabel}
            :   The interpolated command to run

        []{#getInterpolatedFixScriptMessage(com.google.common.collect.ImmutableList,java.lang.String)}

        -   #### getInterpolatedFixScriptMessage

            ``` methodSignature
            public String getInterpolatedFixScriptMessage​(com.google.common.collect.ImmutableList<String> interpolatedFixScript,
                                                          String fixScriptContact)
            ```

            ::: block
            Gets the message to print to users when \`buck fix\` is
            invoked and performs some substitutions
            \`{command}\` is replaced with `interpolatedFixScript`
            \`{contact}\` is replaced with `fixScriptContact`
            :::

            [Parameters:]{.paramLabel}
            :   `interpolatedFixScript` - The fix script per
                [`getInterpolatedFixScript(ImmutableList, Path, Path)`](#getInterpolatedFixScript(com.google.common.collect.ImmutableList,java.nio.file.Path,java.nio.file.Path))
            :   `fixScriptContact` - The contact to use in the message

            [Returns:]{.returnLabel}
            :   A string to be printed before the fix script is invoked,
                with template parameters substituted

        []{#getBuckProvidedScripts()}

        -   #### getBuckProvidedScripts

            ``` methodSignature
            public com.google.common.collect.ImmutableMap<String,​com.google.common.collect.ImmutableList<String>> getBuckProvidedScripts()
            ```

            ::: block
            Get a mapping of short names to Paths for buck provided fix
            scripts
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
