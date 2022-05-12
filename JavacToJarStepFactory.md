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
[Package]{.packageLabelInType} [com.facebook.buck.jvm.java](package-summary.html)
:::

## Class JavacToJarStepFactory {#class-javactojarstepfactory .title title="Class JavacToJarStepFactory"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.jvm.java.CompileToJarStepFactory](CompileToJarStepFactory.html "class in com.facebook.buck.jvm.java")

    -   -   com.facebook.buck.jvm.java.JavacToJarStepFactory

::: description
-   

    All Implemented Interfaces:
    :   `AddsToRuleKey`

    ------------------------------------------------------------------------

        public class JavacToJarStepFactory
        extends CompileToJarStepFactory
        implements AddsToRuleKey
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                Description
          ---------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `JavacToJarStepFactory​(Javac javac,                      JavacOptions javacOptions,                      ExtraClasspathProvider extraClasspathProvider)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `void`                | `                     |                       |
        |                       | createCompileStep​(Bui |                       |
        |                       | ldContext context,    |                       |
        |                       |                Projec |                       |
        |                       | tFilesystem projectFi |                       |
        |                       | lesystem,             |                       |
        |                       |       BuildTarget inv |                       |
        |                       | okingRule,            |                       |
        |                       |        CompilerParame |                       |
        |                       | ters parameters,      |                       |
        |                       |              com.goog |                       |
        |                       | le.common.collect.Imm |                       |
        |                       | utableList.Builder<St |                       |
        |                       | ep> steps,            |                       |
        |                       |        BuildableConte |                       |
        |                       | xt buildableContext)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `createCompi          |                       |
        |                       | leToJarStepImpl​(Proje |                       |
        |                       | ctFilesystem projectF |                       |
        |                       | ilesystem,            |                       |
        |                       |                 Build |                       |
        |                       | Context context,      |                       |
        |                       |                       |                       |
        |                       |  BuildTarget invoking |                       |
        |                       | Rule,                 |                       |
        |                       |            CompilerPa |                       |
        |                       | rameters compilerPara |                       |
        |                       | meters,               |                       |
        |                       |              com.goog |                       |
        |                       | le.common.collect.Imm |                       |
        |                       | utableList<String> po |                       |
        |                       | stprocessClassesComma |                       |
        |                       | nds,                  |                       |
        |                       |           JarParamete |                       |
        |                       | rs abiJarParameters,  |                       |
        |                       |                       |                       |
        |                       |      JarParameters li |                       |
        |                       | braryJarParameters,   |                       |
        |                       |                       |                       |
        |                       |     com.google.common |                       |
        |                       | .collect.ImmutableLis |                       |
        |                       | t.Builder<Step> steps |                       |
        |                       | ,                     |                       |
        |                       |        BuildableConte |                       |
        |                       | xt buildableContext)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `createPipeli         |                       |
        |                       | nedCompileStep​(BuildC |                       |
        |                       | ontext context,       |                       |
        |                       |                       |                       |
        |                       | ProjectFilesystem pro |                       |
        |                       | jectFilesystem,       |                       |
        |                       |                       |                       |
        |                       | JavacPipelineState pi |                       |
        |                       | peline,               |                       |
        |                       |              BuildTar |                       |
        |                       | get invokingRule,     |                       |
        |                       |                       |                       |
        |                       |   com.google.common.c |                       |
        |                       | ollect.ImmutableList. |                       |
        |                       | Builder<Step> steps)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `cre                  |                       |
        |                       | atePipelinedCompileTo |                       |
        |                       | JarStep​(BuildContext  |                       |
        |                       | context,              |                       |
        |                       |                    Pr |                       |
        |                       | ojectFilesystem proje |                       |
        |                       | ctFilesystem,         |                       |
        |                       |                       |                       |
        |                       |    BuildTarget target |                       |
        |                       | ,                     |                       |
        |                       |             JavacPipe |                       |
        |                       | lineState pipeline,   |                       |
        |                       |                       |                       |
        |                       |          ResourcesPar |                       |
        |                       | ameters resourcesPara |                       |
        |                       | meters,               |                       |
        |                       |                   com |                       |
        |                       | .google.common.collec |                       |
        |                       | t.ImmutableList<Strin |                       |
        |                       | g> postprocessClasses |                       |
        |                       | Commands,             |                       |
        |                       |                     c |                       |
        |                       | om.google.common.coll |                       |
        |                       | ect.ImmutableList.Bui |                       |
        |                       | lder<Step> steps,     |                       |
        |                       |                       |                       |
        |                       |        BuildableConte |                       |
        |                       | xt buildableContext)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `JavacPipelineState`  | `                     |                       |
        |                       | createPipelineState​(B |                       |
        |                       | uildTarget invokingRu |                       |
        |                       | le,                   |                       |
        |                       |   CompilerParameters  |                       |
        |                       | compilerParameters,   |                       |
        |                       |                   Jar |                       |
        |                       | Parameters abiJarPara |                       |
        |                       | meters,               |                       |
        |                       |       JarParameters l |                       |
        |                       | ibraryJarParameters)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protec               | `getBootClasspath​(B   | ::: block             |
        | ted Optional<String>` | uildContext context)` | This can be used make |
        |                       |                       | the bootclasspath if  |
        |                       |                       | available, to the     |
        |                       |                       | postprocess classes   |
        |                       |                       | commands.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JavacOptions`        | `getJavacOptions()`   |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `hasAn                |                       |
        |                       | notationProcessing()` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.jvm.java.CompileToJarStepFactory}

            ### Methods inherited from class com.facebook.buck.jvm.java.[CompileToJarStepFactory](CompileToJarStepFactory.html "class in com.facebook.buck.jvm.java")

            `addCompilerSetupSteps, addJarCreationSteps, addJarSetupSteps, createCompileToJarStep, createJarStep, recordDepFileIfNecessary`

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

        []{#<init>(com.facebook.buck.jvm.java.Javac,com.facebook.buck.jvm.java.JavacOptions,com.facebook.buck.jvm.java.ExtraClasspathProvider)}

        -   #### JavacToJarStepFactory

                public JavacToJarStepFactory​(Javac javac,
                                             JavacOptions javacOptions,
                                             ExtraClasspathProvider extraClasspathProvider)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#createPipelineState(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.jvm.java.CompilerParameters,com.facebook.buck.jvm.java.JarParameters,com.facebook.buck.jvm.java.JarParameters)}

        -   #### createPipelineState

            ``` methodSignature
            public JavacPipelineState createPipelineState​(BuildTarget invokingRule,
                                                          CompilerParameters compilerParameters,
                                                          @Nullable
                                                          JarParameters abiJarParameters,
                                                          @Nullable
                                                          JarParameters libraryJarParameters)
            ```

        []{#createCompileStep(com.facebook.buck.core.build.context.BuildContext,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.model.BuildTarget,com.facebook.buck.jvm.java.CompilerParameters,com.google.common.collect.ImmutableList.Builder,com.facebook.buck.core.build.buildable.context.BuildableContext)}

        -   #### createCompileStep

            ``` methodSignature
            public void createCompileStep​(BuildContext context,
                                          ProjectFilesystem projectFilesystem,
                                          BuildTarget invokingRule,
                                          CompilerParameters parameters,
                                          com.google.common.collect.ImmutableList.Builder<Step> steps,
                                          BuildableContext buildableContext)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `createCompileStep` in class `CompileToJarStepFactory`

        []{#createPipelinedCompileToJarStep(com.facebook.buck.core.build.context.BuildContext,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.model.BuildTarget,com.facebook.buck.jvm.java.JavacPipelineState,com.facebook.buck.jvm.java.ResourcesParameters,com.google.common.collect.ImmutableList,com.google.common.collect.ImmutableList.Builder,com.facebook.buck.core.build.buildable.context.BuildableContext)}

        -   #### createPipelinedCompileToJarStep

            ``` methodSignature
            public final void createPipelinedCompileToJarStep​(BuildContext context,
                                                              ProjectFilesystem projectFilesystem,
                                                              BuildTarget target,
                                                              JavacPipelineState pipeline,
                                                              ResourcesParameters resourcesParameters,
                                                              com.google.common.collect.ImmutableList<String> postprocessClassesCommands,
                                                              com.google.common.collect.ImmutableList.Builder<Step> steps,
                                                              BuildableContext buildableContext)
            ```

        []{#getBootClasspath(com.facebook.buck.core.build.context.BuildContext)}

        -   #### getBootClasspath

            ``` methodSignature
            protected Optional<String> getBootClasspath​(BuildContext context)
            ```

            ::: block
            [Description copied from
            class: `CompileToJarStepFactory`]{.descfrmTypeLabel}
            :::

            ::: block
            This can be used make the bootclasspath if available, to the
            postprocess classes commands.
            :::

            [Overrides:]{.overrideSpecifyLabel}
            :   `getBootClasspath` in class `CompileToJarStepFactory`

            [Returns:]{.returnLabel}
            :   the bootclasspath.

        []{#createCompileToJarStepImpl(com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.build.context.BuildContext,com.facebook.buck.core.model.BuildTarget,com.facebook.buck.jvm.java.CompilerParameters,com.google.common.collect.ImmutableList,com.facebook.buck.jvm.java.JarParameters,com.facebook.buck.jvm.java.JarParameters,com.google.common.collect.ImmutableList.Builder,com.facebook.buck.core.build.buildable.context.BuildableContext)}

        -   #### createCompileToJarStepImpl

            ``` methodSignature
            public void createCompileToJarStepImpl​(ProjectFilesystem projectFilesystem,
                                                   BuildContext context,
                                                   BuildTarget invokingRule,
                                                   CompilerParameters compilerParameters,
                                                   com.google.common.collect.ImmutableList<String> postprocessClassesCommands,
                                                   @Nullable
                                                   JarParameters abiJarParameters,
                                                   @Nullable
                                                   JarParameters libraryJarParameters,
                                                   com.google.common.collect.ImmutableList.Builder<Step> steps,
                                                   BuildableContext buildableContext)
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `createCompileToJarStepImpl` in
                class `CompileToJarStepFactory`

        []{#createPipelinedCompileStep(com.facebook.buck.core.build.context.BuildContext,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.jvm.java.JavacPipelineState,com.facebook.buck.core.model.BuildTarget,com.google.common.collect.ImmutableList.Builder)}

        -   #### createPipelinedCompileStep

            ``` methodSignature
            public void createPipelinedCompileStep​(BuildContext context,
                                                   ProjectFilesystem projectFilesystem,
                                                   JavacPipelineState pipeline,
                                                   BuildTarget invokingRule,
                                                   com.google.common.collect.ImmutableList.Builder<Step> steps)
            ```

        []{#getJavacOptions()}

        -   #### getJavacOptions

            ``` methodSignature
            public JavacOptions getJavacOptions()
            ```

        []{#hasAnnotationProcessing()}

        -   #### hasAnnotationProcessing

            ``` methodSignature
            public boolean hasAnnotationProcessing()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `hasAnnotationProcessing` in
                class `CompileToJarStepFactory`
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
