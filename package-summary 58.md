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

-   [Overview](../../../../../../index.html)
-   Package
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../deprecated-list.html)
-   [Index](../../../../../../index-all.html)
-   [Help](../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../allclasses.html)

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
# Package com.facebook.buck.apple.xcode.xcodeproj {#package-com.facebook.buck.apple.xcode.xcodeproj .title title="Package"}
:::

::: contentContainer
-   
      Interface                                                                                                                  Description
      -------------------------------------------------------------------------------------------------------------------------- -------------
      [CopyFilePhaseDestinationSpec](CopyFilePhaseDestinationSpec.html "interface in com.facebook.buck.apple.xcode.xcodeproj")    

      : Interface Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Class                             | Description                       |
    +===================================+===================================+
    | [FileTypes](                      | ::: block                         |
    | FileTypes.html "class in com.face | File types used in Apple targets. |
    | book.buck.apple.xcode.xcodeproj") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [PBXAggregateTarget](PBXAggreg    | ::: block                         |
    | ateTarget.html "class in com.face | Target backed by shell scripts or |
    | book.buck.apple.xcode.xcodeproj") | nothing (only specifying          |
    |                                   | dependencies).                    |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [PBXBuildFile](PBX                | ::: block                         |
    | BuildFile.html "class in com.face | File referenced by a build phase, |
    | book.buck.apple.xcode.xcodeproj") | unique to each build phase.       |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [PBXBuildPhase](PBXB              | ::: block                         |
    | uildPhase.html "class in com.face | Superclass of build phases.       |
    | book.buck.apple.xcode.xcodeproj") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [PBXBuildStyle](PBXB              |                                   |
    | uildStyle.html "class in com.face |                                   |
    | book.buck.apple.xcode.xcodeproj") |                                   |
    +-----------------------------------+-----------------------------------+
    | [PBXContainer](PBX                | ::: block                         |
    | Container.html "class in com.face | Superclass of all container       |
    | book.buck.apple.xcode.xcodeproj") | types.                            |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [PBXContainerItem](PBXCont        | ::: block                         |
    | ainerItem.html "class in com.face | Superclass in Xcode\'s object     |
    | book.buck.apple.xcode.xcodeproj") | hierarchy, has no non-structural  |
    |                                   | functionality here.               |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [PB                               | ::: block                         |
    | XContainerItemProxy](PBXContainer | Reference to another object used  |
    | ItemProxy.html "class in com.face | by                                |
    | book.buck.apple.xcode.xcodeproj") | [`                                |
    |                                   | PBXTargetDependency`](PBXTargetDe |
    |                                   | pendency.html "class in com.faceb |
    |                                   | ook.buck.apple.xcode.xcodeproj"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [PBXC                             |                                   |
    | opyFilesBuildPhase](PBXCopyFilesB |                                   |
    | uildPhase.html "class in com.face |                                   |
    | book.buck.apple.xcode.xcodeproj") |                                   |
    +-----------------------------------+-----------------------------------+
    | [PBXFileReference](PBXFile        | ::: block                         |
    | Reference.html "class in com.face | Reference to a concrete file.     |
    | book.buck.apple.xcode.xcodeproj") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [PBXFra                           | ::: block                         |
    | meworksBuildPhase](PBXFrameworksB | Build phase representing the      |
    | uildPhase.html "class in com.face | linking step of a target.         |
    | book.buck.apple.xcode.xcodeproj") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [PBXGroup]                        | ::: block                         |
    | (PBXGroup.html "class in com.face | A collection of files in Xcode\'s |
    | book.buck.apple.xcode.xcodeproj") | virtual filesystem hierarchy.     |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [                                 | ::: block                         |
    | PBXHeadersBuildPhase](PBXHeadersB | Build phase that copies header    |
    | uildPhase.html "class in com.face | files into the output headers     |
    | book.buck.apple.xcode.xcodeproj") | directory.                        |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [PBXNativeTarget](PBXNat          | ::: block                         |
    | iveTarget.html "class in com.face | Concrete target type representing |
    | book.buck.apple.xcode.xcodeproj") | targets built by xcode itself,    |
    |                                   | rather than an external build     |
    |                                   | system.                           |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [PBXObject](                      |                                   |
    | PBXObject.html "class in com.face |                                   |
    | book.buck.apple.xcode.xcodeproj") |                                   |
    +-----------------------------------+-----------------------------------+
    | [PBXProject](P                    | ::: block                         |
    | BXProject.html "class in com.face | The root object representing the  |
    | book.buck.apple.xcode.xcodeproj") | project itself.                   |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [PBXProjectItem](PBXPr            |                                   |
    | ojectItem.html "class in com.face |                                   |
    | book.buck.apple.xcode.xcodeproj") |                                   |
    +-----------------------------------+-----------------------------------+
    | [PBXReference](PBX                | ::: block                         |
    | Reference.html "class in com.face | Superclass for file, directories, |
    | book.buck.apple.xcode.xcodeproj") | and groups.                       |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [PBXR                             | ::: block                         |
    | esourcesBuildPhase](PBXResourcesB | Lists the files to be copied into |
    | uildPhase.html "class in com.face | the output resources directory    |
    | book.buck.apple.xcode.xcodeproj") | for the containing                |
    |                                   | [`PBXTarget`](P                   |
    |                                   | BXTarget.html "class in com.faceb |
    |                                   | ook.buck.apple.xcode.xcodeproj"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [PBXShell                         | ::: block                         |
    | ScriptBuildPhase](PBXShellScriptB | Build phase which represents      |
    | uildPhase.html "class in com.face | running a shell script.           |
    | book.buck.apple.xcode.xcodeproj") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [                                 | ::: block                         |
    | PBXSourcesBuildPhase](PBXSourcesB | Lists the files to be compiled    |
    | uildPhase.html "class in com.face | for the containing                |
    | book.buck.apple.xcode.xcodeproj") | [`PBXTarget`](P                   |
    |                                   | BXTarget.html "class in com.faceb |
    |                                   | ook.buck.apple.xcode.xcodeproj"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [PBXTarget](                      | ::: block                         |
    | PBXTarget.html "class in com.face | Information for building a        |
    | book.buck.apple.xcode.xcodeproj") | specific artifact (a library,     |
    |                                   | binary, or test).                 |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [PBXTargetDependency](PBXTargetD  | ::: block                         |
    | ependency.html "class in com.face | Element of the                    |
    | book.buck.apple.xcode.xcodeproj") | [`PBXTarget.dependencie           |
    |                                   | s`](PBXTarget.html#dependencies). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [PBXVariantGroup](PBXVar          | ::: block                         |
    | iantGroup.html "class in com.face | Group for referencing localized   |
    | book.buck.apple.xcode.xcodeproj") | resources.                        |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ProductType](Pr                  |                                   |
    | oductType.html "class in com.face |                                   |
    | book.buck.apple.xcode.xcodeproj") |                                   |
    +-----------------------------------+-----------------------------------+
    | [ProductTypes](Pro                | ::: block                         |
    | ductTypes.html "class in com.face | A collection of constants for     |
    | book.buck.apple.xcode.xcodeproj") | common product types.             |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [SourceTreePath](Sourc            | ::: block                         |
    | eTreePath.html "class in com.face | Utility class representing a      |
    | book.buck.apple.xcode.xcodeproj") | tuple of (SourceTree, Path) used  |
    |                                   | for uniquely describing a file    |
    |                                   | reference in a group.             |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [                                 | ::: block                         |
    | XCBuildConfiguration](XCBuildConf | Build configuration containing a  |
    | iguration.html "class in com.face | file reference ton an xcconfig    |
    | book.buck.apple.xcode.xcodeproj") | file and additional inline        |
    |                                   | settings.                         |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [XCConfigurationList](XCConfigur  | ::: block                         |
    | ationList.html "class in com.face | List of build configurations.     |
    | book.buck.apple.xcode.xcodeproj") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [XCVersionGroup](XCVer            |                                   |
    | sionGroup.html "class in com.face |                                   |
    | book.buck.apple.xcode.xcodeproj") |                                   |
    +-----------------------------------+-----------------------------------+

    : Class Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Enum                              | Description                       |
    +===================================+===================================+
    | [PBXContainerItemProxy            |                                   |
    | .ProxyType](PBXContainerItemProxy |                                   |
    | .ProxyType.html "enum in com.face |                                   |
    | book.buck.apple.xcode.xcodeproj") |                                   |
    +-----------------------------------+-----------------------------------+
    | [PBXCopyFilesBuildPhase.Dest      | ::: block                         |
    | ination](PBXCopyFilesBuildPhase.D | The prefix path, this does not    |
    | estination.html "enum in com.face | use SourceTreePath and build      |
    | book.buck.apple.xcode.xcodeproj") | variables but rather some sort of |
    |                                   | enum.                             |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [PBXGroup.SortPolicy](PBXGroup.   | ::: block                         |
    | SortPolicy.html "enum in com.face | Method by which group contents    |
    | book.buck.apple.xcode.xcodeproj") | will be sorted.                   |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [PBXRe                            |                                   |
    | ference.SourceTree](PBXReference. |                                   |
    | SourceTree.html "enum in com.face |                                   |
    | book.buck.apple.xcode.xcodeproj") |                                   |
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

-   [Overview](../../../../../../index.html)
-   Package
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../deprecated-list.html)
-   [Index](../../../../../../index-all.html)
-   [Help](../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../allclasses.html)

<div>

<div>

JavaScript is disabled on your browser.

</div>

</div>

[]{#skip.navbar.bottom}
:::
