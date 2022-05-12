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
[Package]{.packageLabelInType} [com.facebook.buck.jvm.core](package-summary.html)
:::

## Interface JavaLibrary {#interface-javalibrary .title title="Interface JavaLibrary"}
:::

::: contentContainer
::: description
-   

    All Superinterfaces:
    :   `AllowsNonAnnotatedFields`, `BuildEngineAction`, `BuildRule`,
        `Comparable<BuildRule>`, `HasClasspathDeps`,
        `HasClasspathEntries`, `HasDesugarSupport`, `HasJavaAbi`,
        `HasJavaClassHashes`, `HasMavenCoordinates`, `HasNameAndType`,
        `HasRuntimeDeps`, `HasSources`

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `AndroidLibrary`, `AndroidPrebuiltAar`, `DefaultJavaLibrary`,
        `PrebuiltJar`

    ------------------------------------------------------------------------

        public interface JavaLibrary
        extends HasClasspathEntries, HasClasspathDeps, HasDesugarSupport, HasJavaAbi, HasJavaClassHashes, HasMavenCoordinates, HasRuntimeDeps, HasSources
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type   Interface            Description
          ------------------- -------------------- -------------
          `static class `     `JavaLibrary.Data`    

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Field                 | Description           |
        +=======================+=======================+=======================+
        | `static Flavor`       | `GWT_MODULE_FLAVOR`   | ::: block             |
        |                       |                       | This Buildable is     |
        |                       |                       | expected to support   |
        |                       |                       | the GWT flavor, which |
        |                       |                       | is a                  |
        |                       |                       | [`Buil                |
        |                       |                       | dRule`](../../core/ru |
        |                       |                       | les/BuildRule.html "i |
        |                       |                       | nterface in com.faceb |
        |                       |                       | ook.buck.core.rules") |
        |                       |                       | whose output file is  |
        |                       |                       | a JAR containing the  |
        |                       |                       | files necessary to    |
        |                       |                       | use this              |
        |                       |                       | [`JavaLibrar          |
        |                       |                       | y`](JavaLibrary.html  |
        |                       |                       | "interface in com.fac |
        |                       |                       | ebook.buck.jvm.core") |
        |                       |                       | as a GWT module.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static Flavor`       | `MAVEN_JAR`           | ::: block             |
        |                       |                       | For maven publishing  |
        |                       |                       | only dependencies     |
        |                       |                       | containing maven      |
        |                       |                       | coordinates will be   |
        |                       |                       | listed as             |
        |                       |                       | dependencies.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static Flavor`       | `SRC_JAR`             | ::: block             |
        |                       |                       | It\'s possible to ask |
        |                       |                       | a                     |
        |                       |                       | [`JavaLibrar          |
        |                       |                       | y`](JavaLibrary.html  |
        |                       |                       | "interface in com.fac |
        |                       |                       | ebook.buck.jvm.core") |
        |                       |                       | to collect its own    |
        |                       |                       | sources and build a   |
        |                       |                       | source jar.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                            Method                                 Description
          ------------------------------------------------------------ -------------------------------------- -------------
          `Optional<SourcePath>`                                       `getGeneratedAnnotationSourcePath()`    
          `com.google.common.collect.ImmutableSortedSet<SourcePath>`   `getJavaSrcs()`                         
          `com.google.common.collect.ImmutableSortedSet<SourcePath>`   `getResources()`                        
          `Optional<String>`                                           `getResourcesRoot()`                    
          `boolean`                                                    `hasAnnotationProcessing()`             
          `boolean`                                                    `neverMarkAsUnusedDependency()`         

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Abstract
          Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.core.build.action.BuildEngineAction}

            ### Methods inherited from interface com.facebook.buck.core.build.action.[BuildEngineAction](../../core/build/action/BuildEngineAction.html "interface in com.facebook.buck.core.build.action")

            `getDependencies, getSourcePathOutputs`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.BuildRule}

            ### Methods inherited from interface com.facebook.buck.core.rules.[BuildRule](../../core/rules/BuildRule.html "interface in com.facebook.buck.core.rules")

            `compareTo, getBuildDeps, getBuildSteps, getBuildTarget, getFullyQualifiedName, getProjectFilesystem, getSourcePathToOutput, hasBuildSteps, isCacheable, outputFileCanBeCopied, shouldRespectInputSizeLimitForRemoteExecution, toString, updateBuildRuleResolver`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.jvm.core.HasClasspathDeps}

            ### Methods inherited from interface com.facebook.buck.jvm.core.[HasClasspathDeps](HasClasspathDeps.html "interface in com.facebook.buck.jvm.core")

            `getDepsForTransitiveClasspathEntries`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.jvm.core.HasClasspathEntries}

            ### Methods inherited from interface com.facebook.buck.jvm.core.[HasClasspathEntries](HasClasspathEntries.html "interface in com.facebook.buck.jvm.core")

            `getImmediateClasspaths, getOutputClasspaths, getTransitiveClasspathDeps, getTransitiveClasspaths`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.jvm.core.HasDesugarSupport}

            ### Methods inherited from interface com.facebook.buck.jvm.core.[HasDesugarSupport](HasDesugarSupport.html "interface in com.facebook.buck.jvm.core")

            `isDesugarEnabled, isInterfaceMethodsDesugarEnabled`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.jvm.core.HasJavaAbi}

            ### Methods inherited from interface com.facebook.buck.jvm.core.[HasJavaAbi](HasJavaAbi.html "interface in com.facebook.buck.jvm.core")

            `getAbiInfo, getAbiJar, getSourceOnlyAbiJar`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.jvm.core.HasJavaClassHashes}

            ### Methods inherited from interface com.facebook.buck.jvm.core.[HasJavaClassHashes](HasJavaClassHashes.html "interface in com.facebook.buck.jvm.core")

            `getClassHashesProvider, getClassNamesToHashes`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.jvm.core.HasMavenCoordinates}

            ### Methods inherited from interface com.facebook.buck.jvm.core.[HasMavenCoordinates](HasMavenCoordinates.html "interface in com.facebook.buck.jvm.core")

            `getMavenCoords`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.HasNameAndType}

            ### Methods inherited from interface com.facebook.buck.core.rules.[HasNameAndType](../../core/rules/HasNameAndType.html "interface in com.facebook.buck.core.rules")

            `getType`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.attr.HasRuntimeDeps}

            ### Methods inherited from interface com.facebook.buck.core.rules.attr.[HasRuntimeDeps](../../core/rules/attr/HasRuntimeDeps.html "interface in com.facebook.buck.core.rules.attr")

            `getRuntimeDeps`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.jvm.core.HasSources}

            ### Methods inherited from interface com.facebook.buck.jvm.core.[HasSources](HasSources.html "interface in com.facebook.buck.jvm.core")

            `getSources`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#field.detail}

        ### Field Detail

        []{#GWT_MODULE_FLAVOR}

        -   #### GWT_MODULE_FLAVOR

                static final Flavor GWT_MODULE_FLAVOR

            ::: block
            This Buildable is expected to support the GWT flavor, which
            is a
            [`BuildRule`](../../core/rules/BuildRule.html "interface in com.facebook.buck.core.rules")
            whose output file is a JAR containing the files necessary to
            use this
            [`JavaLibrary`](JavaLibrary.html "interface in com.facebook.buck.jvm.core")
            as a GWT module. Normally, this includes Java source code, a
            .gwt.xml file, and static resources, such as stylesheets and
            image files.
            In the event that this
            [`JavaLibrary`](JavaLibrary.html "interface in com.facebook.buck.jvm.core")
            cannot be represented as a GWT module (for example, if it
            has no `srcs` or `resources` of its own, but only exists to
            export deps), then the flavor will be
            [`Optional.empty()`](http://docs.oracle.com/javase/7/docs/api/java/util/Optional.html?is-external=true#empty() "class or interface in java.util"){.externalLink}.

            Note that the output of the
            [`BuildRule`](../../core/rules/BuildRule.html "interface in com.facebook.buck.core.rules")
            for this flavor may contain `.class` files. For example, if
            a third-party releases its `.class` and `.java` files in the
            same JAR, it is common for a `prebuilt_jar()` to declare
            that file as both its `  binary_jar` and its `source_jar`.
            In that case, the output of the
            [`BuildRule`](../../core/rules/BuildRule.html "interface in com.facebook.buck.core.rules")
            will be the original JAR file, which is why it would contain
            `.class` files.
            :::

        []{#SRC_JAR}

        -   #### SRC_JAR

                static final Flavor SRC_JAR

            ::: block
            It\'s possible to ask a
            [`JavaLibrary`](JavaLibrary.html "interface in com.facebook.buck.jvm.core")
            to collect its own sources and build a source jar.
            :::

        []{#MAVEN_JAR}

        -   #### MAVEN_JAR

                static final Flavor MAVEN_JAR

            ::: block
            For maven publishing only dependencies containing maven
            coordinates will be listed as dependencies. Others will be
            packaged-in, and their first-order dependencies considered
            in the same manner
            :::
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getJavaSrcs()}

        -   #### getJavaSrcs

            ``` methodSignature
            com.google.common.collect.ImmutableSortedSet<SourcePath> getJavaSrcs()
            ```

        []{#getResources()}

        -   #### getResources

            ``` methodSignature
            com.google.common.collect.ImmutableSortedSet<SourcePath> getResources()
            ```

        []{#getResourcesRoot()}

        -   #### getResourcesRoot

            ``` methodSignature
            Optional<String> getResourcesRoot()
            ```

        []{#getGeneratedAnnotationSourcePath()}

        -   #### getGeneratedAnnotationSourcePath

            ``` methodSignature
            Optional<SourcePath> getGeneratedAnnotationSourcePath()
            ```

        []{#hasAnnotationProcessing()}

        -   #### hasAnnotationProcessing

            ``` methodSignature
            boolean hasAnnotationProcessing()
            ```

        []{#neverMarkAsUnusedDependency()}

        -   #### neverMarkAsUnusedDependency

            ``` methodSignature
            boolean neverMarkAsUnusedDependency()
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
