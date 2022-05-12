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
[Package]{.packageLabelInType} [com.facebook.buck.remoteexecution.config](package-summary.html)
:::

## Class RemoteExecutionConfig {#class-remoteexecutionconfig .title title="Class RemoteExecutionConfig"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.remoteexecution.config.RemoteExecutionConfig

::: description
-   

    All Implemented Interfaces:
    :   `ConfigView<BuckConfig>`

    ------------------------------------------------------------------------

        public abstract class RemoteExecutionConfig
        extends Object
        implements ConfigView<BuckConfig>

    ::: block
    Config object for the \[remoteexecution\] section of .buckconfig.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Field                 | Description           |
        +=======================+=======================+=======================+
        | `static String`       | `AUTO_RE_BUILD_PR     |                       |
        |                       | OJECTS_WHITELIST_KEY` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static String`       | `AUTO_RE_BUILD        |                       |
        |                       | _USERS_BLACKLIST_KEY` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static String`       | `AUTO_RE_EXP          |                       |
        |                       | ERIMENT_PROPERTY_KEY` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static String`       | `                     | ::: block             |
        |                       | AUTO_RE_STRATEGY_KEY` | Strategy used to      |
        |                       |                       | determine whether to  |
        |                       |                       | enable Remote         |
        |                       |                       | Execution             |
        |                       |                       | automatically for the |
        |                       |                       | current build         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static String`       | `BUILD_TAGS_KEY`      |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static String`       | `CONCURRENT_ACT       | ::: block             |
        |                       | ION_COMPUTATIONS_KEY` | Number of actions to  |
        |                       |                       | compute at a time.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static String`       | `CONCU                | ::: block             |
        |                       | RRENT_EXECUTIONS_KEY` | Limit on the number   |
        |                       |                       | of outstanding        |
        |                       |                       | execution requests.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static String`       | `CONCURRENT           | ::: block             |
        |                       | _PENDING_UPLOADS_KEY` | Number of pending     |
        |                       |                       | uploads at a time.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static String`       | `CONCURRENT           | ::: block             |
        |                       | _RESULT_HANDLING_KEY` | Number of results to  |
        |                       |                       | concurrently handle   |
        |                       |                       | at a time.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static String`       | `DEBUG_F              | ::: block             |
        |                       | ORMAT_STRING_URL_KEY` | URL format string for |
        |                       |                       | debug UI on the super |
        |                       |                       | console               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static String`       | `DEFAULT_AUTO_RE      |                       |
        |                       | _EXPERIMENT_PROPERTY` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static int`          | `DE                   |                       |
        |                       | FAULT_CAS_DEADLINE_S` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static int`          | `DEFAULT_CAS_PORT`    |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static boolean`      | `DEFAULT_IS_LOC       |                       |
        |                       | AL_FALLBACK_DISABLED_ |                       |
        |                       | ON_CORRUPT_ARTIFACTS` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static boolean`      | `DEFAULT_IS_LO        |                       |
        |                       | CAL_FALLBACK_ENABLED` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static boolean`      | `DEFAULT_IS_LO        |                       |
        |                       | CAL_FALLBACK_ENABLED_ |                       |
        |                       | FOR_COMPLETED_ACTION` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static int`          | `DEFA                 |                       |
        |                       | ULT_REMOTE_CONCURRENT |                       |
        |                       | _ACTION_COMPUTATIONS` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static int`          | `DEFAULT_REMOTE_C     |                       |
        |                       | ONCURRENT_EXECUTIONS` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static int`          | `                     |                       |
        |                       | DEFAULT_REMOTE_CONCUR |                       |
        |                       | RENT_PENDING_UPLOADS` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static int`          | `                     |                       |
        |                       | DEFAULT_REMOTE_CONCUR |                       |
        |                       | RENT_RESULT_HANDLING` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static int`          | `DEFA                 |                       |
        |                       | ULT_REMOTE_OUTPUT_MAT |                       |
        |                       | ERIALIZATION_THREADS` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static int`          | `DEFAULT_REMOTE_PORT` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static int`          | `DEFAULT_REM          |                       |
        |                       | OTE_STRATEGY_THREADS` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static String`       | `FORMAT_SESSIO        | ::: block             |
        |                       | N_ID_VARIABLE_STRING` | The variable          |
        |                       |                       | identifier string to  |
        |                       |                       | be replace in any     |
        |                       |                       | configured format     |
        |                       |                       | defined by            |
        |                       |                       | DEBUG_F               |
        |                       |                       | ORMAT_STRING_URL_KEY. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static String`       | `INPUT_IGNORE_KEY`    | ::: block             |
        |                       |                       | Input paths to ignore |
        |                       |                       | for actions           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static String`       | `IS_LOCAL_F           | ::: block             |
        |                       | ALLBACK_DISABLED_ON_C | Whether failed remote |
        |                       | ORRUPT_ARTIFACTS_KEY` | executions are        |
        |                       |                       | retried locally if    |
        |                       |                       | the artifacts are     |
        |                       |                       | corrupted.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static String`       | `IS_LOCAL_            |                       |
        |                       | FALLBACK_ENABLED_FOR_ |                       |
        |                       | COMPLETED_ACTION_KEY` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static String`       | `IS_LOCAL_            | ::: block             |
        |                       | FALLBACK_ENABLED_KEY` | Whether failed remote |
        |                       |                       | executions are        |
        |                       |                       | retried locally.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static String`       | `L                    | ::: block             |
        |                       | ARGE_BLOB_SIZE_BYTES` | The large blob size   |
        |                       |                       | bytes threshold, if   |
        |                       |                       | unset, no threshold.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static Logger`       | `LOG`                 |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static String`       | `                     | ::: block             |
        |                       | MAX_INPUT_SIZE_BYTES` | The maximum size of   |
        |                       |                       | inputs allowed on     |
        |                       |                       | remote execution, if  |
        |                       |                       | unset, no maximum.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static String`       | `MAX_WORKE            | ::: block             |
        |                       | R_SIZE_TO_STEAL_FROM` | Actions which require |
        |                       |                       | a worker of this size |
        |                       |                       | (or higher) will not  |
        |                       |                       | be stolen locally     |
        |                       |                       | when running in       |
        |                       |                       | hybrid mode           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static String`       | `OUTPUT_MATERIA       | ::: block             |
        |                       | LIZATION_THREADS_KEY` | Number of threads to  |
        |                       |                       | handle output         |
        |                       |                       | materialization.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static String`       | `                     | ::: block             |
        |                       | RE_SESSION_LABEL_KEY` | Free form string      |
        |                       |                       | label that can be     |
        |                       |                       | passed along any      |
        |                       |                       | Remote Execution      |
        |                       |                       | session.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static String`       | `SECTION`             |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static String`       | `STRATEG              | ::: block             |
        |                       | Y_WORKER_THREADS_KEY` | Number of threads for |
        |                       |                       | the strategy to do    |
        |                       |                       | its work.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static String`       | `TENANT_ID_KEY`       | ::: block             |
        |                       |                       | Tenant ID that will   |
        |                       |                       | be attached to each   |
        |                       |                       | action \*             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static String`       | `TRY_                 |                       |
        |                       | LARGER_WORKER_ON_OOM` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static String`       | `USE_REMOTE_          |                       |
        |                       | EXECUTION_FOR_GENRULE |                       |
        |                       | _IF_REQUESTED_FORMAT` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static String`       | `WORKER_R             | ::: block             |
        |                       | EQUIREMENTS_FILENAME` | Worker requirements   |
        |                       |                       | filename              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                 Description
          --------------------------- -------------
          `RemoteExecutionConfig()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `String`              | `ge                   | ::: block             |
        |                       | tAuxiliaryBuildTag()` | Provides an auxiliary |
        |                       |                       | tag used for          |
        |                       |                       | capturing any custom  |
        |                       |                       | configurations.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `getCasDeadline()`    |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getCasHost()`        |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `getCasInsecure()`    |                       |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `getCasPort()`        |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Path>`      | `getCertFile()`       | ::: block             |
        |                       |                       | client TLS            |
        |                       |                       | certificate file in   |
        |                       |                       | PEM format            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Path>`      | `getCertific          | ::: block             |
        |                       | ateAuthoritiesFile()` | file containing all   |
        |                       |                       | TLS authorities to    |
        |                       |                       | verify server         |
        |                       |                       | certificate with (PEM |
        |                       |                       | format)               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getDebugURLString​(co |                       |
        |                       | m.facebook.buck.remot |                       |
        |                       | eexecution.proto.RESe |                       |
        |                       | ssionID reSessionID)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `getInsecure()`       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Path>`      | `getKeyFile()`        | ::: block             |
        |                       |                       | client TLS private    |
        |                       |                       | key in PEM format     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<com.face    | `getMaxWor            |                       |
        | book.buck.remoteexecu | kerSizeToStealFrom()` |                       |
        | tion.proto.WorkerRequ |                       |                       |
        | irements.WorkerSize>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getRemoteHost()`     |                       |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `getRemotePort()`     |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getReSessionLabel()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `RemoteExe            | `getStrategyConfig()` |                       |
        | cutionStrategyConfig` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getTenantId()`       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `RemoteExecutionType` | `getType()`           |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static String`       | `getUseRemoteExecuti  |                       |
        |                       | onForGenruleIfRequest |                       |
        |                       | edField​(String type)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isConsoleEnabled()`  | ::: block             |
        |                       |                       | Whether Console       |
        |                       |                       | output of Remote      |
        |                       |                       | Execution information |
        |                       |                       | is enabled.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isDebug()`           |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `                     |                       |
        |                       | isRemoteExecutionAuto |                       |
        |                       | Enabled​(String userna |                       |
        |                       | me,                   |                       |
        |                       |            List<Strin |                       |
        |                       | g> commandArguments)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static R             | `of​(                  |                       |
        | emoteExecutionConfig` | BuckConfig delegate)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `shouldUseRemoteEx    | ::: block             |
        |                       | ecutionForGenruleIfRe | Returns whether or    |
        |                       | quested​(String type)` | not we should honor   |
        |                       |                       | the \`remote\`        |
        |                       |                       | argument to           |
        |                       |                       | \`genrule\`, which    |
        |                       |                       | requests that the     |
        |                       |                       | genrule run remotely. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `validateC            |                       |
        |                       | ertificatesOrThrow()` |                       |
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

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.config.ConfigView}

            ### Methods inherited from interface com.facebook.buck.core.config.[ConfigView](../../core/config/ConfigView.html "interface in com.facebook.buck.core.config")

            `getDelegate`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#field.detail}

        ### Field Detail

        []{#LOG}

        -   #### LOG

                public static final Logger LOG

        []{#SECTION}

        -   #### SECTION

                public static final String SECTION

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.remoteexecution.config.RemoteExecutionConfig.SECTION)

        []{#DEFAULT_REMOTE_PORT}

        -   #### DEFAULT_REMOTE_PORT

                public static final int DEFAULT_REMOTE_PORT

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.remoteexecution.config.RemoteExecutionConfig.DEFAULT_REMOTE_PORT)

        []{#DEFAULT_CAS_PORT}

        -   #### DEFAULT_CAS_PORT

                public static final int DEFAULT_CAS_PORT

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.remoteexecution.config.RemoteExecutionConfig.DEFAULT_CAS_PORT)

        []{#DEFAULT_CAS_DEADLINE_S}

        -   #### DEFAULT_CAS_DEADLINE_S

                public static final int DEFAULT_CAS_DEADLINE_S

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.remoteexecution.config.RemoteExecutionConfig.DEFAULT_CAS_DEADLINE_S)

        []{#DEFAULT_REMOTE_STRATEGY_THREADS}

        -   #### DEFAULT_REMOTE_STRATEGY_THREADS

                public static final int DEFAULT_REMOTE_STRATEGY_THREADS

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.remoteexecution.config.RemoteExecutionConfig.DEFAULT_REMOTE_STRATEGY_THREADS)

        []{#DEFAULT_REMOTE_CONCURRENT_ACTION_COMPUTATIONS}

        -   #### DEFAULT_REMOTE_CONCURRENT_ACTION_COMPUTATIONS

                public static final int DEFAULT_REMOTE_CONCURRENT_ACTION_COMPUTATIONS

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.remoteexecution.config.RemoteExecutionConfig.DEFAULT_REMOTE_CONCURRENT_ACTION_COMPUTATIONS)

        []{#DEFAULT_REMOTE_CONCURRENT_PENDING_UPLOADS}

        -   #### DEFAULT_REMOTE_CONCURRENT_PENDING_UPLOADS

                public static final int DEFAULT_REMOTE_CONCURRENT_PENDING_UPLOADS

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.remoteexecution.config.RemoteExecutionConfig.DEFAULT_REMOTE_CONCURRENT_PENDING_UPLOADS)

        []{#DEFAULT_REMOTE_CONCURRENT_EXECUTIONS}

        -   #### DEFAULT_REMOTE_CONCURRENT_EXECUTIONS

                public static final int DEFAULT_REMOTE_CONCURRENT_EXECUTIONS

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.remoteexecution.config.RemoteExecutionConfig.DEFAULT_REMOTE_CONCURRENT_EXECUTIONS)

        []{#DEFAULT_REMOTE_CONCURRENT_RESULT_HANDLING}

        -   #### DEFAULT_REMOTE_CONCURRENT_RESULT_HANDLING

                public static final int DEFAULT_REMOTE_CONCURRENT_RESULT_HANDLING

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.remoteexecution.config.RemoteExecutionConfig.DEFAULT_REMOTE_CONCURRENT_RESULT_HANDLING)

        []{#DEFAULT_REMOTE_OUTPUT_MATERIALIZATION_THREADS}

        -   #### DEFAULT_REMOTE_OUTPUT_MATERIALIZATION_THREADS

                public static final int DEFAULT_REMOTE_OUTPUT_MATERIALIZATION_THREADS

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.remoteexecution.config.RemoteExecutionConfig.DEFAULT_REMOTE_OUTPUT_MATERIALIZATION_THREADS)

        []{#DEFAULT_IS_LOCAL_FALLBACK_ENABLED}

        -   #### DEFAULT_IS_LOCAL_FALLBACK_ENABLED

                public static final boolean DEFAULT_IS_LOCAL_FALLBACK_ENABLED

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.remoteexecution.config.RemoteExecutionConfig.DEFAULT_IS_LOCAL_FALLBACK_ENABLED)

        []{#DEFAULT_IS_LOCAL_FALLBACK_DISABLED_ON_CORRUPT_ARTIFACTS}

        -   #### DEFAULT_IS_LOCAL_FALLBACK_DISABLED_ON_CORRUPT_ARTIFACTS

                public static final boolean DEFAULT_IS_LOCAL_FALLBACK_DISABLED_ON_CORRUPT_ARTIFACTS

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.remoteexecution.config.RemoteExecutionConfig.DEFAULT_IS_LOCAL_FALLBACK_DISABLED_ON_CORRUPT_ARTIFACTS)

        []{#DEFAULT_IS_LOCAL_FALLBACK_ENABLED_FOR_COMPLETED_ACTION}

        -   #### DEFAULT_IS_LOCAL_FALLBACK_ENABLED_FOR_COMPLETED_ACTION

                public static final boolean DEFAULT_IS_LOCAL_FALLBACK_ENABLED_FOR_COMPLETED_ACTION

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.remoteexecution.config.RemoteExecutionConfig.DEFAULT_IS_LOCAL_FALLBACK_ENABLED_FOR_COMPLETED_ACTION)

        []{#TENANT_ID_KEY}

        -   #### TENANT_ID_KEY

                public static final String TENANT_ID_KEY

            ::: block
            Tenant ID that will be attached to each action \*
            :::

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.remoteexecution.config.RemoteExecutionConfig.TENANT_ID_KEY)

        []{#CONCURRENT_EXECUTIONS_KEY}

        -   #### CONCURRENT_EXECUTIONS_KEY

                public static final String CONCURRENT_EXECUTIONS_KEY

            ::: block
            Limit on the number of outstanding execution requests. This
            is probably the value that\'s most likely to be non-default.
            :::

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.remoteexecution.config.RemoteExecutionConfig.CONCURRENT_EXECUTIONS_KEY)

        []{#CONCURRENT_ACTION_COMPUTATIONS_KEY}

        -   #### CONCURRENT_ACTION_COMPUTATIONS_KEY

                public static final String CONCURRENT_ACTION_COMPUTATIONS_KEY

            ::: block
            Number of actions to compute at a time. These should be
            \<25ms average, but require I/O and cpu.
            :::

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.remoteexecution.config.RemoteExecutionConfig.CONCURRENT_ACTION_COMPUTATIONS_KEY)

        []{#CONCURRENT_RESULT_HANDLING_KEY}

        -   #### CONCURRENT_RESULT_HANDLING_KEY

                public static final String CONCURRENT_RESULT_HANDLING_KEY

            ::: block
            Number of results to concurrently handle at a time.
            :::

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.remoteexecution.config.RemoteExecutionConfig.CONCURRENT_RESULT_HANDLING_KEY)

        []{#OUTPUT_MATERIALIZATION_THREADS_KEY}

        -   #### OUTPUT_MATERIALIZATION_THREADS_KEY

                public static final String OUTPUT_MATERIALIZATION_THREADS_KEY

            ::: block
            Number of threads to handle output materialization.
            :::

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.remoteexecution.config.RemoteExecutionConfig.OUTPUT_MATERIALIZATION_THREADS_KEY)

        []{#IS_LOCAL_FALLBACK_ENABLED_KEY}

        -   #### IS_LOCAL_FALLBACK_ENABLED_KEY

                public static final String IS_LOCAL_FALLBACK_ENABLED_KEY

            ::: block
            Whether failed remote executions are retried locally.
            :::

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.remoteexecution.config.RemoteExecutionConfig.IS_LOCAL_FALLBACK_ENABLED_KEY)

        []{#IS_LOCAL_FALLBACK_DISABLED_ON_CORRUPT_ARTIFACTS_KEY}

        -   #### IS_LOCAL_FALLBACK_DISABLED_ON_CORRUPT_ARTIFACTS_KEY

                public static final String IS_LOCAL_FALLBACK_DISABLED_ON_CORRUPT_ARTIFACTS_KEY

            ::: block
            Whether failed remote executions are retried locally if the
            artifacts are corrupted.
            :::

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.remoteexecution.config.RemoteExecutionConfig.IS_LOCAL_FALLBACK_DISABLED_ON_CORRUPT_ARTIFACTS_KEY)

        []{#MAX_INPUT_SIZE_BYTES}

        -   #### MAX_INPUT_SIZE_BYTES

                public static final String MAX_INPUT_SIZE_BYTES

            ::: block
            The maximum size of inputs allowed on remote execution, if
            unset, no maximum.
            :::

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.remoteexecution.config.RemoteExecutionConfig.MAX_INPUT_SIZE_BYTES)

        []{#LARGE_BLOB_SIZE_BYTES}

        -   #### LARGE_BLOB_SIZE_BYTES

                public static final String LARGE_BLOB_SIZE_BYTES

            ::: block
            The large blob size bytes threshold, if unset, no threshold.
            :::

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.remoteexecution.config.RemoteExecutionConfig.LARGE_BLOB_SIZE_BYTES)

        []{#STRATEGY_WORKER_THREADS_KEY}

        -   #### STRATEGY_WORKER_THREADS_KEY

                public static final String STRATEGY_WORKER_THREADS_KEY

            ::: block
            Number of threads for the strategy to do its work. This
            doesn\'t need to be a lot, but should probably be greater
            than concurrent_result_handling below.
            :::

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.remoteexecution.config.RemoteExecutionConfig.STRATEGY_WORKER_THREADS_KEY)

        []{#CONCURRENT_PENDING_UPLOADS_KEY}

        -   #### CONCURRENT_PENDING_UPLOADS_KEY

                public static final String CONCURRENT_PENDING_UPLOADS_KEY

            ::: block
            Number of pending uploads at a time. While an action is
            pending uploads, it may hold a reference to some large-ish
            data (\>1MB). If this limit is reached, it will also block
            future action computations until uploads finish.
            :::

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.remoteexecution.config.RemoteExecutionConfig.CONCURRENT_PENDING_UPLOADS_KEY)

        []{#DEBUG_FORMAT_STRING_URL_KEY}

        -   #### DEBUG_FORMAT_STRING_URL_KEY

                public static final String DEBUG_FORMAT_STRING_URL_KEY

            ::: block
            URL format string for debug UI on the super console
            :::

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.remoteexecution.config.RemoteExecutionConfig.DEBUG_FORMAT_STRING_URL_KEY)

        []{#FORMAT_SESSION_ID_VARIABLE_STRING}

        -   #### FORMAT_SESSION_ID_VARIABLE_STRING

                public static final String FORMAT_SESSION_ID_VARIABLE_STRING

            ::: block
            The variable identifier string to be replace in any
            configured format defined by DEBUG_FORMAT_STRING_URL_KEY.
            This is being presented to avoid string duplication.
            :::

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.remoteexecution.config.RemoteExecutionConfig.FORMAT_SESSION_ID_VARIABLE_STRING)

        []{#MAX_WORKER_SIZE_TO_STEAL_FROM}

        -   #### MAX_WORKER_SIZE_TO_STEAL_FROM

                public static final String MAX_WORKER_SIZE_TO_STEAL_FROM

            ::: block
            Actions which require a worker of this size (or higher) will
            not be stolen locally when running in hybrid mode
            :::

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.remoteexecution.config.RemoteExecutionConfig.MAX_WORKER_SIZE_TO_STEAL_FROM)

        []{#RE_SESSION_LABEL_KEY}

        -   #### RE_SESSION_LABEL_KEY

                public static final String RE_SESSION_LABEL_KEY

            ::: block
            Free form string label that can be passed along any Remote
            Execution session. Useful for logging.
            :::

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.remoteexecution.config.RemoteExecutionConfig.RE_SESSION_LABEL_KEY)

        []{#WORKER_REQUIREMENTS_FILENAME}

        -   #### WORKER_REQUIREMENTS_FILENAME

                public static final String WORKER_REQUIREMENTS_FILENAME

            ::: block
            Worker requirements filename
            :::

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.remoteexecution.config.RemoteExecutionConfig.WORKER_REQUIREMENTS_FILENAME)

        []{#TRY_LARGER_WORKER_ON_OOM}

        -   #### TRY_LARGER_WORKER_ON_OOM

                public static final String TRY_LARGER_WORKER_ON_OOM

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.remoteexecution.config.RemoteExecutionConfig.TRY_LARGER_WORKER_ON_OOM)

        []{#IS_LOCAL_FALLBACK_ENABLED_FOR_COMPLETED_ACTION_KEY}

        -   #### IS_LOCAL_FALLBACK_ENABLED_FOR_COMPLETED_ACTION_KEY

                public static final String IS_LOCAL_FALLBACK_ENABLED_FOR_COMPLETED_ACTION_KEY

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.remoteexecution.config.RemoteExecutionConfig.IS_LOCAL_FALLBACK_ENABLED_FOR_COMPLETED_ACTION_KEY)

        []{#AUTO_RE_BUILD_PROJECTS_WHITELIST_KEY}

        -   #### AUTO_RE_BUILD_PROJECTS_WHITELIST_KEY

                public static final String AUTO_RE_BUILD_PROJECTS_WHITELIST_KEY

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.remoteexecution.config.RemoteExecutionConfig.AUTO_RE_BUILD_PROJECTS_WHITELIST_KEY)

        []{#AUTO_RE_BUILD_USERS_BLACKLIST_KEY}

        -   #### AUTO_RE_BUILD_USERS_BLACKLIST_KEY

                public static final String AUTO_RE_BUILD_USERS_BLACKLIST_KEY

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.remoteexecution.config.RemoteExecutionConfig.AUTO_RE_BUILD_USERS_BLACKLIST_KEY)

        []{#INPUT_IGNORE_KEY}

        -   #### INPUT_IGNORE_KEY

                public static final String INPUT_IGNORE_KEY

            ::: block
            Input paths to ignore for actions
            :::

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.remoteexecution.config.RemoteExecutionConfig.INPUT_IGNORE_KEY)

        []{#AUTO_RE_STRATEGY_KEY}

        -   #### AUTO_RE_STRATEGY_KEY

                public static final String AUTO_RE_STRATEGY_KEY

            ::: block
            Strategy used to determine whether to enable Remote
            Execution automatically for the current build
            :::

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.remoteexecution.config.RemoteExecutionConfig.AUTO_RE_STRATEGY_KEY)

        []{#BUILD_TAGS_KEY}

        -   #### BUILD_TAGS_KEY

                public static final String BUILD_TAGS_KEY

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.remoteexecution.config.RemoteExecutionConfig.BUILD_TAGS_KEY)

        []{#AUTO_RE_EXPERIMENT_PROPERTY_KEY}

        -   #### AUTO_RE_EXPERIMENT_PROPERTY_KEY

                public static final String AUTO_RE_EXPERIMENT_PROPERTY_KEY

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.remoteexecution.config.RemoteExecutionConfig.AUTO_RE_EXPERIMENT_PROPERTY_KEY)

        []{#DEFAULT_AUTO_RE_EXPERIMENT_PROPERTY}

        -   #### DEFAULT_AUTO_RE_EXPERIMENT_PROPERTY

                public static final String DEFAULT_AUTO_RE_EXPERIMENT_PROPERTY

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.remoteexecution.config.RemoteExecutionConfig.DEFAULT_AUTO_RE_EXPERIMENT_PROPERTY)

        []{#USE_REMOTE_EXECUTION_FOR_GENRULE_IF_REQUESTED_FORMAT}

        -   #### USE_REMOTE_EXECUTION_FOR_GENRULE_IF_REQUESTED_FORMAT

                public static final String USE_REMOTE_EXECUTION_FOR_GENRULE_IF_REQUESTED_FORMAT

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.remoteexecution.config.RemoteExecutionConfig.USE_REMOTE_EXECUTION_FOR_GENRULE_IF_REQUESTED_FORMAT)
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### RemoteExecutionConfig

                public RemoteExecutionConfig()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#of(com.facebook.buck.core.config.BuckConfig)}

        -   #### of

            ``` methodSignature
            public static RemoteExecutionConfig of​(BuckConfig delegate)
            ```

        []{#getUseRemoteExecutionForGenruleIfRequestedField(java.lang.String)}

        -   #### getUseRemoteExecutionForGenruleIfRequestedField

            ``` methodSignature
            public static String getUseRemoteExecutionForGenruleIfRequestedField​(String type)
            ```

        []{#shouldUseRemoteExecutionForGenruleIfRequested(java.lang.String)}

        -   #### shouldUseRemoteExecutionForGenruleIfRequested

            ``` methodSignature
            public boolean shouldUseRemoteExecutionForGenruleIfRequested​(String type)
            ```

            ::: block
            Returns whether or not we should honor the \`remote\`
            argument to \`genrule\`, which requests that the genrule run
            remotely.
            :::

        []{#isRemoteExecutionAutoEnabled(java.lang.String,java.util.List)}

        -   #### isRemoteExecutionAutoEnabled

            ``` methodSignature
            public boolean isRemoteExecutionAutoEnabled​(String username,
                                                        List<String> commandArguments)
            ```

        []{#getRemoteHost()}

        -   #### getRemoteHost

            ``` methodSignature
            public String getRemoteHost()
            ```

        []{#getRemotePort()}

        -   #### getRemotePort

            ``` methodSignature
            public int getRemotePort()
            ```

        []{#getCasHost()}

        -   #### getCasHost

            ``` methodSignature
            public String getCasHost()
            ```

        []{#getCasPort()}

        -   #### getCasPort

            ``` methodSignature
            public int getCasPort()
            ```

        []{#getCasDeadline()}

        -   #### getCasDeadline

            ``` methodSignature
            public int getCasDeadline()
            ```

        []{#getInsecure()}

        -   #### getInsecure

            ``` methodSignature
            public boolean getInsecure()
            ```

        []{#getCasInsecure()}

        -   #### getCasInsecure

            ``` methodSignature
            public boolean getCasInsecure()
            ```

        []{#getCertFile()}

        -   #### getCertFile

            ``` methodSignature
            public Optional<Path> getCertFile()
            ```

            ::: block
            client TLS certificate file in PEM format
            :::

        []{#getKeyFile()}

        -   #### getKeyFile

            ``` methodSignature
            public Optional<Path> getKeyFile()
            ```

            ::: block
            client TLS private key in PEM format
            :::

        []{#getCertificateAuthoritiesFile()}

        -   #### getCertificateAuthoritiesFile

            ``` methodSignature
            public Optional<Path> getCertificateAuthoritiesFile()
            ```

            ::: block
            file containing all TLS authorities to verify server
            certificate with (PEM format)
            :::

        []{#getMaxWorkerSizeToStealFrom()}

        -   #### getMaxWorkerSizeToStealFrom

            ``` methodSignature
            public Optional<com.facebook.buck.remoteexecution.proto.WorkerRequirements.WorkerSize> getMaxWorkerSizeToStealFrom()
            ```

        []{#getTenantId()}

        -   #### getTenantId

            ``` methodSignature
            public String getTenantId()
            ```

        []{#getDebugURLString(com.facebook.buck.remoteexecution.proto.RESessionID)}

        -   #### getDebugURLString

            ``` methodSignature
            public String getDebugURLString​(com.facebook.buck.remoteexecution.proto.RESessionID reSessionID)
            ```

        []{#isDebug()}

        -   #### isDebug

            ``` methodSignature
            public boolean isDebug()
            ```

        []{#getStrategyConfig()}

        -   #### getStrategyConfig

            ``` methodSignature
            @Derived
            public RemoteExecutionStrategyConfig getStrategyConfig()
            ```

        []{#getType()}

        -   #### getType

            ``` methodSignature
            public RemoteExecutionType getType()
            ```

        []{#isConsoleEnabled()}

        -   #### isConsoleEnabled

            ``` methodSignature
            public boolean isConsoleEnabled()
            ```

            ::: block
            Whether Console output of Remote Execution information is
            enabled.
            :::

        []{#getReSessionLabel()}

        -   #### getReSessionLabel

            ``` methodSignature
            public String getReSessionLabel()
            ```

        []{#getAuxiliaryBuildTag()}

        -   #### getAuxiliaryBuildTag

            ``` methodSignature
            public String getAuxiliaryBuildTag()
            ```

            ::: block
            Provides an auxiliary tag used for capturing any custom
            configurations.
            :::

        []{#validateCertificatesOrThrow()}

        -   #### validateCertificatesOrThrow

            ``` methodSignature
            public void validateCertificatesOrThrow()
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
