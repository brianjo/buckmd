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
# Package com.facebook.buck.apple.xcode {#package-com.facebook.buck.apple.xcode .title title="Package"}
:::

::: contentContainer
-   +-----------------------------------+-----------------------------------+
    | Class                             | Description                       |
    +===================================+===================================+
    | [AbstractPBXObjectFactory](Abstr  | ::: block                         |
    | actPBXObjectFactory.html "class i | A factory object for generating   |
    | n com.facebook.buck.apple.xcode") | new PBX object types.             |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [GidGene                          | ::: block                         |
    | rator](GidGenerator.html "class i | Generator for Global ID (GID)     |
    | n com.facebook.buck.apple.xcode") | which are present on every xcode  |
    |                                   | project object.                   |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [PBXObjectGIDFactory](            | ::: block                         |
    | PBXObjectGIDFactory.html "class i | A factory for creating PBXObjects |
    | n com.facebook.buck.apple.xcode") | that assigns a Global ID on       |
    |                                   | initialization.                   |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [XcodeprojSerializer](            | ::: block                         |
    | XcodeprojSerializer.html "class i | Serializer that handles           |
    | n com.facebook.buck.apple.xcode") | conversion of an in-memory object |
    |                                   | graph representation of an xcode  |
    |                                   | project (instances of             |
    |                                   | [`PBXObject`](xcodeproj/P         |
    |                                   | BXObject.html "class in com.faceb |
    |                                   | ook.buck.apple.xcode.xcodeproj")) |
    |                                   | into an Apple property list.      |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [XCScheme](XCScheme.html "class i |                                   |
    | n com.facebook.buck.apple.xcode") |                                   |
    +-----------------------------------+-----------------------------------+
    | [XCScheme.AnalyzeAction](XCS      |                                   |
    | cheme.AnalyzeAction.html "class i |                                   |
    | n com.facebook.buck.apple.xcode") |                                   |
    +-----------------------------------+-----------------------------------+
    | [XCScheme.ArchiveAction](XCS      |                                   |
    | cheme.ArchiveAction.html "class i |                                   |
    | n com.facebook.buck.apple.xcode") |                                   |
    +-----------------------------------+-----------------------------------+
    | [XCSc                             |                                   |
    | heme.BuildableReference](XCScheme |                                   |
    | .BuildableReference.html "class i |                                   |
    | n com.facebook.buck.apple.xcode") |                                   |
    +-----------------------------------+-----------------------------------+
    | [XCScheme.BuildAction](X          |                                   |
    | CScheme.BuildAction.html "class i |                                   |
    | n com.facebook.buck.apple.xcode") |                                   |
    +-----------------------------------+-----------------------------------+
    | [                                 |                                   |
    | XCScheme.BuildActionEntry](XCSche |                                   |
    | me.BuildActionEntry.html "class i |                                   |
    | n com.facebook.buck.apple.xcode") |                                   |
    +-----------------------------------+-----------------------------------+
    | [XCScheme.LaunchAction](XC        |                                   |
    | Scheme.LaunchAction.html "class i |                                   |
    | n com.facebook.buck.apple.xcode") |                                   |
    +-----------------------------------+-----------------------------------+
    | [XCScheme.ProfileAction](XCS      |                                   |
    | cheme.ProfileAction.html "class i |                                   |
    | n com.facebook.buck.apple.xcode") |                                   |
    +-----------------------------------+-----------------------------------+
    | [XCScheme.SchemeAction](XC        |                                   |
    | Scheme.SchemeAction.html "class i |                                   |
    | n com.facebook.buck.apple.xcode") |                                   |
    +-----------------------------------+-----------------------------------+
    | [XCSche                           |                                   |
    | me.SchemePrePostAction](XCScheme. |                                   |
    | SchemePrePostAction.html "class i |                                   |
    | n com.facebook.buck.apple.xcode") |                                   |
    +-----------------------------------+-----------------------------------+
    | [XC                               |                                   |
    | Scheme.TestableReference](XCSchem |                                   |
    | e.TestableReference.html "class i |                                   |
    | n com.facebook.buck.apple.xcode") |                                   |
    +-----------------------------------+-----------------------------------+
    | [XCScheme.TestAction](            |                                   |
    | XCScheme.TestAction.html "class i |                                   |
    | n com.facebook.buck.apple.xcode") |                                   |
    +-----------------------------------+-----------------------------------+

    : Class Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Enum                              | Description                       |
    +===================================+===================================+
    | [X                                |                                   |
    | CScheme.AdditionalActions](XCSche |                                   |
    | me.AdditionalActions.html "enum i |                                   |
    | n com.facebook.buck.apple.xcode") |                                   |
    +-----------------------------------+-----------------------------------+
    | [XCScheme.BuildAct                |                                   |
    | ionEntry.BuildFor](XCScheme.Build |                                   |
    | ActionEntry.BuildFor.html "enum i |                                   |
    | n com.facebook.buck.apple.xcode") |                                   |
    +-----------------------------------+-----------------------------------+
    | [XCScheme.Launch                  |                                   |
    | Action.LaunchStyle](XCScheme.Laun |                                   |
    | chAction.LaunchStyle.html "enum i |                                   |
    | n com.facebook.buck.apple.xcode") |                                   |
    +-----------------------------------+-----------------------------------+
    | [XCScheme.LaunchAction            | ::: block                         |
    | .WatchInterface](XCScheme.LaunchA | Watch Interface property in Watch |
    | ction.WatchInterface.html "enum i | app scheme used to choose which   |
    | n com.facebook.buck.apple.xcode") | interface is launched.            |
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
