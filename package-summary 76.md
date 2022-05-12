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
-   Package
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

[]{#skip.navbar.top}
:::
:::

::: navPadding
 
:::
:::

::: {role="main"}
::: header
# Package com.facebook.buck.features.go {#package-com.facebook.buck.features.go .title title="Package"}
:::

::: contentContainer
-   
      Interface                                                                          Description
      ---------------------------------------------------------------------------------- -------------
      [HasGoLinkable](HasGoLinkable.html "interface in com.facebook.buck.features.go")    

      : Interface Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Class                             | Description                       |
    +===================================+===================================+
    | [CGoCompileS                      |                                   |
    | tep](CGoCompileStep.html "class i |                                   |
    | n com.facebook.buck.features.go") |                                   |
    +-----------------------------------+-----------------------------------+
    | [CGoGenerateImportStep](CG        |                                   |
    | oGenerateImportStep.html "class i |                                   |
    | n com.facebook.buck.features.go") |                                   |
    +-----------------------------------+-----------------------------------+
    | [CGoGenI                          |                                   |
    | mport](CGoGenImport.html "class i |                                   |
    | n com.facebook.buck.features.go") |                                   |
    +-----------------------------------+-----------------------------------+
    | [CGoGenS                          |                                   |
    | ource](CGoGenSource.html "class i |                                   |
    | n com.facebook.buck.features.go") |                                   |
    +-----------------------------------+-----------------------------------+
    | [CGo                              | ::: block                         |
    | Library](CGoLibrary.html "class i | The CGoLibrary represents cgo     |
    | n com.facebook.buck.features.go") | build process which outputs the   |
    |                                   | linkable object that is appended  |
    |                                   | to the native go compiled program |
    |                                   | (via pack tool).                  |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [CgoLibraryDescription](Cg        |                                   |
    | oLibraryDescription.html "class i |                                   |
    | n com.facebook.buck.features.go") |                                   |
    +-----------------------------------+-----------------------------------+
    | [CgoLibraryDescriptionArg](CgoLi  | ::: block                         |
    | braryDescriptionArg.html "class i | Immutable implementation of       |
    | n com.facebook.buck.features.go") | `CgoLibraryDescription.A          |
    |                                   | bstractCgoLibraryDescriptionArg`. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [CgoLibraryDesc                   | ::: block                         |
    | riptionArg.Builder](CgoLibraryDes | Builds instances of type          |
    | criptionArg.Builder.html "class i | [`                                |
    | n com.facebook.buck.features.go") | CgoLibraryDescriptionArg`](CgoLib |
    |                                   | raryDescriptionArg.html "class in |
    |                                   |  com.facebook.buck.features.go"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [FilteredSourceFiles](            |                                   |
    | FilteredSourceFiles.html "class i |                                   |
    | n com.facebook.buck.features.go") |                                   |
    +-----------------------------------+-----------------------------------+
    | [GoAssembleS                      |                                   |
    | tep](GoAssembleStep.html "class i |                                   |
    | n com.facebook.buck.features.go") |                                   |
    +-----------------------------------+-----------------------------------+
    | [GoBinary](GoBinary.html "class i |                                   |
    | n com.facebook.buck.features.go") |                                   |
    +-----------------------------------+-----------------------------------+
    | [GoBinaryDescription](            |                                   |
    | GoBinaryDescription.html "class i |                                   |
    | n com.facebook.buck.features.go") |                                   |
    +-----------------------------------+-----------------------------------+
    | [GoBinaryDescriptionArg](GoB      | ::: block                         |
    | inaryDescriptionArg.html "class i | Immutable implementation of       |
    | n com.facebook.buck.features.go") | `GoBinaryDescription              |
    |                                   | .AbstractGoBinaryDescriptionArg`. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [GoBinaryDe                       | ::: block                         |
    | scriptionArg.Builder](GoBinaryDes | Builds instances of type          |
    | criptionArg.Builder.html "class i | [`GoBinaryDescriptionArg`](GoBi   |
    | n com.facebook.buck.features.go") | naryDescriptionArg.html "class in |
    |                                   |  com.facebook.buck.features.go"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [GoBuckC                          |                                   |
    | onfig](GoBuckConfig.html "class i |                                   |
    | n com.facebook.buck.features.go") |                                   |
    +-----------------------------------+-----------------------------------+
    | [G                                |                                   |
    | oCompile](GoCompile.html "class i |                                   |
    | n com.facebook.buck.features.go") |                                   |
    +-----------------------------------+-----------------------------------+
    | [GoCompile                        |                                   |
    | Step](GoCompileStep.html "class i |                                   |
    | n com.facebook.buck.features.go") |                                   |
    +-----------------------------------+-----------------------------------+
    | [GoDescriptionsProvider](GoD      |                                   |
    | escriptionsProvider.html "class i |                                   |
    | n com.facebook.buck.features.go") |                                   |
    +-----------------------------------+-----------------------------------+
    | [G                                | ::: block                         |
    | oLibrary](GoLibrary.html "class i | Provides information about a Go   |
    | n com.facebook.buck.features.go") | Library rule                      |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [GoLibraryDescription](G          |                                   |
    | oLibraryDescription.html "class i |                                   |
    | n com.facebook.buck.features.go") |                                   |
    +-----------------------------------+-----------------------------------+
    | [GoLibraryDescriptionArg](GoLi    | ::: block                         |
    | braryDescriptionArg.html "class i | Immutable implementation of       |
    | n com.facebook.buck.features.go") | `GoLibraryDescription.            |
    |                                   | AbstractGoLibraryDescriptionArg`. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [GoLibraryDes                     | ::: block                         |
    | criptionArg.Builder](GoLibraryDes | Builds instances of type          |
    | criptionArg.Builder.html "class i | [`GoLibraryDescriptionArg`](GoLib |
    | n com.facebook.buck.features.go") | raryDescriptionArg.html "class in |
    |                                   |  com.facebook.buck.features.go"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [GoL                              |                                   |
    | inkStep](GoLinkStep.html "class i |                                   |
    | n com.facebook.buck.features.go") |                                   |
    +-----------------------------------+-----------------------------------+
    | [GoL                              |                                   |
    | istStep](GoListStep.html "class i |                                   |
    | n com.facebook.buck.features.go") |                                   |
    +-----------------------------------+-----------------------------------+
    | [GoModule](GoModule.html "class i |                                   |
    | n com.facebook.buck.features.go") |                                   |
    +-----------------------------------+-----------------------------------+
    | [GoModuleAdapterPlugin](Go        |                                   |
    | ModuleAdapterPlugin.html "class i |                                   |
    | n com.facebook.buck.features.go") |                                   |
    +-----------------------------------+-----------------------------------+
    | [GoP                              |                                   |
    | ackStep](GoPackStep.html "class i |                                   |
    | n com.facebook.buck.features.go") |                                   |
    +-----------------------------------+-----------------------------------+
    | [GoProjectCommandHelper](GoP      |                                   |
    | rojectCommandHelper.html "class i |                                   |
    | n com.facebook.buck.features.go") |                                   |
    +-----------------------------------+-----------------------------------+
    | [GoProjectSubCommand](            |                                   |
    | GoProjectSubCommand.html "class i |                                   |
    | n com.facebook.buck.features.go") |                                   |
    +-----------------------------------+-----------------------------------+
    | [Go                               |                                   |
    | ProjectSubCommandFactory](GoProje |                                   |
    | ctSubCommandFactory.html "class i |                                   |
    | n com.facebook.buck.features.go") |                                   |
    +-----------------------------------+-----------------------------------+
    | [GoTest](GoTest.html "class i     |                                   |
    | n com.facebook.buck.features.go") |                                   |
    +-----------------------------------+-----------------------------------+
    | [GoTestCoverSource                | ::: block                         |
    | ](GoTestCoverSource.html "class i | GoTestCoverSource is responsible  |
    | n com.facebook.buck.features.go") | for annotating the source files   |
    |                                   | via \`go tool cover\` utilty.     |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [GoTestCoverSt                    |                                   |
    | ep](GoTestCoverStep.html "class i |                                   |
    | n com.facebook.buck.features.go") |                                   |
    +-----------------------------------+-----------------------------------+
    | [GoTestDescription                |                                   |
    | ](GoTestDescription.html "class i |                                   |
    | n com.facebook.buck.features.go") |                                   |
    +-----------------------------------+-----------------------------------+
    | [GoTestDescriptionArg](G          | ::: block                         |
    | oTestDescriptionArg.html "class i | Immutable implementation of       |
    | n com.facebook.buck.features.go") | `GoTestDescripti                  |
    |                                   | on.AbstractGoTestDescriptionArg`. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [GoTest                           | ::: block                         |
    | DescriptionArg.Builder](GoTestDes | Builds instances of type          |
    | criptionArg.Builder.html "class i | [`GoTestDescriptionArg`](Go       |
    | n com.facebook.buck.features.go") | TestDescriptionArg.html "class in |
    |                                   |  com.facebook.buck.features.go"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [GoT                              |                                   |
    | estMain](GoTestMain.html "class i |                                   |
    | n com.facebook.buck.features.go") |                                   |
    +-----------------------------------+-----------------------------------+
    | [GoTestMainS                      |                                   |
    | tep](GoTestMainStep.html "class i |                                   |
    | n com.facebook.buck.features.go") |                                   |
    +-----------------------------------+-----------------------------------+
    | [GoTestR                          | ::: block                         |
    | unner](GoTestRunner.html "class i | Specifies the test runner for     |
    | n com.facebook.buck.features.go") | go_test for test protocol.        |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [GoTestRunnerDescription](GoTe    | ::: block                         |
    | stRunnerDescription.html "class i | A rule for specifying go test     |
    | n com.facebook.buck.features.go") | runners.                          |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Go                               | ::: block                         |
    | TestRunnerDescriptionArg](GoTestR | Immutable implementation of       |
    | unnerDescriptionArg.html "class i | `GoTestRunnerDescription.Abs      |
    | n com.facebook.buck.features.go") | tractGoTestRunnerDescriptionArg`. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [GoTestRunnerDescri               | ::: block                         |
    | ptionArg.Builder](GoTestRunnerDes | Builds instances of type          |
    | criptionArg.Builder.html "class i | [`GoTe                            |
    | n com.facebook.buck.features.go") | stRunnerDescriptionArg`](GoTestRu |
    |                                   | nnerDescriptionArg.html "class in |
    |                                   |  com.facebook.buck.features.go"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [GoT                              | ::: block                         |
    | estStep](GoTestStep.html "class i | Run a go test command and stream  |
    | n com.facebook.buck.features.go") | the output to a file.             |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [GoTestX](GoTestX.html "class i   | ::: block                         |
    | n com.facebook.buck.features.go") | go test that implements the test  |
    |                                   | protocol                          |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [GoToo                            |                                   |
    | lchain](GoToolchain.html "class i |                                   |
    | n com.facebook.buck.features.go") |                                   |
    +-----------------------------------+-----------------------------------+
    | [GoToolchainFactory]              |                                   |
    | (GoToolchainFactory.html "class i |                                   |
    | n com.facebook.buck.features.go") |                                   |
    +-----------------------------------+-----------------------------------+
    | [GoToolchainSupplier](            |                                   |
    | GoToolchainSupplier.html "class i |                                   |
    | n com.facebook.buck.features.go") |                                   |
    +-----------------------------------+-----------------------------------+
    | [Prebui                           |                                   |
    | ltGoLibraryDescription](PrebuiltG |                                   |
    | oLibraryDescription.html "class i |                                   |
    | n com.facebook.buck.features.go") |                                   |
    +-----------------------------------+-----------------------------------+
    | [PrebuiltGoLi                     | ::: block                         |
    | braryDescriptionArg](PrebuiltGoLi | Immutable implementation of       |
    | braryDescriptionArg.html "class i | `Preb                             |
    | n com.facebook.buck.features.go") | uiltGoLibraryDescription.Abstract |
    |                                   | PrebuiltGoLibraryDescriptionArg`. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [PrebuiltGoLibraryDescription     | ::: block                         |
    | Arg.Builder](PrebuiltGoLibraryDes | Builds instances of type          |
    | criptionArg.Builder.html "class i | [`PrebuiltGoLibr                  |
    | n com.facebook.buck.features.go") | aryDescriptionArg`](PrebuiltGoLib |
    |                                   | raryDescriptionArg.html "class in |
    |                                   |  com.facebook.buck.features.go"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+

    : Class Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Enum                              | Description                       |
    +===================================+===================================+
    | [GoArch](GoArch.html "enum i      | ::: block                         |
    | n com.facebook.buck.features.go") | Represents the GOARCH values in   |
    |                                   | Go found at:                      |
    |                                   | https://github.com/golang/go/bl   |
    |                                   | ob/master/src/go/build/syslist.go |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [GoOs](GoOs.html "enum i          | ::: block                         |
    | n com.facebook.buck.features.go") | Represents the GOOS values in Go  |
    |                                   | found at:                         |
    |                                   | https://github.com/golang/go/bl   |
    |                                   | ob/master/src/go/build/syslist.go |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [GoPackStep.Operation](           |                                   |
    | GoPackStep.Operation.html "enum i |                                   |
    | n com.facebook.buck.features.go") |                                   |
    +-----------------------------------+-----------------------------------+

    : Enum Summary[ ]{.tabEnd}
:::
:::

::: bottomNav
[]{#navbar.bottom}

::: skipNav
[Skip navigation links](#skip.navbar.bottom "Skip navigation links")
:::

[]{#navbar.bottom.firstrow}

-   [Overview](../../../../../index.html)
-   Package
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

[]{#skip.navbar.bottom}
:::
