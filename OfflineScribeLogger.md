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
[Package]{.packageLabelInType} [com.facebook.buck.util.network.offline](package-summary.html)
:::

## Class OfflineScribeLogger {#class-offlinescribelogger .title title="Class OfflineScribeLogger"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.util.network.ScribeLogger](../ScribeLogger.html "class in com.facebook.buck.util.network")

    -   -   com.facebook.buck.util.network.offline.OfflineScribeLogger

::: description
-   

    All Implemented Interfaces:
    :   `Closeable`, `AutoCloseable`

    ------------------------------------------------------------------------

        public class OfflineScribeLogger
        extends ScribeLogger

    ::: block
    This logger uses files-related operations (for offline logging i.e.
    storing and delayed logging once network connection is better). Some
    of them may not be supported by all filesystems. E.g. Jimfs uses
    JimfsPath which does not support toFile() operation. For such
    filesystems, the offline logging will not be performed.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type           Field               Description
          --------------------------- ------------------- -------------
          `protected static String`   `LOGFILE_PATTERN`    
          `protected static String`   `LOGFILE_PREFIX`     
          `protected static String`   `LOGFILE_SUFFIX`     

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                                                                         Description
          ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `OfflineScribeLogger​(ScribeLogger scribeLogger,                    com.google.common.collect.ImmutableList<String> blacklistCategories,                    int maxScribeOfflineLogsKB,                    ProjectFilesystem projectFilesystem,                    BuckEventBus buckEventBus,                    BuildId buildId)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                            Method                                                                           Description
          ------------------------------------------------------------ -------------------------------------------------------------------------------- -------------
          `void`                                                       `close()`                                                                         
          `com.google.common.util.concurrent.ListenableFuture<Unit>`   `log​(String category,    Iterable<String> lines,    Optional<Integer> bucket)`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.util.network.ScribeLogger}

            ### Methods inherited from class com.facebook.buck.util.network.[ScribeLogger](../ScribeLogger.html "class in com.facebook.buck.util.network")

            `log`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#field.detail}

        ### Field Detail

        []{#LOGFILE_PATTERN}

        -   #### LOGFILE_PATTERN

                protected static final String LOGFILE_PATTERN

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../constant-values.html#com.facebook.buck.util.network.offline.OfflineScribeLogger.LOGFILE_PATTERN)

        []{#LOGFILE_PREFIX}

        -   #### LOGFILE_PREFIX

                protected static final String LOGFILE_PREFIX

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../constant-values.html#com.facebook.buck.util.network.offline.OfflineScribeLogger.LOGFILE_PREFIX)

        []{#LOGFILE_SUFFIX}

        -   #### LOGFILE_SUFFIX

                protected static final String LOGFILE_SUFFIX

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../constant-values.html#com.facebook.buck.util.network.offline.OfflineScribeLogger.LOGFILE_SUFFIX)
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.util.network.ScribeLogger,com.google.common.collect.ImmutableList,int,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.event.BuckEventBus,com.facebook.buck.core.model.BuildId)}

        -   #### OfflineScribeLogger

                public OfflineScribeLogger​(ScribeLogger scribeLogger,
                                           com.google.common.collect.ImmutableList<String> blacklistCategories,
                                           int maxScribeOfflineLogsKB,
                                           ProjectFilesystem projectFilesystem,
                                           BuckEventBus buckEventBus,
                                           BuildId buildId)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#log(java.lang.String,java.lang.Iterable,java.util.Optional)}

        -   #### log

            ``` methodSignature
            public com.google.common.util.concurrent.ListenableFuture<Unit> log​(String category,
                                                                                Iterable<String> lines,
                                                                                Optional<Integer> bucket)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `log` in class `ScribeLogger`

        []{#close()}

        -   #### close

            ``` methodSignature
            public void close()
                       throws IOException
            ```

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
