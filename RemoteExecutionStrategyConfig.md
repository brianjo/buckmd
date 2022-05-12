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
[Package]{.packageLabelInType} [com.facebook.buck.remoteexecution.config](package-summary.html)
:::

## Interface RemoteExecutionStrategyConfig {#interface-remoteexecutionstrategyconfig .title title="Interface RemoteExecutionStrategyConfig"}
:::

::: contentContainer
::: description
-   

    ------------------------------------------------------------------------

        public interface RemoteExecutionStrategyConfig

    ::: block
    Configuration for the remote execution strategy.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                       Method                                            Description
          ------------------------------------------------------- ------------------------------------------------- -------------
          `com.google.common.collect.ImmutableSet<PathMatcher>`   `getIgnorePaths()`                                 
          `int`                                                   `getMaxConcurrentActionComputations()`             
          `int`                                                   `getMaxConcurrentExecutions()`                     
          `int`                                                   `getMaxConcurrentPendingUploads()`                 
          `int`                                                   `getMaxConcurrentResultHandling()`                 
          `int`                                                   `getOutputMaterializationThreads()`                
          `int`                                                   `getThreads()`                                     
          `String`                                                `getWorkerRequirementsFilename()`                  
          `boolean`                                               `isLocalFallbackDisabledOnCorruptedArtifacts()`    
          `boolean`                                               `isLocalFallbackEnabled()`                         
          `boolean`                                               `isLocalFallbackEnabledForCompletedAction()`       
          `OptionalLong`                                          `largeBlobSizeBytes()`                             
          `OptionalLong`                                          `maxInputSizeBytes()`                              
          `boolean`                                               `tryLargerWorkerOnOom()`                           

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

        []{#getThreads()}

        -   #### getThreads

            ``` methodSignature
            int getThreads()
            ```

        []{#getMaxConcurrentActionComputations()}

        -   #### getMaxConcurrentActionComputations

            ``` methodSignature
            int getMaxConcurrentActionComputations()
            ```

        []{#getMaxConcurrentExecutions()}

        -   #### getMaxConcurrentExecutions

            ``` methodSignature
            int getMaxConcurrentExecutions()
            ```

        []{#getMaxConcurrentResultHandling()}

        -   #### getMaxConcurrentResultHandling

            ``` methodSignature
            int getMaxConcurrentResultHandling()
            ```

        []{#getOutputMaterializationThreads()}

        -   #### getOutputMaterializationThreads

            ``` methodSignature
            int getOutputMaterializationThreads()
            ```

        []{#getMaxConcurrentPendingUploads()}

        -   #### getMaxConcurrentPendingUploads

            ``` methodSignature
            int getMaxConcurrentPendingUploads()
            ```

        []{#isLocalFallbackEnabled()}

        -   #### isLocalFallbackEnabled

            ``` methodSignature
            boolean isLocalFallbackEnabled()
            ```

        []{#isLocalFallbackDisabledOnCorruptedArtifacts()}

        -   #### isLocalFallbackDisabledOnCorruptedArtifacts

            ``` methodSignature
            boolean isLocalFallbackDisabledOnCorruptedArtifacts()
            ```

        []{#isLocalFallbackEnabledForCompletedAction()}

        -   #### isLocalFallbackEnabledForCompletedAction

            ``` methodSignature
            boolean isLocalFallbackEnabledForCompletedAction()
            ```

        []{#maxInputSizeBytes()}

        -   #### maxInputSizeBytes

            ``` methodSignature
            OptionalLong maxInputSizeBytes()
            ```

        []{#largeBlobSizeBytes()}

        -   #### largeBlobSizeBytes

            ``` methodSignature
            OptionalLong largeBlobSizeBytes()
            ```

        []{#getWorkerRequirementsFilename()}

        -   #### getWorkerRequirementsFilename

            ``` methodSignature
            String getWorkerRequirementsFilename()
            ```

        []{#tryLargerWorkerOnOom()}

        -   #### tryLargerWorkerOnOom

            ``` methodSignature
            boolean tryLargerWorkerOnOom()
            ```

        []{#getIgnorePaths()}

        -   #### getIgnorePaths

            ``` methodSignature
            com.google.common.collect.ImmutableSet<PathMatcher> getIgnorePaths()
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
