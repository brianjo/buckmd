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
[Package]{.packageLabelInType} [com.facebook.buck.cli](package-summary.html)
:::

## Class ProjectGeneratorParameters {#class-projectgeneratorparameters .title title="Class ProjectGeneratorParameters"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.cli.ProjectGeneratorParameters

::: description
-   

    ------------------------------------------------------------------------

        public abstract class ProjectGeneratorParameters
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                      Description
          -------------------------------- -------------
          `ProjectGeneratorParameters()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                                                                  Method                           Description
          ------------------------------------------------------------------------------------------------------------------ -------------------------------- -------------
          `abstract java.util.function.Function<Iterable<String>,​com.google.common.collect.ImmutableList<TargetNodeSpec>>`   `getArgsParser()`                 
          `abstract CommandRunnerParams`                                                                                     `getCommandRunnerParams()`        
          `Config`                                                                                                           `getConfig()`                     
          `Console`                                                                                                          `getConsole()`                    
          `abstract boolean`                                                                                                 `getEnableParserProfiling()`      
          `Parser`                                                                                                           `getParser()`                     
          `Path`                                                                                                             `getPath()`                       
          `DirtyPrintStreamDecorator`                                                                                        `getStdErr()`                     
          `DirtyPrintStreamDecorator`                                                                                        `getStdOut()`                     
          `abstract boolean`                                                                                                 `isDryRun()`                      
          `abstract boolean`                                                                                                 `isWithoutDependenciesTests()`    
          `abstract boolean`                                                                                                 `isWithoutTests()`                
          `abstract boolean`                                                                                                 `isWithTests()`                   

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
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

        -   #### ProjectGeneratorParameters

                public ProjectGeneratorParameters()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getCommandRunnerParams()}

        -   #### getCommandRunnerParams

            ``` methodSignature
            public abstract CommandRunnerParams getCommandRunnerParams()
            ```

        []{#getConsole()}

        -   #### getConsole

            ``` methodSignature
            public Console getConsole()
            ```

        []{#getStdErr()}

        -   #### getStdErr

            ``` methodSignature
            public DirtyPrintStreamDecorator getStdErr()
            ```

        []{#getStdOut()}

        -   #### getStdOut

            ``` methodSignature
            public DirtyPrintStreamDecorator getStdOut()
            ```

        []{#getConfig()}

        -   #### getConfig

            ``` methodSignature
            public Config getConfig()
            ```

        []{#getParser()}

        -   #### getParser

            ``` methodSignature
            public Parser getParser()
            ```

        []{#getPath()}

        -   #### getPath

            ``` methodSignature
            public Path getPath()
            ```

        []{#isDryRun()}

        -   #### isDryRun

            ``` methodSignature
            public abstract boolean isDryRun()
            ```

        []{#isWithTests()}

        -   #### isWithTests

            ``` methodSignature
            public abstract boolean isWithTests()
            ```

        []{#isWithoutTests()}

        -   #### isWithoutTests

            ``` methodSignature
            public abstract boolean isWithoutTests()
            ```

        []{#isWithoutDependenciesTests()}

        -   #### isWithoutDependenciesTests

            ``` methodSignature
            public abstract boolean isWithoutDependenciesTests()
            ```

        []{#getEnableParserProfiling()}

        -   #### getEnableParserProfiling

            ``` methodSignature
            public abstract boolean getEnableParserProfiling()
            ```

        []{#getArgsParser()}

        -   #### getArgsParser

            ``` methodSignature
            public abstract java.util.function.Function<Iterable<String>,​com.google.common.collect.ImmutableList<TargetNodeSpec>> getArgsParser()
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
