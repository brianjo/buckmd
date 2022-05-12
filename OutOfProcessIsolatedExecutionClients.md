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
[Package]{.packageLabelInType} [com.facebook.buck.remoteexecution.util](package-summary.html)
:::

## Class OutOfProcessIsolatedExecutionClients {#class-outofprocessisolatedexecutionclients .title title="Class OutOfProcessIsolatedExecutionClients"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.remoteexecution.util.OutOfProcessIsolatedExecutionClients

::: description
-   

    All Implemented Interfaces:
    :   `RemoteExecutionClients`, `Closeable`, `AutoCloseable`

    ------------------------------------------------------------------------

        public class OutOfProcessIsolatedExecutionClients
        extends Object
        implements RemoteExecutionClients

    ::: block
    IsolatedExecution implementation that will run buildrules in a
    subprocess.
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
        | `st                   | `create​(Protoc        | ::: block             |
        | atic OutOfProcessIsol | ol protocol,       Bu | Returns a             |
        | atedExecutionClients` | ckEventBus eventBus)` | RemoteExecution       |
        |                       |                       | implementation that   |
        |                       |                       | uses a local CAS and  |
        |                       |                       | a separate local      |
        |                       |                       | temporary directory   |
        |                       |                       | for execution.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ContentAd            | `getConte             |                       |
        | dressedStorageClient` | ntAddressedStorage()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Protocol`            | `getProtocol()`       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `RemoteEx             | `getRemo              |                       |
        | ecutionServiceClient` | teExecutionService()` |                       |
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

        []{#create(com.facebook.buck.remoteexecution.interfaces.Protocol,com.facebook.buck.event.BuckEventBus)}

        -   #### create

            ``` methodSignature
            public static OutOfProcessIsolatedExecutionClients create​(Protocol protocol,
                                                                      BuckEventBus eventBus)
                                                               throws IOException
            ```

            ::: block
            Returns a RemoteExecution implementation that uses a local
            CAS and a separate local temporary directory for execution.
            :::

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#getRemoteExecutionService()}

        -   #### getRemoteExecutionService

            ``` methodSignature
            public RemoteExecutionServiceClient getRemoteExecutionService()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getRemoteExecutionService` in
                interface `RemoteExecutionClients`

        []{#getContentAddressedStorage()}

        -   #### getContentAddressedStorage

            ``` methodSignature
            public ContentAddressedStorageClient getContentAddressedStorage()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getContentAddressedStorage` in
                interface `RemoteExecutionClients`

        []{#getProtocol()}

        -   #### getProtocol

            ``` methodSignature
            public Protocol getProtocol()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getProtocol` in interface `RemoteExecutionClients`

        []{#close()}

        -   #### close

            ``` methodSignature
            public void close()
                       throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `close` in interface `AutoCloseable`

            [Specified by:]{.overrideSpecifyLabel}
            :   `close` in interface `Closeable`

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
