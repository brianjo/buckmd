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
[Package]{.packageLabelInType} [com.facebook.buck.support.state](package-summary.html)
:::

## Class BuckGlobalStateLifecycleManager {#class-buckglobalstatelifecyclemanager .title title="Class BuckGlobalStateLifecycleManager"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.support.state.BuckGlobalStateLifecycleManager

::: description
-   

    ------------------------------------------------------------------------

        @ThreadSafe
        public class BuckGlobalStateLifecycleManager
        extends Object

    ::: block
    Guards access to the
    [`BuckGlobalState`](BuckGlobalState.html "class in com.facebook.buck.support.state")
    instance behind cell configuration checks. Creates or re-creates the
    daemon state as necessary if the cell configuration changes.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static class `       | `BuckGl               | ::: block             |
        |                       | obalStateLifecycleMan | Indicates whether a   |
        |                       | ager.LifecycleStatus` | daemon\'s             |
        |                       |                       | [`BuckGlobalState`](B |
        |                       |                       | uckGlobalState.html " |
        |                       |                       | class in com.facebook |
        |                       |                       | .buck.support.state") |
        |                       |                       | is reused, or why it  |
        |                       |                       | can\'t be reused      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                           Description
          ------------------------------------- -------------
          `BuckGlobalStateLifecycleManager()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `                     | `getBuckConfig()`     |                       |
        | Optional<BuckConfig>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Pair<Bu              | `getBuck              | ::: block             |
        | ckGlobalState,​BuckGlo | GlobalState​(Cells cel | Get or create Daemon. |
        | balStateLifecycleMana | ls,                   | :::                   |
        | ger.LifecycleStatus>` |  KnownRuleTypesProvid |                       |
        |                       | er knownRuleTypesProv |                       |
        |                       | ider,                 |                       |
        |                       |    Watchman watchman, |                       |
        |                       |                    Co |                       |
        |                       | nsole console,        |                       |
        |                       |             Clock clo |                       |
        |                       | ck,                   |                       |
        |                       |  UnconfiguredBuildTar |                       |
        |                       | getViewFactory unconf |                       |
        |                       | iguredBuildTargetFact |                       |
        |                       | ory,                  |                       |
        |                       |   TargetConfiguration |                       |
        |                       | Serializer targetConf |                       |
        |                       | igurationSerializer)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `hasSto               |                       |
        |                       | redBuckGlobalState()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `re                   | ::: block             |
        |                       | setBuckGlobalState()` | Manually reset the    |
        |                       |                       | [                     |
        |                       |                       | `BuckGlobalState`](Bu |
        |                       |                       | ckGlobalState.html "c |
        |                       |                       | lass in com.facebook. |
        |                       |                       | buck.support.state"), |
        |                       |                       | used for testing.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### BuckGlobalStateLifecycleManager

                public BuckGlobalStateLifecycleManager()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#hasStoredBuckGlobalState()}

        -   #### hasStoredBuckGlobalState

            ``` methodSignature
            public boolean hasStoredBuckGlobalState()
            ```

        []{#getBuckConfig()}

        -   #### getBuckConfig

            ``` methodSignature
            public Optional<BuckConfig> getBuckConfig()
            ```

        []{#getBuckGlobalState(com.facebook.buck.core.cell.Cells,com.facebook.buck.core.rules.knowntypes.provider.KnownRuleTypesProvider,com.facebook.buck.io.watchman.Watchman,com.facebook.buck.util.Console,com.facebook.buck.util.timing.Clock,com.facebook.buck.core.parser.buildtargetparser.UnconfiguredBuildTargetViewFactory,com.facebook.buck.core.model.TargetConfigurationSerializer)}

        -   #### getBuckGlobalState

            ``` methodSignature
            public Pair<BuckGlobalState,​BuckGlobalStateLifecycleManager.LifecycleStatus> getBuckGlobalState​(Cells cells,
                                                                                                                  KnownRuleTypesProvider knownRuleTypesProvider,
                                                                                                                  Watchman watchman,
                                                                                                                  Console console,
                                                                                                                  Clock clock,
                                                                                                                  UnconfiguredBuildTargetViewFactory unconfiguredBuildTargetFactory,
                                                                                                                  TargetConfigurationSerializer targetConfigurationSerializer)
            ```

            ::: block
            Get or create Daemon.
            :::

        []{#resetBuckGlobalState()}

        -   #### resetBuckGlobalState

            ``` methodSignature
            public void resetBuckGlobalState()
            ```

            ::: block
            Manually reset the
            [`BuckGlobalState`](BuckGlobalState.html "class in com.facebook.buck.support.state"),
            used for testing.
            :::
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
