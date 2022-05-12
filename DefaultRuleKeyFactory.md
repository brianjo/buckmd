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
-   [Package](package-summary.html)
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

<div>

-   Summary: 
-   [Nested](#nested.class.summary) \| 
-   Field \| 
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   [Constr](#constructor.detail) \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.top}
:::
:::

::: navPadding
 
:::
:::

::: {role="main"}
::: header
::: subTitle
[Package]{.packageLabelInType} [com.facebook.buck.rules.keys](package-summary.html)
:::

## Class DefaultRuleKeyFactory {#class-defaultrulekeyfactory .title title="Class DefaultRuleKeyFactory"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.rules.keys.DefaultRuleKeyFactory

::: description
-   

    All Implemented Interfaces:
    :   `RuleKeyFactory<RuleKey>`,
        `RuleKeyFactoryWithDiagnostics<RuleKey>`

    ------------------------------------------------------------------------

        public class DefaultRuleKeyFactory
        extends Object
        implements RuleKeyFactoryWithDiagnostics<RuleKey>

    ::: block
    A
    [`RuleKeyFactory`](RuleKeyFactory.html "interface in com.facebook.buck.rules.keys")
    which adds some default settings to
    [`RuleKey`](../../core/rulekey/RuleKey.html "class in com.facebook.buck.core.rulekey")s.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type   Class                                       Description
          ------------------- ------------------------------------------- -------------
          `class `            `DefaultRuleKeyFactory.Builder<RULE_KEY>`    

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                                       Description
          ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `DefaultRuleKeyFactory​(RuleKeyFieldLoader ruleKeyFieldLoader,                      FileHashLoader hashLoader,                      SourcePathRuleFinder ruleFinder)`                                                                                                                               
          `DefaultRuleKeyFactory​(RuleKeyFieldLoader ruleKeyFieldLoader,                      FileHashLoader hashLoader,                      SourcePathRuleFinder ruleFinder,                      RuleKeyCache<RuleKey> ruleKeyCache,                      Optional<ThriftRuleKeyLogger> ruleKeyLogger)`    
          `DefaultRuleKeyFactory​(RuleKeyFieldLoader ruleKeyFieldLoader,                      FileHashLoader hashLoader,                      SourcePathRuleFinder ruleFinder,                      Optional<ThriftRuleKeyLogger> ruleKeyLogger)`                                                             

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `RuleKey`             | `build​(Build          | ::: block             |
        |                       | EngineAction action)` | Creates a new         |
        |                       |                       | `RULE_KEY` for the    |
        |                       |                       | given                 |
        |                       |                       | [`BuildEngineAct      |
        |                       |                       | ion`](../../core/buil |
        |                       |                       | d/action/BuildEngineA |
        |                       |                       | ction.html "interface |
        |                       |                       |  in com.facebook.buck |
        |                       |                       | .core.build.action"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `<DIAG_KEY> Ru        | `buildForDiagn        | ::: block             |
        | leKeyDiagnostics.Resu | ostics​(BuildEngineAct | Builds a diagnostic   |
        | lt<RuleKey,​DIAG_KEY>` | ion action,           | result for the given  |
        |                       |           RuleKeyHash | rule or appendable.   |
        |                       | er<DIAG_KEY> hasher)` | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `<DIAG_KEY> Ru        | `buildForDiagn        |                       |
        | leKeyDiagnostics.Resu | ostics​(AddsToRuleKey  |                       |
        | lt<RuleKey,​DIAG_KEY>` | appendable,           |                       |
        |                       |           RuleKeyHash |                       |
        |                       | er<DIAG_KEY> hasher)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `RuleKey`             | `getFromCache​(Build   | ::: block             |
        |                       | EngineAction action)` | Returns a `RULE_KEY`  |
        |                       |                       | from an internal      |
        |                       |                       | cache, if possible.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `                     |                       |
        | DefaultRuleKeyFactory | newBuilderForTesting​( |                       |
        | .Builder<com.google.c | BuildRule buildRule)` |                       |
        | ommon.hash.HashCode>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.rules.keys.RuleKeyFactory}

            ### Methods inherited from interface com.facebook.buck.rules.keys.[RuleKeyFactory](RuleKeyFactory.html "interface in com.facebook.buck.rules.keys")

            `getInputSizeLimit`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.rules.keys.RuleKeyFieldLoader,com.facebook.buck.util.hashing.FileHashLoader,com.facebook.buck.core.rules.SourcePathRuleFinder,com.facebook.buck.rules.keys.RuleKeyCache,java.util.Optional)}

        -   #### DefaultRuleKeyFactory

                public DefaultRuleKeyFactory​(RuleKeyFieldLoader ruleKeyFieldLoader,
                                             FileHashLoader hashLoader,
                                             SourcePathRuleFinder ruleFinder,
                                             RuleKeyCache<RuleKey> ruleKeyCache,
                                             Optional<ThriftRuleKeyLogger> ruleKeyLogger)

        []{#<init>(com.facebook.buck.rules.keys.RuleKeyFieldLoader,com.facebook.buck.util.hashing.FileHashLoader,com.facebook.buck.core.rules.SourcePathRuleFinder)}

        -   #### DefaultRuleKeyFactory

                public DefaultRuleKeyFactory​(RuleKeyFieldLoader ruleKeyFieldLoader,
                                             FileHashLoader hashLoader,
                                             SourcePathRuleFinder ruleFinder)

        []{#<init>(com.facebook.buck.rules.keys.RuleKeyFieldLoader,com.facebook.buck.util.hashing.FileHashLoader,com.facebook.buck.core.rules.SourcePathRuleFinder,java.util.Optional)}

        -   #### DefaultRuleKeyFactory

                public DefaultRuleKeyFactory​(RuleKeyFieldLoader ruleKeyFieldLoader,
                                             FileHashLoader hashLoader,
                                             SourcePathRuleFinder ruleFinder,
                                             Optional<ThriftRuleKeyLogger> ruleKeyLogger)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#newBuilderForTesting(com.facebook.buck.core.rules.BuildRule)}

        -   #### newBuilderForTesting

            ``` methodSignature
            public DefaultRuleKeyFactory.Builder<com.google.common.hash.HashCode> newBuilderForTesting​(BuildRule buildRule)
            ```

        []{#getFromCache(com.facebook.buck.core.build.action.BuildEngineAction)}

        -   #### getFromCache

            ``` methodSignature
            @Nullable
            public RuleKey getFromCache​(BuildEngineAction action)
            ```

            ::: block
            [Description copied from
            interface: `RuleKeyFactory`]{.descfrmTypeLabel}
            :::

            ::: block
            Returns a `RULE_KEY` from an internal cache, if possible. If
            a non-null value is returned, it is guaranteed to be he same
            as if
            [`RuleKeyFactory.build(com.facebook.buck.core.build.action.BuildEngineAction)`](RuleKeyFactory.html#build(com.facebook.buck.core.build.action.BuildEngineAction))
            were called instead.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getFromCache` in interface `RuleKeyFactory<RuleKey>`

        []{#build(com.facebook.buck.core.build.action.BuildEngineAction)}

        -   #### build

            ``` methodSignature
            public RuleKey build​(BuildEngineAction action)
            ```

            ::: block
            [Description copied from
            interface: `RuleKeyFactory`]{.descfrmTypeLabel}
            :::

            ::: block
            Creates a new `RULE_KEY` for the given
            [`BuildEngineAction`](../../core/build/action/BuildEngineAction.html "interface in com.facebook.buck.core.build.action").
            In most cases `  RULE_KEY` is going to be
            [`RuleKey`](../../core/rulekey/RuleKey.html "class in com.facebook.buck.core.rulekey"),
            but it can be anything really.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `build` in interface `RuleKeyFactory<RuleKey>`

            [Parameters:]{.paramLabel}
            :   `action` - The build rule to create the key for.

            [Returns:]{.returnLabel}
            :   A rule key.

        []{#buildForDiagnostics(com.facebook.buck.core.build.action.BuildEngineAction,com.facebook.buck.rules.keys.hasher.RuleKeyHasher)}

        -   #### buildForDiagnostics

            ``` methodSignature
            public <DIAG_KEY> RuleKeyDiagnostics.Result<RuleKey,​DIAG_KEY> buildForDiagnostics​(BuildEngineAction action,
                                                                                                    RuleKeyHasher<DIAG_KEY> hasher)
            ```

            ::: block
            [Description copied from
            interface: `RuleKeyFactoryWithDiagnostics`]{.descfrmTypeLabel}
            :::

            ::: block
            Builds a diagnostic result for the given rule or appendable.
            This method is intended to be used exclusively for
            diagnostic purposes and not for computing rule keys used for
            build process in any other way.

            The provided custom hasher is used for all the elements
            hashed under this rule or appendable.

            Note however that if the factory chooses to hash nested
            build rules and appendables separately, and only include
            their final hash for the computation of this hash, this
            choice applies both to real rule keys and the diagnostic
            keys. The client may need to perform a separate call for
            each build rule or appendable of interest. Moreover, the
            hash for the nested build rules and appendables is obtained
            by using the default hasher and not the provided custom
            hasher. This is the natural choice as it allows the custom
            hasher to see precisely those elements that the default
            hasher sees. It is also more efficient because factories
            usually cache rule keys computed with the default hasher,
            whereas using the custom hasher prevents that and would
            require hashing all of its transitive dependencies.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `buildForDiagnostics` in
                interface `RuleKeyFactoryWithDiagnostics<RuleKey>`

        []{#buildForDiagnostics(com.facebook.buck.core.rulekey.AddsToRuleKey,com.facebook.buck.rules.keys.hasher.RuleKeyHasher)}

        -   #### buildForDiagnostics

            ``` methodSignature
            public <DIAG_KEY> RuleKeyDiagnostics.Result<RuleKey,​DIAG_KEY> buildForDiagnostics​(AddsToRuleKey appendable,
                                                                                                    RuleKeyHasher<DIAG_KEY> hasher)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `buildForDiagnostics` in
                interface `RuleKeyFactoryWithDiagnostics<RuleKey>`
    :::
:::
:::
:::

::: bottomNav
[]{#navbar.bottom}

::: skipNav
[Skip navigation links](#skip.navbar.bottom "Skip navigation links")
:::

[]{#navbar.bottom.firstrow}

-   [Overview](../../../../../index.html)
-   [Package](package-summary.html)
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

<div>

-   Summary: 
-   [Nested](#nested.class.summary) \| 
-   Field \| 
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   [Constr](#constructor.detail) \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
