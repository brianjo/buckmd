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

## Class ExternalJavac {#class-externaljavac .title title="Class ExternalJavac"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.jvm.java.ExternalJavac

::: description
-   

    All Implemented Interfaces:
    :   `AddsToRuleKey`, `Tool`, `Javac`

    ------------------------------------------------------------------------

        public class ExternalJavac
        extends Object
        implements Javac

    ::: block
    javac implemented in a separate binary.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        -   []{#nested.classes.inherited.from.class.com.facebook.buck.jvm.java.Javac}

            ### Nested classes/interfaces inherited from interface com.facebook.buck.jvm.java.[Javac](Javac.html "interface in com.facebook.buck.jvm.java")

            `Javac.Invocation, Javac.Source`
    :::

    ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        -   []{#fields.inherited.from.class.com.facebook.buck.jvm.java.Javac}

            ### Fields inherited from interface com.facebook.buck.jvm.java.[Javac](Javac.html "interface in com.facebook.buck.jvm.java")

            `ARGFILES_ESCAPER`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                               Description
          ----------------------------------------------------------------------------------------- -------------
          `ExternalJavac​(java.util.function.Supplier<Tool> javac,              String shortName)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `com.go               | `getCommandP          |                       |
        | ogle.common.collect.I | refix​(SourcePathResol |                       |
        | mmutableList<String>` | verAdapter resolver)` |                       |
        +-----------------------+-----------------------+-----------------------+
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
        | `com.google.c         | `getEnviro            |                       |
        | ommon.collect.Immutab | nment​(SourcePathResol |                       |
        | leMap<String,​String>` | verAdapter resolver)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getShortName()`      |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Javac.Invocation`    | `newBuildInvocation​(J | ::: block             |
        |                       | avacExecutionContext  | Prepares an           |
        |                       | context,              | invocation of the     |
        |                       |       SourcePathResol | compiler with the     |
        |                       | verAdapter sourcePath | given parameters.     |
        |                       | ResolverAdapter,      | :::                   |
        |                       |               BuildTa |                       |
        |                       | rget invokingRule,    |                       |
        |                       |                 com.g |                       |
        |                       | oogle.common.collect. |                       |
        |                       | ImmutableList<String> |                       |
        |                       |  options,             |                       |
        |                       |        com.google.com |                       |
        |                       | mon.collect.Immutable |                       |
        |                       | List<JavacPluginJsr19 |                       |
        |                       | 9Fields> annotationPr |                       |
        |                       | ocessors,             |                       |
        |                       |        com.google.com |                       |
        |                       | mon.collect.Immutable |                       |
        |                       | List<JavacPluginJsr19 |                       |
        |                       | 9Fields> javacPlugins |                       |
        |                       | ,                   c |                       |
        |                       | om.google.common.coll |                       |
        |                       | ect.ImmutableSortedSe |                       |
        |                       | t<Path> javaSourceFil |                       |
        |                       | ePaths,               |                       |
        |                       |      Path pathToSrcsL |                       |
        |                       | ist,                  |                       |
        |                       |   Path workingDirecto |                       |
        |                       | ry,                   |                       |
        |                       |  boolean trackClassUs |                       |
        |                       | age,                  |                       |
        |                       |   boolean trackJavacP |                       |
        |                       | haseEvents,           |                       |
        |                       |          JarParameter |                       |
        |                       | s abiJarParaameters,  |                       |
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

        []{#<init>(java.util.function.Supplier,java.lang.String)}

        -   #### ExternalJavac

                public ExternalJavac​(java.util.function.Supplier<Tool> javac,
                                     String shortName)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getCommandPrefix(com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter)}

        -   #### getCommandPrefix

            ``` methodSignature
            public com.google.common.collect.ImmutableList<String> getCommandPrefix​(SourcePathResolverAdapter resolver)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getCommandPrefix` in interface `Tool`

            [Returns:]{.returnLabel}
            :   the prefix command use to run this tool.

        []{#getEnvironment(com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter)}

        -   #### getEnvironment

            ``` methodSignature
            public com.google.common.collect.ImmutableMap<String,​String> getEnvironment​(SourcePathResolverAdapter resolver)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getEnvironment` in interface `Tool`

            [Returns:]{.returnLabel}
            :   the list of environment variables to set when running
                the command.

        []{#getDescription(com.google.common.collect.ImmutableList,com.google.common.collect.ImmutableSortedSet,java.nio.file.Path)}

        -   #### getDescription

            ``` methodSignature
            public String getDescription​(com.google.common.collect.ImmutableList<String> options,
                                         com.google.common.collect.ImmutableSortedSet<Path> javaSourceFilePaths,
                                         Path pathToSrcsList)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getDescription` in interface `Javac`

        []{#getShortName()}

        -   #### getShortName

            ``` methodSignature
            public String getShortName()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getShortName` in interface `Javac`

        []{#newBuildInvocation(com.facebook.buck.jvm.java.JavacExecutionContext,com.facebook.buck.core.sourcepath.resolver.SourcePathResolverAdapter,com.facebook.buck.core.model.BuildTarget,com.google.common.collect.ImmutableList,com.google.common.collect.ImmutableList,com.google.common.collect.ImmutableList,com.google.common.collect.ImmutableSortedSet,java.nio.file.Path,java.nio.file.Path,boolean,boolean,com.facebook.buck.jvm.java.JarParameters,com.facebook.buck.jvm.java.JarParameters,com.facebook.buck.jvm.java.abi.AbiGenerationMode,com.facebook.buck.jvm.java.abi.AbiGenerationMode,com.facebook.buck.jvm.java.abi.source.api.SourceOnlyAbiRuleInfoFactory)}

        -   #### newBuildInvocation

            ``` methodSignature
            public Javac.Invocation newBuildInvocation​(JavacExecutionContext context,
                                                       SourcePathResolverAdapter sourcePathResolverAdapter,
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
                                                       JarParameters abiJarParaameters,
                                                       @Nullable
                                                       JarParameters libraryJarParameters,
                                                       AbiGenerationMode abiGenerationMode,
                                                       AbiGenerationMode abiCompatibilityMode,
                                                       @Nullable
                                                       SourceOnlyAbiRuleInfoFactory ruleInfoFactory)
            ```

            ::: block
            [Description copied from
            interface: `Javac`]{.descfrmTypeLabel}
            :::

            ::: block
            Prepares an invocation of the compiler with the given
            parameters.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `newBuildInvocation` in interface `Javac`
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
