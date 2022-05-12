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
# Package com.facebook.buck.rules.keys {#package-com.facebook.buck.rules.keys .title title="Package"}
:::

::: contentContainer
-   +-----------------------------------+-----------------------------------+
    | Interface                         | Description                       |
    +===================================+===================================+
    | [Arc                              | ::: block                         |
    | hiveDependencySupplier](ArchiveDe | Supplies dependencies that are    |
    | pendencySupplier.html "interface  | archives.                         |
    | in com.facebook.buck.rules.keys") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Dependenc                        |                                   |
    | yFileRuleKeyFactory](DependencyFi |                                   |
    | leRuleKeyFactory.html "interface  |                                   |
    | in com.facebook.buck.rules.keys") |                                   |
    +-----------------------------------+-----------------------------------+
    | [Dependency                       |                                   |
    | FileRuleKeyFactory.RuleKeyAndInpu |                                   |
    | ts](DependencyFileRuleKeyFactory. |                                   |
    | RuleKeyAndInputs.html "interface  |                                   |
    | in com.facebook.buck.rules.keys") |                                   |
    +-----------------------------------+-----------------------------------+
    | [RuleKeyAppendable](R             | Deprecated.                       |
    | uleKeyAppendable.html "interface  |                                   |
    | in com.facebook.buck.rules.keys") |                                   |
    +-----------------------------------+-----------------------------------+
    | [RuleKeyAppendable.RuleKeyAppend  | Deprecated.                       |
    | ableSink](RuleKeyAppendable.RuleK |                                   |
    | eyAppendableSink.html "interface  |                                   |
    | in com.facebook.buck.rules.keys") |                                   |
    +-----------------------------------+-----------------------------------+
    | [RuleKeyCache](R                  | ::: block                         |
    | uleKeyCache.html "interface in co | Interface for caches for rule     |
    | m.facebook.buck.rules.keys")\<V\> | keys.                             |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [RuleKeyCacheScope](RuleKe        | ::: block                         |
    | yCacheScope.html "interface in co | A class managing access to a      |
    | m.facebook.buck.rules.keys")\<V\> | [`RuleKeyCach                     |
    |                                   | e`](RuleKeyCache.html "interface  |
    |                                   | in com.facebook.buck.rules.keys") |
    |                                   | for the duration of a build.      |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [RuleKeyFactory](RuleKeyFac       |                                   |
    | tory.html "interface in com.faceb |                                   |
    | ook.buck.rules.keys")\<RULE_KEY\> |                                   |
    +-----------------------------------+-----------------------------------+
    | [RuleKeyFactoryWithDiagn          | ::: block                         |
    | ostics](RuleKeyFactoryWithDiagnos | A rule key factory that provides  |
    | tics.html "interface in com.faceb | diagnostic facilities.            |
    | ook.buck.rules.keys")\<RULE_KEY\> | :::                               |
    +-----------------------------------+-----------------------------------+
    | [RuleKeyScopedHasher](Rul         | ::: block                         |
    | eKeyScopedHasher.html "interface  | Used to construct rulekey         |
    | in com.facebook.buck.rules.keys") | \"scopes\".                       |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [RuleKeyScopedHasher.C            |                                   |
    | ontainerScope](RuleKeyScopedHashe |                                   |
    | r.ContainerScope.html "interface  |                                   |
    | in com.facebook.buck.rules.keys") |                                   |
    +-----------------------------------+-----------------------------------+
    | [                                 | ::: block                         |
    | TrackableRuleKeyCache](TrackableR | RuleKeyCache that can be tracked  |
    | uleKeyCache.html "interface in co | with `CacheStatsTracker`          |
    | m.facebook.buck.rules.keys")\<V\> | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ValueExtractor                   | ::: block                         |
    | ](ValueExtractor.html "interface  | Extracts a value, e.g.            |
    | in com.facebook.buck.rules.keys") | :::                               |
    +-----------------------------------+-----------------------------------+

    : Interface Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Class                             | Description                       |
    +===================================+===================================+
    | [Abstr                            | ::: block                         |
    | actRuleKeyBuilder](AbstractRuleKe | Base class for rulekey builders.  |
    | yBuilder.html "class in com.faceb | :::                               |
    | ook.buck.rules.keys")\<RULE_KEY\> |                                   |
    +-----------------------------------+-----------------------------------+
    | [AlterRul                         |                                   |
    | eKeys](AlterRuleKeys.html "class  |                                   |
    | in com.facebook.buck.rules.keys") |                                   |
    +-----------------------------------+-----------------------------------+
    | [Content                          | ::: block                         |
    | AgnosticRuleKeyFactory](ContentAg | A factory for generating          |
    | nosticRuleKeyFactory.html "class  | [`RuleKey`](../../cor             |
    | in com.facebook.buck.rules.keys") | e/rulekey/RuleKey.html "class in  |
    |                                   | com.facebook.buck.core.rulekey")s |
    |                                   | that only take into the account   |
    |                                   | the path of a file and not the    |
    |                                   | contents(hash) of the file.       |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [DefaultDependencyFi              | ::: block                         |
    | leRuleKeyFactory](DefaultDependen | A factory for generating          |
    | cyFileRuleKeyFactory.html "class  | dependency-file                   |
    | in com.facebook.buck.rules.keys") | [`RuleKey`](../../core            |
    |                                   | /rulekey/RuleKey.html "class in c |
    |                                   | om.facebook.buck.core.rulekey")s. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [DefaultRuleKeyCache](Defa        | ::: block                         |
    | ultRuleKeyCache.html "class in co | A                                 |
    | m.facebook.buck.rules.keys")\<V\> | [`RuleKey`](../../co              |
    |                                   | re/rulekey/RuleKey.html "class in |
    |                                   |  com.facebook.buck.core.rulekey") |
    |                                   | cache used by a                   |
    |                                   | [`RuleKeyFactory`]                |
    |                                   | (RuleKeyFactory.html "interface i |
    |                                   | n com.facebook.buck.rules.keys"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [DefaultRuleKeyFactory](D         | ::: block                         |
    | efaultRuleKeyFactory.html "class  | A                                 |
    | in com.facebook.buck.rules.keys") | [`RuleKeyFactory`                 |
    |                                   | ](RuleKeyFactory.html "interface  |
    |                                   | in com.facebook.buck.rules.keys") |
    |                                   | which adds some default settings  |
    |                                   | to                                |
    |                                   | [`RuleKey`](../../core            |
    |                                   | /rulekey/RuleKey.html "class in c |
    |                                   | om.facebook.buck.core.rulekey")s. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [DefaultRu                        | ::: block                         |
    | leKeyScopedHasher](DefaultRuleKey | A wrapper of                      |
    | ScopedHasher.html "class in com.f | [`RuleKeyHasher`](hasher/Rule     |
    | acebook.buck.rules.keys")\<HASH\> | KeyHasher.html "interface in com. |
    |                                   | facebook.buck.rules.keys.hasher") |
    |                                   | that provides scoped hashing      |
    |                                   | facilities.                       |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [DefaultRuleK                     |                                   |
    | eyScopedHasher.DefaultContainerSc |                                   |
    | ope](DefaultRuleKeyScopedHasher.D |                                   |
    | efaultContainerScope.html "class  |                                   |
    | in com.facebook.buck.rules.keys") |                                   |
    +-----------------------------------+-----------------------------------+
    | [DependencyFileEntry]             |                                   |
    | (DependencyFileEntry.html "class  |                                   |
    | in com.facebook.buck.rules.keys") |                                   |
    +-----------------------------------+-----------------------------------+
    | [EventPosting                     | ::: block                         |
    | RuleKeyCacheScope](EventPostingRu | A                                 |
    | leKeyCacheScope.html "class in co | [`RuleKeyCacheScope`](R           |
    | m.facebook.buck.rules.keys")\<V\> | uleKeyCacheScope.html "interface  |
    |                                   | in com.facebook.buck.rules.keys") |
    |                                   | which logs stats on close.        |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [FieldValueExtractor]             | ::: block                         |
    | (FieldValueExtractor.html "class  | Extracts a value of a given       |
    | in com.facebook.buck.rules.keys") | field, that is assumed to be      |
    |                                   | accessible.                       |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [InputBasedRuleKeyFactory](Inpu   | ::: block                         |
    | tBasedRuleKeyFactory.html "class  | A factory for generating          |
    | in com.facebook.buck.rules.keys") | input-based                       |
    |                                   | [`RuleKey`](../../core            |
    |                                   | /rulekey/RuleKey.html "class in c |
    |                                   | om.facebook.buck.core.rulekey")s. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [InputBasedRuleKeyFactor          |                                   |
    | y.Result](InputBasedRuleKeyFactor |                                   |
    | y.Result.html "class in com.faceb |                                   |
    | ook.buck.rules.keys")\<RULE_KEY\> |                                   |
    +-----------------------------------+-----------------------------------+
    | [NoopRuleKeyScopedHasher](Noo     | ::: block                         |
    | pRuleKeyScopedHasher.html "class  | Does nothing.                     |
    | in com.facebook.buck.rules.keys") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [RuleKeyBuilder](RuleKe           | ::: block                         |
    | yBuilder.html "class in com.faceb | A base implementation for rule    |
    | ook.buck.rules.keys")\<RULE_KEY\> | key builders.                     |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [RuleKeyCacheRecycler](RuleK      | ::: block                         |
    | eyCacheRecycler.html "class in co | Class which encapsulates all      |
    | m.facebook.buck.rules.keys")\<V\> | effort to cache and reuse a       |
    |                                   | [`RuleKeyCach                     |
    |                                   | e`](RuleKeyCache.html "interface  |
    |                                   | in com.facebook.buck.rules.keys") |
    |                                   | between builds.                   |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Ru                               | ::: block                         |
    | leKeyCacheRecycler.SettingsAffect | Any external settings which, if   |
    | ingCache](RuleKeyCacheRecycler.Se | changed, will cause the entire    |
    | ttingsAffectingCache.html "class  | cache to be invalidated.          |
    | in com.facebook.buck.rules.keys") | :::                               |
    +-----------------------------------+-----------------------------------+
    | [RuleKe                           | ::: block                         |
    | yDiagnostics](RuleKeyDiagnostics. | Contains functionality related to |
    | html "class in com.facebook.buck. | rulekey diagnostics.              |
    | rules.keys")\<RULE_KEY,​DIAG_KEY\> | :::                               |
    +-----------------------------------+-----------------------------------+
    | [RuleKeyDiagnostics.R             |                                   |
    | esult](RuleKeyDiagnostics.Result. |                                   |
    | html "class in com.facebook.buck. |                                   |
    | rules.keys")\<RULE_KEY,​DIAG_KEY\> |                                   |
    +-----------------------------------+-----------------------------------+
    | [RuleKeyFactori                   | ::: block                         |
    | es](RuleKeyFactories.html "class  | The various rule key factories    |
    | in com.facebook.buck.rules.keys") | used by the build engine.         |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [RuleKeyFieldLoader               |                                   |
    | ](RuleKeyFieldLoader.html "class  |                                   |
    | in com.facebook.buck.rules.keys") |                                   |
    +-----------------------------------+-----------------------------------+
    | [RuleKeyResult                    | ::: block                         |
    | ](RuleKeyResult.html "class in co | The result of rule key            |
    | m.facebook.buck.rules.keys")\<R\> | computation, including the deps   |
    |                                   | and inputs used to calculate the  |
    |                                   | value.                            |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [SingleBuildA                     | ::: block                         |
    | ctionRuleKeyCache](SingleBuildAct | A                                 |
    | ionRuleKeyCache.html "class in co | [`RuleKey`](../../co              |
    | m.facebook.buck.rules.keys")\<V\> | re/rulekey/RuleKey.html "class in |
    |                                   |  com.facebook.buck.core.rulekey") |
    |                                   | cache used by a                   |
    |                                   | [`RuleKeyFactory`]                |
    |                                   | (RuleKeyFactory.html "interface i |
    |                                   | n com.facebook.buck.rules.keys"). |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [Size                             | ::: block                         |
    | Limiter](SizeLimiter.html "class  | A class that keeps track of size  |
    | in com.facebook.buck.rules.keys") | and throws an exception if the    |
    |                                   | size limit is exceeded.           |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [TrackedRuleKeyCache](Trac        | ::: block                         |
    | kedRuleKeyCache.html "class in co | A DefaultRuleKeyCache that        |
    | m.facebook.buck.rules.keys")\<V\> | records cache stats information   |
    |                                   | in the corresponding              |
    |                                   | CacheStatsTracker                 |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ValueMethodValueExtractor](Value | ::: block                         |
    | MethodValueExtractor.html "class  | Extracts a value of a given       |
    | in com.facebook.buck.rules.keys") | field, that is assumed to be      |
    |                                   | accessible.                       |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+

    : Class Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Enum                              | Description                       |
    +===================================+===================================+
    | [Rul                              | ::: block                         |
    | eKeyType](RuleKeyType.html "enum  | Enum denoting a type of the       |
    | in com.facebook.buck.rules.keys") | rulekeys produced by various      |
    |                                   | rulekey factories.                |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+

    : Enum Summary[ ]{.tabEnd}

-   
      Exception                                                                                                       Description
      --------------------------------------------------------------------------------------------------------------- -------------
      [SizeLimiter.SizeLimitException](SizeLimiter.SizeLimitException.html "class in com.facebook.buck.rules.keys")    

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
