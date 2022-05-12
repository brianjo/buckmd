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
[Package]{.packageLabelInType} [com.facebook.buck.io.windowspipe](package-summary.html)
:::

## Class WindowsNamedPipe {#class-windowsnamedpipe .title title="Class WindowsNamedPipe"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.io.windowspipe.WindowsNamedPipe

::: description
-   

    All Implemented Interfaces:
    :   `Transport`, `Closeable`, `AutoCloseable`

    ------------------------------------------------------------------------

        public class WindowsNamedPipe
        extends Object
        implements Transport

    ::: block
    Implements a
    [`Transport`](../watchman/Transport.html "interface in com.facebook.buck.io.watchman")
    backed by a windows named pipe under the hood.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `void`                | `close()`             |                       |
        +-----------------------+-----------------------+-----------------------+
        | `sta                  | `createPipeW          | ::: block             |
        | tic WindowsNamedPipe` | ithPath​(String path)` | Creates a Windows     |
        |                       |                       | named pipe bound to a |
        |                       |                       | path                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `InputStream`         | `getInputStream()`    | ::: block             |
        |                       |                       | Returns an input      |
        |                       |                       | stream for reading    |
        |                       |                       | messages              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `OutputStream`        | `getOutputStream()`   | ::: block             |
        |                       |                       | Returns an input      |
        |                       |                       | stream for writing    |
        |                       |                       | messages.             |
        |                       |                       | :::                   |
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
    -   []{#method.detail}

        ### Method Detail

        []{#createPipeWithPath(java.lang.String)}

        -   #### createPipeWithPath

            ``` methodSignature
            public static WindowsNamedPipe createPipeWithPath​(String path)
                                                       throws IOException
            ```

            ::: block
            Creates a Windows named pipe bound to a path
            :::

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#close()}

        -   #### close

            ``` methodSignature
            public void close()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `close` in interface `AutoCloseable`

            [Specified by:]{.overrideSpecifyLabel}
            :   `close` in interface `Closeable`

        []{#getInputStream()}

        -   #### getInputStream

            ``` methodSignature
            public InputStream getInputStream()
            ```

            ::: block
            [Description copied from
            interface: `Transport`]{.descfrmTypeLabel}
            :::

            ::: block
            Returns an input stream for reading messages
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getInputStream` in interface `Transport`

            [Returns:]{.returnLabel}
            :   an input stream for reading messages in this IPC

        []{#getOutputStream()}

        -   #### getOutputStream

            ``` methodSignature
            public OutputStream getOutputStream()
            ```

            ::: block
            [Description copied from
            interface: `Transport`]{.descfrmTypeLabel}
            :::

            ::: block
            Returns an input stream for writing messages.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getOutputStream` in interface `Transport`

            [Returns:]{.returnLabel}
            :   an input stream for writing messages in this IPC
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
