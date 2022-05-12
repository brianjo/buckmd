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
[Package]{.packageLabelInType} [com.facebook.buck.command](package-summary.html)
:::

## Class BuildExecutorArgs {#class-buildexecutorargs .title title="Class BuildExecutorArgs"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.command.BuildExecutorArgs

::: description
-   

    ------------------------------------------------------------------------

        public abstract class BuildExecutorArgs
        extends Object

    ::: block
    Common arguments for running a build.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor             Description
          ----------------------- -------------
          `BuildExecutorArgs()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                                                                            Method                                                                                                                                                                                                                                                                                                                                                                                                    Description
          ---------------------------------------------------------------------------------------------------------------------------- --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `abstract ArtifactCacheFactory`                                                                                              `getArtifactCacheFactory()`                                                                                                                                                                                                                                                                                                                                                                                
          `BuckConfig`                                                                                                                 `getBuckConfig()`                                                                                                                                                                                                                                                                                                                                                                                          
          `abstract BuckEventBus`                                                                                                      `getBuckEventBus()`                                                                                                                                                                                                                                                                                                                                                                                        
          `abstract BuildInfoStoreManager`                                                                                             `getBuildInfoStoreManager()`                                                                                                                                                                                                                                                                                                                                                                               
          `abstract Cells`                                                                                                             `getCells()`                                                                                                                                                                                                                                                                                                                                                                                               
          `abstract Clock`                                                                                                             `getClock()`                                                                                                                                                                                                                                                                                                                                                                                               
          `abstract Console`                                                                                                           `getConsole()`                                                                                                                                                                                                                                                                                                                                                                                             
          `abstract com.google.common.collect.ImmutableMap<ExecutorPool,​com.google.common.util.concurrent.ListeningExecutorService>`   `getExecutors()`                                                                                                                                                                                                                                                                                                                                                                                           
          `abstract Platform`                                                                                                          `getPlatform()`                                                                                                                                                                                                                                                                                                                                                                                            
          `abstract ProjectFilesystemFactory`                                                                                          `getProjectFilesystemFactory()`                                                                                                                                                                                                                                                                                                                                                                            
          `abstract RuleKeyConfiguration`                                                                                              `getRuleKeyConfiguration()`                                                                                                                                                                                                                                                                                                                                                                                
          `static BuildExecutorArgs`                                                                                                   `of​(Console console,   BuckEventBus buckEventBus,   Platform platform,   Clock clock,   Cells cells,   Map<ExecutorPool,​? extends com.google.common.util.concurrent.ListeningExecutorService> executors,   ProjectFilesystemFactory projectFilesystemFactory,   BuildInfoStoreManager buildInfoStoreManager,   ArtifactCacheFactory artifactCacheFactory,   RuleKeyConfiguration ruleKeyConfiguration)`    

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

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### BuildExecutorArgs

                public BuildExecutorArgs()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getConsole()}

        -   #### getConsole

            ``` methodSignature
            public abstract Console getConsole()
            ```

        []{#getBuckEventBus()}

        -   #### getBuckEventBus

            ``` methodSignature
            public abstract BuckEventBus getBuckEventBus()
            ```

        []{#getPlatform()}

        -   #### getPlatform

            ``` methodSignature
            public abstract Platform getPlatform()
            ```

        []{#getClock()}

        -   #### getClock

            ``` methodSignature
            public abstract Clock getClock()
            ```

        []{#getCells()}

        -   #### getCells

            ``` methodSignature
            public abstract Cells getCells()
            ```

        []{#getExecutors()}

        -   #### getExecutors

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableMap<ExecutorPool,​com.google.common.util.concurrent.ListeningExecutorService> getExecutors()
            ```

        []{#getProjectFilesystemFactory()}

        -   #### getProjectFilesystemFactory

            ``` methodSignature
            public abstract ProjectFilesystemFactory getProjectFilesystemFactory()
            ```

        []{#getBuildInfoStoreManager()}

        -   #### getBuildInfoStoreManager

            ``` methodSignature
            public abstract BuildInfoStoreManager getBuildInfoStoreManager()
            ```

        []{#getArtifactCacheFactory()}

        -   #### getArtifactCacheFactory

            ``` methodSignature
            public abstract ArtifactCacheFactory getArtifactCacheFactory()
            ```

        []{#getRuleKeyConfiguration()}

        -   #### getRuleKeyConfiguration

            ``` methodSignature
            public abstract RuleKeyConfiguration getRuleKeyConfiguration()
            ```

        []{#getBuckConfig()}

        -   #### getBuckConfig

            ``` methodSignature
            public BuckConfig getBuckConfig()
            ```

        []{#of(com.facebook.buck.util.Console,com.facebook.buck.event.BuckEventBus,com.facebook.buck.util.environment.Platform,com.facebook.buck.util.timing.Clock,com.facebook.buck.core.cell.Cells,java.util.Map,com.facebook.buck.io.filesystem.ProjectFilesystemFactory,com.facebook.buck.core.build.engine.cache.manager.BuildInfoStoreManager,com.facebook.buck.artifact_cache.ArtifactCacheFactory,com.facebook.buck.rules.keys.config.RuleKeyConfiguration)}

        -   #### of

            ``` methodSignature
            public static BuildExecutorArgs of​(Console console,
                                               BuckEventBus buckEventBus,
                                               Platform platform,
                                               Clock clock,
                                               Cells cells,
                                               Map<ExecutorPool,​? extends com.google.common.util.concurrent.ListeningExecutorService> executors,
                                               ProjectFilesystemFactory projectFilesystemFactory,
                                               BuildInfoStoreManager buildInfoStoreManager,
                                               ArtifactCacheFactory artifactCacheFactory,
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
