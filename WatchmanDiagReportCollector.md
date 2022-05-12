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
[Package]{.packageLabelInType} [com.facebook.buck.doctor](package-summary.html)
:::

## Class WatchmanDiagReportCollector {#class-watchmandiagreportcollector .title title="Class WatchmanDiagReportCollector"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.doctor.WatchmanDiagReportCollector

::: description
-   

    ------------------------------------------------------------------------

        public class WatchmanDiagReportCollector
        extends Object

    ::: block
    Gets watchman diagnostics using the watchman-diag command.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                             Description
          --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `WatchmanDiagReportCollector​(ProjectFilesystem projectFilesystem,                            String watchmanDiagCommand,                            ProcessExecutor processExecutor)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                Method                                                                                                                                                                                                                                                                                                                           Description
          ------------------------------------------------ -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `static Optional<WatchmanDiagReportCollector>`   `newInstanceIfWatchmanUsed​(Watchman watchman,                          ProjectFilesystem projectFilesystem,                          ProcessExecutor processExecutor,                          ExecutableFinder executableFinder,                          com.google.common.collect.ImmutableMap<String,​String> environment)`    
          `Path`                                           `run()`                                                                                                                                                                                                                                                                                                                           

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

        []{#<init>(com.facebook.buck.io.filesystem.ProjectFilesystem,java.lang.String,com.facebook.buck.util.ProcessExecutor)}

        -   #### WatchmanDiagReportCollector

                public WatchmanDiagReportCollector​(ProjectFilesystem projectFilesystem,
                                                   String watchmanDiagCommand,
                                                   ProcessExecutor processExecutor)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#run()}

        -   #### run

            ``` methodSignature
            public Path run()
                     throws IOException,
                            InterruptedException,
                            ExtraInfoCollector.ExtraInfoExecutionException
            ```

            [Throws:]{.throwsLabel}
            :   `IOException`
            :   `InterruptedException`
            :   `ExtraInfoCollector.ExtraInfoExecutionException`

        []{#newInstanceIfWatchmanUsed(com.facebook.buck.io.watchman.Watchman,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.util.ProcessExecutor,com.facebook.buck.io.ExecutableFinder,com.google.common.collect.ImmutableMap)}

        -   #### newInstanceIfWatchmanUsed

            ``` methodSignature
            public static Optional<WatchmanDiagReportCollector> newInstanceIfWatchmanUsed​(Watchman watchman,
                                                                                          ProjectFilesystem projectFilesystem,
                                                                                          ProcessExecutor processExecutor,
                                                                                          ExecutableFinder executableFinder,
                                                                                          com.google.common.collect.ImmutableMap<String,​String> environment)
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
