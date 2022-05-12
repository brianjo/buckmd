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
[Package]{.packageLabelInType} [com.facebook.buck.event.listener](package-summary.html)
:::

## Class RenderingConsole {#class-renderingconsole .title title="Class RenderingConsole"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.event.listener.RenderingConsole

::: description
-   

    ------------------------------------------------------------------------

        public class RenderingConsole
        extends Object

    ::: block
    A console that supports rendering.
    The Delegate provides the \"Super\" lines for the rendered frame,
    log lines will be queued by the RenderingConsole.

    If no delegate is configured (or if rendering is not running), lines
    will be logged immediately and won\'t be queued for the next frame.

    If something writes to the underlying Console\'s stderr/stdout
    streams, rendering will be disabled. If something writes to the real
    underlying stderr/stdout, we won\'t notice and it will get
    overwritten.

    TODO(cjhopman): For both those stderr/stdout cases, we should just
    capture the logging and queue it the same as logging that goes
    explicitly to the RenderingConsole. For real System.err/System.out
    we might need something a little fancy.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                        Description
          ------------------------------------------------------------------ -------------
          `RenderingConsole​(Clock clock,                 Console console)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `protected void`      | `cl                   |                       |
        |                       | earPendingLogLines()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `close()`             | ::: block             |
        |                       |                       | Shuts down rendering. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Ansi`                | `getAnsi()`           |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected com.go     | `                     |                       |
        | ogle.common.collect.I | getPendingLogLines()` |                       |
        | mmutableList<String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Verbosity`           | `getVerbosity()`      |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isRendering()`       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `logLi                | ::: block             |
        |                       | nes​(String... lines)` | Logs the provided     |
        |                       |                       | lines to stderr.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `logLines​(Colle       | ::: block             |
        |                       | ction<String> lines)` | Logs the provided     |
        |                       |                       | lines to stderr.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `printToStdOu         | ::: block             |
        |                       | t​(String testOutput)` | [Deprecate            |
        |                       |                       | d.]{.deprecatedLabel} |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `re                   | ::: block             |
        |                       | gisterDelegate​(com.fa | Registers a delegate  |
        |                       | cebook.buck.event.lis | to provide the data   |
        |                       | tener.RenderingConsol | to render and starts  |
        |                       | e.Delegate delegate)` | the rendering thread. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4
        .tableTab}[[Deprecated
        Methods](javascript:show(32);)[ ]{.tabEnd}]{#t6 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.util.timing.Clock,com.facebook.buck.util.Console)}

        -   #### RenderingConsole

                public RenderingConsole​(Clock clock,
                                        Console console)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getAnsi()}

        -   #### getAnsi

            ``` methodSignature
            public Ansi getAnsi()
            ```

        []{#getVerbosity()}

        -   #### getVerbosity

            ``` methodSignature
            public Verbosity getVerbosity()
            ```

        []{#registerDelegate(com.facebook.buck.event.listener.RenderingConsole.Delegate)}

        -   #### registerDelegate

            ``` methodSignature
            public void registerDelegate​(com.facebook.buck.event.listener.RenderingConsole.Delegate delegate)
            ```

            ::: block
            Registers a delegate to provide the data to render and
            starts the rendering thread.
            :::

        []{#logLines(java.lang.String...)}

        -   #### logLines

            ``` methodSignature
            public void logLines​(String... lines)
            ```

            ::: block
            Logs the provided lines to stderr. When rendering, this will
            be queued until the next rendered frame.
            :::

        []{#logLines(java.util.Collection)}

        -   #### logLines

            ``` methodSignature
            public void logLines​(Collection<String> lines)
            ```

            ::: block
            Logs the provided lines to stderr. When rendering, this will
            be queued until the next rendered frame.
            :::

        []{#printToStdOut(java.lang.String)}

        -   #### printToStdOut

            ``` methodSignature
            @Deprecated
            public void printToStdOut​(String testOutput)
            ```

            ::: deprecationBlock
            [Deprecated.]{.deprecatedLabel}
            :::

            ::: block
            This prints to stdout and disables rendering. It shouldn\'t
            be used.
            :::

        []{#getPendingLogLines()}

        -   #### getPendingLogLines

            ``` methodSignature
            protected com.google.common.collect.ImmutableList<String> getPendingLogLines()
            ```

        []{#clearPendingLogLines()}

        -   #### clearPendingLogLines

            ``` methodSignature
            protected void clearPendingLogLines()
            ```

        []{#close()}

        -   #### close

            ``` methodSignature
            public void close()
            ```

            ::: block
            Shuts down rendering. If rendering, will print at least one
            final frame.
            Logging after calling close() will not be queued.
            :::

        []{#isRendering()}

        -   #### isRendering

            ``` methodSignature
            public boolean isRendering()
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
