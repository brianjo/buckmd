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
-   [Nested](#nested.class.summary) \| 
-   Field \| 
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.android](package-summary.html)
:::

## Class AndroidInstrumentationApk {#class-androidinstrumentationapk .title title="Class AndroidInstrumentationApk"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.core.rules.impl.AbstractBuildRule](../core/rules/impl/AbstractBuildRule.html "class in com.facebook.buck.core.rules.impl")

    -   -   [com.facebook.buck.android.AndroidBinary](AndroidBinary.html "class in com.facebook.buck.android")

        -   -   com.facebook.buck.android.AndroidInstrumentationApk

::: description
-   

    All Implemented Interfaces:
    :   `HasInstallableApk`, `BuildEngineAction`,
        `AllowsNonAnnotatedFields`, `HasDeclaredAndExtraDeps`,
        `HasInstallHelpers`, `HasRuntimeDeps`,
        `SupportsInputBasedRuleKey`, `BuildRule`, `HasNameAndType`,
        `HasClasspathDeps`, `HasClasspathEntries`,
        `Comparable<BuildRule>`

    ------------------------------------------------------------------------

        public class AndroidInstrumentationApk
        extends AndroidBinary

    ::: block
    Apk that functions as a test package in Android.
    Android\'s [Testing
    Fundamentals](http://developer.android.com/tools/testing/testing_android.html)
    documentation includes a diagram that shows the relationship between
    an \"application package\" and a \"test package\" when running a
    test. This corresponds to a test package. Note that a test package
    has an interesting quirk where it is *compiled against* an
    application package, but *must not include* the resources or Java
    classes of the application package. Therefore, this class takes
    responsibility for making sure the appropriate bits are excluded.
    Failing to do so will generate mysterious runtime errors when
    running the test.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        -   []{#nested.classes.inherited.from.class.com.facebook.buck.android.HasInstallableApk}

            ### Nested classes/interfaces inherited from interface com.facebook.buck.android.[HasInstallableApk](HasInstallableApk.html "interface in com.facebook.buck.android")

            `HasInstallableApk.ApkInfo`
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                        Method                                                  Description
          ---------------------------------------- ------------------------------------------------------- -------------
          `AndroidBinary`                          `getApkUnderTest()`                                      
          `java.util.stream.Stream<BuildTarget>`   `getInstallHelpers()`                                    
          `java.util.stream.Stream<BuildTarget>`   `getRuntimeDeps​(BuildRuleResolver buildRuleResolver)`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.android.AndroidBinary}

            ### Methods inherited from class com.facebook.buck.android.[AndroidBinary](AndroidBinary.html "class in com.facebook.buck.android")

            `deprecatedGetExtraDeps, getAndroidPackageableCollection, getApkInfo, getBuildDeps, getBuildSteps, getBuildTargetsToExcludeFromDex, getCpuFilters, getDeclaredDeps, getDepsForTransitiveClasspathEntries, getImmediateClasspaths, getKeystore, getManifestEntries, getOptimizationPasses, getOutputClasspaths, getProguardConfig, getProguardJvmArgs, getResourceCompressionMode, getResourceFilter, getRulesToExcludeFromDex, getSkipProguard, getSourcePathToOutput, getTargetGraphOnlyDeps, getTransitiveClasspathDeps, getTransitiveClasspaths, inputBasedRuleKeyIsEnabled, isCacheable`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.impl.AbstractBuildRule}

            ### Methods inherited from class com.facebook.buck.core.rules.impl.[AbstractBuildRule](../core/rules/impl/AbstractBuildRule.html "class in com.facebook.buck.core.rules.impl")

            `equals, getBuildTarget, getDependencies, getProjectFilesystem, getSourcePathOutputs, getType, hasBuildSteps, hashCode, injectFields, toString, updateBuildRuleResolver`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, finalize, getClass, notify, notifyAll, wait, wait, wait`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.build.action.BuildEngineAction}

            ### Methods inherited from interface com.facebook.buck.core.build.action.[BuildEngineAction](../core/build/action/BuildEngineAction.html "interface in com.facebook.buck.core.build.action")

            `getDependencies, getSourcePathOutputs`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.BuildRule}

            ### Methods inherited from interface com.facebook.buck.core.rules.[BuildRule](../core/rules/BuildRule.html "interface in com.facebook.buck.core.rules")

            `compareTo, getBuildTarget, getFullyQualifiedName, getProjectFilesystem, hasBuildSteps, outputFileCanBeCopied, shouldRespectInputSizeLimitForRemoteExecution, toString, updateBuildRuleResolver`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.android.HasInstallableApk}

            ### Methods inherited from interface com.facebook.buck.android.[HasInstallableApk](HasInstallableApk.html "interface in com.facebook.buck.android")

            `getBuildTarget, getProjectFilesystem`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.HasNameAndType}

            ### Methods inherited from interface com.facebook.buck.core.rules.[HasNameAndType](../core/rules/HasNameAndType.html "interface in com.facebook.buck.core.rules")

            `getType`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getInstallHelpers()}

        -   #### getInstallHelpers

            ``` methodSignature
            public java.util.stream.Stream<BuildTarget> getInstallHelpers()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getInstallHelpers` in interface `HasInstallHelpers`

            [Overrides:]{.overrideSpecifyLabel}
            :   `getInstallHelpers` in class `AndroidBinary`

        []{#getApkUnderTest()}

        -   #### getApkUnderTest

            ``` methodSignature
            public AndroidBinary getApkUnderTest()
            ```

        []{#getRuntimeDeps(com.facebook.buck.core.rules.BuildRuleResolver)}

        -   #### getRuntimeDeps

            ``` methodSignature
            public java.util.stream.Stream<BuildTarget> getRuntimeDeps​(BuildRuleResolver buildRuleResolver)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getRuntimeDeps` in interface `HasRuntimeDeps`

            [Overrides:]{.overrideSpecifyLabel}
            :   `getRuntimeDeps` in class `AndroidBinary`
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
-   [Nested](#nested.class.summary) \| 
-   Field \| 
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   Constr \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
