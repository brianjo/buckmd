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
-   Nested \| 
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

## Class EventPostingRuleKeyCacheScope\<V\> {#class-eventpostingrulekeycachescopev .title title="Class EventPostingRuleKeyCacheScope"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.rules.keys.EventPostingRuleKeyCacheScope\<V\>

::: description
-   

    All Implemented Interfaces:
    :   `RuleKeyCacheScope<V>`, `AutoCloseable`

    ------------------------------------------------------------------------

        public class EventPostingRuleKeyCacheScope<V>
        extends Object
        implements RuleKeyCacheScope<V>

    ::: block
    A
    [`RuleKeyCacheScope`](RuleKeyCacheScope.html "interface in com.facebook.buck.rules.keys")
    which logs stats on close.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                             Description
          ----------------------------------------------------------------------------------------------------------------------- -------------
          `EventPostingRuleKeyCacheScope​(BuckEventBus buckEventBus,                              TrackedRuleKeyCache<V> cache)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `protected void`      | `cleanup​(SimplePe     | ::: block             |
        |                       | rfEvent.Scope scope)` | Additional cleanup.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `close()`             |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Tr                   | `getCache()`          |                       |
        | ackedRuleKeyCache<V>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected void`      | `setup​(SimplePe       | ::: block             |
        |                       | rfEvent.Scope scope)` | Additional setup.     |
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

        []{#<init>(com.facebook.buck.event.BuckEventBus,com.facebook.buck.rules.keys.TrackedRuleKeyCache)}

        -   #### EventPostingRuleKeyCacheScope

                public EventPostingRuleKeyCacheScope​(BuckEventBus buckEventBus,
                                                     TrackedRuleKeyCache<V> cache)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#setup(com.facebook.buck.event.SimplePerfEvent.Scope)}

        -   #### setup

            ``` methodSignature
            protected void setup​(SimplePerfEvent.Scope scope)
            ```

            ::: block
            Additional setup. To be implemented by sub-classes.
            :::

        []{#cleanup(com.facebook.buck.event.SimplePerfEvent.Scope)}

        -   #### cleanup

            ``` methodSignature
            protected void cleanup​(SimplePerfEvent.Scope scope)
            ```

            ::: block
            Additional cleanup. To be implemented by sub-classes.
            :::

        []{#getCache()}

        -   #### getCache

            ``` methodSignature
            public final TrackedRuleKeyCache<V> getCache()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getCache` in interface `RuleKeyCacheScope<V>`

            [Returns:]{.returnLabel}
            :   the scoped
                [`RuleKeyCache`](RuleKeyCache.html "interface in com.facebook.buck.rules.keys").

        []{#close()}

        -   #### close

            ``` methodSignature
            public final void close()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `close` in interface `AutoCloseable`

            [Specified by:]{.overrideSpecifyLabel}
            :   `close` in interface `RuleKeyCacheScope<V>`
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
-   Nested \| 
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
