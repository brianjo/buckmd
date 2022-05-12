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
[Package]{.packageLabelInType} [com.facebook.buck.remoteexecution.event.listener](package-summary.html)
:::

## Class RemoteExecutionConsoleLineProvider {#class-remoteexecutionconsolelineprovider .title title="Class RemoteExecutionConsoleLineProvider"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.remoteexecution.event.listener.RemoteExecutionConsoleLineProvider

::: description
-   

    All Implemented Interfaces:
    :   `AdditionalConsoleLineProvider`

    ------------------------------------------------------------------------

        public class RemoteExecutionConsoleLineProvider
        extends Object
        implements AdditionalConsoleLineProvider

    ::: block
    Provides output lines to the console about the current state of
    Remote Execution.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                   Description
          --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `RemoteExecutionConsoleLineProvider​(RemoteExecutionStatsProvider statsProvider,                                   String sessionIdInfo,                                   boolean isDebug)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `com.go               | `createC              | ::: block             |
        | ogle.common.collect.I | onsoleLinesAtTime​(lon | Returns additional    |
        | mmutableList<String>` | g currentTimeMillis)` | console lines         |
        |                       |                       | representing the      |
        |                       |                       | current state of      |
        |                       |                       | running a command.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static String`       | `prettyPrint          |                       |
        |                       | Size​(long sizeBytes)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
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
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.remoteexecution.event.RemoteExecutionStatsProvider,java.lang.String,boolean)}

        -   #### RemoteExecutionConsoleLineProvider

                public RemoteExecutionConsoleLineProvider​(RemoteExecutionStatsProvider statsProvider,
                                                          String sessionIdInfo,
                                                          boolean isDebug)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#createConsoleLinesAtTime(long)}

        -   #### createConsoleLinesAtTime

            ``` methodSignature
            public com.google.common.collect.ImmutableList<String> createConsoleLinesAtTime​(long currentTimeMillis)
            ```

            ::: block
            [Description copied from
            interface: `AdditionalConsoleLineProvider`]{.descfrmTypeLabel}
            :::

            ::: block
            Returns additional console lines representing the current
            state of running a command.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `createConsoleLinesAtTime` in
                interface `AdditionalConsoleLineProvider`

        []{#prettyPrintSize(long)}

        -   #### prettyPrintSize

            ``` methodSignature
            public static String prettyPrintSize​(long sizeBytes)
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