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
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.event.external.events](package-summary.html)
:::

## Interface ProgressEventInterface {#interface-progresseventinterface .title title="Interface ProgressEventInterface"}
:::

::: contentContainer
::: description
-   

    All Superinterfaces:
    :   `BuckEventExternalInterface`

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `ProgressEvent`, `ProgressEvent.BuildProgressUpdated`,
        `ProgressEvent.ParsingProgressUpdated`,
        `ProgressEvent.ProjectGenerationProgressUpdated`

    ------------------------------------------------------------------------

        public interface ProgressEventInterface
        extends BuckEventExternalInterface

    ::: block
    Describes the progress made by buck with the operations described
    below. This type is intended to be used by external applications
    (like the Intellij Buck plugin) to deserialize events coming from
    the webserver.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type   Field                                   Description
          ------------------- --------------------------------------- -------------
          `static String`     `BUILD_PROGRESS_UPDATED`                 
          `static String`     `PARSING_PROGRESS_UPDATED`               
          `static String`     `PROJECT_GENERATION_PROGRESS_UPDATED`    

          : Fields[ ]{.tabEnd}

        -   []{#fields.inherited.from.class.com.facebook.buck.event.external.events.BuckEventExternalInterface}

            ### Fields inherited from interface com.facebook.buck.event.external.events.[BuckEventExternalInterface](BuckEventExternalInterface.html "interface in com.facebook.buck.event.external.events")

            `BUILD_FINISHED, BUILD_REPORT, BUILD_STARTED, BUILD_STATUS_EVENT, CACHE_RATE_STATS_UPDATE_EVENT, INDIVIDUAL_TEST_AWAITING_RESULTS, INSTALL_STARTED, PARSE_FINISHED, PARSE_STARTED, PROJECT_GENERATION_FINISHED, PROJECT_GENERATION_STARTED, TEST_RUN_STARTED`
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                 Description
          ------------------- ---------------------- -------------
          `double`            `getProgressValue()`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Abstract
          Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.event.external.events.BuckEventExternalInterface}

            ### Methods inherited from interface com.facebook.buck.event.external.events.[BuckEventExternalInterface](BuckEventExternalInterface.html "interface in com.facebook.buck.event.external.events")

            `getEventName, getTimestampMillis, storeLastInstanceAndReplayForNewClients`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#field.detail}

        ### Field Detail

        []{#PARSING_PROGRESS_UPDATED}

        -   #### PARSING_PROGRESS_UPDATED

                static final String PARSING_PROGRESS_UPDATED

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../constant-values.html#com.facebook.buck.event.external.events.ProgressEventInterface.PARSING_PROGRESS_UPDATED)

        []{#PROJECT_GENERATION_PROGRESS_UPDATED}

        -   #### PROJECT_GENERATION_PROGRESS_UPDATED

                static final String PROJECT_GENERATION_PROGRESS_UPDATED

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../constant-values.html#com.facebook.buck.event.external.events.ProgressEventInterface.PROJECT_GENERATION_PROGRESS_UPDATED)

        []{#BUILD_PROGRESS_UPDATED}

        -   #### BUILD_PROGRESS_UPDATED

                static final String BUILD_PROGRESS_UPDATED

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../constant-values.html#com.facebook.buck.event.external.events.ProgressEventInterface.BUILD_PROGRESS_UPDATED)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getProgressValue()}

        -   #### getProgressValue

            ``` methodSignature
            double getProgressValue()
            ```

            [Returns:]{.returnLabel}
            :   the current progress value for any of the build, parse
                or project generation events
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
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
-   Constr \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
