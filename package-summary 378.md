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

-   [Overview](../../../../../../../index.html)
-   Package
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../index-all.html)
-   [Help](../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../allclasses.html)

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
# Package com.facebook.buck.features.project.intellij.model {#package-com.facebook.buck.features.project.intellij.model .title title="Package"}
:::

::: contentContainer
-   +-----------------------------------+-----------------------------------+
    | Interface                         | Description                       |
    +===================================+===================================+
    | [IjLibraryFactoryResolv           |                                   |
    | er](IjLibraryFactoryResolver.html |                                   |
    |  "interface in com.facebook.buck. |                                   |
    | features.project.intellij.model") |                                   |
    +-----------------------------------+-----------------------------------+
    | [IjMo                             | ::: block                         |
    | duleFactory](IjModuleFactory.html | Builds                            |
    |  "interface in com.facebook.buck. | [`IjModule`](IjModule.h           |
    | features.project.intellij.model") | tml "class in com.facebook.buck.f |
    |                                   | eatures.project.intellij.model")s |
    |                                   | out of                            |
    |                                   | [`TargetNode`](../../../.         |
    |                                   | ./core/model/targetgraph/TargetNo |
    |                                   | de.html "interface in com.faceboo |
    |                                   | k.buck.core.model.targetgraph")s. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [IjModuleFactoryResol             | ::: block                         |
    | ver](IjModuleFactoryResolver.html | Provides the                      |
    |  "interface in com.facebook.buck. | [`IjMod                           |
    | features.project.intellij.model") | uleFactory`](IjModuleFactory.html |
    |                                   |  "interface in com.facebook.buck. |
    |                                   | features.project.intellij.model") |
    |                                   | with                              |
    |                                   | [`Path`](http                     |
    |                                   | ://docs.oracle.com/javase/7/docs/ |
    |                                   | api/java/nio/file/Path.html?is-ex |
    |                                   | ternal=true "class or interface i |
    |                                   | n java.nio.file"){.externalLink}s |
    |                                   | to various elements of the        |
    |                                   | project.                          |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [I                                | ::: block                         |
    | jModuleRule](IjModuleRule.html "i | Rule describing which aspects of  |
    | nterface in com.facebook.buck.fea | the supplied                      |
    | tures.project.intellij.model")\<T | [`TargetNode`](../../..           |
    | extends                           | /../core/model/targetgraph/Target |
    | [BuildRuleArg](../../..           | Node.html "interface in com.faceb |
    | /../core/description/arg/BuildRul | ook.buck.core.model.targetgraph") |
    | eArg.html "interface in com.faceb | to transfer to the                |
    | ook.buck.core.description.arg")\> | [`IjModule`](IjModule.            |
    |                                   | html "class in com.facebook.buck. |
    |                                   | features.project.intellij.model") |
    |                                   | being constructed.                |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [IjProj                           | ::: block                         |
    | ectElement](IjProjectElement.html | Common interface shared between   |
    |  "interface in com.facebook.buck. | [`IjModule`](IjModule.            |
    | features.project.intellij.model") | html "class in com.facebook.buck. |
    |                                   | features.project.intellij.model") |
    |                                   | and                               |
    |                                   | [`IjLibrary`](IjLibrary.h         |
    |                                   | tml "class in com.facebook.buck.f |
    |                                   | eatures.project.intellij.model"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+

    : Interface Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Class                             | Description                       |
    +===================================+===================================+
    | [ContentRoot](ContentRoot.        |                                   |
    | html "class in com.facebook.buck. |                                   |
    | features.project.intellij.model") |                                   |
    +-----------------------------------+-----------------------------------+
    | [IjLibrary](IjLibrary.            | ::: block                         |
    | html "class in com.facebook.buck. | Represents a prebuilt library     |
    | features.project.intellij.model") | (.jar or .aar) as seen by         |
    |                                   | IntelliJ.                         |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [IjLi                             |                                   |
    | brary.Builder](IjLibrary.Builder. |                                   |
    | html "class in com.facebook.buck. |                                   |
    | features.project.intellij.model") |                                   |
    +-----------------------------------+-----------------------------------+
    | [Ij                               | ::: block                         |
    | LibraryFactory](IjLibraryFactory. | Interface for building            |
    | html "class in com.facebook.buck. | [`IjLibrary`](IjLibrary.          |
    | features.project.intellij.model") | html "class in com.facebook.buck. |
    |                                   | features.project.intellij.model") |
    |                                   | objects from                      |
    |                                   | [`TargetNode`](../../../.         |
    |                                   | ./core/model/targetgraph/TargetNo |
    |                                   | de.html "interface in com.faceboo |
    |                                   | k.buck.core.model.targetgraph")s. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [IjModule](IjModule.              | ::: block                         |
    | html "class in com.facebook.buck. | Represents a single IntelliJ      |
    | features.project.intellij.model") | module.                           |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Ij                               |                                   |
    | Module.Builder](IjModule.Builder. |                                   |
    | html "class in com.facebook.buck. |                                   |
    | features.project.intellij.model") |                                   |
    +-----------------------------------+-----------------------------------+
    | [IjModuleAn                       | ::: block                         |
    | droidFacet](IjModuleAndroidFacet. | The information necessary to add  |
    | html "class in com.facebook.buck. | the Android facet to the module.  |
    | features.project.intellij.model") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [IjModuleAndroidFacet.Build       |                                   |
    | er](IjModuleAndroidFacet.Builder. |                                   |
    | html "class in com.facebook.buck. |                                   |
    | features.project.intellij.model") |                                   |
    +-----------------------------------+-----------------------------------+
    | [                                 |                                   |
    | IjProjectConfig](IjProjectConfig. |                                   |
    | html "class in com.facebook.buck. |                                   |
    | features.project.intellij.model") |                                   |
    +-----------------------------------+-----------------------------------+
    | [IjProjectConfig.                 |                                   |
    | Builder](IjProjectConfig.Builder. |                                   |
    | html "class in com.facebook.buck. |                                   |
    | features.project.intellij.model") |                                   |
    +-----------------------------------+-----------------------------------+
    | [Mo                               |                                   |
    | duleIndexEntry](ModuleIndexEntry. |                                   |
    | html "class in com.facebook.buck. |                                   |
    | features.project.intellij.model") |                                   |
    +-----------------------------------+-----------------------------------+

    : Class Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Enum                              | Description                       |
    +===================================+===================================+
    | [DependencyType](DependencyType   |                                   |
    | .html "enum in com.facebook.buck. |                                   |
    | features.project.intellij.model") |                                   |
    +-----------------------------------+-----------------------------------+
    | [IjLibrary.Type](IjLibrary.Type   | ::: block                         |
    | .html "enum in com.facebook.buck. | Types of IjLibrary                |
    | features.project.intellij.model") | [`IjLibrary.Type.DEFAUL           |
    |                                   | T`](IjLibrary.Type.html#DEFAULT): |
    |                                   | Generated by a Buck target        |
    |                                   | [`IjLibrary.Ty                    |
    |                                   | pe.KOTLIN_JAVA_RUNTIME`](IjLibrar |
    |                                   | y.Type.html#KOTLIN_JAVA_RUNTIME): |
    |                                   | Generated for Kotlin code support |
    |                                   | in IDE                            |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [IjModuleType](IjModuleType       | ::: block                         |
    | .html "enum in com.facebook.buck. | List of module types that are     |
    | features.project.intellij.model") | recognized by the model.          |
    |                                   | :::                               |
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

-   [Overview](../../../../../../../index.html)
-   Package
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../index-all.html)
-   [Help](../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../allclasses.html)

<div>

<div>

JavaScript is disabled on your browser.

</div>

</div>

[]{#skip.navbar.bottom}
:::
