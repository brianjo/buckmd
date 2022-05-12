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
[Package]{.packageLabelInType} [com.facebook.buck.core.toolchain](package-summary.html)
:::

## Interface ToolchainCreationContext {#interface-toolchaincreationcontext .title title="Interface ToolchainCreationContext"}
:::

::: contentContainer
::: description
-   

    ------------------------------------------------------------------------

        public interface ToolchainCreationContext

    ::: block
    Contains objects that can be used during the creation of a
    toolchain.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                         Method                                                                                                                                                                                                                         Description
          --------------------------------------------------------- ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ -------------
          `BuckConfig`                                              `getBuckConfig()`                                                                                                                                                                                                               
          `com.google.common.collect.ImmutableMap<String,​String>`   `getEnvironment()`                                                                                                                                                                                                              
          `ExecutableFinder`                                        `getExecutableFinder()`                                                                                                                                                                                                         
          `ProjectFilesystem`                                       `getFilesystem()`                                                                                                                                                                                                               
          `ProcessExecutor`                                         `getProcessExecutor()`                                                                                                                                                                                                          
          `RuleKeyConfiguration`                                    `getRuleKeyConfiguration()`                                                                                                                                                                                                     
          `static ToolchainCreationContext`                         `of​(Map<String,​? extends String> environment,   BuckConfig buckConfig,   ProjectFilesystem filesystem,   ProcessExecutor processExecutor,   ExecutableFinder executableFinder,   RuleKeyConfiguration ruleKeyConfiguration)`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
          Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
          .tableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Abstract
          Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getEnvironment()}

        -   #### getEnvironment

            ``` methodSignature
            com.google.common.collect.ImmutableMap<String,​String> getEnvironment()
            ```

        []{#getBuckConfig()}

        -   #### getBuckConfig

            ``` methodSignature
            BuckConfig getBuckConfig()
            ```

        []{#getFilesystem()}

        -   #### getFilesystem

            ``` methodSignature
            ProjectFilesystem getFilesystem()
            ```

        []{#getProcessExecutor()}

        -   #### getProcessExecutor

            ``` methodSignature
            ProcessExecutor getProcessExecutor()
            ```

        []{#getExecutableFinder()}

        -   #### getExecutableFinder

            ``` methodSignature
            ExecutableFinder getExecutableFinder()
            ```

        []{#getRuleKeyConfiguration()}

        -   #### getRuleKeyConfiguration

            ``` methodSignature
            RuleKeyConfiguration getRuleKeyConfiguration()
            ```

        []{#of(java.util.Map,com.facebook.buck.core.config.BuckConfig,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.util.ProcessExecutor,com.facebook.buck.io.ExecutableFinder,com.facebook.buck.rules.keys.config.RuleKeyConfiguration)}

        -   #### of

            ``` methodSignature
            static ToolchainCreationContext of​(Map<String,​? extends String> environment,
                                               BuckConfig buckConfig,
                                               ProjectFilesystem filesystem,
                                               ProcessExecutor processExecutor,
                                               ExecutableFinder executableFinder,
                                               RuleKeyConfiguration ruleKeyConfiguration)
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
