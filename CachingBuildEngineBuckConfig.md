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

-   [Overview](../../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../index-all.html)
-   [Help](../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.core.build.engine.config](package-summary.html)
:::

## Class CachingBuildEngineBuckConfig {#class-cachingbuildenginebuckconfig .title title="Class CachingBuildEngineBuckConfig"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.build.engine.config.CachingBuildEngineBuckConfig

::: description
-   

    All Implemented Interfaces:
    :   `ConfigView<BuckConfig>`

    ------------------------------------------------------------------------

        public abstract class CachingBuildEngineBuckConfig
        extends Object
        implements ConfigView<BuckConfig>
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                        Description
          ---------------------------------- -------------
          `CachingBuildEngineBuckConfig()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                       Method                                     Description
          --------------------------------------- ------------------------------------------ -------------
          `Optional<Long>`                        `getBuildArtifactCacheSizeLimit()`          
          `DepFiles`                              `getBuildDepFiles()`                        
          `BuildType`                             `getBuildEngineMode()`                      
          `long`                                  `getBuildMaxDepFileCacheEntries()`          
          `boolean`                               `getConsoleLogBuildRuleFailuresInline()`    
          `ResourceAwareSchedulingInfo`           `getResourceAwareSchedulingInfo()`          
          `static CachingBuildEngineBuckConfig`   `of​(BuckConfig delegate)`                   

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

            ### Methods inherited from interface com.facebook.buck.core.config.[ConfigView](../../../config/ConfigView.html "interface in com.facebook.buck.core.config")

            `getDelegate`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### CachingBuildEngineBuckConfig

                public CachingBuildEngineBuckConfig()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#of(com.facebook.buck.core.config.BuckConfig)}

        -   #### of

            ``` methodSignature
            public static CachingBuildEngineBuckConfig of​(BuckConfig delegate)
            ```

        []{#getBuildEngineMode()}

        -   #### getBuildEngineMode

            ``` methodSignature
            public BuildType getBuildEngineMode()
            ```

            [Returns:]{.returnLabel}
            :   the mode with which to run the build engine.

        []{#getBuildDepFiles()}

        -   #### getBuildDepFiles

            ``` methodSignature
            public DepFiles getBuildDepFiles()
            ```

            [Returns:]{.returnLabel}
            :   the mode with which to run the build engine.

        []{#getConsoleLogBuildRuleFailuresInline()}

        -   #### getConsoleLogBuildRuleFailuresInline

            ``` methodSignature
            public boolean getConsoleLogBuildRuleFailuresInline()
            ```

            [Returns:]{.returnLabel}
            :   whether to log to console build rule failures as they
                happen, including rule name and error text. If false,
                then depending on keepGoing/verbosity settings, failures
                may not appear in the console at all, may only appear at
                the end of the build, or may be missing important
                details (e.g. name of rule is logged, but no error
                message, or vice-versa).

        []{#getBuildMaxDepFileCacheEntries()}

        -   #### getBuildMaxDepFileCacheEntries

            ``` methodSignature
            public long getBuildMaxDepFileCacheEntries()
            ```

            [Returns:]{.returnLabel}
            :   the maximum number of entries to support in the depfile
                cache.

        []{#getBuildArtifactCacheSizeLimit()}

        -   #### getBuildArtifactCacheSizeLimit

            ``` methodSignature
            public Optional<Long> getBuildArtifactCacheSizeLimit()
            ```

            [Returns:]{.returnLabel}
            :   the maximum size an artifact can be for the build engine
                to cache it.

        []{#getResourceAwareSchedulingInfo()}

        -   #### getResourceAwareSchedulingInfo

            ``` methodSignature
            public ResourceAwareSchedulingInfo getResourceAwareSchedulingInfo()
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

-   [Overview](../../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../index-all.html)
-   [Help](../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../allclasses.html)

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
