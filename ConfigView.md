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
[Package]{.packageLabelInType} [com.facebook.buck.core.config](package-summary.html)
:::

## Interface ConfigView\<T\> {#interface-configviewt .title title="Interface ConfigView"}
:::

::: contentContainer
::: description
-   

    [Type Parameters:]{.paramLabel}
    :   `T` - Config type.

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `ActionGraphConfig`, `AdbConfig`, `AliasConfig`, `AppleConfig`,
        `ArtifactCacheBuckConfig`, `BuildBuckConfig`,
        `BuildReportConfig`, `CachingBuildEngineBuckConfig`,
        `ChromeTraceBuckConfig`, `CleanCommandBuckConfig`, `CliConfig`,
        `ConfigIgnoredByDaemon`, `CounterBuckConfig`,
        `DepsAwareExecutorConfig`, `DoctorConfig`, `DotnetBuckConfig`,
        `ErrorHandlingBuckConfig`, `FixBuckConfig`, `InferConfig`,
        `JavaBuckConfig`, `KotlinBuckConfig`, `LogBuckConfig`,
        `ModernBuildRuleConfig`, `ParserConfig`,
        `RemoteExecutionConfig`, `ResourcesConfig`,
        `RuleAnalysisConfig`, `RuleKeyConfig`, `SandboxConfig`,
        `ScribeEventListenerConfig`, `SwiftBuckConfig`,
        `TestBuckConfig`, `ToolConfig`

    ------------------------------------------------------------------------

        public interface ConfigView<T>

    ::: block
    A view of a particular config class.
    A config class may implement extra state and accessors beyond the
    bare Config. ConfigViews provides domain-specific accessors to
    Config values.

    ConfigViews should be defined following this pattern.

         @BuckStyleValue
          abstract class FooConfigView implements ConfigView {
            // Additional accessors.

            static FooConfigView of(T delegate) {
              return ImmutableFooConfigView.of(delegate);
            }
          }
         

    Config views should also not declare any additional non-derived
    immutable fields if it\'s to be used with
    [`ConfigViewCache`](ConfigViewCache.html "class in com.facebook.buck.core.config").
    As the cache assumes one-to-one correspondence with the main config
    instance, it uses the generated factory
    `FooConfigView.of(T delegate)` to instantiate the view.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method            Description
          ------------------- ----------------- -------------
          `T`                 `getDelegate()`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Abstract
          Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getDelegate()}

        -   #### getDelegate

            ``` methodSignature
            T getDelegate()
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
