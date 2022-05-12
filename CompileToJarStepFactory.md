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

## Class CompileToJarStepFactory {#class-compiletojarstepfactory .title title="Class CompileToJarStepFactory"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.jvm.java.CompileToJarStepFactory

::: description
-   

    All Implemented Interfaces:
    :   `AddsToRuleKey`

    ```{=html}
    <!-- -->
    ```

    Direct Known Subclasses:
    :   `JavacToJarStepFactory`, `KotlincToJarStepFactory`,
        `ScalacToJarStepFactory`

    ------------------------------------------------------------------------

        public abstract class CompileToJarStepFactory
        extends Object
        implements AddsToRuleKey

    ::: block
    Provides a base implementation for post compile steps.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Modifier       Constructor                   Description
          -------------- ----------------------------- -------------
          `protected `   `CompileToJarStepFactory()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `protected void`      | `addCompiler          |                       |
        |                       | SetupSteps​(BuildConte |                       |
        |                       | xt context,           |                       |
        |                       |             ProjectFi |                       |
        |                       | lesystem projectFiles |                       |
        |                       | ystem,                |                       |
        |                       |        BuildTarget ta |                       |
        |                       | rget,                 |                       |
        |                       |       CompilerParamet |                       |
        |                       | ers compilerParameter |                       |
        |                       | s,                    |                       |
        |                       |    ResourcesParameter |                       |
        |                       | s resourcesParameters |                       |
        |                       | ,                     |                       |
        |                       |   com.google.common.c |                       |
        |                       | ollect.ImmutableList. |                       |
        |                       | Builder<Step> steps)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected void`      | `add                  |                       |
        |                       | JarCreationSteps​(Proj |                       |
        |                       | ectFilesystem project |                       |
        |                       | Filesystem,           |                       |
        |                       |           CompilerPar |                       |
        |                       | ameters compilerParam |                       |
        |                       | eters,                |                       |
        |                       |      com.google.commo |                       |
        |                       | n.collect.ImmutableLi |                       |
        |                       | st.Builder<Step> step |                       |
        |                       | s,                    |                       |
        |                       |  BuildableContext bui |                       |
        |                       | ldableContext,        |                       |
        |                       |              JarParam |                       |
        |                       | eters jarParameters)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected void`      | `addJ                 |                       |
        |                       | arSetupSteps​(ProjectF |                       |
        |                       | ilesystem projectFile |                       |
        |                       | system,               |                       |
        |                       |    BuildContext conte |                       |
        |                       | xt,                 J |                       |
        |                       | arParameters jarParam |                       |
        |                       | eters,                |                       |
        |                       |   com.google.common.c |                       |
        |                       | ollect.ImmutableList. |                       |
        |                       | Builder<Step> steps)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract void`       | `                     |                       |
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
        |                       | leToJarStep​(BuildCont |                       |
        |                       | ext context,          |                       |
        |                       |               Project |                       |
        |                       | Filesystem projectFil |                       |
        |                       | esystem,              |                       |
        |                       |           BuildTarget |                       |
        |                       |  target,              |                       |
        |                       |           CompilerPar |                       |
        |                       | ameters compilerParam |                       |
        |                       | eters,                |                       |
        |                       |         ResourcesPara |                       |
        |                       | meters resourcesParam |                       |
        |                       | eters,                |                       |
        |                       |         com.google.co |                       |
        |                       | mmon.collect.Immutabl |                       |
        |                       | eList<String> postpro |                       |
        |                       | cessClassesCommands,  |                       |
        |                       |                       |                       |
        |                       |  JarParameters abiJar |                       |
        |                       | Parameters,           |                       |
        |                       |              JarParam |                       |
        |                       | eters libraryJarParam |                       |
        |                       | eters,                |                       |
        |                       |         com.google.co |                       |
        |                       | mmon.collect.Immutabl |                       |
        |                       | eList.Builder<Step> s |                       |
        |                       | teps,                 |                       |
        |                       |        BuildableConte |                       |
        |                       | xt buildableContext)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected void`      | `creat                |                       |
        |                       | eCompileToJarStepImpl |                       |
        |                       | ​(ProjectFilesystem pr |                       |
        |                       | ojectFilesystem,      |                       |
        |                       |                       |                       |
        |                       |  BuildContext context |                       |
        |                       | ,                     |                       |
        |                       |        BuildTarget ta |                       |
        |                       | rget,                 |                       |
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
        | `void`                | `createJarStep​(Pro    |                       |
        |                       | jectFilesystem projec |                       |
        |                       | tFilesystem,          |                       |
        |                       |      JarParameters pa |                       |
        |                       | rameters,             |                       |
        |                       |   com.google.common.c |                       |
        |                       | ollect.ImmutableList. |                       |
        |                       | Builder<Step> steps)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protec               | `getBootClasspath​(B   | ::: block             |
        | ted Optional<String>` | uildContext context)` | This can be used make |
        |                       |                       | the bootclasspath if  |
        |                       |                       | available, to the     |
        |                       |                       | postprocess classes   |
        |                       |                       | commands.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `abstract boolean`    | `hasAn                |                       |
        |                       | notationProcessing()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected void`      | `recordDepFileIfN     |                       |
        |                       | ecessary​(ProjectFiles |                       |
        |                       | ystem filesystem,     |                       |
        |                       |                       |                       |
        |                       | BuildTarget buildTarg |                       |
        |                       | et,                   |                       |
        |                       |        CompilerParame |                       |
        |                       | ters compilerParamete |                       |
        |                       | rs,                   |                       |
        |                       |        BuildableConte |                       |
        |                       | xt buildableContext)` |                       |
        +-----------------------+-----------------------+-----------------------+

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

        -   #### CompileToJarStepFactory

                protected CompileToJarStepFactory()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#createCompileToJarStep(com.facebook.buck.core.build.context.BuildContext,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.model.BuildTarget,com.facebook.buck.jvm.java.CompilerParameters,com.facebook.buck.jvm.java.ResourcesParameters,com.google.common.collect.ImmutableList,com.facebook.buck.jvm.java.JarParameters,com.facebook.buck.jvm.java.JarParameters,com.google.common.collect.ImmutableList.Builder,com.facebook.buck.core.build.buildable.context.BuildableContext)}

        -   #### createCompileToJarStep

            ``` methodSignature
            public final void createCompileToJarStep​(BuildContext context,
                                                     ProjectFilesystem projectFilesystem,
                                                     BuildTarget target,
                                                     CompilerParameters compilerParameters,
                                                     ResourcesParameters resourcesParameters,
                                                     com.google.common.collect.ImmutableList<String> postprocessClassesCommands,
                                                     @Nullable
                                                     JarParameters abiJarParameters,
                                                     @Nullable
                                                     JarParameters libraryJarParameters,
                                                     com.google.common.collect.ImmutableList.Builder<Step> steps,
                                                     BuildableContext buildableContext)
            ```

        []{#addCompilerSetupSteps(com.facebook.buck.core.build.context.BuildContext,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.model.BuildTarget,com.facebook.buck.jvm.java.CompilerParameters,com.facebook.buck.jvm.java.ResourcesParameters,com.google.common.collect.ImmutableList.Builder)}

        -   #### addCompilerSetupSteps

            ``` methodSignature
            protected void addCompilerSetupSteps​(BuildContext context,
                                                 ProjectFilesystem projectFilesystem,
                                                 BuildTarget target,
                                                 CompilerParameters compilerParameters,
                                                 ResourcesParameters resourcesParameters,
                                                 com.google.common.collect.ImmutableList.Builder<Step> steps)
            ```

        []{#addJarSetupSteps(com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.build.context.BuildContext,com.facebook.buck.jvm.java.JarParameters,com.google.common.collect.ImmutableList.Builder)}

        -   #### addJarSetupSteps

            ``` methodSignature
            protected void addJarSetupSteps​(ProjectFilesystem projectFilesystem,
                                            BuildContext context,
                                            JarParameters jarParameters,
                                            com.google.common.collect.ImmutableList.Builder<Step> steps)
            ```

        []{#recordDepFileIfNecessary(com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.model.BuildTarget,com.facebook.buck.jvm.java.CompilerParameters,com.facebook.buck.core.build.buildable.context.BuildableContext)}

        -   #### recordDepFileIfNecessary

            ``` methodSignature
            protected void recordDepFileIfNecessary​(ProjectFilesystem filesystem,
                                                    BuildTarget buildTarget,
                                                    CompilerParameters compilerParameters,
                                                    BuildableContext buildableContext)
            ```

        []{#addJarCreationSteps(com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.jvm.java.CompilerParameters,com.google.common.collect.ImmutableList.Builder,com.facebook.buck.core.build.buildable.context.BuildableContext,com.facebook.buck.jvm.java.JarParameters)}

        -   #### addJarCreationSteps

            ``` methodSignature
            protected void addJarCreationSteps​(ProjectFilesystem projectFilesystem,
                                               CompilerParameters compilerParameters,
                                               com.google.common.collect.ImmutableList.Builder<Step> steps,
                                               BuildableContext buildableContext,
                                               JarParameters jarParameters)
            ```

        []{#createCompileToJarStepImpl(com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.build.context.BuildContext,com.facebook.buck.core.model.BuildTarget,com.facebook.buck.jvm.java.CompilerParameters,com.google.common.collect.ImmutableList,com.facebook.buck.jvm.java.JarParameters,com.facebook.buck.jvm.java.JarParameters,com.google.common.collect.ImmutableList.Builder,com.facebook.buck.core.build.buildable.context.BuildableContext)}

        -   #### createCompileToJarStepImpl

            ``` methodSignature
            protected void createCompileToJarStepImpl​(ProjectFilesystem projectFilesystem,
                                                      BuildContext context,
                                                      BuildTarget target,
                                                      CompilerParameters compilerParameters,
                                                      com.google.common.collect.ImmutableList<String> postprocessClassesCommands,
                                                      @Nullable
                                                      JarParameters abiJarParameters,
                                                      @Nullable
                                                      JarParameters libraryJarParameters,
                                                      com.google.common.collect.ImmutableList.Builder<Step> steps,
                                                      BuildableContext buildableContext)
            ```

        []{#createJarStep(com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.jvm.java.JarParameters,com.google.common.collect.ImmutableList.Builder)}

        -   #### createJarStep

            ``` methodSignature
            public void createJarStep​(ProjectFilesystem projectFilesystem,
                                      JarParameters parameters,
                                      com.google.common.collect.ImmutableList.Builder<Step> steps)
            ```

        []{#getBootClasspath(com.facebook.buck.core.build.context.BuildContext)}

        -   #### getBootClasspath

            ``` methodSignature
            protected Optional<String> getBootClasspath​(BuildContext context)
            ```

            ::: block
            This can be used make the bootclasspath if available, to the
            postprocess classes commands.
            :::

            [Returns:]{.returnLabel}
            :   the bootclasspath.

        []{#createCompileStep(com.facebook.buck.core.build.context.BuildContext,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.model.BuildTarget,com.facebook.buck.jvm.java.CompilerParameters,com.google.common.collect.ImmutableList.Builder,com.facebook.buck.core.build.buildable.context.BuildableContext)}

        -   #### createCompileStep

            ``` methodSignature
            public abstract void createCompileStep​(BuildContext context,
                                                   ProjectFilesystem projectFilesystem,
                                                   BuildTarget invokingRule,
                                                   CompilerParameters parameters,
                                                   com.google.common.collect.ImmutableList.Builder<Step> steps,
                                                   BuildableContext buildableContext)
            ```

        []{#hasAnnotationProcessing()}

        -   #### hasAnnotationProcessing

            ``` methodSignature
            public abstract boolean hasAnnotationProcessing()
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
