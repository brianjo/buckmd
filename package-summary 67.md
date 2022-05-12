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
# Package com.facebook.buck.rules.keys.hasher {#package-com.facebook.buck.rules.keys.hasher .title title="Package"}
:::

::: contentContainer
-   +-----------------------------------+-----------------------------------+
    | Interface                         | Description                       |
    +===================================+===================================+
    | [RuleKeyHasher](RuleKeyHashe      | ::: block                         |
    | r.html "interface in com.facebook | A hasher used for the rule key    |
    | .buck.rules.keys.hasher")\<HASH\> | construction.                     |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+

    : Interface Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Class                             | Description                       |
    +===================================+===================================+
    | [Counti                           | ::: block                         |
    | ngRuleKeyHasher](CountingRuleKeyH | A delegating                      |
    | asher.html "class in com.facebook | [`RuleKeyHasher`](Rule            |
    | .buck.rules.keys.hasher")\<HASH\> | KeyHasher.html "interface in com. |
    |                                   | facebook.buck.rules.keys.hasher") |
    |                                   | that counts the number of values  |
    |                                   | put in it.                        |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ForwardingRuleKe                 | ::: block                         |
    | yHasher](ForwardingRuleKeyHasher. | A                                 |
    | html "class in com.facebook.buck. | [`RuleKeyHasher`](Rule            |
    | rules.keys.hasher")\<HASH,​HASH2\> | KeyHasher.html "interface in com. |
    |                                   | facebook.buck.rules.keys.hasher") |
    |                                   | that forwards all the methods to  |
    |                                   | the two underlying hashers.       |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [GuavaRuleKeyHasher](Guava        | ::: block                         |
    | RuleKeyHasher.html "class in com. | An implementation of              |
    | facebook.buck.rules.keys.hasher") | [`RuleKeyHasher`](Rule            |
    |                                   | KeyHasher.html "interface in com. |
    |                                   | facebook.buck.rules.keys.hasher") |
    |                                   | that wraps Guava\'s `Hasher`.     |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [RuleKeyHasherTypes](RuleK        |                                   |
    | eyHasherTypes.html "class in com. |                                   |
    | facebook.buck.rules.keys.hasher") |                                   |
    +-----------------------------------+-----------------------------------+
    | [StringRuleKeyHasher](String      | ::: block                         |
    | RuleKeyHasher.html "class in com. | An implementation of              |
    | facebook.buck.rules.keys.hasher") | [`RuleKeyHasher`](Rule            |
    |                                   | KeyHasher.html "interface in com. |
    |                                   | facebook.buck.rules.keys.hasher") |
    |                                   | that serializes to                |
    |                                   | [`String`                         |
    |                                   | ](http://docs.oracle.com/javase/7 |
    |                                   | /docs/api/java/lang/String.html?i |
    |                                   | s-external=true "class or interfa |
    |                                   | ce in java.lang"){.externalLink}. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ThriftRuleKeyHasher](Thrift      | ::: block                         |
    | RuleKeyHasher.html "class in com. | A rule key hasher that attempts   |
    | facebook.buck.rules.keys.hasher") | to create thrift structures       |
    |                                   | representing rule keys as hashing |
    |                                   | occurs, and writes out the        |
    |                                   | serialized data once the rule key |
    |                                   | is \"complete\"                   |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+

    : Class Summary[ ]{.tabEnd}

-   
      Enum                                                                                                    Description
      ------------------------------------------------------------------------------------------------------- -------------
      [RuleKeyHasher.Container](RuleKeyHasher.Container.html "enum in com.facebook.buck.rules.keys.hasher")    
      [RuleKeyHasher.Wrapper](RuleKeyHasher.Wrapper.html "enum in com.facebook.buck.rules.keys.hasher")        

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
