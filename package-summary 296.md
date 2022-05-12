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
# Package com.facebook.buck.core.rules.platform {#package-com.facebook.buck.core.rules.platform .title title="Package"}
:::

::: contentContainer
-   +-----------------------------------+-----------------------------------+
    | Interface                         | Description                       |
    +===================================+===================================+
    | [MultiPlatformRule](MultiPlatf    | ::: block                         |
    | ormRule.html "interface in com.fa | Represents multiplatform.         |
    | cebook.buck.core.rules.platform") | :::                               |
    +-----------------------------------+-----------------------------------+

    : Interface Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Class                             | Description                       |
    +===================================+===================================+
    | [Cach                             | ::: block                         |
    | ingPlatformResolver](CachingPlatf | An implementation of              |
    | ormResolver.html "class in com.fa | [`PlatformResolver                |
    | cebook.buck.core.rules.platform") | `](../../model/platform/PlatformR |
    |                                   | esolver.html "interface in com.fa |
    |                                   | cebook.buck.core.model.platform") |
    |                                   | that caches platforms created by  |
    |                                   | a given delegate.                 |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Combin                           | ::: block                         |
    | edPlatformResolver](CombinedPlatf | [`PlatformResolver                |
    | ormResolver.html "class in com.fa | `](../../model/platform/PlatformR |
    | cebook.buck.core.rules.platform") | esolver.html "interface in com.fa |
    |                                   | cebook.buck.core.model.platform") |
    |                                   | that supports both multiplatforms |
    |                                   | and regular platforms.            |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ConstraintRulesDescription       |                                   |
    | Provider](ConstraintRulesDescript |                                   |
    | ionProvider.html "class in com.fa |                                   |
    | cebook.buck.core.rules.platform") |                                   |
    +-----------------------------------+-----------------------------------+
    | [ConstraintSettingArg](Constrain  | ::: block                         |
    | tSettingArg.html "class in com.fa | Immutable implementation of       |
    | cebook.buck.core.rules.platform") | `ConstraintSettingDescripti       |
    |                                   | on.AbstractConstraintSettingArg`. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ConstraintSett                   | ::: block                         |
    | ingArg.Builder](ConstraintSetting | Builds instances of type          |
    | Arg.Builder.html "class in com.fa | [`                                |
    | cebook.buck.core.rules.platform") | ConstraintSettingArg`](Constraint |
    |                                   | SettingArg.html "class in com.fac |
    |                                   | ebook.buck.core.rules.platform"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ConstraintSett                   | ::: block                         |
    | ingDescription](ConstraintSetting | A description for                 |
    | Description.html "class in com.fa | `constraint_setting`.             |
    | cebook.buck.core.rules.platform") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [                                 | ::: block                         |
    | ConstraintSettingRule](Constraint | A configuration rule that         |
    | SettingRule.html "class in com.fa | represents `config_setting`       |
    | cebook.buck.core.rules.platform") | target.                           |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ConstraintValueArg](Constra      | ::: block                         |
    | intValueArg.html "class in com.fa | Immutable implementation of       |
    | cebook.buck.core.rules.platform") | `ConstraintValueDescrip           |
    |                                   | tion.AbstractConstraintValueArg`. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Constraint                       | ::: block                         |
    | ValueArg.Builder](ConstraintValue | Builds instances of type          |
    | Arg.Builder.html "class in com.fa | [`ConstraintValueArg`](Constrai   |
    | cebook.buck.core.rules.platform") | ntValueArg.html "class in com.fac |
    |                                   | ebook.buck.core.rules.platform"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Constraint                       | ::: block                         |
    | ValueDescription](ConstraintValue | A description for                 |
    | Description.html "class in com.fa | `constraint_value`.               |
    | cebook.buck.core.rules.platform") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ConstraintValueRule](Constrai    | ::: block                         |
    | ntValueRule.html "class in com.fa | `constraint_value` rule.          |
    | cebook.buck.core.rules.platform") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [DefaultTargetPla                 | ::: block                         |
    | tformResolver](DefaultTargetPlatf | [`TargetPlatformResolver`](../    |
    | ormResolver.html "class in com.fa | ../model/platform/TargetPlatformR |
    | cebook.buck.core.rules.platform") | esolver.html "interface in com.fa |
    |                                   | cebook.buck.core.model.platform") |
    |                                   | that supports both rule based     |
    |                                   | platforms and a platform for an   |
    |                                   | empty target configuration.       |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [PlatformArg](                    | ::: block                         |
    | PlatformArg.html "class in com.fa | Immutable implementation of       |
    | cebook.buck.core.rules.platform") | `Platform                         |
    |                                   | Description.AbstractPlatformArg`. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [PlatformArg.Builder](Platform    | ::: block                         |
    | Arg.Builder.html "class in com.fa | Builds instances of type          |
    | cebook.buck.core.rules.platform") | [`PlatformArg`](P                 |
    |                                   | latformArg.html "class in com.fac |
    |                                   | ebook.buck.core.rules.platform"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [PlatformDescription](Platform    | ::: block                         |
    | Description.html "class in com.fa | A description for `platform`.     |
    | cebook.buck.core.rules.platform") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [PlatformRuleDescript             |                                   |
    | ionProvider](PlatformRuleDescript |                                   |
    | ionProvider.html "class in com.fa |                                   |
    | cebook.buck.core.rules.platform") |                                   |
    +-----------------------------------+-----------------------------------+
    | [RuleBasedCon                     | ::: block                         |
    | straintResolver](RuleBasedConstra | [`ConstraintResolver`]            |
    | intResolver.html "class in com.fa | (../../model/platform/ConstraintR |
    | cebook.buck.core.rules.platform") | esolver.html "interface in com.fa |
    |                                   | cebook.buck.core.model.platform") |
    |                                   | that uses configuration rules     |
    |                                   | obtained from                     |
    |                                   | [`ConfigurationRuleReso           |
    |                                   | lver`](../config/ConfigurationRul |
    |                                   | eResolver.html "interface in com. |
    |                                   | facebook.buck.core.rules.config") |
    |                                   | to create                         |
    |                                   | [`ConstraintSett                  |
    |                                   | ing`](../../model/platform/Constr |
    |                                   | aintSetting.html "class in com.fa |
    |                                   | cebook.buck.core.model.platform") |
    |                                   | and                               |
    |                                   | [`Constraint                      |
    |                                   | Value`](../../model/platform/Cons |
    |                                   | traintValue.html "class in com.fa |
    |                                   | cebook.buck.core.model.platform") |
    |                                   | instances.                        |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [RuleBasedMultiPlat               | ::: block                         |
    | formResolver](RuleBasedMultiPlatf | [`PlatformResolver                |
    | ormResolver.html "class in com.fa | `](../../model/platform/PlatformR |
    | cebook.buck.core.rules.platform") | esolver.html "interface in com.fa |
    |                                   | cebook.buck.core.model.platform") |
    |                                   | that supports multiplatforms.     |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [RuleBase                         |                                   |
    | dPlatformResolver](RuleBasedPlatf |                                   |
    | ormResolver.html "class in com.fa |                                   |
    | cebook.buck.core.rules.platform") |                                   |
    +-----------------------------------+-----------------------------------+
    | [RuleBasedTargetPlatf             | ::: block                         |
    | ormResolver](RuleBasedTargetPlatf | An implementation of              |
    | ormResolver.html "class in com.fa | [`TargetPlatformResolver`](../    |
    | cebook.buck.core.rules.platform") | ../model/platform/TargetPlatformR |
    |                                   | esolver.html "interface in com.fa |
    |                                   | cebook.buck.core.model.platform") |
    |                                   | that creates                      |
    |                                   | [`                                |
    |                                   | Platform`](../../model/platform/P |
    |                                   | latform.html "interface in com.fa |
    |                                   | cebook.buck.core.model.platform") |
    |                                   | from `PlatformRule` for           |
    |                                   | [`RuleBasedTargetConf             |
    |                                   | iguration`](../../model/RuleBased |
    |                                   | TargetConfiguration.html "class i |
    |                                   | n com.facebook.buck.core.model"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ThrowingCo                       | ::: block                         |
    | nstraintResolver](ThrowingConstra | Constraint resolver that always   |
    | intResolver.html "class in com.fa | throws.                           |
    | cebook.buck.core.rules.platform") | :::                               |
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
