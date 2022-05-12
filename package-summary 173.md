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
# Package com.facebook.buck.features.python {#package-com.facebook.buck.features.python .title title="Package"}
:::

::: contentContainer
-   +-----------------------------------+-----------------------------------+
    | Interface                         | Description                       |
    +===================================+===================================+
    | [PythonComponents](Pytho          | ::: block                         |
    | nComponents.html "interface in co | Interface representing the        |
    | m.facebook.buck.features.python") | modules, resources, etc.          |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [PythonCo                         | ::: block                         |
    | mponents.Resolved](PythonComponen | Resolve this                      |
    | ts.Resolved.html "interface in co | [`PythonComponents`](Pytho        |
    | m.facebook.buck.features.python") | nComponents.html "interface in co |
    |                                   | m.facebook.buck.features.python") |
    |                                   | into a class usable by            |
    |                                   | [`St                              |
    |                                   | ep`](../../step/Step.html "interf |
    |                                   | ace in com.facebook.buck.step")s. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [PythonCompo                      | ::: block                         |
    | nents.Resolved.ComponentConsumer] | A `BiConsumer` which throws a     |
    | (PythonComponents.Resolved.Compon | [`IOException`                    |
    | entConsumer.html "interface in co | ](http://docs.oracle.com/javase/7 |
    | m.facebook.buck.features.python") | /docs/api/java/io/IOException.htm |
    |                                   | l?is-external=true "class or inte |
    |                                   | rface in java.io"){.externalLink} |
    |                                   | for use by executing              |
    |                                   | [`S                               |
    |                                   | tep`](../../step/Step.html "inter |
    |                                   | face in com.facebook.buck.step")s |
    |                                   | to process the                    |
    |                                   | [`Path`](http                     |
    |                                   | ://docs.oracle.com/javase/7/docs/ |
    |                                   | api/java/nio/file/Path.html?is-ex |
    |                                   | ternal=true "class or interface i |
    |                                   | n java.nio.file"){.externalLink}s |
    |                                   | to the components from this       |
    |                                   | object.                           |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [PythonPackagable](Pytho          | ::: block                         |
    | nPackagable.html "interface in co | Represents a                      |
    | m.facebook.buck.features.python") | [`BuildRule`](../../core          |
    |                                   | /rules/BuildRule.html "interface  |
    |                                   | in com.facebook.buck.core.rules") |
    |                                   | which contributes components to a |
    |                                   | top-level Python binary or test.  |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+

    : Interface Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Class                             | Description                       |
    +===================================+===================================+
    | [CxxPythonExtension](Cxx          |                                   |
    | PythonExtension.html "class in co |                                   |
    | m.facebook.buck.features.python") |                                   |
    +-----------------------------------+-----------------------------------+
    | [CxxPythonExt                     |                                   |
    | ensionDescription](CxxPythonExten |                                   |
    | sionDescription.html "class in co |                                   |
    | m.facebook.buck.features.python") |                                   |
    +-----------------------------------+-----------------------------------+
    | [CxxPythonExtension               | ::: block                         |
    | DescriptionArg](CxxPythonExtensio | Immutable implementation of       |
    | nDescriptionArg.html "class in co | `CxxPyt                           |
    | m.facebook.buck.features.python") | honExtensionDescription.AbstractC |
    |                                   | xxPythonExtensionDescriptionArg`. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [C                                | ::: block                         |
    | xxPythonExtensionDescriptionArg.B | Builds instances of type          |
    | uilder](CxxPythonExtensionDescrip | [`CxxPythonExtensionDe            |
    | tionArg.Builder.html "class in co | scriptionArg`](CxxPythonExtension |
    | m.facebook.buck.features.python") | DescriptionArg.html "class in com |
    |                                   | .facebook.buck.features.python"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [MovePythonWhlDataStep](MovePy    | ::: block                         |
    | thonWhlDataStep.html "class in co | A                                 |
    | m.facebook.buck.features.python") | [`                                |
    |                                   | Step`](../../step/Step.html "inte |
    |                                   | rface in com.facebook.buck.step") |
    |                                   | that moves the contents of the    |
    |                                   | {package}-{version}.data          |
    |                                   | directory within an extracted     |
    |                                   | .whl if that directory exists.    |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [P                                |                                   |
    | exStep](PexStep.html "class in co |                                   |
    | m.facebook.buck.features.python") |                                   |
    +-----------------------------------+-----------------------------------+
    | [PrebuiltPythonLibrary](Prebui    |                                   |
    | ltPythonLibrary.html "class in co |                                   |
    | m.facebook.buck.features.python") |                                   |
    +-----------------------------------+-----------------------------------+
    | [PrebuiltPythonLibr               |                                   |
    | aryDescription](PrebuiltPythonLib |                                   |
    | raryDescription.html "class in co |                                   |
    | m.facebook.buck.features.python") |                                   |
    +-----------------------------------+-----------------------------------+
    | [PrebuiltPythonLibraryDes         | ::: block                         |
    | criptionArg](PrebuiltPythonLibrar | Immutable implementation of       |
    | yDescriptionArg.html "class in co | `PrebuiltPyth                     |
    | m.facebook.buck.features.python") | onLibraryDescription.AbstractPreb |
    |                                   | uiltPythonLibraryDescriptionArg`. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Prebuil                          | ::: block                         |
    | tPythonLibraryDescriptionArg.Buil | Builds instances of type          |
    | der](PrebuiltPythonLibraryDescrip | [`PrebuiltPythonLibraryDescr      |
    | tionArg.Builder.html "class in co | iptionArg`](PrebuiltPythonLibrary |
    | m.facebook.buck.features.python") | DescriptionArg.html "class in com |
    |                                   | .facebook.buck.features.python"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [PythonBinar                      |                                   |
    | y](PythonBinary.html "class in co |                                   |
    | m.facebook.buck.features.python") |                                   |
    +-----------------------------------+-----------------------------------+
    | [                                 |                                   |
    | PythonBinaryDescription](PythonBi |                                   |
    | naryDescription.html "class in co |                                   |
    | m.facebook.buck.features.python") |                                   |
    +-----------------------------------+-----------------------------------+
    | [Python                           | ::: block                         |
    | BinaryDescriptionArg](PythonBinar | Immutable implementation of       |
    | yDescriptionArg.html "class in co | `PythonBinaryDescription.Abs      |
    | m.facebook.buck.features.python") | tractPythonBinaryDescriptionArg`. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [PythonBinaryDescriptio           | ::: block                         |
    | nArg.Builder](PythonBinaryDescrip | Builds instances of type          |
    | tionArg.Builder.html "class in co | [`PythonBi                        |
    | m.facebook.buck.features.python") | naryDescriptionArg`](PythonBinary |
    |                                   | DescriptionArg.html "class in com |
    |                                   | .facebook.buck.features.python"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [PythonBuckConfig](P              |                                   |
    | ythonBuckConfig.html "class in co |                                   |
    | m.facebook.buck.features.python") |                                   |
    +-----------------------------------+-----------------------------------+
    | [PythonCompileRule](Py            | ::: block                         |
    | thonCompileRule.html "class in co | Compile the given module sources  |
    | m.facebook.buck.features.python") | into their respective bytecode.   |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Python                           |                                   |
    | DescriptionsProvider](PythonDescr |                                   |
    | iptionsProvider.html "class in co |                                   |
    | m.facebook.buck.features.python") |                                   |
    +-----------------------------------+-----------------------------------+
    | [PythonInPlaceBinary](Pyth        |                                   |
    | onInPlaceBinary.html "class in co |                                   |
    | m.facebook.buck.features.python") |                                   |
    +-----------------------------------+-----------------------------------+
    | [PythonLibrary                    |                                   |
    | ](PythonLibrary.html "class in co |                                   |
    | m.facebook.buck.features.python") |                                   |
    +-----------------------------------+-----------------------------------+
    | [Py                               | ::: block                         |
    | thonLibraryDescription](PythonLib | Python library rule description   |
    | raryDescription.html "class in co | :::                               |
    | m.facebook.buck.features.python") |                                   |
    +-----------------------------------+-----------------------------------+
    | [PythonLi                         | ::: block                         |
    | braryDescriptionArg](PythonLibrar | Immutable implementation of       |
    | yDescriptionArg.html "class in co | `PythonLibraryDescription.Abst    |
    | m.facebook.buck.features.python") | ractPythonLibraryDescriptionArg`. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [PythonLibraryDescription         | ::: block                         |
    | Arg.Builder](PythonLibraryDescrip | Builds instances of type          |
    | tionArg.Builder.html "class in co | [`PythonLibr                      |
    | m.facebook.buck.features.python") | aryDescriptionArg`](PythonLibrary |
    |                                   | DescriptionArg.html "class in com |
    |                                   | .facebook.buck.features.python"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [PythonMappedComponents](PythonM  | ::: block                         |
    | appedComponents.html "class in co | An implementation of              |
    | m.facebook.buck.features.python") | [`PythonComponents`](Pytho        |
    |                                   | nComponents.html "interface in co |
    |                                   | m.facebook.buck.features.python") |
    |                                   | wrapping a fixed map of sources,  |
    |                                   | where the keys determine where in |
    |                                   | the Python package the sources    |
    |                                   | get added.                        |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [PythonMappedComp                 | ::: block                         |
    | onents.Resolved](PythonMappedComp | An implementation of              |
    | onents.Resolved.html "class in co | [`PythonCom                       |
    | m.facebook.buck.features.python") | ponents.Resolved`](PythonComponen |
    |                                   | ts.Resolved.html "interface in co |
    |                                   | m.facebook.buck.features.python") |
    |                                   | for                               |
    |                                   | [                                 |
    |                                   | `PythonMappedComponents`](PythonM |
    |                                   | appedComponents.html "class in co |
    |                                   | m.facebook.buck.features.python") |
    |                                   | with                              |
    |                                   | [`So                              |
    |                                   | urcePath`](../../core/sourcepath/ |
    |                                   | SourcePath.html "interface in com |
    |                                   | .facebook.buck.core.sourcepath")s |
    |                                   | resolved to                       |
    |                                   | [`Path`](http                     |
    |                                   | ://docs.oracle.com/javase/7/docs/ |
    |                                   | api/java/nio/file/Path.html?is-ex |
    |                                   | ternal=true "class or interface i |
    |                                   | n java.nio.file"){.externalLink}s |
    |                                   | for use with                      |
    |                                   | [`S                               |
    |                                   | tep`](../../step/Step.html "inter |
    |                                   | face in com.facebook.buck.step"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [PythonModul                      |                                   |
    | e](PythonModule.html "class in co |                                   |
    | m.facebook.buck.features.python") |                                   |
    +-----------------------------------+-----------------------------------+
    | [Pyth                             |                                   |
    | onModuleAdapterPlugin](PythonModu |                                   |
    | leAdapterPlugin.html "class in co |                                   |
    | m.facebook.buck.features.python") |                                   |
    +-----------------------------------+-----------------------------------+
    | [                                 | ::: block                         |
    | PythonPackageComponents](PythonPa | All per-rule components that      |
    | ckageComponents.html "class in co | contribute to a Python binary.    |
    | m.facebook.buck.features.python") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [PythonPackageCom                 | ::: block                         |
    | ponents.Builder](PythonPackageCom | A helper class to construct a     |
    | ponents.Builder.html "class in co | PythonPackageComponents instance  |
    | m.facebook.buck.features.python") | which throws human readable error |
    |                                   | messages on duplicates.           |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [PythonPackagedBinary](Pytho      |                                   |
    | nPackagedBinary.html "class in co |                                   |
    | m.facebook.buck.features.python") |                                   |
    +-----------------------------------+-----------------------------------+
    | [PythonRunTestsStep](Pyt          |                                   |
    | honRunTestsStep.html "class in co |                                   |
    | m.facebook.buck.features.python") |                                   |
    +-----------------------------------+-----------------------------------+
    | [PythonSymlinkTree](Py            | ::: block                         |
    | thonSymlinkTree.html "class in co | Creates a tree of symlinks inside |
    | m.facebook.buck.features.python") | of a given directory              |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [PythonT                          |                                   |
    | est](PythonTest.html "class in co |                                   |
    | m.facebook.buck.features.python") |                                   |
    +-----------------------------------+-----------------------------------+
    | [PythonTestDescription](Python    |                                   |
    | TestDescription.html "class in co |                                   |
    | m.facebook.buck.features.python") |                                   |
    +-----------------------------------+-----------------------------------+
    | [Py                               | ::: block                         |
    | thonTestDescriptionArg](PythonTes | Immutable implementation of       |
    | tDescriptionArg.html "class in co | `PythonTestDescription.A          |
    | m.facebook.buck.features.python") | bstractPythonTestDescriptionArg`. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [PythonTestDescript               | ::: block                         |
    | ionArg.Builder](PythonTestDescrip | Builds instances of type          |
    | tionArg.Builder.html "class in co | [`Pyth                            |
    | m.facebook.buck.features.python") | onTestDescriptionArg`](PythonTest |
    |                                   | DescriptionArg.html "class in com |
    |                                   | .facebook.buck.features.python"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [PythonTestRunner](P              | ::: block                         |
    | ythonTestRunner.html "class in co | Test runner for Python for the    |
    | m.facebook.buck.features.python") | new TestX protocol.               |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [PythonTe                         | ::: block                         |
    | stRunnerDescription](PythonTestRu | A rule for specifying Python test |
    | nnerDescription.html "class in co | runners.                          |
    | m.facebook.buck.features.python") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [PythonTestRunn                   | ::: block                         |
    | erDescriptionArg](PythonTestRunne | Immutable implementation of       |
    | rDescriptionArg.html "class in co | `Py                               |
    | m.facebook.buck.features.python") | thonTestRunnerDescription.Abstrac |
    |                                   | tPythonTestRunnerDescriptionArg`. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [PythonTestRunnerDescriptionArg   | ::: block                         |
    | .Builder](PythonTestRunnerDescrip | Builds instances of type          |
    | tionArg.Builder.html "class in co | [`PythonTestRunner                |
    | m.facebook.buck.features.python") | DescriptionArg`](PythonTestRunner |
    |                                   | DescriptionArg.html "class in com |
    |                                   | .facebook.buck.features.python"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [PythonTes                        | ::: block                         |
    | tX](PythonTestX.html "class in co | New Python Test rule that uses    |
    | m.facebook.buck.features.python") | the TestX protocol to run.        |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [PythonU                          |                                   |
    | til](PythonUtil.html "class in co |                                   |
    | m.facebook.buck.features.python") |                                   |
    +-----------------------------------+-----------------------------------+

    : Class Summary[ ]{.tabEnd}

-   
      Enum                                                                                                                        Description
      --------------------------------------------------------------------------------------------------------------------------- -------------
      [CxxPythonExtensionDescription.Type](CxxPythonExtensionDescription.Type.html "enum in com.facebook.buck.features.python")    
      [PythonBuckConfig.PackageStyle](PythonBuckConfig.PackageStyle.html "enum in com.facebook.buck.features.python")              

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
