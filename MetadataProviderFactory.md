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
[Package]{.packageLabelInType} [com.facebook.buck.remoteexecution](package-summary.html)
:::

## Class MetadataProviderFactory {#class-metadataproviderfactory .title title="Class MetadataProviderFactory"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.remoteexecution.MetadataProviderFactory

::: description
-   

    ------------------------------------------------------------------------

        public class MetadataProviderFactory
        extends Object

    ::: block
    Static class providing factory methods for instances of
    MetadataProviders.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `sta                  | `emp                  |                       |
        | tic MetadataProvider` | tyMetadataProvider()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `sta                  | `mi                   |                       |
        | tic MetadataProvider` | nimalMetadataProvider |                       |
        |                       | ForBuild​(BuildId buil |                       |
        |                       | dId,                  |                       |
        |                       |                String |                       |
        |                       |  username,            |                       |
        |                       |                       |                       |
        |                       | String repository,    |                       |
        |                       |                       |                       |
        |                       |         String schedu |                       |
        |                       | leType,               |                       |
        |                       |                   Str |                       |
        |                       | ing reSessionLabel,   |                       |
        |                       |                       |                       |
        |                       |          String tenan |                       |
        |                       | tId,                  |                       |
        |                       |                String |                       |
        |                       |  auxiliaryBuildTag,   |                       |
        |                       |                       |                       |
        |                       |          String proje |                       |
        |                       | ctPrefix,             |                       |
        |                       |                     E |                       |
        |                       | xecutionEnvironment e |                       |
        |                       | xecutionEnvironment)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `sta                  | `wr                   | ::: block             |
        | tic MetadataProvider` | apForRuleWithWorkerRe | Wraps the argument    |
        |                       | quirements​(MetadataPr | MetadataProvider with |
        |                       | ovider metadataProvid | worker requirements   |
        |                       | er,                   | info                  |
        |                       |                 java. | :::                   |
        |                       | util.function.Supplie |                       |
        |                       | r<com.facebook.buck.r |                       |
        |                       | emoteexecution.proto. |                       |
        |                       | WorkerRequirements> r |                       |
        |                       | equirementsSupplier)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `sta                  | `wr                   | ::: block             |
        | tic MetadataProvider` | apWithTraceInfo​(Metad | Wraps the argument    |
        |                       | ataProvider metadataP | MetadataProvider      |
        |                       | rovider,              | return value with     |
        |                       |      TraceInfoProvide | info about tracing.   |
        |                       | r traceInfoProvider)` | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
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

        []{#emptyMetadataProvider()}

        -   #### emptyMetadataProvider

            ``` methodSignature
            public static MetadataProvider emptyMetadataProvider()
            ```

            [Returns:]{.returnLabel}
            :   Metadata provider that always returns empty Metadata.

        []{#minimalMetadataProviderForBuild(com.facebook.buck.core.model.BuildId,java.lang.String,java.lang.String,java.lang.String,java.lang.String,java.lang.String,java.lang.String,java.lang.String,com.facebook.buck.util.environment.ExecutionEnvironment)}

        -   #### minimalMetadataProviderForBuild

            ``` methodSignature
            public static MetadataProvider minimalMetadataProviderForBuild​(BuildId buildId,
                                                                           String username,
                                                                           String repository,
                                                                           String scheduleType,
                                                                           String reSessionLabel,
                                                                           String tenantId,
                                                                           String auxiliaryBuildTag,
                                                                           String projectPrefix,
                                                                           ExecutionEnvironment executionEnvironment)
            ```

            [Returns:]{.returnLabel}
            :   Metadata provider that provides minimal amount
                information that should be passed along remote execution
                requests.

        []{#wrapWithTraceInfo(com.facebook.buck.remoteexecution.interfaces.MetadataProvider,com.facebook.buck.log.TraceInfoProvider)}

        -   #### wrapWithTraceInfo

            ``` methodSignature
            public static MetadataProvider wrapWithTraceInfo​(MetadataProvider metadataProvider,
                                                             TraceInfoProvider traceInfoProvider)
            ```

            ::: block
            Wraps the argument MetadataProvider return value with info
            about tracing.
            :::

        []{#wrapForRuleWithWorkerRequirements(com.facebook.buck.remoteexecution.interfaces.MetadataProvider,java.util.function.Supplier)}

        -   #### wrapForRuleWithWorkerRequirements

            ``` methodSignature
            public static MetadataProvider wrapForRuleWithWorkerRequirements​(MetadataProvider metadataProvider,
                                                                             java.util.function.Supplier<com.facebook.buck.remoteexecution.proto.WorkerRequirements> requirementsSupplier)
            ```

            ::: block
            Wraps the argument MetadataProvider with worker requirements
            info
            :::
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
