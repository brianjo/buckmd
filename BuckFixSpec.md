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

## Class BuckFixSpec {#class-buckfixspec .title title="Class BuckFixSpec"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.support.fix.BuckFixSpec

::: description
-   

    ------------------------------------------------------------------------

        public abstract class BuckFixSpec
        extends Object

    ::: block
    Information about the build that is provided to \'fix\' scripts as a
    json file
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor       Description
          ----------------- -------------
          `BuckFixSpec()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `abstract com.google. | `getB                 | ::: block             |
        | common.collect.Immuta | uckProvidedScripts()` | Get a mapping of      |
        | bleMap<String,​com.goo |                       | names to paths of     |
        | gle.common.collect.Im |                       | fix-scripts that are  |
        | mutableList<String>>` |                       | built into buck (such |
        |                       |                       | as the original       |
        |                       |                       | JASABI fix script).   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `abstract BuildId`    | `getBuildId()`        | ::: block             |
        |                       |                       | The build ID.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `abstract String`     | `getCommand()`        | ::: block             |
        |                       |                       | The name of the       |
        |                       |                       | command that was run. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `abstr                | `getCommandData()`    | ::: block             |
        | act Optional<Object>` |                       | Arbitrary additional  |
        |                       |                       | data from the         |
        |                       |                       | specific command.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `abstract int`        | `getExitCode()`       | ::: block             |
        |                       |                       | The exit code of the  |
        |                       |                       | command               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `abstract com.go      | `getExpandedArgs()`   | ::: block             |
        | ogle.common.collect.I |                       | The fully evaluated   |
        | mmutableList<String>` |                       | arguments to this     |
        |                       |                       | buck invocation.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `abstract             | `getLogs()`           | ::: block             |
        |  com.google.common.co |                       | Get a mapping of log  |
        | llect.ImmutableMap<St |                       | short names to paths  |
        | ring,​Optional<Path>>` |                       | for those logs.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `abstract boolean`    | `                     | ::: block             |
        |                       | getManuallyInvoked()` | Whether the fix       |
        |                       |                       | script was requested  |
        |                       |                       | explicitly (through   |
        |                       |                       | \`buck fix\`), or     |
        |                       |                       | automatically from    |
        |                       |                       | another command       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `abstract com.go      | `getUserArgs()`       | ::: block             |
        | ogle.common.collect.I |                       | The arguments that    |
        | mmutableList<String>` |                       | the user sent to      |
        |                       |                       | buck.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}

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

        -   #### BuckFixSpec

                public BuckFixSpec()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getBuildId()}

        -   #### getBuildId

            ``` methodSignature
            public abstract BuildId getBuildId()
            ```

            ::: block
            The build ID. Generally a UUID
            :::

        []{#getCommand()}

        -   #### getCommand

            ``` methodSignature
            public abstract String getCommand()
            ```

            ::: block
            The name of the command that was run. e.g. \'build\' or
            \'query\'
            :::

        []{#getExitCode()}

        -   #### getExitCode

            ``` methodSignature
            public abstract int getExitCode()
            ```

            ::: block
            The exit code of the command
            :::

        []{#getUserArgs()}

        -   #### getUserArgs

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableList<String> getUserArgs()
            ```

            ::: block
            The arguments that the user sent to buck. This may include
            unexpanded arguments such as flagfiles
            :::

        []{#getExpandedArgs()}

        -   #### getExpandedArgs

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableList<String> getExpandedArgs()
            ```

            ::: block
            The fully evaluated arguments to this buck invocation.
            :::

        []{#getManuallyInvoked()}

        -   #### getManuallyInvoked

            ``` methodSignature
            public abstract boolean getManuallyInvoked()
            ```

            ::: block
            Whether the fix script was requested explicitly (through
            \`buck fix\`), or automatically from another command
            :::

        []{#getCommandData()}

        -   #### getCommandData

            ``` methodSignature
            public abstract Optional<Object> getCommandData()
            ```

            ::: block
            Arbitrary additional data from the specific command. This is
            used to allow the script to not need to know how to parse
            the buck machine log or the main buck log
            :::

            [Returns:]{.returnLabel}
            :   Additional data for the specific command

        []{#getBuckProvidedScripts()}

        -   #### getBuckProvidedScripts

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableMap<String,​com.google.common.collect.ImmutableList<String>> getBuckProvidedScripts()
            ```

            ::: block
            Get a mapping of names to paths of fix-scripts that are
            built into buck (such as the original JASABI fix script).
            These will generally be in the .buckd resources directory
            :::

        []{#getLogs()}

        -   #### getLogs

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableMap<String,​Optional<Path>> getLogs()
            ```

            ::: block
            Get a mapping of log short names to paths for those logs.
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
