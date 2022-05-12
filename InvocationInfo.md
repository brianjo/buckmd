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
[Package]{.packageLabelInType} [com.facebook.buck.log](package-summary.html)
:::

## Class InvocationInfo {#class-invocationinfo .title title="Class InvocationInfo"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.log.InvocationInfo

::: description
-   

    ------------------------------------------------------------------------

        public abstract class InvocationInfo
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor          Description
          -------------------- -------------
          `InvocationInfo()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                            Method                                                                                                                                                                                                                                                                                                                                                         Description
          ------------------------------------------------------------ -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `abstract Path`                                              `getBuckLogDir()`                                                                                                                                                                                                                                                                                                                                               
          `abstract BuildId`                                           `getBuildId()`                                                                                                                                                                                                                                                                                                                                                  
          `abstract com.google.common.collect.ImmutableList<String>`   `getCommandArgs()`                                                                                                                                                                                                                                                                                                                                              
          `String`                                                     `getCommandId()`                                                                                                                                                                                                                                                                                                                                                
          `abstract boolean`                                           `getIsDaemon()`                                                                                                                                                                                                                                                                                                                                                 
          `abstract boolean`                                           `getIsRemoteExecution()`                                                                                                                                                                                                                                                                                                                                        
          `Path`                                                       `getLogDirectoryPath()`                                                                                                                                                                                                                                                                                                                                         
          `Path`                                                       `getLogFilePath()`                                                                                                                                                                                                                                                                                                                                              
          `abstract String`                                            `getRepository()`                                                                                                                                                                                                                                                                                                                                               
          `Path`                                                       `getSimpleConsoleOutputFilePath()`                                                                                                                                                                                                                                                                                                                              
          `abstract String`                                            `getSubCommand()`                                                                                                                                                                                                                                                                                                                                               
          `abstract boolean`                                           `getSuperConsoleEnabled()`                                                                                                                                                                                                                                                                                                                                      
          `abstract long`                                              `getTimestampMillis()`                                                                                                                                                                                                                                                                                                                                          
          `abstract com.google.common.collect.ImmutableList<String>`   `getUnexpandedCommandArgs()`                                                                                                                                                                                                                                                                                                                                    
          `abstract String`                                            `getWatchmanVersion()`                                                                                                                                                                                                                                                                                                                                          
          `static InvocationInfo`                                      `of​(BuildId buildId,   boolean superConsoleEnabled,   boolean isDaemon,   String subCommand,   com.google.common.collect.ImmutableList<String> commandArgs,   com.google.common.collect.ImmutableList<String> unexpandedCommandArgs,   Path buckLogDir,   boolean isRemoteExecution,   String repository,   String watchmanVersion)`                            
          `static InvocationInfo`                                      `of​(BuildId buildId,   boolean superConsoleEnabled,   boolean isDaemon,   String subCommand,   com.google.common.collect.ImmutableList<String> commandArgs,   com.google.common.collect.ImmutableList<String> unexpandedCommandArgs,   Path buckLogDir,   boolean isRemoteExecution,   String repository,   String watchmanVersion,   long timestampMillis)`    
          `String`                                                     `toLogLine()`                                                                                                                                                                                                                                                                                                                                                   
          `String`                                                     `toString()`                                                                                                                                                                                                                                                                                                                                                    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
          Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
          .tableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Abstract
          Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### InvocationInfo

                public InvocationInfo()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getBuildId()}

        -   #### getBuildId

            ``` methodSignature
            public abstract BuildId getBuildId()
            ```

        []{#getSuperConsoleEnabled()}

        -   #### getSuperConsoleEnabled

            ``` methodSignature
            public abstract boolean getSuperConsoleEnabled()
            ```

        []{#getIsDaemon()}

        -   #### getIsDaemon

            ``` methodSignature
            public abstract boolean getIsDaemon()
            ```

        []{#getSubCommand()}

        -   #### getSubCommand

            ``` methodSignature
            public abstract String getSubCommand()
            ```

        []{#getCommandArgs()}

        -   #### getCommandArgs

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableList<String> getCommandArgs()
            ```

        []{#getUnexpandedCommandArgs()}

        -   #### getUnexpandedCommandArgs

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableList<String> getUnexpandedCommandArgs()
            ```

        []{#getBuckLogDir()}

        -   #### getBuckLogDir

            ``` methodSignature
            public abstract Path getBuckLogDir()
            ```

        []{#getCommandId()}

        -   #### getCommandId

            ``` methodSignature
            public String getCommandId()
            ```

        []{#toLogLine()}

        -   #### toLogLine

            ``` methodSignature
            public String toLogLine()
            ```

        []{#getIsRemoteExecution()}

        -   #### getIsRemoteExecution

            ``` methodSignature
            public abstract boolean getIsRemoteExecution()
            ```

        []{#getRepository()}

        -   #### getRepository

            ``` methodSignature
            public abstract String getRepository()
            ```

        []{#getWatchmanVersion()}

        -   #### getWatchmanVersion

            ``` methodSignature
            public abstract String getWatchmanVersion()
            ```

        []{#getTimestampMillis()}

        -   #### getTimestampMillis

            ``` methodSignature
            public abstract long getTimestampMillis()
            ```

        []{#getLogDirectoryPath()}

        -   #### getLogDirectoryPath

            ``` methodSignature
            public Path getLogDirectoryPath()
            ```

        []{#getLogFilePath()}

        -   #### getLogFilePath

            ``` methodSignature
            public Path getLogFilePath()
            ```

        []{#getSimpleConsoleOutputFilePath()}

        -   #### getSimpleConsoleOutputFilePath

            ``` methodSignature
            public Path getSimpleConsoleOutputFilePath()
            ```

        []{#toString()}

        -   #### toString

            ``` methodSignature
            public String toString()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `toString` in class `Object`

        []{#of(com.facebook.buck.core.model.BuildId,boolean,boolean,java.lang.String,com.google.common.collect.ImmutableList,com.google.common.collect.ImmutableList,java.nio.file.Path,boolean,java.lang.String,java.lang.String)}

        -   #### of

            ``` methodSignature
            public static InvocationInfo of​(BuildId buildId,
                                            boolean superConsoleEnabled,
                                            boolean isDaemon,
                                            String subCommand,
                                            com.google.common.collect.ImmutableList<String> commandArgs,
                                            com.google.common.collect.ImmutableList<String> unexpandedCommandArgs,
                                            Path buckLogDir,
                                            boolean isRemoteExecution,
                                            String repository,
                                            String watchmanVersion)
            ```

        []{#of(com.facebook.buck.core.model.BuildId,boolean,boolean,java.lang.String,com.google.common.collect.ImmutableList,com.google.common.collect.ImmutableList,java.nio.file.Path,boolean,java.lang.String,java.lang.String,long)}

        -   #### of

            ``` methodSignature
            public static InvocationInfo of​(BuildId buildId,
                                            boolean superConsoleEnabled,
                                            boolean isDaemon,
                                            String subCommand,
                                            com.google.common.collect.ImmutableList<String> commandArgs,
                                            com.google.common.collect.ImmutableList<String> unexpandedCommandArgs,
                                            Path buckLogDir,
                                            boolean isRemoteExecution,
                                            String repository,
                                            String watchmanVersion,
                                            long timestampMillis)
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
