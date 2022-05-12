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
[Package]{.packageLabelInType} [com.facebook.buck.core.rules.actions](package-summary.html)
:::

## Class ActionExecutionContext {#class-actionexecutioncontext .title title="Class ActionExecutionContext"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.rules.actions.ActionExecutionContext

::: description
-   

    ------------------------------------------------------------------------

        public abstract class ActionExecutionContext
        extends Object

    ::: block
    Holds the information
    [`Action`](Action.html "interface in com.facebook.buck.core.rules.actions")s
    can use for its
    [`Action.execute(ActionExecutionContext)`](Action.html#execute(com.facebook.buck.core.rules.actions.ActionExecutionContext))
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                  Description
          ---------------------------- -------------
          `ActionExecutionContext()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `abstrac              | `get                  |                       |
        | t ArtifactFilesystem` | ArtifactFilesystem()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected a          | `getBuckEventBus()`   |                       |
        | bstract BuckEventBus` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstrac              | `getEnvironment()`    |                       |
        | t Map<String,​String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abst                 | `                     |                       |
        | ract ProcessExecutor` | getProcessExecutor()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract Path`       | `g                    |                       |
        |                       | etWorkingDirectory()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `logError​(            | ::: block             |
        |                       | Throwable e,          | Logs an error         |
        |                       | String msg,         O | :::                   |
        |                       | bject... formatArgs)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static Ac            | `of​(Buck              |                       |
        | tionExecutionContext` | EventBus buckEventBus |                       |
        |                       | ,   ArtifactFilesyste |                       |
        |                       | m artifactFilesystem, |                       |
        |                       |    ProcessExecutor pr |                       |
        |                       | ocessExecutor,   Map< |                       |
        |                       | String,​? extends Stri |                       |
        |                       | ng> environment,   Pa |                       |
        |                       | th workingDirectory)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `postEv               | ::: block             |
        |                       | ent​(BuckEvent event)` | posts the given event |
        |                       |                       | to the global event   |
        |                       |                       | bus                   |
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

        -   #### ActionExecutionContext

                public ActionExecutionContext()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getBuckEventBus()}

        -   #### getBuckEventBus

            ``` methodSignature
            protected abstract BuckEventBus getBuckEventBus()
            ```

        []{#getArtifactFilesystem()}

        -   #### getArtifactFilesystem

            ``` methodSignature
            public abstract ArtifactFilesystem getArtifactFilesystem()
            ```

            [Returns:]{.returnLabel}
            :   an
                [`ArtifactFilesystem`](../../artifact/ArtifactFilesystem.html "class in com.facebook.buck.core.artifact")
                the
                [`Action`](Action.html "interface in com.facebook.buck.core.rules.actions")
                can access for it\'s execution. This is a filesystem
                that operates on
                [`Artifact`](../../artifact/Artifact.html "interface in com.facebook.buck.core.artifact")s
                without requiring actions to be aware of the actual
                underlying paths.

        []{#logError(java.lang.Throwable,java.lang.String,java.lang.Object...)}

        -   #### logError

            ``` methodSignature
            public void logError​(Throwable e,
                                 String msg,
                                 Object... formatArgs)
            ```

            ::: block
            Logs an error
            :::

        []{#postEvent(com.facebook.buck.event.BuckEvent)}

        -   #### postEvent

            ``` methodSignature
            public void postEvent​(BuckEvent event)
            ```

            ::: block
            posts the given event to the global event bus
            :::

        []{#getProcessExecutor()}

        -   #### getProcessExecutor

            ``` methodSignature
            public abstract ProcessExecutor getProcessExecutor()
            ```

            [Returns:]{.returnLabel}
            :   The executor to run processes in

        []{#getEnvironment()}

        -   #### getEnvironment

            ``` methodSignature
            public abstract Map<String,​String> getEnvironment()
            ```

            [Returns:]{.returnLabel}
            :   The environment of the current context

        []{#getWorkingDirectory()}

        -   #### getWorkingDirectory

            ``` methodSignature
            public abstract Path getWorkingDirectory()
            ```

            [Returns:]{.returnLabel}
            :   The working directory for the current context

        []{#of(com.facebook.buck.event.BuckEventBus,com.facebook.buck.core.artifact.ArtifactFilesystem,com.facebook.buck.util.ProcessExecutor,java.util.Map,java.nio.file.Path)}

        -   #### of

            ``` methodSignature
            public static ActionExecutionContext of​(BuckEventBus buckEventBus,
                                                    ArtifactFilesystem artifactFilesystem,
                                                    ProcessExecutor processExecutor,
                                                    Map<String,​? extends String> environment,
                                                    Path workingDirectory)
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
