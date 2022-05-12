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
[Package]{.packageLabelInType} [com.facebook.buck.doctor](package-summary.html)
:::

## Class DefaultExtraInfoCollector {#class-defaultextrainfocollector .title title="Class DefaultExtraInfoCollector"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.doctor.DefaultExtraInfoCollector

::: description
-   

    All Implemented Interfaces:
    :   `ExtraInfoCollector`

    ------------------------------------------------------------------------

        public class DefaultExtraInfoCollector
        extends Object
        implements ExtraInfoCollector

    ::: block
    Runs an optional user-specified command to get extra info for the
    rage report.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        -   []{#nested.classes.inherited.from.class.com.facebook.buck.doctor.ExtraInfoCollector}

            ### Nested classes/interfaces inherited from interface com.facebook.buck.doctor.[ExtraInfoCollector](ExtraInfoCollector.html "interface in com.facebook.buck.doctor")

            `ExtraInfoCollector.ExtraInfoExecutionException, ExtraInfoCollector.ExtraInfoResult`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                      Description
          -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `DefaultExtraInfoCollector​(DoctorConfig doctorConfig,                          ProjectFilesystem projectFilesystem,                          ProcessExecutor processExecutor)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                Method                                                                                                                                                                 Description
          ------------------------------------------------ ---------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `Optional<ExtraInfoCollector.ExtraInfoResult>`   `run()`                                                                                                                                                                 
          `static String`                                  `runCommandAndGetStdout​(Iterable<String> command,                       ProjectFilesystem projectFilesystem,                       ProcessExecutor processExecutor)`    

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

        []{#<init>(com.facebook.buck.doctor.config.DoctorConfig,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.util.ProcessExecutor)}

        -   #### DefaultExtraInfoCollector

                public DefaultExtraInfoCollector​(DoctorConfig doctorConfig,
                                                 ProjectFilesystem projectFilesystem,
                                                 ProcessExecutor processExecutor)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#run()}

        -   #### run

            ``` methodSignature
            public Optional<ExtraInfoCollector.ExtraInfoResult> run()
                                                             throws IOException,
                                                                    InterruptedException,
                                                                    ExtraInfoCollector.ExtraInfoExecutionException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `run` in interface `ExtraInfoCollector`

            [Throws:]{.throwsLabel}
            :   `IOException`
            :   `InterruptedException`
            :   `ExtraInfoCollector.ExtraInfoExecutionException`

        []{#runCommandAndGetStdout(java.lang.Iterable,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.util.ProcessExecutor)}

        -   #### runCommandAndGetStdout

            ``` methodSignature
            public static String runCommandAndGetStdout​(Iterable<String> command,
                                                        ProjectFilesystem projectFilesystem,
                                                        ProcessExecutor processExecutor)
                                                 throws InterruptedException,
                                                        ExtraInfoCollector.ExtraInfoExecutionException
            ```

            [Throws:]{.throwsLabel}
            :   `InterruptedException`
            :   `ExtraInfoCollector.ExtraInfoExecutionException`
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
