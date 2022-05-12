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
[Package]{.packageLabelInType} [com.facebook.buck.util](package-summary.html)
:::

## Class ProcessExecutor.LaunchedProcessImpl {#class-processexecutor.launchedprocessimpl .title title="Class ProcessExecutor.LaunchedProcessImpl"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.util.ProcessExecutor.LaunchedProcessImpl

::: description
-   

    All Implemented Interfaces:
    :   `ProcessExecutor.LaunchedProcess`

    ```{=html}
    <!-- -->
    ```

    Enclosing interface:
    :   [ProcessExecutor](ProcessExecutor.html "interface in com.facebook.buck.util")

    ------------------------------------------------------------------------

        public static class ProcessExecutor.LaunchedProcessImpl
        extends Object
        implements ProcessExecutor.LaunchedProcess

    ::: block
    Wraps a
    [`Process`](http://docs.oracle.com/javase/7/docs/api/java/lang/Process.html?is-external=true "class or interface in java.lang"){.externalLink}
    and exposes only its I/O streams, so callers have to pass it back to
    this class.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type                                   Field       Description
          --------------------------------------------------- ----------- -------------
          `com.google.common.collect.ImmutableList<String>`   `command`    
          `Process`                                           `process`    

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                       Description
          --------------------------------------------------------------------------------- -------------
          `LaunchedProcessImpl​(Process process,                    List<String> command)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `com.go               | `getCommand()`        |                       |
        | ogle.common.collect.I |                       |                       |
        | mmutableList<String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `InputStream`         | `getStderr()`         | ::: block             |
        |                       |                       | Input stream that     |
        |                       |                       | maps into stderr of   |
        |                       |                       | the process.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `OutputStream`        | `getStdin()`          | ::: block             |
        |                       |                       | Output stream that    |
        |                       |                       | maps into stdin of    |
        |                       |                       | the process.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `InputStream`         | `getStdout()`         | ::: block             |
        |                       |                       | Input stream that     |
        |                       |                       | maps into stdout of   |
        |                       |                       | the process.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isAlive()`           |                       |
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

        []{#process}

        -   #### process

                public final Process process

        []{#command}

        -   #### command

                public final com.google.common.collect.ImmutableList<String> command
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(java.lang.Process,java.util.List)}

        -   #### LaunchedProcessImpl

                public LaunchedProcessImpl​(Process process,
                                           List<String> command)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#isAlive()}

        -   #### isAlive

            ``` methodSignature
            public boolean isAlive()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `isAlive` in interface `ProcessExecutor.LaunchedProcess`

            [Returns:]{.returnLabel}
            :   false if process is killed, or true if it is alive.

        []{#getCommand()}

        -   #### getCommand

            ``` methodSignature
            public com.google.common.collect.ImmutableList<String> getCommand()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getCommand` in
                interface `ProcessExecutor.LaunchedProcess`

        []{#getStdin()}

        -   #### getStdin

            ``` methodSignature
            public OutputStream getStdin()
            ```

            ::: block
            [Description copied from
            interface: `ProcessExecutor.LaunchedProcess`]{.descfrmTypeLabel}
            :::

            ::: block
            Output stream that maps into stdin of the process. You\'d
            write into process\' stdin using it.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getStdin` in
                interface `ProcessExecutor.LaunchedProcess`

        []{#getStdout()}

        -   #### getStdout

            ``` methodSignature
            public InputStream getStdout()
            ```

            ::: block
            [Description copied from
            interface: `ProcessExecutor.LaunchedProcess`]{.descfrmTypeLabel}
            :::

            ::: block
            Input stream that maps into stdout of the process. You\'d
            read process\' stdout from it.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getStdout` in
                interface `ProcessExecutor.LaunchedProcess`

        []{#getStderr()}

        -   #### getStderr

            ``` methodSignature
            public InputStream getStderr()
            ```

            ::: block
            [Description copied from
            interface: `ProcessExecutor.LaunchedProcess`]{.descfrmTypeLabel}
            :::

            ::: block
            Input stream that maps into stderr of the process. You\'d
            read process\' stderr from it.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getStderr` in
                interface `ProcessExecutor.LaunchedProcess`
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
-   [Field](#field.detail) \| 
-   [Constr](#constructor.detail) \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
