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
[Package]{.packageLabelInType} [com.facebook.buck.features.python](package-summary.html)
:::

## Class CxxPythonExtension {#class-cxxpythonextension .title title="Class CxxPythonExtension"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.core.rules.impl.AbstractBuildRule](../../core/rules/impl/AbstractBuildRule.html "class in com.facebook.buck.core.rules.impl")

    -   -   [com.facebook.buck.core.rules.impl.AbstractBuildRuleWithDeclaredAndExtraDeps](../../core/rules/impl/AbstractBuildRuleWithDeclaredAndExtraDeps.html "class in com.facebook.buck.core.rules.impl")

        -   -   [com.facebook.buck.core.rules.impl.NoopBuildRuleWithDeclaredAndExtraDeps](../../core/rules/impl/NoopBuildRuleWithDeclaredAndExtraDeps.html "class in com.facebook.buck.core.rules.impl")

            -   -   com.facebook.buck.features.python.CxxPythonExtension

::: description
-   

    All Implemented Interfaces:
    :   `BuildEngineAction`, `HasBuildTarget`,
        `AllowsNonAnnotatedFields`, `HasDeclaredAndExtraDeps`,
        `HasRuntimeDeps`, `BuildRule`, `HasNameAndType`,
        `PythonPackagable`, `Comparable<BuildRule>`

    ------------------------------------------------------------------------

        public abstract class CxxPythonExtension
        extends NoopBuildRuleWithDeclaredAndExtraDeps
        implements PythonPackagable, HasRuntimeDeps
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                      Description
          ------------------------------------------------------------------------------------------------------------------------------------------------ -------------
          `CxxPythonExtension​(BuildTarget buildTarget,                   ProjectFilesystem projectFilesystem,                   BuildRuleParams params)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `protecte             | `                     |                       |
        | d abstract BuildRule` | getExtension​(PythonPl |                       |
        |                       | atform pythonPlatform |                       |
        |                       | ,             CxxPlat |                       |
        |                       | form cxxPlatform,     |                       |
        |                       |          ActionGraphB |                       |
        |                       | uilder graphBuilder)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract Path`       | `getModule()`         |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstr                | `getNativeLin         |                       |
        | act NativeLinkTarget` | kTarget​(PythonPlatfor |                       |
        |                       | m pythonPlatform,     |                       |
        |                       |                 CxxPl |                       |
        |                       | atform cxxPlatform,   |                       |
        |                       |                   Act |                       |
        |                       | ionGraphBuilder graph |                       |
        |                       | Builder,              |                       |
        |                       |        boolean includ |                       |
        |                       | ePrivateLinkerFlags)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getPythonMod         | ::: block             |
        | abstract Optional<Pyt | ules​(PythonPlatform p | Python modules (i.e.  |
        | honMappedComponents>` | ythonPlatform,        | :::                   |
        |                       |           CxxPlatform |                       |
        |                       |  cxxPlatform,         |                       |
        |                       |          ActionGraphB |                       |
        |                       | uilder graphBuilder)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Boolean>`   | `isPythonZipSafe()`   |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

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
        -   []{#methods.inherited.from.class.com.facebook.buck.core.model.HasBuildTarget}

            ### Methods inherited from interface com.facebook.buck.core.model.[HasBuildTarget](../../core/model/HasBuildTarget.html "interface in com.facebook.buck.core.model")

            `getBuildTarget`

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
        -   []{#methods.inherited.from.class.com.facebook.buck.features.python.PythonPackagable}

            ### Methods inherited from interface com.facebook.buck.features.python.[PythonPackagable](PythonPackagable.html "interface in com.facebook.buck.features.python")

            `doesPythonPackageDisallowOmnibus, getPythonBytecode, getPythonPackageDeps, getPythonResources`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.rules.BuildRuleParams)}

        -   #### CxxPythonExtension

                public CxxPythonExtension​(BuildTarget buildTarget,
                                          ProjectFilesystem projectFilesystem,
                                          BuildRuleParams params)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getExtension(com.facebook.buck.features.python.toolchain.PythonPlatform,com.facebook.buck.cxx.toolchain.CxxPlatform,com.facebook.buck.core.rules.ActionGraphBuilder)}

        -   #### getExtension

            ``` methodSignature
            protected abstract BuildRule getExtension​(PythonPlatform pythonPlatform,
                                                      CxxPlatform cxxPlatform,
                                                      ActionGraphBuilder graphBuilder)
            ```

        []{#getModule()}

        -   #### getModule

            ``` methodSignature
            public abstract Path getModule()
            ```

        []{#getPythonModules(com.facebook.buck.features.python.toolchain.PythonPlatform,com.facebook.buck.cxx.toolchain.CxxPlatform,com.facebook.buck.core.rules.ActionGraphBuilder)}

        -   #### getPythonModules

            ``` methodSignature
            public abstract Optional<PythonMappedComponents> getPythonModules​(PythonPlatform pythonPlatform,
                                                                              CxxPlatform cxxPlatform,
                                                                              ActionGraphBuilder graphBuilder)
            ```

            ::: block
            [Description copied from
            interface: `PythonPackagable`]{.descfrmTypeLabel}
            :::

            ::: block
            Python modules (i.e. sources, bytecode, or native
            extensions) associated with this rule.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getPythonModules` in interface `PythonPackagable`

            [Returns:]{.returnLabel}
            :   a map of modules, where the key is the module in
                [`Path`](http://docs.oracle.com/javase/7/docs/api/java/nio/file/Path.html?is-external=true "class or interface in java.nio.file"){.externalLink}
                form (including extension).

        []{#isPythonZipSafe()}

        -   #### isPythonZipSafe

            ``` methodSignature
            public Optional<Boolean> isPythonZipSafe()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `isPythonZipSafe` in interface `PythonPackagable`

            [Returns:]{.returnLabel}
            :   whether the modules in this rule can be imported/run
                transparently from a Zip file (e.g. via zipimport). This
                is almost always the case, but in rare situations (e.g.
                execution expects to find packaged files in disk) rules
                can opt-out.

        []{#getNativeLinkTarget(com.facebook.buck.features.python.toolchain.PythonPlatform,com.facebook.buck.cxx.toolchain.CxxPlatform,com.facebook.buck.core.rules.ActionGraphBuilder,boolean)}

        -   #### getNativeLinkTarget

            ``` methodSignature
            public abstract NativeLinkTarget getNativeLinkTarget​(PythonPlatform pythonPlatform,
                                                                 CxxPlatform cxxPlatform,
                                                                 ActionGraphBuilder graphBuilder,
                                                                 boolean includePrivateLinkerFlags)
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
