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
# Package com.facebook.buck.core.toolchain {#package-com.facebook.buck.core.toolchain .title title="Package"}
:::

::: contentContainer
-   +-----------------------------------+-----------------------------------+
    | Interface                         | Description                       |
    +===================================+===================================+
    | [ComparableToolchain](Compara     | ::: block                         |
    | bleToolchain.html "interface in c | Interface that indicates that     |
    | om.facebook.buck.core.toolchain") | changes in a toolchain cause      |
    |                                   | restarting `Daemon`.              |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [RuleAnalysi                      | ::: block                         |
    | sLegacyToolchain](RuleAnalysisLeg | Allows legacy                     |
    | acyToolchain.html "interface in c | [`Toolchain`                      |
    | om.facebook.buck.core.toolchain") | ](Toolchain.html "interface in co |
    |                                   | m.facebook.buck.core.toolchain")s |
    |                                   | to be exposed in a generic way to |
    |                                   | the rule analysis graph via       |
    |                                   | providers.                        |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Toolchai                         | ::: block                         |
    | n](Toolchain.html "interface in c | Interface indicating that the     |
    | om.facebook.buck.core.toolchain") | class is a toolchain.             |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Toolc                            | ::: block                         |
    | hainCreationContext](ToolchainCre | Contains objects that can be used |
    | ationContext.html "interface in c | during the creation of a          |
    | om.facebook.buck.core.toolchain") | toolchain.                        |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ToolchainDescriptor](ToolchainD  | ::: block                         |
    | escriptor.html "interface in com. | Contains basic information about  |
    | facebook.buck.core.toolchain")\<T | a                                 |
    | extends                           | [`Toolchain                       |
    | [Toolchain]                       | `](Toolchain.html "interface in c |
    | (Toolchain.html "interface in com | om.facebook.buck.core.toolchain") |
    | .facebook.buck.core.toolchain")\> | that can be used to identify and  |
    |                                   | construct an instance of a        |
    |                                   | particular Toolchain.             |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ToolchainFactory](Toolcha        |                                   |
    | inFactory.html "interface in com. |                                   |
    | facebook.buck.core.toolchain")\<T |                                   |
    | extends                           |                                   |
    | [Toolchain]                       |                                   |
    | (Toolchain.html "interface in com |                                   |
    | .facebook.buck.core.toolchain")\> |                                   |
    +-----------------------------------+-----------------------------------+
    | [ToolchainProvider](Toolc         | ::: block                         |
    | hainProvider.html "interface in c | An interface that give access to  |
    | om.facebook.buck.core.toolchain") | specific toolchains by toolchain  |
    |                                   | name.                             |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Toolc                            | ::: block                         |
    | hainProviderFactory](ToolchainPro | A factory that is used when       |
    | viderFactory.html "interface in c | [`ToolchainProvider`](Toolc       |
    | om.facebook.buck.core.toolchain") | hainProvider.html "interface in c |
    |                                   | om.facebook.buck.core.toolchain") |
    |                                   | needs to be created without       |
    |                                   | depending on a specific           |
    |                                   | implementation of                 |
    |                                   | [`ToolchainProvider`](Toolch      |
    |                                   | ainProvider.html "interface in co |
    |                                   | m.facebook.buck.core.toolchain"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ToolchainSupplier](Toolc         | ::: block                         |
    | hainSupplier.html "interface in c | An `ExtensionPoint` which         |
    | om.facebook.buck.core.toolchain") | provides a way to register an     |
    |                                   | arbitrary set of                  |
    |                                   | [`ToolchainDescriptor`](Toolchain |
    |                                   | Descriptor.html "interface in com |
    |                                   | .facebook.buck.core.toolchain")s. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Too                              | ::: block                         |
    | lchainWithCapability](ToolchainWi | Generic interface that indicates  |
    | thCapability.html "interface in c | that a Toolchain supports         |
    | om.facebook.buck.core.toolchain") | somecapability.                   |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+

    : Interface Summary[ ]{.tabEnd}

-   
      Class                                                                                             Description
      ------------------------------------------------------------------------------------------------- -------------
      [BaseToolchain](BaseToolchain.html "class in com.facebook.buck.core.toolchain")                    
      [BaseToolchainProvider](BaseToolchainProvider.html "class in com.facebook.buck.core.toolchain")    

      : Class Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Exception                         | Description                       |
    +===================================+===================================+
    | [ToolchainInstan                  | ::: block                         |
    | tiationException](ToolchainInstan | An exception that indicates a     |
    | tiationException.html "class in c | problem during toolchain          |
    | om.facebook.buck.core.toolchain") | creation.                         |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+

    : Exception Summary[ ]{.tabEnd}
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
