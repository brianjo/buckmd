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
[Package]{.packageLabelInType} [com.facebook.buck.event.chrome_trace](package-summary.html)
:::

## Class ChromeTraceBuckConfig {#class-chrometracebuckconfig .title title="Class ChromeTraceBuckConfig"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.event.chrome_trace.ChromeTraceBuckConfig

::: description
-   

    All Implemented Interfaces:
    :   `ConfigView<BuckConfig>`

    ------------------------------------------------------------------------

        public class ChromeTraceBuckConfig
        extends Object
        implements ConfigView<BuckConfig>
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `boolean`             | `getCompressTraces()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `BuckConfig`          | `getDelegate()`       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `LogUploadMode`       | `getLogUploadMode()`  | ::: block             |
        |                       |                       | Returns whether and   |
        |                       |                       | when to upload logs.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `getMaxTraces()`      |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<URI>`       | `getTraceUploadUri()` | ::: block             |
        |                       |                       | Get URL to upload     |
        |                       |                       | trace.                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<URI>`       | `getTrace             | ::: block             |
        |                       | UploadUriIfEnabled()` | Get URL to upload     |
        |                       |                       | trace if the config   |
        |                       |                       | is enabled.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isChromeTr           |                       |
        |                       | aceCreationEnabled()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static C             | `of​(                  |                       |
        | hromeTraceBuckConfig` | BuckConfig delegate)` |                       |
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

        []{#of(com.facebook.buck.core.config.BuckConfig)}

        -   #### of

            ``` methodSignature
            public static ChromeTraceBuckConfig of​(BuckConfig delegate)
            ```

        []{#getMaxTraces()}

        -   #### getMaxTraces

            ``` methodSignature
            public int getMaxTraces()
            ```

        []{#isChromeTraceCreationEnabled()}

        -   #### isChromeTraceCreationEnabled

            ``` methodSignature
            public boolean isChromeTraceCreationEnabled()
            ```

        []{#getCompressTraces()}

        -   #### getCompressTraces

            ``` methodSignature
            public boolean getCompressTraces()
            ```

        []{#getTraceUploadUriIfEnabled()}

        -   #### getTraceUploadUriIfEnabled

            ``` methodSignature
            public Optional<URI> getTraceUploadUriIfEnabled()
            ```

            ::: block
            Get URL to upload trace if the config is enabled.
            :::

        []{#getTraceUploadUri()}

        -   #### getTraceUploadUri

            ``` methodSignature
            public Optional<URI> getTraceUploadUri()
            ```

            ::: block
            Get URL to upload trace.
            :::

        []{#getLogUploadMode()}

        -   #### getLogUploadMode

            ``` methodSignature
            public LogUploadMode getLogUploadMode()
            ```

            ::: block
            Returns whether and when to upload logs.
            :::

        []{#getDelegate()}

        -   #### getDelegate

            ``` methodSignature
            public BuckConfig getDelegate()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getDelegate` in interface `ConfigView<BuckConfig>`
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
