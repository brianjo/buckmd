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
# Package com.facebook.buck.core.rulekey {#package-com.facebook.buck.core.rulekey .title title="Package"}
:::

::: contentContainer
-   +-----------------------------------+-----------------------------------+
    | Interface                         | Description                       |
    +===================================+===================================+
    | [AddsToRuleKey]                   | ::: block                         |
    | (AddsToRuleKey.html "interface in | Identifies a class that uses      |
    |  com.facebook.buck.core.rulekey") | [`AddToRuleKey`]                  |
    |                                   | (AddToRuleKey.html "annotation in |
    |                                   |  com.facebook.buck.core.rulekey") |
    |                                   | annotations to indicate fields    |
    |                                   | that should be added to rule      |
    |                                   | keys.                             |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [All                              | ::: block                         |
    | owsNonAnnotatedFields](AllowsNonA | Marks classes where we shouldn\'t |
    | nnotatedFields.html "interface in | report on fields that aren\'t     |
    |  com.facebook.buck.core.rulekey") | annotated with                    |
    |                                   | \@                                |
    |                                   | AddToRuleKey/@ExcludeFromRuleKey. |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [BuildRuleKeys]                   |                                   |
    | (BuildRuleKeys.html "interface in |                                   |
    |  com.facebook.buck.core.rulekey") |                                   |
    +-----------------------------------+-----------------------------------+
    | [CustomFieldBehaviorTag](CustomFi | ::: block                         |
    | eldBehaviorTag.html "interface in | Root interface for any            |
    |  com.facebook.buck.core.rulekey") | CustomFieldBehavior values.       |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [CustomFieldDepsTag](Cust         | ::: block                         |
    | omFieldDepsTag.html "interface in | Tag to indicate custom field deps |
    |  com.facebook.buck.core.rulekey") | derivation.                       |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [CustomFieldInputsTag](Custom     | ::: block                         |
    | FieldInputsTag.html "interface in | Tag to indicate custom field      |
    |  com.facebook.buck.core.rulekey") | inputs derivation.                |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [CustomFie                        | ::: block                         |
    | ldSerializationTag](CustomFieldSe | Tag to indicate custom field      |
    | rializationTag.html "interface in | serialization.                    |
    |  com.facebook.buck.core.rulekey") | :::                               |
    +-----------------------------------+-----------------------------------+

    : Interface Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Class                             | Description                       |
    +===================================+===================================+
    | [DefaultFieldDeps                 | ::: block                         |
    | ](DefaultFieldDeps.html "class in | This indicates that a field that  |
    |  com.facebook.buck.core.rulekey") | is not annotated with             |
    |                                   | \@AddToRuleKey should still have  |
    |                                   | its deps derived as if it were    |
    |                                   | added to the rule key.            |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [DefaultFieldInputs](             | ::: block                         |
    | DefaultFieldInputs.html "class in | This indicates that a field that  |
    |  com.facebook.buck.core.rulekey") | is not annotated with             |
    |                                   | \@AddToRuleKey should still have  |
    |                                   | its inputs derived as if it were  |
    |                                   | added to the rule key.            |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [D                                | ::: block                         |
    | efaultFieldSerialization](Default | This indicates that a field that  |
    | FieldSerialization.html "class in | is not annotated with             |
    |  com.facebook.buck.core.rulekey") | \@AddToRuleKey should still be    |
    |                                   | serialized/deserialized as if it  |
    |                                   | were added to the rule key (i.e.  |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [IgnoredFieldDeps                 | ::: block                         |
    | ](IgnoredFieldDeps.html "class in | Used to indicate that this field  |
    |  com.facebook.buck.core.rulekey") | should be ignored for deps        |
    |                                   | derivation.                       |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [IgnoredFieldInputs](             | ::: block                         |
    | IgnoredFieldInputs.html "class in | Used to indicate that this field  |
    |  com.facebook.buck.core.rulekey") | should be ignored for inputs      |
    |                                   | derivation.                       |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [MissingExcludeReporter](Miss     | ::: block                         |
    | ingExcludeReporter.html "class in | Utility for reporting issues of   |
    |  com.facebook.buck.core.rulekey") | fields/methods not being          |
    |                                   | annotated to be added to          |
    |                                   | rulekeys.                         |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [RuleKey](RuleKey.html "class in  | ::: block                         |
    |  com.facebook.buck.core.rulekey") | RuleKey encapsulates regimented   |
    |                                   | computation of SHA-1 keys that    |
    |                                   | incorporate all BuildRule state   |
    |                                   | relevant to idempotency.          |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [ThrowingSerialization](Thr       | ::: block                         |
    | owingSerialization.html "class in | Used to indicate that this field  |
    |  com.facebook.buck.core.rulekey") | doesn\'t support serialization.   |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+

    : Class Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Enum                              | Description                       |
    +===================================+===================================+
    | [RuleKeyDiagnosticsMode](Rul      | ::: block                         |
    | eKeyDiagnosticsMode.html "enum in | Whether and when to perform       |
    |  com.facebook.buck.core.rulekey") | rulekey diagnostics.              |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+

    : Enum Summary[ ]{.tabEnd}

-   +-----------------------------------+-----------------------------------+
    | Annotation Type                   | Description                       |
    +===================================+===================================+
    | [AddToRuleKey]                    | ::: block                         |
    | (AddToRuleKey.html "annotation in | Indicates that a field or method  |
    |  com.facebook.buck.core.rulekey") | of a class should be added to     |
    |                                   | rulekeys when an instance of that |
    |                                   | class is added to a rulekey.      |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+
    | [CustomFieldBehavior](Custom      |                                   |
    | FieldBehavior.html "annotation in |                                   |
    |  com.facebook.buck.core.rulekey") |                                   |
    +-----------------------------------+-----------------------------------+
    | [ExcludeFromRuleKey](Exclu        | ::: block                         |
    | deFromRuleKey.html "annotation in | Marks a field/method of a class   |
    |  com.facebook.buck.core.rulekey") | explicitly excluded from          |
    |                                   | rulekeys.                         |
    |                                   | :::                               |
    +-----------------------------------+-----------------------------------+

    : Annotation Types Summary[ ]{.tabEnd}
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
