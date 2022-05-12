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
[Package]{.packageLabelInType} [com.facebook.buck.util](package-summary.html)
:::

## Class ProcessExecutorParams {#class-processexecutorparams .title title="Class ProcessExecutorParams"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.util.ProcessExecutorParams

::: description
-   

    ------------------------------------------------------------------------

        public abstract class ProcessExecutorParams
        extends Object

    ::: block
    Value type passed to
    [`ProcessExecutor`](ProcessExecutor.html "interface in com.facebook.buck.util")
    to launch a process.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type   Class                             Description
          ------------------- --------------------------------- -------------
          `static class `     `ProcessExecutorParams.Builder`    

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                 Description
          --------------------------- -------------
          `ProcessExecutorParams()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static ProcessEx     | `builder()`           |                       |
        | ecutorParams.Builder` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract com.go      | `getCommand()`        | ::: block             |
        | ogle.common.collect.I |                       | The command and       |
        | mmutableList<String>` |                       | arguments to launch.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `abs                  | `getDirectory()`      | ::: block             |
        | tract Optional<Path>` |                       | If present, the       |
        |                       |                       | current working       |
        |                       |                       | directory for the     |
        |                       |                       | launched process.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `abstract O           | `getEnvironment()`    | ::: block             |
        | ptional<com.google.co |                       | If present, the map   |
        | mmon.collect.Immutabl |                       | of environment        |
        | eMap<String,​String>>` |                       | variables used for    |
        |                       |                       | the launched process. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `a                    | `getRedirectError()`  | ::: block             |
        | bstract Optional<Proc |                       | If present, redirects |
        | essBuilder.Redirect>` |                       | stderr for the        |
        |                       |                       | process to this       |
        |                       |                       | location.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `abstra               | `getR                 |                       |
        | ct Optional<Boolean>` | edirectErrorStream()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `a                    | `getRedirectInput()`  | ::: block             |
        | bstract Optional<Proc |                       | If present, redirects |
        | essBuilder.Redirect>` |                       | stdout for the        |
        |                       |                       | process to this       |
        |                       |                       | location.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `a                    | `getRedirectOutput()` | ::: block             |
        | bstract Optional<Proc |                       | If present, redirects |
        | essBuilder.Redirect>` |                       | stdin for the process |
        |                       |                       | to this location.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static P             | `ofCom                |                       |
        | rocessExecutorParams` | mand​(String... args)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `P                    | `withEnvironment​(com. |                       |
        | rocessExecutorParams` | google.common.collect |                       |
        |                       | .ImmutableMap<String, |                       |
        |                       | ​String> environment)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `P                    | `withRedirectErr      |                       |
        | rocessExecutorParams` | or​(ProcessBuilder.Red |                       |
        |                       | irect redirectError)` |                       |
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

        -   #### ProcessExecutorParams

                public ProcessExecutorParams()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#ofCommand(java.lang.String...)}

        -   #### ofCommand

            ``` methodSignature
            public static ProcessExecutorParams ofCommand​(String... args)
            ```

        []{#getCommand()}

        -   #### getCommand

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableList<String> getCommand()
            ```

            ::: block
            The command and arguments to launch.
            :::

        []{#getDirectory()}

        -   #### getDirectory

            ``` methodSignature
            public abstract Optional<Path> getDirectory()
            ```

            ::: block
            If present, the current working directory for the launched
            process.
            :::

        []{#getEnvironment()}

        -   #### getEnvironment

            ``` methodSignature
            public abstract Optional<com.google.common.collect.ImmutableMap<String,​String>> getEnvironment()
            ```

            ::: block
            If present, the map of environment variables used for the
            launched process. Otherwise, inherits the current process\'s
            environment.
            :::

        []{#getRedirectInput()}

        -   #### getRedirectInput

            ``` methodSignature
            public abstract Optional<ProcessBuilder.Redirect> getRedirectInput()
            ```

            ::: block
            If present, redirects stdout for the process to this
            location. Otherwise, opens a pipe for stdout.
            :::

        []{#getRedirectOutput()}

        -   #### getRedirectOutput

            ``` methodSignature
            public abstract Optional<ProcessBuilder.Redirect> getRedirectOutput()
            ```

            ::: block
            If present, redirects stdin for the process to this
            location. Otherwise, opens a pipe for stdin.
            :::

        []{#getRedirectError()}

        -   #### getRedirectError

            ``` methodSignature
            public abstract Optional<ProcessBuilder.Redirect> getRedirectError()
            ```

            ::: block
            If present, redirects stderr for the process to this
            location. Otherwise, opens a pipe for stderr.
            :::

        []{#getRedirectErrorStream()}

        -   #### getRedirectErrorStream

            ``` methodSignature
            public abstract Optional<Boolean> getRedirectErrorStream()
            ```

        []{#withRedirectError(java.lang.ProcessBuilder.Redirect)}

        -   #### withRedirectError

            ``` methodSignature
            public ProcessExecutorParams withRedirectError​(ProcessBuilder.Redirect redirectError)
            ```

        []{#withEnvironment(com.google.common.collect.ImmutableMap)}

        -   #### withEnvironment

            ``` methodSignature
            public ProcessExecutorParams withEnvironment​(com.google.common.collect.ImmutableMap<String,​String> environment)
            ```

        []{#builder()}

        -   #### builder

            ``` methodSignature
            public static ProcessExecutorParams.Builder builder()
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
