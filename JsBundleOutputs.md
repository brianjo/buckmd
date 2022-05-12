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
-   [Field](#field.summary) \| 
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
-   Constr \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.features.js](package-summary.html)
:::

## Interface JsBundleOutputs {#interface-jsbundleoutputs .title title="Interface JsBundleOutputs"}
:::

::: contentContainer
::: description
-   

    All Superinterfaces:
    :   `AllowsNonAnnotatedFields`, `BuildEngineAction`, `BuildRule`,
        `Comparable<BuildRule>`, `HasNameAndType`

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `JsBundle`, `JsBundleAndroid`, `JsBundleGenrule`

    ------------------------------------------------------------------------

        public interface JsBundleOutputs
        extends BuildRule

    ::: block
    Represents output paths of JS builds, consisting of JavaScript build
    output, a corresponding source map, \"misc\" directory that can
    contain diverse assets not meant to be part of the app being shipped
    and assets/resources used from within the packaged JS source code.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type   Field           Description
          ------------------- --------------- -------------
          `static String`     `JS_DIR_NAME`    

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type         Method                                                        Description
          ------------------------- ------------------------------------------------------------- -------------
          `String`                  `getBundleName()`                                              
          `JsDependenciesOutputs`   `getJsDependenciesOutputs​(ActionGraphBuilder graphBuilder)`    
          `default SourcePath`      `getSourcePathToMisc()`                                        
          `default SourcePath`      `getSourcePathToOutput()`                                      
          `default SourcePath`      `getSourcePathToResources()`                                   
          `default SourcePath`      `getSourcePathToSourceMap()`                                   

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Abstract
          Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
          .tableTab}[[Default
          Methods](javascript:show(16);)[ ]{.tabEnd}]{#t5 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.core.build.action.BuildEngineAction}

            ### Methods inherited from interface com.facebook.buck.core.build.action.[BuildEngineAction](../../core/build/action/BuildEngineAction.html "interface in com.facebook.buck.core.build.action")

            `getDependencies, getSourcePathOutputs`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.BuildRule}

            ### Methods inherited from interface com.facebook.buck.core.rules.[BuildRule](../../core/rules/BuildRule.html "interface in com.facebook.buck.core.rules")

            `compareTo, getBuildDeps, getBuildSteps, getBuildTarget, getFullyQualifiedName, getProjectFilesystem, hasBuildSteps, isCacheable, outputFileCanBeCopied, shouldRespectInputSizeLimitForRemoteExecution, toString, updateBuildRuleResolver`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.HasNameAndType}

            ### Methods inherited from interface com.facebook.buck.core.rules.[HasNameAndType](../../core/rules/HasNameAndType.html "interface in com.facebook.buck.core.rules")

            `getType`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#field.detail}

        ### Field Detail

        []{#JS_DIR_NAME}

        -   #### JS_DIR_NAME

                static final String JS_DIR_NAME

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.features.js.JsBundleOutputs.JS_DIR_NAME)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getBundleName()}

        -   #### getBundleName

            ``` methodSignature
            String getBundleName()
            ```

            [Returns:]{.returnLabel}
            :   the file name of the main JavaScript bundle file. This
                does not necessarily have to be the only JavaScript file
                written.

        []{#getSourcePathToOutput()}

        -   #### getSourcePathToOutput

            ``` methodSignature
            default SourcePath getSourcePathToOutput()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getSourcePathToOutput` in interface `BuildRule`

            [Returns:]{.returnLabel}
            :   the
                [`SourcePath`](../../core/sourcepath/SourcePath.html "interface in com.facebook.buck.core.sourcepath")
                to the directory containing the built JavaScript.

        []{#getSourcePathToSourceMap()}

        -   #### getSourcePathToSourceMap

            ``` methodSignature
            default SourcePath getSourcePathToSourceMap()
            ```

            [Returns:]{.returnLabel}
            :   a
                [`SourcePath`](../../core/sourcepath/SourcePath.html "interface in com.facebook.buck.core.sourcepath")
                to a source map belonging to the built JavaScript.
                Typically a single file.

        []{#getSourcePathToResources()}

        -   #### getSourcePathToResources

            ``` methodSignature
            default SourcePath getSourcePathToResources()
            ```

            [Returns:]{.returnLabel}
            :   the
                [`SourcePath`](../../core/sourcepath/SourcePath.html "interface in com.facebook.buck.core.sourcepath")
                to a directory containing the resources (or assets) used
                by the bundled JavaScript source code.

        []{#getSourcePathToMisc()}

        -   #### getSourcePathToMisc

            ``` methodSignature
            default SourcePath getSourcePathToMisc()
            ```

            [Returns:]{.returnLabel}
            :   the
                [`SourcePath`](../../core/sourcepath/SourcePath.html "interface in com.facebook.buck.core.sourcepath")
                to a directory containing various metadata that can be
                used by dependent rules but are not meant to be shipped
                with the application.

        []{#getJsDependenciesOutputs(com.facebook.buck.core.rules.ActionGraphBuilder)}

        -   #### getJsDependenciesOutputs

            ``` methodSignature
            JsDependenciesOutputs getJsDependenciesOutputs​(ActionGraphBuilder graphBuilder)
            ```

            [Returns:]{.returnLabel}
            :   the
                [`JsDependenciesOutputs`](JsDependenciesOutputs.html "interface in com.facebook.buck.features.js")
                rule which is responsible for building the dependencies
                file.
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
-   [Field](#field.summary) \| 
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
-   Constr \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
