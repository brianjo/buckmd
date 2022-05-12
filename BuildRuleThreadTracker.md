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
[Package]{.packageLabelInType} [com.facebook.buck.event.listener](package-summary.html)
:::

## Class BuildRuleThreadTracker {#class-buildrulethreadtracker .title title="Class BuildRuleThreadTracker"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.event.listener.BuildRuleThreadTracker

::: description
-   

    ------------------------------------------------------------------------

        public class BuildRuleThreadTracker
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                           Description
          --------------------------------------------------------------------- -------------
          `BuildRuleThreadTracker​(ExecutionEnvironment executionEnvironment)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                                  Method                                                      Description
          ---------------------------------------------------------------------------------- ----------------------------------------------------------- -------------
          `void`                                                                             `didFinishBuildRule​(BuildRuleEvent.Finished finished)`       
          `void`                                                                             `didFinishTestRule​(TestRuleEvent.Finished finished)`         
          `void`                                                                             `didResumeBuildRule​(BuildRuleEvent.Resumed resumed)`         
          `void`                                                                             `didStartBuildRule​(BuildRuleEvent.Started started)`          
          `void`                                                                             `didStartTestRule​(TestRuleEvent.Started started)`            
          `void`                                                                             `didSuspendBuildRule​(BuildRuleEvent.Suspended suspended)`    
          `ConcurrentMap<Long,​Optional<? extends BuildRuleEvent.BeginningBuildRuleEvent>>`   `getBuildEventsByThread()`                                   
          `ConcurrentMap<Long,​Optional<? extends TestRuleEvent>>`                            `getTestEventsByThread()`                                    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
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

        []{#<init>(com.facebook.buck.util.environment.ExecutionEnvironment)}

        -   #### BuildRuleThreadTracker

                public BuildRuleThreadTracker​(ExecutionEnvironment executionEnvironment)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getBuildEventsByThread()}

        -   #### getBuildEventsByThread

            ``` methodSignature
            public ConcurrentMap<Long,​Optional<? extends BuildRuleEvent.BeginningBuildRuleEvent>> getBuildEventsByThread()
            ```

        []{#getTestEventsByThread()}

        -   #### getTestEventsByThread

            ``` methodSignature
            public ConcurrentMap<Long,​Optional<? extends TestRuleEvent>> getTestEventsByThread()
            ```

        []{#didStartBuildRule(com.facebook.buck.core.build.event.BuildRuleEvent.Started)}

        -   #### didStartBuildRule

            ``` methodSignature
            public void didStartBuildRule​(BuildRuleEvent.Started started)
            ```

        []{#didResumeBuildRule(com.facebook.buck.core.build.event.BuildRuleEvent.Resumed)}

        -   #### didResumeBuildRule

            ``` methodSignature
            public void didResumeBuildRule​(BuildRuleEvent.Resumed resumed)
            ```

        []{#didSuspendBuildRule(com.facebook.buck.core.build.event.BuildRuleEvent.Suspended)}

        -   #### didSuspendBuildRule

            ``` methodSignature
            public void didSuspendBuildRule​(BuildRuleEvent.Suspended suspended)
            ```

        []{#didFinishBuildRule(com.facebook.buck.core.build.event.BuildRuleEvent.Finished)}

        -   #### didFinishBuildRule

            ``` methodSignature
            public void didFinishBuildRule​(BuildRuleEvent.Finished finished)
            ```

        []{#didStartTestRule(com.facebook.buck.test.TestRuleEvent.Started)}

        -   #### didStartTestRule

            ``` methodSignature
            public void didStartTestRule​(TestRuleEvent.Started started)
            ```

        []{#didFinishTestRule(com.facebook.buck.test.TestRuleEvent.Finished)}

        -   #### didFinishTestRule

            ``` methodSignature
            public void didFinishTestRule​(TestRuleEvent.Finished finished)
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
