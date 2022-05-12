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

-   [Overview](../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../deprecated-list.html)
-   [Index](../../../../index-all.html)
-   [Help](../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.cxx](package-summary.html)
:::

## Interface CxxLibraryDescriptionDelegate.ConfiguredDelegate {#interface-cxxlibrarydescriptiondelegate.configureddelegate .title title="Interface CxxLibraryDescriptionDelegate.ConfiguredDelegate"}
:::

::: contentContainer
::: description
-   

    Enclosing interface:
    :   [CxxLibraryDescriptionDelegate](CxxLibraryDescriptionDelegate.html "interface in com.facebook.buck.cxx")

    ------------------------------------------------------------------------

        public static interface CxxLibraryDescriptionDelegate.ConfiguredDelegate

    ::: block
    The delegate for a specific target and platform.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `com                  | `getAdditionalE       | ::: block             |
        | .google.common.collec | xportedLinkerFlags()` | Provides the ability  |
        | t.ImmutableList<Arg>` |                       | to inject additional  |
        |                       |                       | exported linker       |
        |                       |                       | flags.                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Optional             | `getNativeLi          | ::: block             |
        | <com.google.common.co | nkableExportedDeps()` | Provides the ability  |
        | llect.ImmutableList<N |                       | for the plugin to     |
        | ativeLinkableGroup>>` |                       | provide additional    |
        |                       |                       | `NativeLinkable`s     |
        |                       |                       | that will be          |
        |                       |                       | exported.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.google           | `                     | ::: block             |
        | .common.collect.Immut | getObjectFilePaths()` | Defines the paths to  |
        | ableList<SourcePath>` |                       | object files (i.e.,   |
        |                       |                       | .o files) that will   |
        |                       |                       | be combined into the  |
        |                       |                       | final product of      |
        |                       |                       | [`C                   |
        |                       |                       | xxLibraryDescription` |
        |                       |                       | ](CxxLibraryDescripti |
        |                       |                       | on.html "class in com |
        |                       |                       | .facebook.buck.cxx"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<C           | `ge                   | ::: block             |
        | xxPreprocessorInput>` | tPreprocessorInput()` | Defines an additional |
        |                       |                       | preprocessor input    |
        |                       |                       | for the public        |
        |                       |                       | interface exposed by  |
        |                       |                       | a target.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Optiona              | `getPrivat            | ::: block             |
        | l<HeaderSymlinkTree>` | eHeaderSymlinkTree()` | Defines an additional |
        |                       |                       | private               |
        |                       |                       | [`HeaderSymlin        |
        |                       |                       | kTree`](toolchain/Hea |
        |                       |                       | derSymlinkTree.html " |
        |                       |                       | class in com.facebook |
        |                       |                       | .buck.cxx.toolchain") |
        |                       |                       | that will be used     |
        |                       |                       | when compiling the    |
        |                       |                       | the library.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<C           | `getPrivat            | ::: block             |
        | xxPreprocessorInput>` | ePreprocessorInput()` | Defines an additional |
        |                       |                       | preprocessor input    |
        |                       |                       | for the private       |
        |                       |                       | interface exposed by  |
        |                       |                       | a target.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `getShouldProd        | ::: block             |
        |                       | uceLibraryArtifact()` | Specifies whether a   |
        |                       |                       | library artifact      |
        |                       |                       | (e.g., libName.a)     |
        |                       |                       | should be produced.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getPreprocessorInput()}

        -   #### getPreprocessorInput

            ``` methodSignature
            Optional<CxxPreprocessorInput> getPreprocessorInput()
            ```

            ::: block
            Defines an additional preprocessor input for the public
            interface exposed by a target. The returned input will be
            concatenated with
            [`CxxLibraryDescription`](CxxLibraryDescription.html "class in com.facebook.buck.cxx")\'s
            public input.
            :::

        []{#getPrivatePreprocessorInput()}

        -   #### getPrivatePreprocessorInput

            ``` methodSignature
            Optional<CxxPreprocessorInput> getPrivatePreprocessorInput()
            ```

            ::: block
            Defines an additional preprocessor input for the private
            interface exposed by a target. The returned input will be
            concatenated with
            [`CxxLibraryDescription`](CxxLibraryDescription.html "class in com.facebook.buck.cxx")\'s
            private input.
            :::

        []{#getPrivateHeaderSymlinkTree()}

        -   #### getPrivateHeaderSymlinkTree

            ``` methodSignature
            Optional<HeaderSymlinkTree> getPrivateHeaderSymlinkTree()
            ```

            ::: block
            Defines an additional private
            [`HeaderSymlinkTree`](toolchain/HeaderSymlinkTree.html "class in com.facebook.buck.cxx.toolchain")
            that will be used when compiling the the library.
            :::

        []{#getObjectFilePaths()}

        -   #### getObjectFilePaths

            ``` methodSignature
            com.google.common.collect.ImmutableList<SourcePath> getObjectFilePaths()
            ```

            ::: block
            Defines the paths to object files (i.e., .o files) that will
            be combined into the final product of
            [`CxxLibraryDescription`](CxxLibraryDescription.html "class in com.facebook.buck.cxx").
            If the paths depend on build rules, you must use
            [`ExplicitBuildTargetSourcePath`](../core/sourcepath/ExplicitBuildTargetSourcePath.html "class in com.facebook.buck.core.sourcepath")
            to make sure the build rule deps are correctly set up.
            :::

        []{#getNativeLinkableExportedDeps()}

        -   #### getNativeLinkableExportedDeps

            ``` methodSignature
            Optional<com.google.common.collect.ImmutableList<NativeLinkableGroup>> getNativeLinkableExportedDeps()
            ```

            ::: block
            Provides the ability for the plugin to provide additional
            `NativeLinkable`s that will be exported.
            :::

        []{#getAdditionalExportedLinkerFlags()}

        -   #### getAdditionalExportedLinkerFlags

            ``` methodSignature
            com.google.common.collect.ImmutableList<Arg> getAdditionalExportedLinkerFlags()
            ```

            ::: block
            Provides the ability to inject additional exported linker
            flags.
            :::

        []{#getShouldProduceLibraryArtifact()}

        -   #### getShouldProduceLibraryArtifact

            ``` methodSignature
            boolean getShouldProduceLibraryArtifact()
            ```

            ::: block
            Specifies whether a library artifact (e.g., libName.a)
            should be produced. For example, header-only libs will not
            normally produce a library. Since
            [`CxxLibraryDescription`](CxxLibraryDescription.html "class in com.facebook.buck.cxx")
            is not aware of other sources, it uses this method as an
            additional signal to determine whether it should produce a
            final artifact, even it doesn\'t have to if looking at just
            its own sources.
            :::
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

-   [Overview](../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../deprecated-list.html)
-   [Index](../../../../index-all.html)
-   [Help](../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../allclasses.html)

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
