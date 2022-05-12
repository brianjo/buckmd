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

-   [Overview](../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../deprecated-list.html)
-   [Index](../../../../index-all.html)
-   [Help](../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.cli](package-summary.html)
:::

## Class TargetsCommand {#class-targetscommand .title title="Class TargetsCommand"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.cli.CommandWithPluginManager](CommandWithPluginManager.html "class in com.facebook.buck.cli")

    -   -   [com.facebook.buck.cli.AbstractCommand](AbstractCommand.html "class in com.facebook.buck.cli")

        -   -   com.facebook.buck.cli.TargetsCommand

::: description
-   

    All Implemented Interfaces:
    :   `Command`

    ------------------------------------------------------------------------

        public class TargetsCommand
        extends AbstractCommand
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        -   []{#fields.inherited.from.class.com.facebook.buck.cli.AbstractCommand}

            ### Fields inherited from class com.facebook.buck.cli.[AbstractCommand](AbstractCommand.html "class in com.facebook.buck.cli")

            `commandArgsFile`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor          Description
          -------------------- -------------
          `TargetsCommand()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `com.facebo           | `getReferencedFiles​(  |                       |
        | ok.buck.cli.PathArgum | AbsPath projectRoot)` |                       |
        | ents.ReferencedFiles` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `g                    |                       |
        |                       | etShortDescription()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com                  | `getTarge             |                       |
        | .google.common.collec | tHashModifiedPaths()` |                       |
        | t.ImmutableSet<Path>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.g                | `getTypes()`          |                       |
        | oogle.common.collect. |                       |                       |
        | ImmutableSet<String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isReadOnly()`        |                       |
        +-----------------------+-----------------------+-----------------------+
        | `ExitCode`            | `r                    |                       |
        |                       | unWithoutHelp​(Command |                       |
        |                       | RunnerParams params)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `s                    | ::: block             |
        |                       | houldUseJsonFormat()` | Determines if the     |
        |                       |                       | results should be in  |
        |                       |                       | JSON format.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.cli.AbstractCommand}

            ### Methods inherited from class com.facebook.buck.cli.[AbstractCommand](AbstractCommand.html "class in com.facebook.buck.cli")

            `addCommandSpecificConfigOverrides, convertArgumentsToBuildTargets, createParsingContext, getCommandArgsFile, getCommandLineBuildTargetNormalizer, getConcurrencyLimit, getConfigOverrides, getEnableParserProfiling, getEventListeners, getEventsOutputPath, getExcludeIncompatibleTargets, getExecutionContext, getExecutionContextBuilder, getHostPlatform, getLogConfig, getTargetPlatforms, handleException, handleException, isNoCache, isReuseCurrentConfig, isSourceControlStatsGatheringEnabled, matchBuildTargetsWithLabelsFromSpecs, performsBuild, prepareExecutionContext, printUsage, printWarning, printWarning, run, runHelp`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.cli.CommandWithPluginManager}

            ### Methods inherited from class com.facebook.buck.cli.[CommandWithPluginManager](CommandWithPluginManager.html "class in com.facebook.buck.cli")

            `getPluginManager, setPluginManager`

        ```{=html}
        <!-- -->
        ```
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

        -   #### TargetsCommand

                public TargetsCommand()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getTypes()}

        -   #### getTypes

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<String> getTypes()
            ```

        []{#getReferencedFiles(com.facebook.buck.core.filesystems.AbsPath)}

        -   #### getReferencedFiles

            ``` methodSignature
            public com.facebook.buck.cli.PathArguments.ReferencedFiles getReferencedFiles​(AbsPath projectRoot)
                                                                                   throws IOException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#shouldUseJsonFormat()}

        -   #### shouldUseJsonFormat

            ``` methodSignature
            public boolean shouldUseJsonFormat()
            ```

            ::: block
            Determines if the results should be in JSON format. This is
            true either when explicitly required by the `--json`
            argument or when there is at least one item in the
            `  --output-attributes` arguments.
            The `--output--attributes` arguments implicitly enables JSON
            format because there is currently no way to output
            attributes in non-JSON format. Also, it keeps this command
            consistent with the query command.
            :::

        []{#getTargetHashModifiedPaths()}

        -   #### getTargetHashModifiedPaths

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<Path> getTargetHashModifiedPaths()
            ```

            [Returns:]{.returnLabel}
            :   set of paths passed to `--assume-modified-files` if
                either `      --assume-modified-files` or
                `--assume-no-modified-files` is used, absent otherwise.

        []{#runWithoutHelp(com.facebook.buck.cli.CommandRunnerParams)}

        -   #### runWithoutHelp

            ``` methodSignature
            public ExitCode runWithoutHelp​(CommandRunnerParams params)
                                    throws Exception
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `runWithoutHelp` in class `AbstractCommand`

            [Throws:]{.throwsLabel}
            :   `Exception`

        []{#isReadOnly()}

        -   #### isReadOnly

            ``` methodSignature
            public boolean isReadOnly()
            ```

            [Returns:]{.returnLabel}
            :   whether the command doesn\'t modify the state of the
                filesystem

        []{#getShortDescription()}

        -   #### getShortDescription

            ``` methodSignature
            public String getShortDescription()
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

-   [Overview](../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../deprecated-list.html)
-   [Index](../../../../index-all.html)
-   [Help](../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../allclasses.html)

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
-   Field \| 
-   [Constr](#constructor.detail) \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
