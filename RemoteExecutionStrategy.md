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
-   [Nested](#nested.class.summary) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.rules.modern.builders](package-summary.html)
:::

## Class RemoteExecutionStrategy {#class-remoteexecutionstrategy .title title="Class RemoteExecutionStrategy"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.rules.modern.builders.RemoteExecutionStrategy

::: description
-   

    All Implemented Interfaces:
    :   `BuildRuleStrategy`, `Closeable`, `AutoCloseable`

    ------------------------------------------------------------------------

        public class RemoteExecutionStrategy
        extends Object

    ::: block
    A
    [`BuildRuleStrategy`](../../../core/rules/build/strategy/BuildRuleStrategy.html "interface in com.facebook.buck.core.rules.build.strategy")
    that uses a Remote Execution service for executing BuildRules. It
    currently only supports ModernBuildRule and creates a remote Action
    With
    [`ModernBuildRuleRemoteExecutionHelper`](ModernBuildRuleRemoteExecutionHelper.html "class in com.facebook.buck.rules.modern.builders").
    See
    https://docs.google.com/document/d/1AaGk7fOPByEvpAbqeXIyE8HX_A3_axxNnvroblTZ_6s/preview
    for a high-level description of the approach to remote execution.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static interface `   | `RemoteExecutionSt    | ::: block             |
        |                       | rategy.RemoteExecutio | StrategyBuildResult   |
        |                       | nStrategyBuildResult` | for Remote Execution  |
        |                       |                       | Strategy which        |
        |                       |                       | includes RuleContext  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}

        -   []{#nested.classes.inherited.from.class.com.facebook.buck.core.rules.build.strategy.BuildRuleStrategy}

            ### Nested classes/interfaces inherited from interface com.facebook.buck.core.rules.build.strategy.[BuildRuleStrategy](../../../core/rules/build/strategy/BuildRuleStrategy.html "interface in com.facebook.buck.core.rules.build.strategy")

            `BuildRuleStrategy.StrategyBuildResult`
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `BuildRuleStrategy    | `bu                   | ::: block             |
        | .StrategyBuildResult` | ild​(BuildRule rule,   | Builds the rule.      |
        |                       |     BuildStrategyCont | :::                   |
        |                       | ext strategyContext)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `canBuild             | ::: block             |
        |                       | ​(BuildRule instance)` | A rule will be built  |
        |                       |                       | by the custom         |
        |                       |                       | strategy only if      |
        |                       |                       | canBuild() returns    |
        |                       |                       | true.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `close()`             |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#canBuild(com.facebook.buck.core.rules.BuildRule)}

        -   #### canBuild

            ``` methodSignature
            public boolean canBuild​(BuildRule instance)
            ```

            ::: block
            [Description copied from
            interface: `BuildRuleStrategy`]{.descfrmTypeLabel}
            :::

            ::: block
            A rule will be built by the custom strategy only if
            canBuild() returns true.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `canBuild` in interface `BuildRuleStrategy`

        []{#close()}

        -   #### close

            ``` methodSignature
            public void close()
                       throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `close` in interface `AutoCloseable`

            [Specified by:]{.overrideSpecifyLabel}
            :   `close` in interface `BuildRuleStrategy`

            [Specified by:]{.overrideSpecifyLabel}
            :   `close` in interface `Closeable`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#build(com.facebook.buck.core.rules.BuildRule,com.facebook.buck.core.build.engine.BuildStrategyContext)}

        -   #### build

            ``` methodSignature
            public BuildRuleStrategy.StrategyBuildResult build​(BuildRule rule,
                                                               BuildStrategyContext strategyContext)
            ```

            ::: block
            [Description copied from
            interface: `BuildRuleStrategy`]{.descfrmTypeLabel}
            :::

            ::: block
            Builds the rule.
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
-   [Nested](#nested.class.summary) \| 
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
