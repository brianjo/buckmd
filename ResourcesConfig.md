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
-   [Field](#field.summary) \| 
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.core.resources](package-summary.html)
:::

## Class ResourcesConfig {#class-resourcesconfig .title title="Class ResourcesConfig"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.resources.ResourcesConfig

::: description
-   

    All Implemented Interfaces:
    :   `ConfigView<BuckConfig>`

    ------------------------------------------------------------------------

        public abstract class ResourcesConfig
        extends Object
        implements ConfigView<BuckConfig>
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type   Field                                 Description
          ------------------- ------------------------------------- -------------
          `static String`     `RESOURCES_PER_RULE_SECTION_HEADER`    
          `static String`     `RESOURCES_SECTION_HEADER`             

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor           Description
          --------------------- -------------
          `ResourcesConfig()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `ConcurrencyLimit`    | `g                    | ::: block             |
        |                       | etConcurrencyLimit()` | Construct a default   |
        |                       |                       | ConcurrencyLimit      |
        |                       |                       | instance from this    |
        |                       |                       | config.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ResourceAmounts`     | `getDefa              |                       |
        |                       | ultResourceAmounts()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract BuckConfig` | `getDelegate()`       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `get                  |                       |
        |                       | ManagedThreadCount()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `ResourceAmounts`     | `getMaxi              |                       |
        |                       | mumResourceAmounts()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Resour               | `getResource          |                       |
        | ceAllocationFairness` | AllocationFairness()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getResource          |                       |
        | com.google.common.col | AmountsPerRuleType()` |                       |
        | lect.ImmutableMap<Str |                       |                       |
        | ing,​ResourceAmounts>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isResourceAwar       |                       |
        |                       | eSchedulingEnabled()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `st                   | `of​(                  |                       |
        | atic ResourcesConfig` | BuckConfig delegate)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#field.detail}

        ### Field Detail

        []{#RESOURCES_SECTION_HEADER}

        -   #### RESOURCES_SECTION_HEADER

                public static final String RESOURCES_SECTION_HEADER

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.core.resources.ResourcesConfig.RESOURCES_SECTION_HEADER)

        []{#RESOURCES_PER_RULE_SECTION_HEADER}

        -   #### RESOURCES_PER_RULE_SECTION_HEADER

                public static final String RESOURCES_PER_RULE_SECTION_HEADER

            [See Also:]{.seeLabel}
            :   [Constant Field
                Values](../../../../../constant-values.html#com.facebook.buck.core.resources.ResourcesConfig.RESOURCES_PER_RULE_SECTION_HEADER)
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### ResourcesConfig

                public ResourcesConfig()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getDelegate()}

        -   #### getDelegate

            ``` methodSignature
            public abstract BuckConfig getDelegate()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getDelegate` in interface `ConfigView<BuckConfig>`

        []{#of(com.facebook.buck.core.config.BuckConfig)}

        -   #### of

            ``` methodSignature
            public static ResourcesConfig of​(BuckConfig delegate)
            ```

        []{#getResourceAllocationFairness()}

        -   #### getResourceAllocationFairness

            ``` methodSignature
            @Lazy
            public ResourceAllocationFairness getResourceAllocationFairness()
            ```

        []{#isResourceAwareSchedulingEnabled()}

        -   #### isResourceAwareSchedulingEnabled

            ``` methodSignature
            @Lazy
            public boolean isResourceAwareSchedulingEnabled()
            ```

        []{#getResourceAmountsPerRuleType()}

        -   #### getResourceAmountsPerRuleType

            ``` methodSignature
            @Lazy
            public com.google.common.collect.ImmutableMap<String,​ResourceAmounts> getResourceAmountsPerRuleType()
            ```

        []{#getManagedThreadCount()}

        -   #### getManagedThreadCount

            ``` methodSignature
            @Lazy
            public int getManagedThreadCount()
            ```

        []{#getDefaultResourceAmounts()}

        -   #### getDefaultResourceAmounts

            ``` methodSignature
            @Lazy
            public ResourceAmounts getDefaultResourceAmounts()
            ```

        []{#getMaximumResourceAmounts()}

        -   #### getMaximumResourceAmounts

            ``` methodSignature
            @Lazy
            public ResourceAmounts getMaximumResourceAmounts()
            ```

        []{#getConcurrencyLimit()}

        -   #### getConcurrencyLimit

            ``` methodSignature
            @Lazy
            public ConcurrencyLimit getConcurrencyLimit()
            ```

            ::: block
            Construct a default ConcurrencyLimit instance from this
            config.
            :::

            [Returns:]{.returnLabel}
            :   New instance of ConcurrencyLimit.
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
-   [Field](#field.summary) \| 
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
-   [Constr](#constructor.detail) \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
