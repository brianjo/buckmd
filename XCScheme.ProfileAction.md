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
[Package]{.packageLabelInType} [com.facebook.buck.apple.xcode](package-summary.html)
:::

## Class XCScheme.ProfileAction {#class-xcscheme.profileaction .title title="Class XCScheme.ProfileAction"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.apple.xcode.XCScheme.SchemeAction](XCScheme.SchemeAction.html "class in com.facebook.buck.apple.xcode")

    -   -   com.facebook.buck.apple.xcode.XCScheme.ProfileAction

::: description
-   

    Enclosing class:
    :   [XCScheme](XCScheme.html "class in com.facebook.buck.apple.xcode")

    ------------------------------------------------------------------------

        public static class XCScheme.ProfileAction
        extends XCScheme.SchemeAction
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   Description
          ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `ProfileAction​(XCScheme.BuildableReference buildableReference,              String buildConfiguration,              Optional<com.google.common.collect.ImmutableMap<String,​String>> environmentVariables,              Optional<XCScheme.BuildableReference> expandVariablesBasedOn,              Optional<com.google.common.collect.ImmutableMap<String,​String>> commandLineArguments,              Optional<com.google.common.collect.ImmutableList<XCScheme.SchemePrePostAction>> preActions,              Optional<com.google.common.collect.ImmutableList<XCScheme.SchemePrePostAction>> postActions)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                   Method                          Description
          ------------------------------------------------------------------- ------------------------------- -------------
          `XCScheme.BuildableReference`                                       `getBuildableReference()`        
          `String`                                                            `getBuildConfiguration()`        
          `Optional<com.google.common.collect.ImmutableMap<String,​String>>`   `getCommandLineArguments()`      
          `Optional<com.google.common.collect.ImmutableMap<String,​String>>`   `getEnvironmentVariables()`      
          `Optional<XCScheme.BuildableReference>`                             `getExpandVariablesBasedOn()`    

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

        []{#<init>(com.facebook.buck.apple.xcode.XCScheme.BuildableReference,java.lang.String,java.util.Optional,java.util.Optional,java.util.Optional,java.util.Optional,java.util.Optional)}

        -   #### ProfileAction

                public ProfileAction​(XCScheme.BuildableReference buildableReference,
                                     String buildConfiguration,
                                     Optional<com.google.common.collect.ImmutableMap<String,​String>> environmentVariables,
                                     Optional<XCScheme.BuildableReference> expandVariablesBasedOn,
                                     Optional<com.google.common.collect.ImmutableMap<String,​String>> commandLineArguments,
                                     Optional<com.google.common.collect.ImmutableList<XCScheme.SchemePrePostAction>> preActions,
                                     Optional<com.google.common.collect.ImmutableList<XCScheme.SchemePrePostAction>> postActions)
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
