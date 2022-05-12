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

-   [Overview](../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../deprecated-list.html)
-   [Index](../../../../../../index-all.html)
-   [Help](../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../allclasses.html)

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
-   [Field](#field.summary) \| 
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.event.listener.util](package-summary.html)
:::

## Class ProgressEstimator {#class-progressestimator .title title="Class ProgressEstimator"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.event.listener.util.ProgressEstimator

::: description
-   

    All Implemented Interfaces:
    :   `AutoCloseable`

    ------------------------------------------------------------------------

        public class ProgressEstimator
        extends Object
        implements AutoCloseable
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type   Field                                          Description
          ------------------- ---------------------------------------------- -------------
          `static String`     `EXPECTED_NUMBER_OF_GENERATED_PROJECT_FILES`    
          `static String`     `EXPECTED_NUMBER_OF_PARSED_BUCK_FILES`          
          `static String`     `EXPECTED_NUMBER_OF_PARSED_RULES`               
          `static String`     `PROGRESS_ESTIMATIONS_JSON`                     

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                   Description
          --------------------------------------------------------------------------------------------- -------------
          `ProgressEstimator​(Optional<Path> storageFile,                  BuckEventBus buckEventBus)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `void`                | `close()`             |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `didFinishBuild()`    |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Future<?>`           | `didFinishParsing()`  | ::: block             |
        |                       |                       | Indicates that buck   |
        |                       |                       | has finished parsing, |
        |                       |                       | updating the progress |
        |                       |                       | estimation            |
        |                       |                       | accordingly           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Future<?>`           | `didFinis             | ::: block             |
        |                       | hProjectGeneration()` | Indicates that        |
        |                       |                       | project generation is |
        |                       |                       | finished              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `didFinishRule()`     |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Future<?>`           | `didGenera            | ::: block             |
        |                       | teProjectForTarget()` | Indicates that a      |
        |                       |                       | project file has been |
        |                       |                       | generated             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Future<?>`           | `didParseB            | ::: block             |
        |                       | uckRules​(int amount)` | Updates the amount of |
        |                       |                       | rules done parsing    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `didStartBuild()`     |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Double>`    | `getApprox            |                       |
        |                       | imateBuildProgress()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `ProgressEstimation`  | `ge                   |                       |
        |                       | tEstimatedProgressOfC |                       |
        |                       | reatingActionGraph()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Double>`    | `getEs                |                       |
        |                       | timatedProgressOfGene |                       |
        |                       | ratingProjectFiles()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `ProgressEstimation`  | `getEstimatedProgress |                       |
        |                       | OfParsingBuckFiles()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Future<?>`           | `setCurrentC          | ::: block             |
        |                       | ommand​(String command | Sets the current      |
        |                       | Name,                 | command that we are   |
        |                       |   com.google.common.c | estimating            |
        |                       | ollect.ImmutableList< | :::                   |
        |                       | String> commandArgs)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `setNumb              |                       |
        |                       | erOfRules​(int count)` |                       |
        +-----------------------+-----------------------+-----------------------+

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
    -   []{#field.detail}

        ### Field Detail

        []{#EXPECTED_NUMBER_OF_PARSED_RULES}

        -   #### EXPECTED_NUMBER_OF_PARSED_RULES

                public static final String EXPECTED_NUMBER_OF_PARSED_RULES

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../constant-values.html#com.facebook.buck.event.listener.util.ProgressEstimator.EXPECTED_NUMBER_OF_PARSED_RULES)

        []{#EXPECTED_NUMBER_OF_PARSED_BUCK_FILES}

        -   #### EXPECTED_NUMBER_OF_PARSED_BUCK_FILES

                public static final String EXPECTED_NUMBER_OF_PARSED_BUCK_FILES

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../constant-values.html#com.facebook.buck.event.listener.util.ProgressEstimator.EXPECTED_NUMBER_OF_PARSED_BUCK_FILES)

        []{#EXPECTED_NUMBER_OF_GENERATED_PROJECT_FILES}

        -   #### EXPECTED_NUMBER_OF_GENERATED_PROJECT_FILES

                public static final String EXPECTED_NUMBER_OF_GENERATED_PROJECT_FILES

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../constant-values.html#com.facebook.buck.event.listener.util.ProgressEstimator.EXPECTED_NUMBER_OF_GENERATED_PROJECT_FILES)

        []{#PROGRESS_ESTIMATIONS_JSON}

        -   #### PROGRESS_ESTIMATIONS_JSON

                public static final String PROGRESS_ESTIMATIONS_JSON

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../../constant-values.html#com.facebook.buck.event.listener.util.ProgressEstimator.PROGRESS_ESTIMATIONS_JSON)
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(java.util.Optional,com.facebook.buck.event.BuckEventBus)}

        -   #### ProgressEstimator

                public ProgressEstimator​(Optional<Path> storageFile,
                                         BuckEventBus buckEventBus)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#setCurrentCommand(java.lang.String,com.google.common.collect.ImmutableList)}

        -   #### setCurrentCommand

            ``` methodSignature
            public Future<?> setCurrentCommand​(String commandName,
                                               com.google.common.collect.ImmutableList<String> commandArgs)
            ```

            ::: block
            Sets the current command that we are estimating
            :::

            [Parameters:]{.paramLabel}
            :   `commandName` - the name of the command
            :   `commandArgs` - the arguments to the command

            [Returns:]{.returnLabel}
            :   a future that completes when estimation calculation is
                complete

        []{#didParseBuckRules(int)}

        -   #### didParseBuckRules

            ``` methodSignature
            public Future<?> didParseBuckRules​(int amount)
            ```

            ::: block
            Updates the amount of rules done parsing
            :::

            [Parameters:]{.paramLabel}
            :   `amount` - the number of rules done parsing

            [Returns:]{.returnLabel}
            :   a future that completes when estimation calculation is
                complete

        []{#didFinishParsing()}

        -   #### didFinishParsing

            ``` methodSignature
            public Future<?> didFinishParsing()
            ```

            ::: block
            Indicates that buck has finished parsing, updating the
            progress estimation accordingly
            :::

            [Returns:]{.returnLabel}
            :   a future that completes when estimation calculation is
                complete

        []{#didGenerateProjectForTarget()}

        -   #### didGenerateProjectForTarget

            ``` methodSignature
            public Future<?> didGenerateProjectForTarget()
            ```

            ::: block
            Indicates that a project file has been generated
            :::

            [Returns:]{.returnLabel}
            :   a future that completes when estimation calculation is
                complete

        []{#didFinishProjectGeneration()}

        -   #### didFinishProjectGeneration

            ``` methodSignature
            public Future<?> didFinishProjectGeneration()
            ```

            ::: block
            Indicates that project generation is finished
            :::

            [Returns:]{.returnLabel}
            :   a future that completes when estimation calculation is
                complete

        []{#setNumberOfRules(int)}

        -   #### setNumberOfRules

            ``` methodSignature
            public void setNumberOfRules​(int count)
            ```

        []{#didFinishRule()}

        -   #### didFinishRule

            ``` methodSignature
            public void didFinishRule()
            ```

        []{#didStartBuild()}

        -   #### didStartBuild

            ``` methodSignature
            public void didStartBuild()
            ```

        []{#didFinishBuild()}

        -   #### didFinishBuild

            ``` methodSignature
            public void didFinishBuild()
            ```

        []{#getEstimatedProgressOfParsingBuckFiles()}

        -   #### getEstimatedProgressOfParsingBuckFiles

            ``` methodSignature
            public ProgressEstimation getEstimatedProgressOfParsingBuckFiles()
            ```

            [Returns:]{.returnLabel}
            :   Estimated progress of parsing files stage.

        []{#getEstimatedProgressOfCreatingActionGraph()}

        -   #### getEstimatedProgressOfCreatingActionGraph

            ``` methodSignature
            public ProgressEstimation getEstimatedProgressOfCreatingActionGraph()
            ```

            [Returns:]{.returnLabel}
            :   Estimated progress of parsing files in action graph
                stage.

        []{#getEstimatedProgressOfGeneratingProjectFiles()}

        -   #### getEstimatedProgressOfGeneratingProjectFiles

            ``` methodSignature
            public Optional<Double> getEstimatedProgressOfGeneratingProjectFiles()
            ```

            [Returns:]{.returnLabel}
            :   Estimated progress of generating projects stage. If
                return value is absent, it\'s impossible to compute the
                estimated progress.

        []{#getApproximateBuildProgress()}

        -   #### getApproximateBuildProgress

            ``` methodSignature
            public Optional<Double> getApproximateBuildProgress()
            ```

            [Returns:]{.returnLabel}
            :   Approximated progress of current build. Returns absent
                value if number of rules wasn\'t determined.

        []{#close()}

        -   #### close

            ``` methodSignature
            public void close()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `close` in interface `AutoCloseable`
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

-   [Overview](../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../deprecated-list.html)
-   [Index](../../../../../../index-all.html)
-   [Help](../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../allclasses.html)

<div>

<div>

JavaScript is disabled on your browser.

</div>

</div>

<div>

-   Summary: 
-   Nested \| 
-   [Field](#field.summary) \| 
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
-   [Constr](#constructor.detail) \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
