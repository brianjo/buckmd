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

## Class XCScheme {#class-xcscheme .title title="Class XCScheme"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.apple.xcode.XCScheme

::: description
-   

    ------------------------------------------------------------------------

        public class XCScheme
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type   Class                            Description
          ------------------- -------------------------------- -------------
          `static class `     `XCScheme.AdditionalActions`      
          `static class `     `XCScheme.AnalyzeAction`          
          `static class `     `XCScheme.ArchiveAction`          
          `static class `     `XCScheme.BuildableReference`     
          `static class `     `XCScheme.BuildAction`            
          `static class `     `XCScheme.BuildActionEntry`       
          `static class `     `XCScheme.LaunchAction`           
          `static class `     `XCScheme.ProfileAction`          
          `static class `     `XCScheme.SchemeAction`           
          `static class `     `XCScheme.SchemePrePostAction`    
          `static class `     `XCScheme.TestableReference`      
          `static class `     `XCScheme.TestAction`             

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                                                                                                                                           Description
          ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `XCScheme​(String name,         boolean wasCreatedForExtension,         Optional<XCScheme.BuildAction> buildAction,         Optional<XCScheme.TestAction> testAction,         Optional<XCScheme.LaunchAction> launchAction,         Optional<XCScheme.ProfileAction> profileAction,         Optional<XCScheme.AnalyzeAction> analyzeAction,         Optional<XCScheme.ArchiveAction> archiveAction)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                    Method                          Description
          ------------------------------------ ------------------------------- -------------
          `Optional<XCScheme.AnalyzeAction>`   `getAnalyzeAction()`             
          `Optional<XCScheme.ArchiveAction>`   `getArchiveAction()`             
          `Optional<XCScheme.BuildAction>`     `getBuildAction()`               
          `Optional<XCScheme.LaunchAction>`    `getLaunchAction()`              
          `String`                             `getName()`                      
          `Optional<XCScheme.ProfileAction>`   `getProfileAction()`             
          `Optional<XCScheme.TestAction>`      `getTestAction()`                
          `boolean`                            `getWasCreatedForExtension()`    

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

        []{#<init>(java.lang.String,boolean,java.util.Optional,java.util.Optional,java.util.Optional,java.util.Optional,java.util.Optional,java.util.Optional)}

        -   #### XCScheme

                public XCScheme​(String name,
                                boolean wasCreatedForExtension,
                                Optional<XCScheme.BuildAction> buildAction,
                                Optional<XCScheme.TestAction> testAction,
                                Optional<XCScheme.LaunchAction> launchAction,
                                Optional<XCScheme.ProfileAction> profileAction,
                                Optional<XCScheme.AnalyzeAction> analyzeAction,
                                Optional<XCScheme.ArchiveAction> archiveAction)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getName()}

        -   #### getName

            ``` methodSignature
            public String getName()
            ```

        []{#getWasCreatedForExtension()}

        -   #### getWasCreatedForExtension

            ``` methodSignature
            public boolean getWasCreatedForExtension()
            ```

        []{#getBuildAction()}

        -   #### getBuildAction

            ``` methodSignature
            public Optional<XCScheme.BuildAction> getBuildAction()
            ```

        []{#getTestAction()}

        -   #### getTestAction

            ``` methodSignature
            public Optional<XCScheme.TestAction> getTestAction()
            ```

        []{#getLaunchAction()}

        -   #### getLaunchAction

            ``` methodSignature
            public Optional<XCScheme.LaunchAction> getLaunchAction()
            ```

        []{#getProfileAction()}

        -   #### getProfileAction

            ``` methodSignature
            public Optional<XCScheme.ProfileAction> getProfileAction()
            ```

        []{#getAnalyzeAction()}

        -   #### getAnalyzeAction

            ``` methodSignature
            public Optional<XCScheme.AnalyzeAction> getAnalyzeAction()
            ```

        []{#getArchiveAction()}

        -   #### getArchiveAction

            ``` methodSignature
            public Optional<XCScheme.ArchiveAction> getArchiveAction()
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
