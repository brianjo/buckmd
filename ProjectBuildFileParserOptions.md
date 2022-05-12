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
[Package]{.packageLabelInType} [com.facebook.buck.parser.options](package-summary.html)
:::

## Class ProjectBuildFileParserOptions {#class-projectbuildfileparseroptions .title title="Class ProjectBuildFileParserOptions"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.parser.options.ProjectBuildFileParserOptions

::: description
-   

    ------------------------------------------------------------------------

        public abstract class ProjectBuildFileParserOptions
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type   Class                                     Description
          ------------------- ----------------------------------------- -------------
          `static class `     `ProjectBuildFileParserOptions.Builder`    

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                         Description
          ----------------------------------- -------------
          `ProjectBuildFileParserOptions()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                                                                 Method                            Description
          ----------------------------------------------------------------------------------------------------------------- --------------------------------- -------------
          `static ProjectBuildFileParserOptions.Builder`                                                                    `builder()`                        
          `abstract boolean`                                                                                                `getAllowEmptyGlobs()`             
          `abstract List<String>`                                                                                           `getBuildFileImportWhitelist()`    
          `abstract String`                                                                                                 `getBuildFileName()`               
          `String`                                                                                                          `getCellName()`                    
          `abstract com.google.common.collect.ImmutableMap<String,​AbsPath>`                                                 `getCellRoots()`                   
          `abstract List<String>`                                                                                           `getDefaultIncludes()`             
          `abstract com.google.common.collect.ImmutableSet<BaseDescription<?>>`                                             `getDescriptions()`                
          `boolean`                                                                                                         `getEnableProfiling()`             
          `abstract com.google.common.collect.ImmutableSet<PathMatcher>`                                                    `getIgnorePaths()`                 
          `ImplicitNativeRulesState`                                                                                        `getImplicitNativeRulesState()`    
          `abstract com.google.common.collect.ImmutableMap<String,​ImplicitInclude>`                                         `getPackageImplicitIncludes()`     
          `abstract com.google.common.collect.ImmutableSet<BuiltInProvider<?>>`                                             `getPerFeatureProviders()`         
          `abstract AbsPath`                                                                                                `getProjectRoot()`                 
          `abstract String`                                                                                                 `getPythonInterpreter()`           
          `abstract Optional<String>`                                                                                       `getPythonModuleSearchPath()`      
          `abstract com.google.common.collect.ImmutableMap<String,​com.google.common.collect.ImmutableMap<String,​String>>`   `getRawConfig()`                   
          `UserDefinedRulesState`                                                                                           `getUserDefinedRulesState()`       
          `boolean`                                                                                                         `getUseWatchmanGlob()`             
          `Watchman`                                                                                                        `getWatchman()`                    
          `boolean`                                                                                                         `getWatchmanGlobStatResults()`     
          `abstract Optional<Long>`                                                                                         `getWatchmanQueryTimeoutMs()`      
          `boolean`                                                                                                         `getWatchmanUseGlobGenerator()`    
          `boolean`                                                                                                         `isWarnAboutDeprecatedSyntax()`    

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

        -   #### ProjectBuildFileParserOptions

                public ProjectBuildFileParserOptions()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getProjectRoot()}

        -   #### getProjectRoot

            ``` methodSignature
            public abstract AbsPath getProjectRoot()
            ```

        []{#getCellRoots()}

        -   #### getCellRoots

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableMap<String,​AbsPath> getCellRoots()
            ```

        []{#getPythonInterpreter()}

        -   #### getPythonInterpreter

            ``` methodSignature
            public abstract String getPythonInterpreter()
            ```

        []{#getPythonModuleSearchPath()}

        -   #### getPythonModuleSearchPath

            ``` methodSignature
            public abstract Optional<String> getPythonModuleSearchPath()
            ```

        []{#getAllowEmptyGlobs()}

        -   #### getAllowEmptyGlobs

            ``` methodSignature
            public abstract boolean getAllowEmptyGlobs()
            ```

        []{#getIgnorePaths()}

        -   #### getIgnorePaths

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableSet<PathMatcher> getIgnorePaths()
            ```

        []{#getBuildFileName()}

        -   #### getBuildFileName

            ``` methodSignature
            public abstract String getBuildFileName()
            ```

        []{#getDefaultIncludes()}

        -   #### getDefaultIncludes

            ``` methodSignature
            public abstract List<String> getDefaultIncludes()
            ```

        []{#getPackageImplicitIncludes()}

        -   #### getPackageImplicitIncludes

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableMap<String,​ImplicitInclude> getPackageImplicitIncludes()
            ```

        []{#getDescriptions()}

        -   #### getDescriptions

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableSet<BaseDescription<?>> getDescriptions()
            ```

        []{#getRawConfig()}

        -   #### getRawConfig

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableMap<String,​com.google.common.collect.ImmutableMap<String,​String>> getRawConfig()
            ```

        []{#getCellName()}

        -   #### getCellName

            ``` methodSignature
            @Default
            public String getCellName()
            ```

        []{#getUseWatchmanGlob()}

        -   #### getUseWatchmanGlob

            ``` methodSignature
            @Default
            public boolean getUseWatchmanGlob()
            ```

        []{#getWatchmanGlobStatResults()}

        -   #### getWatchmanGlobStatResults

            ``` methodSignature
            @Default
            public boolean getWatchmanGlobStatResults()
            ```

        []{#getWatchmanUseGlobGenerator()}

        -   #### getWatchmanUseGlobGenerator

            ``` methodSignature
            @Default
            public boolean getWatchmanUseGlobGenerator()
            ```

        []{#getWatchman()}

        -   #### getWatchman

            ``` methodSignature
            @Default
            public Watchman getWatchman()
            ```

        []{#getEnableProfiling()}

        -   #### getEnableProfiling

            ``` methodSignature
            @Default
            public boolean getEnableProfiling()
            ```

        []{#getWatchmanQueryTimeoutMs()}

        -   #### getWatchmanQueryTimeoutMs

            ``` methodSignature
            public abstract Optional<Long> getWatchmanQueryTimeoutMs()
            ```

        []{#getBuildFileImportWhitelist()}

        -   #### getBuildFileImportWhitelist

            ``` methodSignature
            public abstract List<String> getBuildFileImportWhitelist()
            ```

        []{#getPerFeatureProviders()}

        -   #### getPerFeatureProviders

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableSet<BuiltInProvider<?>> getPerFeatureProviders()
            ```

        []{#getImplicitNativeRulesState()}

        -   #### getImplicitNativeRulesState

            ``` methodSignature
            @Default
            public ImplicitNativeRulesState getImplicitNativeRulesState()
            ```

        []{#getUserDefinedRulesState()}

        -   #### getUserDefinedRulesState

            ``` methodSignature
            @Default
            public UserDefinedRulesState getUserDefinedRulesState()
            ```

        []{#isWarnAboutDeprecatedSyntax()}

        -   #### isWarnAboutDeprecatedSyntax

            ``` methodSignature
            @Default
            public boolean isWarnAboutDeprecatedSyntax()
            ```

        []{#builder()}

        -   #### builder

            ``` methodSignature
            public static ProjectBuildFileParserOptions.Builder builder()
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
