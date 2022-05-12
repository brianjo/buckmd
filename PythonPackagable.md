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

## Interface PythonPackagable {#interface-pythonpackagable .title title="Interface PythonPackagable"}
:::

::: contentContainer
::: description
-   

    All Superinterfaces:
    :   `HasBuildTarget`

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `CxxPythonExtension`, `PrebuiltPythonLibrary`, `PythonLibrary`

    ------------------------------------------------------------------------

        public interface PythonPackagable
        extends HasBuildTarget

    ::: block
    Represents a
    [`BuildRule`](../../core/rules/BuildRule.html "interface in com.facebook.buck.core.rules")
    which contributes components to a top-level Python binary or test.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `default boolean`     | `doesPythonPackageD   | ::: block             |
        |                       | isallowOmnibus​(Python | Allow this rule to    |
        |                       | Platform pythonPlatfo | opt-out it\'s         |
        |                       | rm,                   | transitive            |
        |                       |                CxxPla | dependencies from     |
        |                       | tform cxxPlatform,    | omnibus linking.      |
        |                       |                       | :::                   |
        |                       |          ActionGraphB |                       |
        |                       | uilder graphBuilder)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `default Option       | `getPythonByteco      | ::: block             |
        | al<PythonComponents>` | de​(PythonPlatform pyt | Compiled Python       |
        |                       | honPlatform,          | bytecode (e.g.        |
        |                       |          CxxPlatform  | :::                   |
        |                       | cxxPlatform,          |                       |
        |                       |          ActionGraphB |                       |
        |                       | uilder graphBuilder)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `def                  | `getPythonMod         | ::: block             |
        | ault Optional<? exten | ules​(PythonPlatform p | Python modules (i.e.  |
        | ds PythonComponents>` | ythonPlatform,        | :::                   |
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
        | `def                  | `getPythonResources   | ::: block             |
        | ault Optional<? exten | ​(PythonPlatform pytho | Resources (e.g.       |
        | ds PythonComponents>` | nPlatform,            | :::                   |
        |                       |         CxxPlatform c |                       |
        |                       | xxPlatform,           |                       |
        |                       |          ActionGraphB |                       |
        |                       | uilder graphBuilder)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `defau                | `isPythonZipSafe()`   |                       |
        | lt Optional<Boolean>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
        .tableTab}[[Default
        Methods](javascript:show(16);)[ ]{.tabEnd}]{#t5 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.core.model.HasBuildTarget}

            ### Methods inherited from interface com.facebook.buck.core.model.[HasBuildTarget](../../core/model/HasBuildTarget.html "interface in com.facebook.buck.core.model")

            `getBuildTarget`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getPythonPackageDeps(com.facebook.buck.features.python.toolchain.PythonPlatform,com.facebook.buck.cxx.toolchain.CxxPlatform,com.facebook.buck.core.rules.ActionGraphBuilder)}

        -   #### getPythonPackageDeps

            ``` methodSignature
            Iterable<BuildRule> getPythonPackageDeps​(PythonPlatform pythonPlatform,
                                                     CxxPlatform cxxPlatform,
                                                     ActionGraphBuilder graphBuilder)
            ```

        []{#getPythonModules(com.facebook.buck.features.python.toolchain.PythonPlatform,com.facebook.buck.cxx.toolchain.CxxPlatform,com.facebook.buck.core.rules.ActionGraphBuilder)}

        -   #### getPythonModules

            ``` methodSignature
            default Optional<? extends PythonComponents> getPythonModules​(PythonPlatform pythonPlatform,
                                                                          CxxPlatform cxxPlatform,
                                                                          ActionGraphBuilder graphBuilder)
            ```

            ::: block
            Python modules (i.e. sources, bytecode, or native
            extensions) associated with this rule.
            :::

            [Returns:]{.returnLabel}
            :   a map of modules, where the key is the module in
                [`Path`](http://docs.oracle.com/javase/7/docs/api/java/nio/file/Path.html?is-external=true "class or interface in java.nio.file"){.externalLink}
                form (including extension).

        []{#getPythonResources(com.facebook.buck.features.python.toolchain.PythonPlatform,com.facebook.buck.cxx.toolchain.CxxPlatform,com.facebook.buck.core.rules.ActionGraphBuilder)}

        -   #### getPythonResources

            ``` methodSignature
            default Optional<? extends PythonComponents> getPythonResources​(PythonPlatform pythonPlatform,
                                                                            CxxPlatform cxxPlatform,
                                                                            ActionGraphBuilder graphBuilder)
            ```

            ::: block
            Resources (e.g. data files) associated with this rule.
            :::

            [Returns:]{.returnLabel}
            :   a map of native libraries, where the key is the soname
                wrapped as a
                [`Path`](http://docs.oracle.com/javase/7/docs/api/java/nio/file/Path.html?is-external=true "class or interface in java.nio.file"){.externalLink}.

        []{#getPythonBytecode(com.facebook.buck.features.python.toolchain.PythonPlatform,com.facebook.buck.cxx.toolchain.CxxPlatform,com.facebook.buck.core.rules.ActionGraphBuilder)}

        -   #### getPythonBytecode

            ``` methodSignature
            default Optional<PythonComponents> getPythonBytecode​(PythonPlatform pythonPlatform,
                                                                 CxxPlatform cxxPlatform,
                                                                 ActionGraphBuilder graphBuilder)
            ```

            ::: block
            Compiled Python bytecode (e.g. \`.pyc\`) associated with
            this rule.
            :::

            [Returns:]{.returnLabel}
            :   a map of compiled Python bytecode, where the key is the
                module in
                [`Path`](http://docs.oracle.com/javase/7/docs/api/java/nio/file/Path.html?is-external=true "class or interface in java.nio.file"){.externalLink}
                form (including extension).

        []{#isPythonZipSafe()}

        -   #### isPythonZipSafe

            ``` methodSignature
            default Optional<Boolean> isPythonZipSafe()
            ```

            [Returns:]{.returnLabel}
            :   whether the modules in this rule can be imported/run
                transparently from a Zip file (e.g. via zipimport). This
                is almost always the case, but in rare situations (e.g.
                execution expects to find packaged files in disk) rules
                can opt-out.

        []{#doesPythonPackageDisallowOmnibus(com.facebook.buck.features.python.toolchain.PythonPlatform,com.facebook.buck.cxx.toolchain.CxxPlatform,com.facebook.buck.core.rules.ActionGraphBuilder)}

        -   #### doesPythonPackageDisallowOmnibus

            ``` methodSignature
            default boolean doesPythonPackageDisallowOmnibus​(PythonPlatform pythonPlatform,
                                                             CxxPlatform cxxPlatform,
                                                             ActionGraphBuilder graphBuilder)
            ```

            ::: block
            Allow this rule to opt-out it\'s transitive dependencies
            from omnibus linking. This is mainly useful for the case of
            prebuilt python packages including prebuilt native
            extensions in their sources parameter, which expect any
            native library dependencies to not be merged.
            :::

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
