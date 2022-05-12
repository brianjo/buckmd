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
[Package]{.packageLabelInType} [com.facebook.buck.features.python](package-summary.html)
:::

## Class PythonLibrary {#class-pythonlibrary .title title="Class PythonLibrary"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.core.rules.impl.AbstractBuildRule](../../core/rules/impl/AbstractBuildRule.html "class in com.facebook.buck.core.rules.impl")

    -   -   [com.facebook.buck.core.rules.impl.AbstractBuildRuleWithDeclaredAndExtraDeps](../../core/rules/impl/AbstractBuildRuleWithDeclaredAndExtraDeps.html "class in com.facebook.buck.core.rules.impl")

        -   -   [com.facebook.buck.core.rules.impl.NoopBuildRuleWithDeclaredAndExtraDeps](../../core/rules/impl/NoopBuildRuleWithDeclaredAndExtraDeps.html "class in com.facebook.buck.core.rules.impl")

            -   -   com.facebook.buck.features.python.PythonLibrary

::: description
-   

    All Implemented Interfaces:
    :   `BuildEngineAction`, `HasBuildTarget`,
        `AllowsNonAnnotatedFields`, `HasDeclaredAndExtraDeps`,
        `HasRuntimeDeps`, `BuildRule`, `HasNameAndType`,
        `PythonPackagable`, `Comparable<BuildRule>`

    ------------------------------------------------------------------------

        public class PythonLibrary
        extends NoopBuildRuleWithDeclaredAndExtraDeps
        implements PythonPackagable, HasRuntimeDeps
:::

::: summary
-   ::: {.section role="region"}
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
        | `Option               | `getPythonByteco      | ::: block             |
        | al<PythonComponents>` | de​(PythonPlatform pyt | Compiled Python       |
        |                       | honPlatform,          | bytecode (e.g.        |
        |                       |          CxxPlatform  | :::                   |
        |                       | cxxPlatform,          |                       |
        |                       |          ActionGraphB |                       |
        |                       | uilder graphBuilder)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Pyt         | `getPythonMod         | ::: block             |
        | honMappedComponents>` | ules​(PythonPlatform p | Python modules (i.e.  |
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
        | `Optional<Pyt         | `getPythonResources   | ::: block             |
        | honMappedComponents>` | ​(PythonPlatform pytho | Resources (e.g.       |
        |                       | nPlatform,            | :::                   |
        |                       |         CxxPlatform c |                       |
        |                       | xxPlatform,           |                       |
        |                       |          ActionGraphB |                       |
        |                       | uilder graphBuilder)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `java.util.stream     | `getRuntime           |                       |
        | .Stream<BuildTarget>` | Deps​(BuildRuleResolve |                       |
        |                       | r buildRuleResolver)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Boolean>`   | `isPythonZipSafe()`   |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
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
    :::
:::

::: details
-   ::: {.section role="region"}
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
            public Optional<PythonMappedComponents> getPythonModules​(PythonPlatform pythonPlatform,
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
            public Optional<PythonMappedComponents> getPythonResources​(PythonPlatform pythonPlatform,
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

        []{#getRuntimeDeps(com.facebook.buck.core.rules.BuildRuleResolver)}

        -   #### getRuntimeDeps

            ``` methodSignature
            public java.util.stream.Stream<BuildTarget> getRuntimeDeps​(BuildRuleResolver buildRuleResolver)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getRuntimeDeps` in interface `HasRuntimeDeps`

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
