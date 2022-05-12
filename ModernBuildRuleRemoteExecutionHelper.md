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
[Package]{.packageLabelInType} [com.facebook.buck.rules.modern.builders](package-summary.html)
:::

## Class ModernBuildRuleRemoteExecutionHelper {#class-modernbuildruleremoteexecutionhelper .title title="Class ModernBuildRuleRemoteExecutionHelper"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.rules.modern.builders.ModernBuildRuleRemoteExecutionHelper

::: description
-   

    All Implemented Interfaces:
    :   `RemoteExecutionHelper`

    ------------------------------------------------------------------------

        public class ModernBuildRuleRemoteExecutionHelper
        extends Object
        implements RemoteExecutionHelper

    ::: block
    ModernBuildRuleRemoteExecutionHelper is used to create remote
    execution actions for a
    [`ModernBuildRule`](../ModernBuildRule.html "class in com.facebook.buck.rules.modern").
    To create the remote action, we serialize the MBR (in a graph of
    serialized
    [`AddsToRuleKey`](../../../core/rulekey/AddsToRuleKey.html "interface in com.facebook.buck.core.rulekey")
    parts such that different rules will share serialization if they
    share references). We then send all the cells BuckConfigs in a
    serialized form, all of Buck\'s classpath (including plugin
    classpath) and run the action remotely with the
    [`OutOfProcessIsolatedBuilder`](OutOfProcessIsolatedBuilder.html "class in com.facebook.buck.rules.modern.builders")
    (via trampoline.sh).
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type   Field               Description
          ------------------- ------------------- -------------
          `static Path`       `METADATA_PATH`      
          `static Path`       `TRAMPOLINE_PATH`    

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                                                                                                                                                        Description
          ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ -------------
          `ModernBuildRuleRemoteExecutionHelper​(BuckEventBus eventBus,                                     Protocol protocol,                                     SourcePathRuleFinder ruleFinder,                                     Cell rootCell,                                     FileHashLoader fileHasher,                                     com.google.common.collect.ImmutableSet<PathMatcher> ignorePaths)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `Path`                | `getCellPathPrefix()` | ::: block             |
        |                       |                       | The cell path prefix  |
        |                       |                       | is the path that all  |
        |                       |                       | remote execution      |
        |                       |                       | related paths will be |
        |                       |                       | relative to.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Remot                | `prepareRemoteExecu   | ::: block             |
        | eExecutionActionInfo` | tion​(ModernBuildRule< | Gets all the          |
        |                       | ?> rule,              | information needed to |
        |                       |           java.util.f | run the rule via      |
        |                       | unction.BiPredicate<P | Remote Execution      |
        |                       | rotocol.Digest,​String | (inputs merkle tree,  |
        |                       | > requiredDataPredica | action and digest,    |
        |                       | te,                   | outputs).             |
        |                       |      com.facebook.buc | :::                   |
        |                       | k.remoteexecution.pro |                       |
        |                       | to.WorkerRequirements |                       |
        |                       |  workerRequirements)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `support              | ::: block             |
        |                       | sRemoteExecution​(Mode | Returns whether       |
        |                       | rnBuildRule<?> rule)` | remote execution is   |
        |                       |                       | supported by this     |
        |                       |                       | rule.                 |
        |                       |                       | :::                   |
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
    -   []{#field.detail}

        ### Field Detail

        []{#TRAMPOLINE_PATH}

        -   #### TRAMPOLINE_PATH

                public static final Path TRAMPOLINE_PATH

        []{#METADATA_PATH}

        -   #### METADATA_PATH

                public static final Path METADATA_PATH
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.event.BuckEventBus,com.facebook.buck.remoteexecution.interfaces.Protocol,com.facebook.buck.core.rules.SourcePathRuleFinder,com.facebook.buck.core.cell.Cell,com.facebook.buck.util.hashing.FileHashLoader,com.google.common.collect.ImmutableSet)}

        -   #### ModernBuildRuleRemoteExecutionHelper

                public ModernBuildRuleRemoteExecutionHelper​(BuckEventBus eventBus,
                                                            Protocol protocol,
                                                            SourcePathRuleFinder ruleFinder,
                                                            Cell rootCell,
                                                            FileHashLoader fileHasher,
                                                            com.google.common.collect.ImmutableSet<PathMatcher> ignorePaths)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getCellPathPrefix()}

        -   #### getCellPathPrefix

            ``` methodSignature
            public Path getCellPathPrefix()
            ```

            ::: block
            [Description copied from
            interface: `RemoteExecutionHelper`]{.descfrmTypeLabel}
            :::

            ::: block
            The cell path prefix is the path that all remote execution
            related paths will be relative to.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getCellPathPrefix` in interface `RemoteExecutionHelper`

        []{#supportsRemoteExecution(com.facebook.buck.rules.modern.ModernBuildRule)}

        -   #### supportsRemoteExecution

            ``` methodSignature
            public boolean supportsRemoteExecution​(ModernBuildRule<?> rule)
            ```

            ::: block
            [Description copied from
            interface: `RemoteExecutionHelper`]{.descfrmTypeLabel}
            :::

            ::: block
            Returns whether remote execution is supported by this rule.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `supportsRemoteExecution` in
                interface `RemoteExecutionHelper`

        []{#prepareRemoteExecution(com.facebook.buck.rules.modern.ModernBuildRule,java.util.function.BiPredicate,com.facebook.buck.remoteexecution.proto.WorkerRequirements)}

        -   #### prepareRemoteExecution

            ``` methodSignature
            public RemoteExecutionActionInfo prepareRemoteExecution​(ModernBuildRule<?> rule,
                                                                    java.util.function.BiPredicate<Protocol.Digest,​String> requiredDataPredicate,
                                                                    com.facebook.buck.remoteexecution.proto.WorkerRequirements workerRequirements)
                                                             throws IOException
            ```

            ::: block
            [Description copied from
            interface: `RemoteExecutionHelper`]{.descfrmTypeLabel}
            :::

            ::: block
            Gets all the information needed to run the rule via Remote
            Execution (inputs merkle tree, action and digest, outputs).
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `prepareRemoteExecution` in
                interface `RemoteExecutionHelper`

            [Throws:]{.throwsLabel}
            :   `IOException`
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
