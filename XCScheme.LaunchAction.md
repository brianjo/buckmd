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
-   [Nested](#nested.class.summary) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.apple.xcode](package-summary.html)
:::

## Class XCScheme.LaunchAction {#class-xcscheme.launchaction .title title="Class XCScheme.LaunchAction"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.apple.xcode.XCScheme.SchemeAction](XCScheme.SchemeAction.html "class in com.facebook.buck.apple.xcode")

    -   -   com.facebook.buck.apple.xcode.XCScheme.LaunchAction

::: description
-   

    Enclosing class:
    :   [XCScheme](XCScheme.html "class in com.facebook.buck.apple.xcode")

    ------------------------------------------------------------------------

        public static class XCScheme.LaunchAction
        extends XCScheme.SchemeAction
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static class `       | `XCScheme.Laun        |                       |
        |                       | chAction.LaunchStyle` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static class `       | `XCScheme.LaunchA     | ::: block             |
        |                       | ction.WatchInterface` | Watch Interface       |
        |                       |                       | property in Watch app |
        |                       |                       | scheme used to choose |
        |                       |                       | which interface is    |
        |                       |                       | launched.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      Description
          ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ -------------
          `LaunchAction​(XCScheme.BuildableReference buildableReference,             String buildConfiguration,             Optional<String> runnablePath,             Optional<String> remoteRunnablePath,             Optional<XCScheme.LaunchAction.WatchInterface> watchInterface,             XCScheme.LaunchAction.LaunchStyle launchStyle,             Optional<com.google.common.collect.ImmutableMap<String,​String>> environmentVariables,             Optional<XCScheme.BuildableReference> expandVariablesBasedOn,             Optional<com.google.common.collect.ImmutableMap<String,​String>> commandLineArguments,             Optional<com.google.common.collect.ImmutableList<XCScheme.SchemePrePostAction>> preActions,             Optional<com.google.common.collect.ImmutableList<XCScheme.SchemePrePostAction>> postActions,             Optional<String> notificationPayloadFile,             Optional<String> applicationLanguage,             Optional<String> applicationRegion)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                   Method                           Description
          ------------------------------------------------------------------- -------------------------------- -------------
          `Optional<String>`                                                  `getApplicationLanguage()`        
          `Optional<String>`                                                  `getApplicationRegion()`          
          `XCScheme.BuildableReference`                                       `getBuildableReference()`         
          `String`                                                            `getBuildConfiguration()`         
          `Optional<com.google.common.collect.ImmutableMap<String,​String>>`   `getCommandLineArguments()`       
          `Optional<com.google.common.collect.ImmutableMap<String,​String>>`   `getEnvironmentVariables()`       
          `Optional<XCScheme.BuildableReference>`                             `getExpandVariablesBasedOn()`     
          `XCScheme.LaunchAction.LaunchStyle`                                 `getLaunchStyle()`                
          `Optional<String>`                                                  `getNotificationPayloadFile()`    
          `Optional<String>`                                                  `getRemoteRunnablePath()`         
          `Optional<String>`                                                  `getRunnablePath()`               
          `Optional<XCScheme.LaunchAction.WatchInterface>`                    `getWatchInterface()`             

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.apple.xcode.XCScheme.SchemeAction}

            ### Methods inherited from class com.facebook.buck.apple.xcode.[XCScheme.SchemeAction](XCScheme.SchemeAction.html "class in com.facebook.buck.apple.xcode")

            `getPostActions, getPreActions`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.apple.xcode.XCScheme.BuildableReference,java.lang.String,java.util.Optional,java.util.Optional,java.util.Optional,com.facebook.buck.apple.xcode.XCScheme.LaunchAction.LaunchStyle,java.util.Optional,java.util.Optional,java.util.Optional,java.util.Optional,java.util.Optional,java.util.Optional,java.util.Optional,java.util.Optional)}

        -   #### LaunchAction

                public LaunchAction​(XCScheme.BuildableReference buildableReference,
                                    String buildConfiguration,
                                    Optional<String> runnablePath,
                                    Optional<String> remoteRunnablePath,
                                    Optional<XCScheme.LaunchAction.WatchInterface> watchInterface,
                                    XCScheme.LaunchAction.LaunchStyle launchStyle,
                                    Optional<com.google.common.collect.ImmutableMap<String,​String>> environmentVariables,
                                    Optional<XCScheme.BuildableReference> expandVariablesBasedOn,
                                    Optional<com.google.common.collect.ImmutableMap<String,​String>> commandLineArguments,
                                    Optional<com.google.common.collect.ImmutableList<XCScheme.SchemePrePostAction>> preActions,
                                    Optional<com.google.common.collect.ImmutableList<XCScheme.SchemePrePostAction>> postActions,
                                    Optional<String> notificationPayloadFile,
                                    Optional<String> applicationLanguage,
                                    Optional<String> applicationRegion)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getBuildableReference()}

        -   #### getBuildableReference

            ``` methodSignature
            public XCScheme.BuildableReference getBuildableReference()
            ```

        []{#getBuildConfiguration()}

        -   #### getBuildConfiguration

            ``` methodSignature
            public String getBuildConfiguration()
            ```

        []{#getRunnablePath()}

        -   #### getRunnablePath

            ``` methodSignature
            public Optional<String> getRunnablePath()
            ```

        []{#getRemoteRunnablePath()}

        -   #### getRemoteRunnablePath

            ``` methodSignature
            public Optional<String> getRemoteRunnablePath()
            ```

        []{#getWatchInterface()}

        -   #### getWatchInterface

            ``` methodSignature
            public Optional<XCScheme.LaunchAction.WatchInterface> getWatchInterface()
            ```

        []{#getNotificationPayloadFile()}

        -   #### getNotificationPayloadFile

            ``` methodSignature
            public Optional<String> getNotificationPayloadFile()
            ```

        []{#getLaunchStyle()}

        -   #### getLaunchStyle

            ``` methodSignature
            public XCScheme.LaunchAction.LaunchStyle getLaunchStyle()
            ```

        []{#getEnvironmentVariables()}

        -   #### getEnvironmentVariables

            ``` methodSignature
            public Optional<com.google.common.collect.ImmutableMap<String,​String>> getEnvironmentVariables()
            ```

        []{#getExpandVariablesBasedOn()}

        -   #### getExpandVariablesBasedOn

            ``` methodSignature
            public Optional<XCScheme.BuildableReference> getExpandVariablesBasedOn()
            ```

        []{#getCommandLineArguments()}

        -   #### getCommandLineArguments

            ``` methodSignature
            public Optional<com.google.common.collect.ImmutableMap<String,​String>> getCommandLineArguments()
            ```

        []{#getApplicationLanguage()}

        -   #### getApplicationLanguage

            ``` methodSignature
            public Optional<String> getApplicationLanguage()
            ```

        []{#getApplicationRegion()}

        -   #### getApplicationRegion

            ``` methodSignature
            public Optional<String> getApplicationRegion()
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
-   [Nested](#nested.class.summary) \| 
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
