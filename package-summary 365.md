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
# Package com.facebook.buck.core.rules.attr {#package-com.facebook.buck.core.rules.attr .title title="Package"}
:::

::: contentContainer
-   +-----------------------------------+-----------------------------------+
    | Interface                         | Description                       |
    +===================================+===================================+
    | [ExportDependencies](ExportD      | ::: block                         |
    | ependencies.html "interface in co | [`BuildRul                        |
    | m.facebook.buck.core.rules.attr") | e`](../BuildRule.html "interface  |
    |                                   | in com.facebook.buck.core.rules") |
    |                                   | that can export a subset of it\'s |
    |                                   | dependencies.                     |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [HasCustomDepsLogic](HasCust      | Deprecated.                       |
    | omDepsLogic.html "interface in co |                                   |
    | m.facebook.buck.core.rules.attr") |                                   |
    +-----------------------------------+-----------------------------------+
    | [HasD                             | ::: block                         |
    | eclaredAndExtraDeps](HasDeclaredA | Some rules have a legacy behavior |
    | ndExtraDeps.html "interface in co | of distinguishing between         |
    | m.facebook.buck.core.rules.attr") | \"declared\" deps (i.e.           |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [HasInstallHelpers](HasIns        |                                   |
    | tallHelpers.html "interface in co |                                   |
    | m.facebook.buck.core.rules.attr") |                                   |
    +-----------------------------------+-----------------------------------+
    | [HasMultipleOutputs](HasMult      | ::: block                         |
    | ipleOutputs.html "interface in co | [`BuildRul                        |
    | m.facebook.buck.core.rules.attr") | e`](../BuildRule.html "interface  |
    |                                   | in com.facebook.buck.core.rules") |
    |                                   | instances that support multiple   |
    |                                   | outputs via output labels.        |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [HasPostBuildSteps](HasPos        | ::: block                         |
    | tBuildSteps.html "interface in co | Deprecated interface used by      |
    | m.facebook.buck.core.rules.attr") | [`BuildRule                       |
    |                                   | `](../BuildRule.html "interface i |
    |                                   | n com.facebook.buck.core.rules")s |
    |                                   | which perform operations after    |
    |                                   | the build.                        |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [HasRuntimeDeps](Has              | ::: block                         |
    | RuntimeDeps.html "interface in co | Provides a facility for a rule to |
    | m.facebook.buck.core.rules.attr") | list dependencies it\'ll need at  |
    |                                   | runtime.                          |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [HasS                             | ::: block                         |
    | upplementaryOutputs](HasSupplemen | BuildRules which supports         |
    | taryOutputs.html "interface in co | supplementary outputs.            |
    | m.facebook.buck.core.rules.attr") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Initi                            | ::: block                         |
    | alizableFromDisk](InitializableFr | Object that has in-memory data    |
    | omDisk.html "interface in com.fac | structures that need to be        |
    | ebook.buck.core.rules.attr")\<T\> | populated as a result of          |
    |                                   | executing its steps.              |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [NoopInstallable](Noop            | ::: block                         |
    | Installable.html "interface in co | An interface that allows a rule   |
    | m.facebook.buck.core.rules.attr") | to be specified in a \`buck       |
    |                                   | install\` command, but that       |
    |                                   | doesn\'t require any post-build   |
    |                                   | work for installation.            |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [SupportsDependen                 | ::: block                         |
    | cyFileRuleKey](SupportsDependency | Used to tag a rule that supports  |
    | FileRuleKey.html "interface in co | dependency-file input-based rule  |
    | m.facebook.buck.core.rules.attr") | keys.                             |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Supports                         | ::: block                         |
    | InputBasedRuleKey](SupportsInputB | Used to tag a rule that supports  |
    | asedRuleKey.html "interface in co | input-based rule keys.            |
    | m.facebook.buck.core.rules.attr") | :::                               |
    +-----------------------------------+-----------------------------------+

    : Interface Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Class                             | Description                       |
    +===================================+===================================+
    | [Bui                              | ::: block                         |
    | ldOutputInitializer](BuildOutputI | Delegates the actual reading of   |
    | nitializer.html "class in com.fac | disk-cached data to the           |
    | ebook.buck.core.rules.attr")\<T\> | [`I                               |
    |                                   | nitializableFromDisk`](Initializa |
    |                                   | bleFromDisk.html "interface in co |
    |                                   | m.facebook.buck.core.rules.attr") |
    |                                   | and is responsible for safely     |
    |                                   | storing and retrieving the        |
    |                                   | in-memory data structures.        |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+

    : Class Summary[ ]{.tabEnd}
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
