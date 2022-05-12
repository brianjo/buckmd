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
[Package]{.packageLabelInType} [com.facebook.buck.support.cli.config](package-summary.html)
:::

## Class CliConfig {#class-cliconfig .title title="Class CliConfig"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.support.cli.config.CliConfig

::: description
-   

    All Implemented Interfaces:
    :   `ConfigView<BuckConfig>`

    ------------------------------------------------------------------------

        public abstract class CliConfig
        extends Object
        implements ConfigView<BuckConfig>
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type   Field                               Description
          ------------------- ----------------------------------- -------------
          `static String`     `TRUNCATE_FAILING_COMMAND_CONFIG`    

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor     Description
          --------------- -------------
          `CliConfig()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `Ansi`                | `                     | ::: block             |
        |                       | createAnsi​(Optional<S | Create an Ansi object |
        |                       | tring> defaultColor)` | appropriate for the   |
        |                       |                       | current output.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `abstract BuckConfig` | `getDelegate()`       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `getEnableFailin      |                       |
        |                       | gCommandTruncation()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `getEnabl             |                       |
        |                       | eShowOutputWarning()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `getFlu               |                       |
        |                       | shEventsBeforeExit()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `JsonAttributeFormat` | `getJ                 | ::: block             |
        |                       | sonAttributeFormat()` | When printing out     |
        |                       |                       | json representation   |
        |                       |                       | of targets, what      |
        |                       |                       | formatting should be  |
        |                       |                       | applied               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.go               | `                     |                       |
        | ogle.common.collect.I | getMessageOfTheDay()` |                       |
        | mmutableList<String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `getRelativizeTargets |                       |
        |                       | ToWorkingDirectory()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `getWarnOnC           |                       |
        |                       | onfigFileOverrides()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com                  | `g                    |                       |
        | .google.common.collec | etWarnOnConfigFileOve |                       |
        | t.ImmutableSet<Path>` | rridesIgnoredFiles()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static CliConfig`    | `of​(                  |                       |
        |                       | BuckConfig delegate)` |                       |
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
    -   []{#field.detail}

        ### Field Detail

        []{#TRUNCATE_FAILING_COMMAND_CONFIG}

        -   #### TRUNCATE_FAILING_COMMAND_CONFIG

                public static final String TRUNCATE_FAILING_COMMAND_CONFIG

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../constant-values.html#com.facebook.buck.support.cli.config.CliConfig.TRUNCATE_FAILING_COMMAND_CONFIG)
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### CliConfig

                public CliConfig()
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
            public static CliConfig of​(BuckConfig delegate)
            ```

        []{#createAnsi(java.util.Optional)}

        -   #### createAnsi

            ``` methodSignature
            @Derived
            public Ansi createAnsi​(Optional<String> defaultColor)
            ```

            ::: block
            Create an Ansi object appropriate for the current output.
            First respect the user\'s preferences, if set. Next, respect
            any default provided by the caller. (This is used by buckd
            to tell the daemon about the client\'s terminal.) Finally,
            allow the Ansi class to autodetect whether the current
            output is a tty.
            :::

            [Parameters:]{.paramLabel}
            :   `defaultColor` - Default value provided by the caller
                (e.g. the client of buckd)

        []{#getJsonAttributeFormat()}

        -   #### getJsonAttributeFormat

            ``` methodSignature
            @Derived
            public JsonAttributeFormat getJsonAttributeFormat()
            ```

            ::: block
            When printing out json representation of targets, what
            formatting should be applied
            :::

        []{#getWarnOnConfigFileOverrides()}

        -   #### getWarnOnConfigFileOverrides

            ``` methodSignature
            @Lazy
            public boolean getWarnOnConfigFileOverrides()
            ```

        []{#getWarnOnConfigFileOverridesIgnoredFiles()}

        -   #### getWarnOnConfigFileOverridesIgnoredFiles

            ``` methodSignature
            @Lazy
            public com.google.common.collect.ImmutableSet<Path> getWarnOnConfigFileOverridesIgnoredFiles()
            ```

        []{#getFlushEventsBeforeExit()}

        -   #### getFlushEventsBeforeExit

            ``` methodSignature
            @Lazy
            public boolean getFlushEventsBeforeExit()
            ```

        []{#getMessageOfTheDay()}

        -   #### getMessageOfTheDay

            ``` methodSignature
            @Lazy
            public com.google.common.collect.ImmutableList<String> getMessageOfTheDay()
            ```

        []{#getRelativizeTargetsToWorkingDirectory()}

        -   #### getRelativizeTargetsToWorkingDirectory

            ``` methodSignature
            @Lazy
            public boolean getRelativizeTargetsToWorkingDirectory()
            ```

            [Returns:]{.returnLabel}
            :   whether relative targets given on the command line
                should be relativized to the user\'s working dir

        []{#getEnableShowOutputWarning()}

        -   #### getEnableShowOutputWarning

            ``` methodSignature
            @Lazy
            public boolean getEnableShowOutputWarning()
            ```

        []{#getEnableFailingCommandTruncation()}

        -   #### getEnableFailingCommandTruncation

            ``` methodSignature
            @Lazy
            public boolean getEnableFailingCommandTruncation()
            ```

            [Returns:]{.returnLabel}
            :   whether truncation of failing executed command is
                enabled. Defaults to true.
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
