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
[Package]{.packageLabelInType} [com.facebook.buck.cli](package-summary.html)
:::

## Class AbstractQueryCommand {#class-abstractquerycommand .title title="Class AbstractQueryCommand"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.cli.CommandWithPluginManager](CommandWithPluginManager.html "class in com.facebook.buck.cli")

    -   -   [com.facebook.buck.cli.AbstractCommand](AbstractCommand.html "class in com.facebook.buck.cli")

        -   -   com.facebook.buck.cli.AbstractQueryCommand

::: description
-   

    All Implemented Interfaces:
    :   `Command`

    ```{=html}
    <!-- -->
    ```

    Direct Known Subclasses:
    :   `QueryCommand`, `UnconfiguredQueryCommand`

    ------------------------------------------------------------------------

        public abstract class AbstractQueryCommand
        extends AbstractCommand

    ::: block
    Provides base functionality for query commands.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `pro                  | `AbstractQuery        | ::: block             |
        | tected static class ` | Command.OutputFormat` | Enum with values for  |
        |                       |                       | \`\--output-format\`  |
        |                       |                       | CLI parameter         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static class `       | `AbstractQueryComm    | ::: block             |
        |                       | and.SortOutputFormat` | Sort Output format.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `pro                  | `AbstractQueryComma   | ::: block             |
        | tected static class ` | nd.WhichQueryCommand` | Which of \*query      |
        |                       |                       | commands was invoked  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Field                 | Description           |
        +=======================+=======================+=======================+
        | `pr                   | `arguments`           |                       |
        | otected List<String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected boolean`   | `generateJsonOutput`  | ::: block             |
        |                       |                       | [Deprecate            |
        |                       |                       | d.]{.deprecatedLabel} |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `pr                   | `outputFormat`        |                       |
        | otected AbstractQuery |                       |                       |
        | Command.OutputFormat` |                       |                       |
        +-----------------------+-----------------------+-----------------------+

        : Fields[ ]{.tabEnd}

        -   []{#fields.inherited.from.class.com.facebook.buck.cli.AbstractCommand}

            ### Fields inherited from class com.facebook.buck.cli.[AbstractCommand](AbstractCommand.html "class in com.facebook.buck.cli")

            `commandArgsFile`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                Description
          -------------------------- -------------
          `AbstractQueryCommand()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                             Method                                                      Description
          ------------------------------------------------------------- ----------------------------------------------------------- -------------
          `static Set<QueryBuildTarget>`                                `asQueryBuildTargets​(Set<? extends QueryTarget> set)`        
          `static String`                                               `getEscapedArgumentsListAsString​(List<String> arguments)`    
          `boolean`                                                     `isReadOnly()`                                               
          `protected boolean`                                           `shouldOutputAttributes()`                                   
          `protected abstract AbstractQueryCommand.WhichQueryCommand`   `whichQueryCommand()`                                        

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
          Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
          .tableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Abstract
          Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.cli.AbstractCommand}

            ### Methods inherited from class com.facebook.buck.cli.[AbstractCommand](AbstractCommand.html "class in com.facebook.buck.cli")

            `addCommandSpecificConfigOverrides, convertArgumentsToBuildTargets, createParsingContext, getCommandArgsFile, getCommandLineBuildTargetNormalizer, getConcurrencyLimit, getConfigOverrides, getEnableParserProfiling, getEventListeners, getEventsOutputPath, getExcludeIncompatibleTargets, getExecutionContext, getExecutionContextBuilder, getHostPlatform, getLogConfig, getTargetPlatforms, handleException, handleException, isNoCache, isReuseCurrentConfig, isSourceControlStatsGatheringEnabled, matchBuildTargetsWithLabelsFromSpecs, performsBuild, prepareExecutionContext, printUsage, printWarning, printWarning, run, runHelp, runWithoutHelp`

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

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.cli.Command}

            ### Methods inherited from interface com.facebook.buck.cli.[Command](Command.html "interface in com.facebook.buck.cli")

            `getShortDescription`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#field.detail}

        ### Field Detail

        []{#generateJsonOutput}

        -   #### generateJsonOutput

                @Deprecated
                protected boolean generateJsonOutput

            ::: deprecationBlock
            [Deprecated.]{.deprecatedLabel}
            :::

        []{#outputFormat}

        -   #### outputFormat

                protected AbstractQueryCommand.OutputFormat outputFormat

        []{#arguments}

        -   #### arguments

                protected List<String> arguments
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### AbstractQueryCommand

                public AbstractQueryCommand()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#whichQueryCommand()}

        -   #### whichQueryCommand

            ``` methodSignature
            protected abstract AbstractQueryCommand.WhichQueryCommand whichQueryCommand()
            ```

        []{#shouldOutputAttributes()}

        -   #### shouldOutputAttributes

            ``` methodSignature
            protected boolean shouldOutputAttributes()
            ```

        []{#asQueryBuildTargets(java.util.Set)}

        -   #### asQueryBuildTargets

            ``` methodSignature
            public static Set<QueryBuildTarget> asQueryBuildTargets​(Set<? extends QueryTarget> set)
            ```

            [Returns:]{.returnLabel}
            :   set as
                [`QueryBuildTarget`](../query/QueryBuildTarget.html "class in com.facebook.buck.query")s
                or throw
                [`IllegalArgumentException`](http://docs.oracle.com/javase/7/docs/api/java/lang/IllegalArgumentException.html?is-external=true "class or interface in java.lang"){.externalLink}

        []{#isReadOnly()}

        -   #### isReadOnly

            ``` methodSignature
            public boolean isReadOnly()
            ```

            [Returns:]{.returnLabel}
            :   whether the command doesn\'t modify the state of the
                filesystem

        []{#getEscapedArgumentsListAsString(java.util.List)}

        -   #### getEscapedArgumentsListAsString

            ``` methodSignature
            public static String getEscapedArgumentsListAsString​(List<String> arguments)
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
