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
[Package]{.packageLabelInType} [com.facebook.buck.doctor.config](package-summary.html)
:::

## Interface BuildLogEntry {#interface-buildlogentry .title title="Interface BuildLogEntry"}
:::

::: contentContainer
::: description
-   

    ------------------------------------------------------------------------

        public interface BuildLogEntry
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type          Method                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              Description
          -------------------------- --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `Optional<Path>`           `getBuckFixSpecFile()`                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               
          `Optional<BuildId>`        `getBuildId()`                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       
          `OptionalInt`              `getBuildTimeMs()`                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   
          `Optional<List<String>>`   `getCommandArgs()`                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   
          `Optional<Path>`           `getConfigJsonFile()`                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                
          `OptionalInt`              `getExitCode()`                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      
          `Optional<List<String>>`   `getExpandedCommandArgs()`                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           
          `Date`                     `getLastModifiedTime()`                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              
          `Optional<Path>`           `getMachineReadableLogFile()`                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        
          `Path`                     `getRelativePath()`                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  
          `Optional<Path>`           `getRuleKeyDiagGraphFile()`                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          
          `Optional<Path>`           `getRuleKeyDiagKeysFile()`                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           
          `Optional<Path>`           `getRuleKeyLoggerLogFile()`                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          
          `long`                     `getSize()`                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          
          `Optional<Path>`           `getTraceFile()`                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     
          `static BuildLogEntry`     `of​(Path relativePath,   Optional<? extends BuildId> buildId,   Optional<? extends List<String>> commandArgs,   Optional<? extends List<String>> expandedCommandArgs,   OptionalInt exitCode,   OptionalInt buildTimeMs,   Optional<? extends Path> ruleKeyLoggerLogFile,   Optional<? extends Path> machineReadableLogFile,   Optional<? extends Path> ruleKeyDiagKeysFile,   Optional<? extends Path> ruleKeyDiagGraphFile,   Optional<? extends Path> traceFile,   Optional<? extends Path> configJsonFile,   Optional<? extends Path> buckFixSpecFile,   long size,   Date lastModifiedTime)`    
          `default void`             `pathIsRelative()`                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
          Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
          .tableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Abstract
          Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
          .tableTab}[[Default
          Methods](javascript:show(16);)[ ]{.tabEnd}]{#t5 .tableTab}
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getRelativePath()}

        -   #### getRelativePath

            ``` methodSignature
            Path getRelativePath()
            ```

        []{#getBuildId()}

        -   #### getBuildId

            ``` methodSignature
            Optional<BuildId> getBuildId()
            ```

        []{#getCommandArgs()}

        -   #### getCommandArgs

            ``` methodSignature
            Optional<List<String>> getCommandArgs()
            ```

        []{#getExpandedCommandArgs()}

        -   #### getExpandedCommandArgs

            ``` methodSignature
            Optional<List<String>> getExpandedCommandArgs()
            ```

        []{#getExitCode()}

        -   #### getExitCode

            ``` methodSignature
            OptionalInt getExitCode()
            ```

        []{#getBuildTimeMs()}

        -   #### getBuildTimeMs

            ``` methodSignature
            OptionalInt getBuildTimeMs()
            ```

        []{#getRuleKeyLoggerLogFile()}

        -   #### getRuleKeyLoggerLogFile

            ``` methodSignature
            Optional<Path> getRuleKeyLoggerLogFile()
            ```

        []{#getMachineReadableLogFile()}

        -   #### getMachineReadableLogFile

            ``` methodSignature
            Optional<Path> getMachineReadableLogFile()
            ```

        []{#getRuleKeyDiagKeysFile()}

        -   #### getRuleKeyDiagKeysFile

            ``` methodSignature
            Optional<Path> getRuleKeyDiagKeysFile()
            ```

        []{#getRuleKeyDiagGraphFile()}

        -   #### getRuleKeyDiagGraphFile

            ``` methodSignature
            Optional<Path> getRuleKeyDiagGraphFile()
            ```

        []{#getTraceFile()}

        -   #### getTraceFile

            ``` methodSignature
            Optional<Path> getTraceFile()
            ```

        []{#getConfigJsonFile()}

        -   #### getConfigJsonFile

            ``` methodSignature
            Optional<Path> getConfigJsonFile()
            ```

        []{#getBuckFixSpecFile()}

        -   #### getBuckFixSpecFile

            ``` methodSignature
            Optional<Path> getBuckFixSpecFile()
            ```

        []{#getSize()}

        -   #### getSize

            ``` methodSignature
            long getSize()
            ```

        []{#getLastModifiedTime()}

        -   #### getLastModifiedTime

            ``` methodSignature
            Date getLastModifiedTime()
            ```

        []{#pathIsRelative()}

        -   #### pathIsRelative

            ``` methodSignature
            @Check
            default void pathIsRelative()
            ```

        []{#of(java.nio.file.Path,java.util.Optional,java.util.Optional,java.util.Optional,java.util.OptionalInt,java.util.OptionalInt,java.util.Optional,java.util.Optional,java.util.Optional,java.util.Optional,java.util.Optional,java.util.Optional,java.util.Optional,long,java.util.Date)}

        -   #### of

            ``` methodSignature
            static BuildLogEntry of​(Path relativePath,
                                    Optional<? extends BuildId> buildId,
                                    Optional<? extends List<String>> commandArgs,
                                    Optional<? extends List<String>> expandedCommandArgs,
                                    OptionalInt exitCode,
                                    OptionalInt buildTimeMs,
                                    Optional<? extends Path> ruleKeyLoggerLogFile,
                                    Optional<? extends Path> machineReadableLogFile,
                                    Optional<? extends Path> ruleKeyDiagKeysFile,
                                    Optional<? extends Path> ruleKeyDiagGraphFile,
                                    Optional<? extends Path> traceFile,
                                    Optional<? extends Path> configJsonFile,
                                    Optional<? extends Path> buckFixSpecFile,
                                    long size,
                                    Date lastModifiedTime)
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
