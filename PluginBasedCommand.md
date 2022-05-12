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

## Interface PluginBasedCommand {#interface-pluginbasedcommand .title title="Interface PluginBasedCommand"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `ProjectCommand`

    ------------------------------------------------------------------------

        public interface PluginBasedCommand

    ::: block
    An abstract class that provides basic capabilities for commands that
    use subcommands loaded from plugins.
    Implementations of this class will have logic to control common
    logic of a particular plugin-based command. For example,
    `buck project` command will have an implementation that implements
    this class and adds some common domain-independent logic to route a
    particular invocation to some implementation loaded from plugins.

    Typical example of usage:

           class ExamplePluginBasedCommand extends PluginBasedCommand {
            @PluginBasedSubCommands(factoryClass = ExamplePluginBasedSubCommandFactory.class)
            @SuppressFieldNotInitialized
             private ImmutableList modes;

            @Override
             protected ImmutableList<? extends PluginBasedSubCommand> getSubCommands() {
               return modes;
             }

            @Override
             protected String getTypeOptionName() {
               return "--mode";
             }
           }

           interface ExamplePluginBasedSubCommandFactory extends PluginBasedSubCommandFactory {
           }

           @Extention
           class SomeExamplePluginBasedSubCommand implements ExamplePluginBasedSubCommandFactory {
             @Override
             SomeExamplePluginBasedSubCommand createSubCommand() {
               return new SomeExamplePluginBasedSubCommand();
             }
           }
         

    Key points:

    -   Sub commands needs to be instantiated using factories
    -   Plugin subcommand factories have to implement
        `PluginBasedSubCommandFactory`.
    -   Plugin subcommands have to implement `PluginBasedSubCommand`.
    -   [`getTypeOptionName()`](#getTypeOptionName()) is used to control
        which option is used to select a subcommand. The logic in this
        class uses that method for help screen only. The particular
        implementations need to use the option with that name to select
        a particular subcommand.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `String`              | `g                    |                       |
        |                       | etShortDescription()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google           | `getSubCommands()`    |                       |
        | .common.collect.Immut |                       |                       |
        | ableList<? extends Pl |                       |                       |
        | uginBasedSubCommand>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getTypeOptionName()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `default void`        | `printUsage           | ::: block             |
        |                       | ​(PrintStream stream)` | Prints the usage to   |
        |                       |                       | the provided stream.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
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

        []{#getSubCommands()}

        -   #### getSubCommands

            ``` methodSignature
            com.google.common.collect.ImmutableList<? extends PluginBasedSubCommand> getSubCommands()
            ```

            [Returns:]{.returnLabel}
            :   all subcommands known to this command.

        []{#getTypeOptionName()}

        -   #### getTypeOptionName

            ``` methodSignature
            String getTypeOptionName()
            ```

            [Returns:]{.returnLabel}
            :   the name of the option that is used to control which
                subcommand is invoked.

        []{#getShortDescription()}

        -   #### getShortDescription

            ``` methodSignature
            String getShortDescription()
            ```

            [Returns:]{.returnLabel}
            :   a pharse that describes the purpose of this command.

        []{#printUsage(java.io.PrintStream)}

        -   #### printUsage

            ``` methodSignature
            default void printUsage​(PrintStream stream)
            ```

            ::: block
            Prints the usage to the provided stream.
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
