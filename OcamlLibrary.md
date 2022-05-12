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
[Package]{.packageLabelInType} [com.facebook.buck.features.ocaml](package-summary.html)
:::

## Class OcamlLibrary {#class-ocamllibrary .title title="Class OcamlLibrary"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.core.rules.impl.AbstractBuildRule](../../core/rules/impl/AbstractBuildRule.html "class in com.facebook.buck.core.rules.impl")

    -   -   [com.facebook.buck.core.rules.impl.AbstractBuildRuleWithDeclaredAndExtraDeps](../../core/rules/impl/AbstractBuildRuleWithDeclaredAndExtraDeps.html "class in com.facebook.buck.core.rules.impl")

        -   -   [com.facebook.buck.core.rules.impl.NoopBuildRuleWithDeclaredAndExtraDeps](../../core/rules/impl/NoopBuildRuleWithDeclaredAndExtraDeps.html "class in com.facebook.buck.core.rules.impl")

            -   -   com.facebook.buck.features.ocaml.OcamlLibrary

::: description
-   

    All Implemented Interfaces:
    :   `BuildEngineAction`, `AllowsNonAnnotatedFields`,
        `HasDeclaredAndExtraDeps`, `BuildRule`, `HasNameAndType`,
        `Comparable<BuildRule>`

    ------------------------------------------------------------------------

        public abstract class OcamlLibrary
        extends NoopBuildRuleWithDeclaredAndExtraDeps

    ::: block
    An action graph representation of an OCaml library.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                             Description
          --------------------------------------------------------------------------------------------------------------------------------------- -------------
          `OcamlLibrary​(BuildTarget buildTarget,             ProjectFilesystem projectFilesystem,             BuildRuleParams buildRuleParams)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `ab                   | `getBytecodeCompil    | ::: block             |
        | stract com.google.com | eDeps​(com.facebook.bu | Dependencies for the  |
        | mon.collect.Immutable | ck.features.ocaml.Oca | bytecode (ocamlc)     |
        | SortedSet<BuildRule>` | mlPlatform platform)` | build                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `abstr                | `getBytecodeInclud    |                       |
        | act Iterable<String>` | eDirs​(com.facebook.bu |                       |
        |                       | ck.features.ocaml.Oca |                       |
        |                       | mlPlatform platform)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract             | `getBytecodeLinkable  |                       |
        |  NativeLinkableInput` | Input​(com.facebook.bu |                       |
        |                       | ck.features.ocaml.Oca |                       |
        |                       | mlPlatform platform)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `ab                   | `getBytecodeLin       |                       |
        | stract com.google.com | kDeps​(com.facebook.bu |                       |
        | mon.collect.Immutable | ck.features.ocaml.Oca |                       |
        | SortedSet<BuildRule>` | mlPlatform platform)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract Path`       | `getIncludeL          |                       |
        |                       | ibDir​(com.facebook.bu |                       |
        |                       | ck.features.ocaml.Oca |                       |
        |                       | mlPlatform platform)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `ab                   | `getNativeCompil      | ::: block             |
        | stract com.google.com | eDeps​(com.facebook.bu | Dependencies for the  |
        | mon.collect.Immutable | ck.features.ocaml.Oca | native (ocamlopt)     |
        | SortedSet<BuildRule>` | mlPlatform platform)` | build                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `abstract             | `getNativeLinkable    |                       |
        |  NativeLinkableInput` | Input​(com.facebook.bu |                       |
        |                       | ck.features.ocaml.Oca |                       |
        |                       | mlPlatform platform)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract             | `getOcam              |                       |
        |  Iterable<BuildRule>` | lLibraryDeps​(BuildRul |                       |
        |                       | eResolver buildRuleRe |                       |
        |                       | solver,               |                       |
        |                       |       com.facebook.bu |                       |
        |                       | ck.features.ocaml.Oca |                       |
        |                       | mlPlatform platform)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.impl.NoopBuildRuleWithDeclaredAndExtraDeps}

            ### Methods inherited from class com.facebook.buck.core.rules.impl.[NoopBuildRuleWithDeclaredAndExtraDeps](../../core/rules/impl/NoopBuildRuleWithDeclaredAndExtraDeps.html "class in com.facebook.buck.core.rules.impl")

            `getBuildSteps, getSourcePathToOutput, hasBuildSteps, isCacheable`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.impl.AbstractBuildRuleWithDeclaredAndExtraDeps}

            ### Methods inherited from class com.facebook.buck.core.rules.impl.[AbstractBuildRuleWithDeclaredAndExtraDeps](../../core/rules/impl/AbstractBuildRuleWithDeclaredAndExtraDeps.html "class in com.facebook.buck.core.rules.impl")

            `deprecatedGetExtraDeps, getBuildDeps, getDeclaredDeps, getTargetGraphOnlyDeps`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.impl.AbstractBuildRule}

            ### Methods inherited from class com.facebook.buck.core.rules.impl.[AbstractBuildRule](../../core/rules/impl/AbstractBuildRule.html "class in com.facebook.buck.core.rules.impl")

            `equals, getBuildTarget, getDependencies, getProjectFilesystem, getSourcePathOutputs, getType, hashCode, injectFields, toString, updateBuildRuleResolver`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, finalize, getClass, notify, notifyAll, wait, wait, wait`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.BuildRule}

            ### Methods inherited from interface com.facebook.buck.core.rules.[BuildRule](../../core/rules/BuildRule.html "interface in com.facebook.buck.core.rules")

            `compareTo, getFullyQualifiedName, outputFileCanBeCopied, shouldRespectInputSizeLimitForRemoteExecution`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.rules.BuildRuleParams)}

        -   #### OcamlLibrary

                public OcamlLibrary​(BuildTarget buildTarget,
                                    ProjectFilesystem projectFilesystem,
                                    BuildRuleParams buildRuleParams)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getIncludeLibDir(com.facebook.buck.features.ocaml.OcamlPlatform)}

        -   #### getIncludeLibDir

            ``` methodSignature
            public abstract Path getIncludeLibDir​(com.facebook.buck.features.ocaml.OcamlPlatform platform)
            ```

        []{#getBytecodeIncludeDirs(com.facebook.buck.features.ocaml.OcamlPlatform)}

        -   #### getBytecodeIncludeDirs

            ``` methodSignature
            public abstract Iterable<String> getBytecodeIncludeDirs​(com.facebook.buck.features.ocaml.OcamlPlatform platform)
            ```

        []{#getNativeCompileDeps(com.facebook.buck.features.ocaml.OcamlPlatform)}

        -   #### getNativeCompileDeps

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableSortedSet<BuildRule> getNativeCompileDeps​(com.facebook.buck.features.ocaml.OcamlPlatform platform)
            ```

            ::: block
            Dependencies for the native (ocamlopt) build
            :::

        []{#getBytecodeCompileDeps(com.facebook.buck.features.ocaml.OcamlPlatform)}

        -   #### getBytecodeCompileDeps

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableSortedSet<BuildRule> getBytecodeCompileDeps​(com.facebook.buck.features.ocaml.OcamlPlatform platform)
            ```

            ::: block
            Dependencies for the bytecode (ocamlc) build
            :::

        []{#getBytecodeLinkDeps(com.facebook.buck.features.ocaml.OcamlPlatform)}

        -   #### getBytecodeLinkDeps

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableSortedSet<BuildRule> getBytecodeLinkDeps​(com.facebook.buck.features.ocaml.OcamlPlatform platform)
            ```

        []{#getNativeLinkableInput(com.facebook.buck.features.ocaml.OcamlPlatform)}

        -   #### getNativeLinkableInput

            ``` methodSignature
            public abstract NativeLinkableInput getNativeLinkableInput​(com.facebook.buck.features.ocaml.OcamlPlatform platform)
            ```

        []{#getBytecodeLinkableInput(com.facebook.buck.features.ocaml.OcamlPlatform)}

        -   #### getBytecodeLinkableInput

            ``` methodSignature
            public abstract NativeLinkableInput getBytecodeLinkableInput​(com.facebook.buck.features.ocaml.OcamlPlatform platform)
            ```

        []{#getOcamlLibraryDeps(com.facebook.buck.core.rules.BuildRuleResolver,com.facebook.buck.features.ocaml.OcamlPlatform)}

        -   #### getOcamlLibraryDeps

            ``` methodSignature
            public abstract Iterable<BuildRule> getOcamlLibraryDeps​(BuildRuleResolver buildRuleResolver,
                                                                    com.facebook.buck.features.ocaml.OcamlPlatform platform)
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
