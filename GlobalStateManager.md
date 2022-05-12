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
[Package]{.packageLabelInType} [com.facebook.buck.log](package-summary.html)
:::

## Class GlobalStateManager {#class-globalstatemanager .title title="Class GlobalStateManager"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.log.GlobalStateManager

::: description
-   

    ------------------------------------------------------------------------

        public class GlobalStateManager
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type     Class                                              Description
          --------------------- -------------------------------------------------- -------------
          `static interface `   `GlobalStateManager.LoggerIsMappedToThreadScope`    

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor              Description
          ------------------------ -------------
          `GlobalStateManager()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `protected void`      | `finalize()`          | ::: block             |
        |                       |                       | Since this is a       |
        |                       |                       | Singleton class, make |
        |                       |                       | sure it cleans after  |
        |                       |                       | itself once it\'s     |
        |                       |                       | GC\'ed.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Comma                | `getCommand           |                       |
        | ndIdToIsDaemonMapper` | IdToIsDaemonMapper()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `CommandIdToIsR       | `getCommandIdToIsRem  |                       |
        | emoteExecutionMapper` | oteExecutionMapper()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `CommandIdToIsSuper   | `ge                   |                       |
        | ConsoleEnabledMapper` | tCommandIdToIsSuperCo |                       |
        |                       | nsoleEnabledMapper()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `ConsoleHandlerState` | `getC                 |                       |
        |                       | onsoleHandlerState()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `LogFileHandlerState` | `getL                 | ::: block             |
        |                       | ogFileHandlerState()` | Writers obtained by   |
        |                       |                       | [`                    |
        |                       |                       | LogFileHandlerState.g |
        |                       |                       | etWriters(java.lang.S |
        |                       |                       | tring)`](LogFileHandl |
        |                       |                       | erState.html#getWrite |
        |                       |                       | rs(java.lang.String)) |
        |                       |                       | must not be closed!   |
        |                       |                       | This class manages    |
        |                       |                       | their lifetime.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getRepository()`     |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Threa                | `getThreadI           |                       |
        | dIdToCommandIdMapper` | dToCommandIdMapper()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Comm                 | `getThrea             |                       |
        | onThreadFactoryState` | dToCommandRegister()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Globa                | `setupLoggers​(In      |                       |
        | lStateManager.LoggerI | vocationInfo info,    |                       |
        | sMappedToThreadScope` |           OutputStrea |                       |
        |                       | m consoleHandlerStrea |                       |
        |                       | m,             Output |                       |
        |                       | Stream consoleHandler |                       |
        |                       | OriginalStream,       |                       |
        |                       |        Verbosity cons |                       |
        |                       | oleHandlerVerbosity)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `stati                | `singleton()`         |                       |
        | c GlobalStateManager` |                       |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### GlobalStateManager

                public GlobalStateManager()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#singleton()}

        -   #### singleton

            ``` methodSignature
            public static GlobalStateManager singleton()
            ```

        []{#setupLoggers(com.facebook.buck.log.InvocationInfo,java.io.OutputStream,java.io.OutputStream,com.facebook.buck.util.Verbosity)}

        -   #### setupLoggers

            ``` methodSignature
            public GlobalStateManager.LoggerIsMappedToThreadScope setupLoggers​(InvocationInfo info,
                                                                               OutputStream consoleHandlerStream,
                                                                               OutputStream consoleHandlerOriginalStream,
                                                                               Verbosity consoleHandlerVerbosity)
            ```

        []{#getThreadToCommandRegister()}

        -   #### getThreadToCommandRegister

            ``` methodSignature
            public CommonThreadFactoryState getThreadToCommandRegister()
            ```

        []{#getConsoleHandlerState()}

        -   #### getConsoleHandlerState

            ``` methodSignature
            public ConsoleHandlerState getConsoleHandlerState()
            ```

        []{#getThreadIdToCommandIdMapper()}

        -   #### getThreadIdToCommandIdMapper

            ``` methodSignature
            public ThreadIdToCommandIdMapper getThreadIdToCommandIdMapper()
            ```

        []{#getCommandIdToIsDaemonMapper()}

        -   #### getCommandIdToIsDaemonMapper

            ``` methodSignature
            public CommandIdToIsDaemonMapper getCommandIdToIsDaemonMapper()
            ```

        []{#getCommandIdToIsRemoteExecutionMapper()}

        -   #### getCommandIdToIsRemoteExecutionMapper

            ``` methodSignature
            public CommandIdToIsRemoteExecutionMapper getCommandIdToIsRemoteExecutionMapper()
            ```

        []{#getCommandIdToIsSuperConsoleEnabledMapper()}

        -   #### getCommandIdToIsSuperConsoleEnabledMapper

            ``` methodSignature
            public CommandIdToIsSuperConsoleEnabledMapper getCommandIdToIsSuperConsoleEnabledMapper()
            ```

        []{#getRepository()}

        -   #### getRepository

            ``` methodSignature
            public String getRepository()
            ```

        []{#getLogFileHandlerState()}

        -   #### getLogFileHandlerState

            ``` methodSignature
            public LogFileHandlerState getLogFileHandlerState()
            ```

            ::: block
            Writers obtained by
            [`LogFileHandlerState.getWriters(java.lang.String)`](LogFileHandlerState.html#getWriters(java.lang.String))
            must not be closed! This class manages their lifetime.
            :::

        []{#finalize()}

        -   #### finalize

            ``` methodSignature
            protected void finalize()
            ```

            ::: block
            Since this is a Singleton class, make sure it cleans after
            itself once it\'s GC\'ed.
            :::

            [Overrides:]{.overrideSpecifyLabel}
            :   `finalize` in class `Object`

            [Throws:]{.throwsLabel}
            :   `IOException` - if an I/O error occurs.
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
