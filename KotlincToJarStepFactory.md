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
[Package]{.packageLabelInType} [com.facebook.buck.jvm.kotlin](package-summary.html)
:::

## Class KotlincToJarStepFactory {#class-kotlinctojarstepfactory .title title="Class KotlincToJarStepFactory"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.jvm.java.CompileToJarStepFactory](../java/CompileToJarStepFactory.html "class in com.facebook.buck.jvm.java")

    -   -   com.facebook.buck.jvm.kotlin.KotlincToJarStepFactory

::: description
-   

    All Implemented Interfaces:
    :   `AddsToRuleKey`

    ------------------------------------------------------------------------

        public class KotlincToJarStepFactory
        extends CompileToJarStepFactory
        implements AddsToRuleKey
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `void`                | `creat                |                       |
        |                       | eCompileStep​(BuildCon |                       |
        |                       | text buildContext,    |                       |
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
        | `protec               | `getBootClasspath​(B   | ::: block             |
        | ted Optional<String>` | uildContext context)` | This can be used make |
        |                       |                       | the bootclasspath if  |
        |                       |                       | available, to the     |
        |                       |                       | postprocess classes   |
        |                       |                       | commands.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static Path`         | `getKap               |                       |
        |                       | tAnnotationGenPath​(Pr |                       |
        |                       | ojectFilesystem proje |                       |
        |                       | ctFilesystem,         |                       |
        |                       |                  Buil |                       |
        |                       | dTarget buildTarget)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `hasAn                |                       |
        |                       | notationProcessing()` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.jvm.java.CompileToJarStepFactory}

            ### Methods inherited from class com.facebook.buck.jvm.java.[CompileToJarStepFactory](../java/CompileToJarStepFactory.html "class in com.facebook.buck.jvm.java")

            `addCompilerSetupSteps, addJarCreationSteps, addJarSetupSteps, createCompileToJarStep, createCompileToJarStepImpl, createJarStep, recordDepFileIfNecessary`

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
    -   []{#method.detail}

        ### Method Detail

        []{#createCompileStep(com.facebook.buck.core.build.context.BuildContext,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.model.BuildTarget,com.facebook.buck.jvm.java.CompilerParameters,com.google.common.collect.ImmutableList.Builder,com.facebook.buck.core.build.buildable.context.BuildableContext)}

        -   #### createCompileStep

            ``` methodSignature
            public void createCompileStep​(BuildContext buildContext,
                                          ProjectFilesystem projectFilesystem,
                                          BuildTarget invokingRule,
                                          CompilerParameters parameters,
                                          com.google.common.collect.ImmutableList.Builder<Step> steps,
                                          BuildableContext buildableContext)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `createCompileStep` in class `CompileToJarStepFactory`

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

        []{#hasAnnotationProcessing()}

        -   #### hasAnnotationProcessing

            ``` methodSignature
            public boolean hasAnnotationProcessing()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `hasAnnotationProcessing` in
                class `CompileToJarStepFactory`

        []{#getKaptAnnotationGenPath(com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.model.BuildTarget)}

        -   #### getKaptAnnotationGenPath

            ``` methodSignature
            public static Path getKaptAnnotationGenPath​(ProjectFilesystem projectFilesystem,
                                                        BuildTarget buildTarget)
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
