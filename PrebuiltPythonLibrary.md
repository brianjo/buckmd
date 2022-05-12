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

## Class PrebuiltPythonLibrary {#class-prebuiltpythonlibrary .title title="Class PrebuiltPythonLibrary"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.core.rules.impl.AbstractBuildRule](../../core/rules/impl/AbstractBuildRule.html "class in com.facebook.buck.core.rules.impl")

    -   -   [com.facebook.buck.core.rules.impl.AbstractBuildRuleWithDeclaredAndExtraDeps](../../core/rules/impl/AbstractBuildRuleWithDeclaredAndExtraDeps.html "class in com.facebook.buck.core.rules.impl")

        -   -   com.facebook.buck.features.python.PrebuiltPythonLibrary

::: description
-   

    All Implemented Interfaces:
    :   `BuildEngineAction`, `HasBuildTarget`,
        `AllowsNonAnnotatedFields`, `HasDeclaredAndExtraDeps`,
        `BuildRule`, `HasNameAndType`, `PythonPackagable`,
        `Comparable<BuildRule>`

    ------------------------------------------------------------------------

        public class PrebuiltPythonLibrary
        extends AbstractBuildRuleWithDeclaredAndExtraDeps
        implements PythonPackagable
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                                     Description
          ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `PrebuiltPythonLibrary​(BuildTarget buildTarget,                      ProjectFilesystem projectFilesystem,                      BuildRuleParams params,                      SourcePath binarySrc,                      boolean excludeDepsFromOmnibus,                      boolean compile)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `boolean`             | `doesPythonPackageD   | ::: block             |
        |                       | isallowOmnibus​(Python | Allow this rule to    |
        |                       | Platform pythonPlatfo | opt-out it\'s         |
        |                       | rm,                   | transitive            |
        |                       |                CxxPla | dependencies from     |
        |                       | tform cxxPlatform,    | omnibus linking.      |
        |                       |                       | :::                   |
        |                       |          ActionGraphB |                       |
        |                       | uilder graphBuilder)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.com       | `                     |                       |
        | mon.collect.Immutable | getBuildSteps​(BuildCo |                       |
        | List<? extends Step>` | ntext context,        |                       |
        |                       |        BuildableConte |                       |
        |                       | xt buildableContext)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Option               | `getPythonByteco      | ::: block             |
        | al<PythonComponents>` | de​(PythonPlatform pyt | Compiled Python       |
        |                       | honPlatform,          | bytecode (e.g.        |
        |                       |          CxxPlatform  | :::                   |
        |                       | cxxPlatform,          |                       |
        |                       |          ActionGraphB |                       |
        |                       | uilder graphBuilder)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Option               | `getPythonMod         | ::: block             |
        | al<PythonComponents>` | ules​(PythonPlatform p | Python modules (i.e.  |
        |                       | ythonPlatform,        | :::                   |
        |                       |           CxxPlatform |                       |
        |                       |  cxxPlatform,         |                       |
        |                       |          ActionGraphB |                       |
        |                       | uilder graphBuilder)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Iterable<BuildRule>` | `get                  |                       |
        |                       | PythonPackageDeps​(Pyt |                       |
        |                       | honPlatform pythonPla |                       |
        |                       | tform,                |                       |
        |                       |       CxxPlatform cxx |                       |
        |                       | Platform,             |                       |
        |                       |          ActionGraphB |                       |
        |                       | uilder graphBuilder)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Option               | `getPythonResources   | ::: block             |
        | al<PythonComponents>` | ​(PythonPlatform pytho | Resources (e.g.       |
        |                       | nPlatform,            | :::                   |
        |                       |         CxxPlatform c |                       |
        |                       | xxPlatform,           |                       |
        |                       |          ActionGraphB |                       |
        |                       | uilder graphBuilder)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `SourcePath`          | `get                  |                       |
        |                       | SourcePathToOutput()` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.impl.AbstractBuildRuleWithDeclaredAndExtraDeps}

            ### Methods inherited from class com.facebook.buck.core.rules.impl.[AbstractBuildRuleWithDeclaredAndExtraDeps](../../core/rules/impl/AbstractBuildRuleWithDeclaredAndExtraDeps.html "class in com.facebook.buck.core.rules.impl")

            `deprecatedGetExtraDeps, getBuildDeps, getDeclaredDeps, getTargetGraphOnlyDeps`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.impl.AbstractBuildRule}

            ### Methods inherited from class com.facebook.buck.core.rules.impl.[AbstractBuildRule](../../core/rules/impl/AbstractBuildRule.html "class in com.facebook.buck.core.rules.impl")

            `equals, getBuildTarget, getDependencies, getProjectFilesystem, getSourcePathOutputs, getType, hasBuildSteps, hashCode, injectFields, isCacheable, toString, updateBuildRuleResolver`

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

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.model.HasBuildTarget}

            ### Methods inherited from interface com.facebook.buck.core.model.[HasBuildTarget](../../core/model/HasBuildTarget.html "interface in com.facebook.buck.core.model")

            `getBuildTarget`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.features.python.PythonPackagable}

            ### Methods inherited from interface com.facebook.buck.features.python.[PythonPackagable](PythonPackagable.html "interface in com.facebook.buck.features.python")

            `isPythonZipSafe`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.rules.BuildRuleParams,com.facebook.buck.core.sourcepath.SourcePath,boolean,boolean)}

        -   #### PrebuiltPythonLibrary

                public PrebuiltPythonLibrary​(BuildTarget buildTarget,
                                             ProjectFilesystem projectFilesystem,
                                             BuildRuleParams params,
                                             SourcePath binarySrc,
                                             boolean excludeDepsFromOmnibus,
                                             boolean compile)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getPythonPackageDeps(com.facebook.buck.features.python.toolchain.PythonPlatform,com.facebook.buck.cxx.toolchain.CxxPlatform,com.facebook.buck.core.rules.ActionGraphBuilder)}

        -   #### getPythonPackageDeps

            ``` methodSignature
            public Iterable<BuildRule> getPythonPackageDeps​(PythonPlatform pythonPlatform,
                                                            CxxPlatform cxxPlatform,
                                                            ActionGraphBuilder graphBuilder)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getPythonPackageDeps` in interface `PythonPackagable`

        []{#getPythonModules(com.facebook.buck.features.python.toolchain.PythonPlatform,com.facebook.buck.cxx.toolchain.CxxPlatform,com.facebook.buck.core.rules.ActionGraphBuilder)}

        -   #### getPythonModules

            ``` methodSignature
            public Optional<PythonComponents> getPythonModules​(PythonPlatform pythonPlatform,
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

        []{#getPythonResources(com.facebook.buck.features.python.toolchain.PythonPlatform,com.facebook.buck.cxx.toolchain.CxxPlatform,com.facebook.buck.core.rules.ActionGraphBuilder)}

        -   #### getPythonResources

            ``` methodSignature
            public Optional<PythonComponents> getPythonResources​(PythonPlatform pythonPlatform,
                                                                 CxxPlatform cxxPlatform,
                                                                 ActionGraphBuilder graphBuilder)
            ```

            ::: block
            [Description copied from
            interface: `PythonPackagable`]{.descfrmTypeLabel}
            :::

            ::: block
            Resources (e.g. data files) associated with this rule.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getPythonResources` in interface `PythonPackagable`

            [Returns:]{.returnLabel}
            :   a map of native libraries, where the key is the soname
                wrapped as a
                [`Path`](http://docs.oracle.com/javase/7/docs/api/java/nio/file/Path.html?is-external=true "class or interface in java.nio.file"){.externalLink}.

        []{#getPythonBytecode(com.facebook.buck.features.python.toolchain.PythonPlatform,com.facebook.buck.cxx.toolchain.CxxPlatform,com.facebook.buck.core.rules.ActionGraphBuilder)}

        -   #### getPythonBytecode

            ``` methodSignature
            public Optional<PythonComponents> getPythonBytecode​(PythonPlatform pythonPlatform,
                                                                CxxPlatform cxxPlatform,
                                                                ActionGraphBuilder graphBuilder)
            ```

            ::: block
            [Description copied from
            interface: `PythonPackagable`]{.descfrmTypeLabel}
            :::

            ::: block
            Compiled Python bytecode (e.g. \`.pyc\`) associated with
            this rule.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getPythonBytecode` in interface `PythonPackagable`

            [Returns:]{.returnLabel}
            :   a map of compiled Python bytecode, where the key is the
                module in
                [`Path`](http://docs.oracle.com/javase/7/docs/api/java/nio/file/Path.html?is-external=true "class or interface in java.nio.file"){.externalLink}
                form (including extension).

        []{#getBuildSteps(com.facebook.buck.core.build.context.BuildContext,com.facebook.buck.core.build.buildable.context.BuildableContext)}

        -   #### getBuildSteps

            ``` methodSignature
            public com.google.common.collect.ImmutableList<? extends Step> getBuildSteps​(BuildContext context,
                                                                                         BuildableContext buildableContext)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getBuildSteps` in interface `BuildRule`

        []{#getSourcePathToOutput()}

        -   #### getSourcePathToOutput

            ``` methodSignature
            @Nullable
            public SourcePath getSourcePathToOutput()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getSourcePathToOutput` in interface `BuildRule`

        []{#doesPythonPackageDisallowOmnibus(com.facebook.buck.features.python.toolchain.PythonPlatform,com.facebook.buck.cxx.toolchain.CxxPlatform,com.facebook.buck.core.rules.ActionGraphBuilder)}

        -   #### doesPythonPackageDisallowOmnibus

            ``` methodSignature
            public boolean doesPythonPackageDisallowOmnibus​(PythonPlatform pythonPlatform,
                                                            CxxPlatform cxxPlatform,
                                                            ActionGraphBuilder graphBuilder)
            ```

            ::: block
            [Description copied from
            interface: `PythonPackagable`]{.descfrmTypeLabel}
            :::

            ::: block
            Allow this rule to opt-out it\'s transitive dependencies
            from omnibus linking. This is mainly useful for the case of
            prebuilt python packages including prebuilt native
            extensions in their sources parameter, which expect any
            native library dependencies to not be merged.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `doesPythonPackageDisallowOmnibus` in
                interface `PythonPackagable`

            [Returns:]{.returnLabel}
            :   whether this
                [`PythonPackagable`](PythonPackagable.html "interface in com.facebook.buck.features.python")\'s
                transitive deps must be excluded from omnibus linking.
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
