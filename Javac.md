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
[Package]{.packageLabelInType} [com.facebook.buck.jvm.java](package-summary.html)
:::

## Interface Javac {#interface-javac .title title="Interface Javac"}
:::

::: contentContainer
::: description
-   

    All Superinterfaces:
    :   `AddsToRuleKey`, `Tool`

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `ExternalJavac`, `JarBackedJavac`, `JdkProvidedInMemoryJavac`,
        `Jsr199Javac`

    ------------------------------------------------------------------------

        public interface Javac
        extends Tool

    ::: block
    Interface for a javac tool.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type     Interface            Description
          --------------------- -------------------- -------------
          `static interface `   `Javac.Invocation`    
          `static class `       `Javac.Source`        

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Field                 | Description           |
        +=======================+=======================+=======================+
        | `static j             | `ARGFILES_ESCAPER`    | ::: block             |
        | ava.util.function.Fun |                       | An escaper for        |
        | ction<String,​String>` |                       | arguments written to  |
        |                       |                       | \@argfiles.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `String`              | `getD                 |                       |
        |                       | escription​(com.google |                       |
        |                       | .common.collect.Immut |                       |
        |                       | ableList<String> opti |                       |
        |                       | ons,               co |                       |
        |                       | m.google.common.colle |                       |
        |                       | ct.ImmutableSortedSet |                       |
        |                       | <Path> javaSourceFile |                       |
        |                       | Paths,                |                       |
        |                       | Path pathToSrcsList)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getShortName()`      |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Javac.Invocation`    | `ne                   | ::: block             |
        |                       | wBuildInvocation​(Java | Prepares an           |
        |                       | cExecutionContext con | invocation of the     |
        |                       | text,                 | compiler with the     |
        |                       |    SourcePathResolver | given parameters.     |
        |                       | Adapter resolver,     | :::                   |
        |                       |                BuildT |                       |
        |                       | arget invokingRule,   |                       |
        |                       |                  com. |                       |
        |                       | google.common.collect |                       |
        |                       | .ImmutableList<String |                       |
        |                       | > options,            |                       |
        |                       |         com.google.co |                       |
        |                       | mmon.collect.Immutabl |                       |
        |                       | eList<JavacPluginJsr1 |                       |
        |                       | 99Fields> annotationP |                       |
        |                       | rocessors,            |                       |
        |                       |         com.google.co |                       |
        |                       | mmon.collect.Immutabl |                       |
        |                       | eList<JavacPluginJsr1 |                       |
        |                       | 99Fields> javacPlugin |                       |
        |                       | s,                    |                       |
        |                       | com.google.common.col |                       |
        |                       | lect.ImmutableSortedS |                       |
        |                       | et<Path> javaSourceFi |                       |
        |                       | lePaths,              |                       |
        |                       |       Path pathToSrcs |                       |
        |                       | List,                 |                       |
        |                       |    Path workingDirect |                       |
        |                       | ory,                  |                       |
        |                       |   boolean trackClassU |                       |
        |                       | sage,                 |                       |
        |                       |    boolean trackJavac |                       |
        |                       | PhaseEvents,          |                       |
        |                       |           JarParamete |                       |
        |                       | rs abiJarParameters,  |                       |
        |                       |                   Jar |                       |
        |                       | Parameters libraryJar |                       |
        |                       | Parameters,           |                       |
        |                       |          AbiGeneratio |                       |
        |                       | nMode abiGenerationMo |                       |
        |                       | de,                   |                       |
        |                       |  AbiGenerationMode ab |                       |
        |                       | iCompatibilityMode,   |                       |
        |                       |                  Sour |                       |
        |                       | ceOnlyAbiRuleInfoFact |                       |
        |                       | ory ruleInfoFactory)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.core.toolchain.tool.Tool}

            ### Methods inherited from interface com.facebook.buck.core.toolchain.tool.[Tool](../../core/toolchain/tool/Tool.html "interface in com.facebook.buck.core.toolchain.tool")

            `getCommandPrefix, getEnvironment`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#field.detail}

        ### Field Detail

        []{#ARGFILES_ESCAPER}

        -   #### ARGFILES_ESCAPER

                static final java.util.function.Function<String,​String> ARGFILES_ESCAPER

            ::: block
            An escaper for arguments written to \@argfiles.
            :::
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#newBuildInvocation(com.facebook.buck.jvm.java.JavacExecutionContext,com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter,com.facebook.buck.core.model.BuildTarget,com.google.common.collect.ImmutableList,com.google.common.collect.ImmutableList,com.google.common.collect.ImmutableList,com.google.common.collect.ImmutableSortedSet,java.nio.file.Path,java.nio.file.Path,boolean,boolean,com.facebook.buck.jvm.java.JarParameters,com.facebook.buck.jvm.java.JarParameters,com.facebook.buck.jvm.java.abi.AbiGenerationMode,com.facebook.buck.jvm.java.abi.AbiGenerationMode,com.facebook.buck.jvm.java.abi.source.api.SourceOnlyAbiRuleInfoFactory)}

        -   #### newBuildInvocation

            ``` methodSignature
            Javac.Invocation newBuildInvocation​(JavacExecutionContext context,
                                                SourcePathResolverAdapter resolver,
                                                BuildTarget invokingRule,
                                                com.google.common.collect.ImmutableList<String> options,
                                                com.google.common.collect.ImmutableList<JavacPluginJsr199Fields> annotationProcessors,
                                                com.google.common.collect.ImmutableList<JavacPluginJsr199Fields> javacPlugins,
                                                com.google.common.collect.ImmutableSortedSet<Path> javaSourceFilePaths,
                                                Path pathToSrcsList,
                                                Path workingDirectory,
                                                boolean trackClassUsage,
                                                boolean trackJavacPhaseEvents,
                                                @Nullable
                                                JarParameters abiJarParameters,
                                                @Nullable
                                                JarParameters libraryJarParameters,
                                                AbiGenerationMode abiGenerationMode,
                                                AbiGenerationMode abiCompatibilityMode,
                                                @Nullable
                                                SourceOnlyAbiRuleInfoFactory ruleInfoFactory)
            ```

            ::: block
            Prepares an invocation of the compiler with the given
            parameters.
            :::

        []{#getDescription(com.google.common.collect.ImmutableList,com.google.common.collect.ImmutableSortedSet,java.nio.file.Path)}

        -   #### getDescription

            ``` methodSignature
            String getDescription​(com.google.common.collect.ImmutableList<String> options,
                                  com.google.common.collect.ImmutableSortedSet<Path> javaSourceFilePaths,
                                  Path pathToSrcsList)
            ```

        []{#getShortName()}

        -   #### getShortName

            ``` methodSignature
            String getShortName()
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
