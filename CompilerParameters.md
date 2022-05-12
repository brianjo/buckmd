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
[Package]{.packageLabelInType} [com.facebook.buck.jvm.java](package-summary.html)
:::

## Class CompilerParameters {#class-compilerparameters .title title="Class CompilerParameters"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.jvm.java.CompilerParameters

::: description
-   

    ------------------------------------------------------------------------

        public abstract class CompilerParameters
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type   Class                          Description
          ------------------- ------------------------------ -------------
          `static class `     `CompilerParameters.Builder`    

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor              Description
          ------------------------ -------------
          `CompilerParameters()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                      Method                                Description
          ------------------------------------------------------ ------------------------------------- -------------
          `static CompilerParameters.Builder`                    `builder()`                            
          `AbiGenerationMode`                                    `getAbiCompatibilityMode()`            
          `AbiGenerationMode`                                    `getAbiGenerationMode()`               
          `com.google.common.collect.ImmutableSortedSet<Path>`   `getClasspathEntries()`                
          `abstract CompilerOutputPaths`                         `getOutputPaths()`                     
          `com.google.common.collect.ImmutableSortedSet<Path>`   `getSourceFilePaths()`                 
          `abstract SourceOnlyAbiRuleInfoFactory`                `getSourceOnlyAbiRuleInfoFactory()`    
          `boolean`                                              `shouldTrackClassUsage()`              
          `boolean`                                              `shouldTrackJavacPhaseEvents()`        

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

        -   #### CompilerParameters

                public CompilerParameters()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getSourceFilePaths()}

        -   #### getSourceFilePaths

            ``` methodSignature
            @Default
            public com.google.common.collect.ImmutableSortedSet<Path> getSourceFilePaths()
            ```

        []{#getClasspathEntries()}

        -   #### getClasspathEntries

            ``` methodSignature
            @Default
            public com.google.common.collect.ImmutableSortedSet<Path> getClasspathEntries()
            ```

        []{#getOutputPaths()}

        -   #### getOutputPaths

            ``` methodSignature
            public abstract CompilerOutputPaths getOutputPaths()
            ```

        []{#getAbiGenerationMode()}

        -   #### getAbiGenerationMode

            ``` methodSignature
            @Default
            public AbiGenerationMode getAbiGenerationMode()
            ```

        []{#getAbiCompatibilityMode()}

        -   #### getAbiCompatibilityMode

            ``` methodSignature
            @Default
            public AbiGenerationMode getAbiCompatibilityMode()
            ```

        []{#shouldTrackClassUsage()}

        -   #### shouldTrackClassUsage

            ``` methodSignature
            @Default
            public boolean shouldTrackClassUsage()
            ```

        []{#shouldTrackJavacPhaseEvents()}

        -   #### shouldTrackJavacPhaseEvents

            ``` methodSignature
            @Default
            public boolean shouldTrackJavacPhaseEvents()
            ```

        []{#getSourceOnlyAbiRuleInfoFactory()}

        -   #### getSourceOnlyAbiRuleInfoFactory

            ``` methodSignature
            @Nullable
            public abstract SourceOnlyAbiRuleInfoFactory getSourceOnlyAbiRuleInfoFactory()
            ```

        []{#builder()}

        -   #### builder

            ``` methodSignature
            public static CompilerParameters.Builder builder()
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
