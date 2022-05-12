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
[Package]{.packageLabelInType} [com.facebook.buck.core.rules.attr](package-summary.html)
:::

## Interface HasRuntimeDeps {#interface-hasruntimedeps .title title="Interface HasRuntimeDeps"}
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

    All Known Subinterfaces:
    :   `JavaLibrary`

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `AndroidBinary`, `AndroidBinaryNonExoInstaller`,
        `AndroidBundle`, `AndroidInstrumentationApk`,
        `AndroidInstrumentationTest`, `AndroidLibrary`,
        `AndroidPrebuiltAar`, `ApkGenrule`, `AppleBundle`,
        `AppleDebuggableBinary`, `AppleTest`, `AppleTestX`,
        `BinaryWrapperRule`, `CommandAlias`, `CxxBinary`,
        `CxxCompilationDatabase`, `CxxLibraryGroup`,
        `CxxPythonExtension`, `CxxTest`, `DBinary`,
        `DefaultJavaLibrary`, `DefaultWorkerToolRule`,
        `DependencyAggregation`, `DTest`, `ExportFile`, `GoBinary`,
        `GoTest`, `GoTestX`, `HaskellBinary`, `HeaderSymlinkTree`,
        `HeaderSymlinkTreeWithHeaderMap`,
        `HeaderSymlinkTreeWithModuleMap`, `JavaBinary`, `JavaTest`,
        `JavaTestX`, `JsBundleGenrule`, `LuaBinary`,
        `MappedSymlinkTree`, `OcamlBinary`, `PrebuiltJar`,
        `PythonBinary`, `PythonInPlaceBinary`, `PythonLibrary`,
        `PythonPackagedBinary`, `PythonSymlinkTree`, `PythonTest`,
        `PythonTestX`, `RobolectricTest`, `RobolectricTestX`,
        `RustTest`, `ShBinary`, `ShTest`, `SymlinkTree`,
        `UnstrippedNativeLibraries`

    ------------------------------------------------------------------------

        public interface HasRuntimeDeps
        extends BuildRule

    ::: block
    Provides a facility for a rule to list dependencies it\'ll need at
    runtime.
    Consider the case of a Java test. The
    [`JavaTest`](../../../jvm/java/JavaTest.html "class in com.facebook.buck.jvm.java")
    rule itself is just a
    [`DefaultJavaLibrary`](../../../jvm/java/DefaultJavaLibrary.html "class in com.facebook.buck.jvm.java")
    and so only lists its immediate compile time deps as its normal
    first-order dependencies. However, to actually run a Java test, we
    need it\'s entire transitive dependency tree locally on disk. Since
    this is outside the contract of normal build dependencies (e.g. a
    top-down build engine may decide not to pull a dependency locally if
    the top-level target can be pulled from cache, and therefore won\'t
    need to be built), we need some other way to convey to the build
    engine that a set of rules that need to be on disk by the end of the
    build.

    Enter this interface. While it serves an important purpose, its
    long-term semantics aren\'t entirely clear yet, so expect how we
    model this and how the build engine uses this to change in the
    future.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                        Method                                                  Description
          ---------------------------------------- ------------------------------------------------------- -------------
          `java.util.stream.Stream<BuildTarget>`   `getRuntimeDeps​(BuildRuleResolver buildRuleResolver)`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Abstract
          Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.core.build.action.BuildEngineAction}

            ### Methods inherited from interface com.facebook.buck.core.build.action.[BuildEngineAction](../../build/action/BuildEngineAction.html "interface in com.facebook.buck.core.build.action")

            `getDependencies, getSourcePathOutputs`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.BuildRule}

            ### Methods inherited from interface com.facebook.buck.core.rules.[BuildRule](../BuildRule.html "interface in com.facebook.buck.core.rules")

            `compareTo, getBuildDeps, getBuildSteps, getBuildTarget, getFullyQualifiedName, getProjectFilesystem, getSourcePathToOutput, hasBuildSteps, isCacheable, outputFileCanBeCopied, shouldRespectInputSizeLimitForRemoteExecution, toString, updateBuildRuleResolver`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.HasNameAndType}

            ### Methods inherited from interface com.facebook.buck.core.rules.[HasNameAndType](../HasNameAndType.html "interface in com.facebook.buck.core.rules")

            `getType`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getRuntimeDeps(com.facebook.buck.core.rules.BuildRuleResolver)}

        -   #### getRuntimeDeps

            ``` methodSignature
            java.util.stream.Stream<BuildTarget> getRuntimeDeps​(BuildRuleResolver buildRuleResolver)
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
