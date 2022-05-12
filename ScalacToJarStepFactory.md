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
[Package]{.packageLabelInType} [com.facebook.buck.jvm.scala](package-summary.html)
:::

## Class ScalacToJarStepFactory {#class-scalactojarstepfactory .title title="Class ScalacToJarStepFactory"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.jvm.java.CompileToJarStepFactory](../java/CompileToJarStepFactory.html "class in com.facebook.buck.jvm.java")

    -   -   com.facebook.buck.jvm.scala.ScalacToJarStepFactory

::: description
-   

    All Implemented Interfaces:
    :   `AddsToRuleKey`

    ------------------------------------------------------------------------

        public class ScalacToJarStepFactory
        extends CompileToJarStepFactory
        implements AddsToRuleKey
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                                                                                                                                                                                                        Description
          ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ -------------
          `ScalacToJarStepFactory​(Tool scalac,                       com.google.common.collect.ImmutableList<String> configCompilerFlags,                       com.google.common.collect.ImmutableList<String> extraArguments,                       com.google.common.collect.ImmutableSet<BuildRule> compilerPlugins,                       Javac javac,                       JavacOptions javacOptions,                       ExtraClasspathProvider extraClassPath)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                                                                                                                                                                                                                                                                                                                         Description
          ------------------- ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ -------------
          `void`              `createCompileStep​(BuildContext context,                  ProjectFilesystem projectFilesystem,                  BuildTarget invokingRule,                  CompilerParameters parameters,                  com.google.common.collect.ImmutableList.Builder<Step> steps,                  BuildableContext buildableContext)`    
          `boolean`           `hasAnnotationProcessing()`                                                                                                                                                                                                                                                                                                     

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.jvm.java.CompileToJarStepFactory}

            ### Methods inherited from class com.facebook.buck.jvm.java.[CompileToJarStepFactory](../java/CompileToJarStepFactory.html "class in com.facebook.buck.jvm.java")

            `addCompilerSetupSteps, addJarCreationSteps, addJarSetupSteps, createCompileToJarStep, createCompileToJarStepImpl, createJarStep, getBootClasspath, recordDepFileIfNecessary`

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

        []{#<init>(com.facebook.buck.core.toolchain.tool.Tool,com.google.common.collect.ImmutableList,com.google.common.collect.ImmutableList,com.google.common.collect.ImmutableSet,com.facebook.buck.jvm.java.Javac,com.facebook.buck.jvm.java.JavacOptions,com.facebook.buck.jvm.java.ExtraClasspathProvider)}

        -   #### ScalacToJarStepFactory

                public ScalacToJarStepFactory​(Tool scalac,
                                              com.google.common.collect.ImmutableList<String> configCompilerFlags,
                                              com.google.common.collect.ImmutableList<String> extraArguments,
                                              com.google.common.collect.ImmutableSet<BuildRule> compilerPlugins,
                                              Javac javac,
                                              JavacOptions javacOptions,
                                              ExtraClasspathProvider extraClassPath)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

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
