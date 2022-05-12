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

-   [Overview](../../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../index-all.html)
-   [Help](../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.core.build.engine.config](package-summary.html)
:::

## Class ResourceAwareSchedulingInfo {#class-resourceawareschedulinginfo .title title="Class ResourceAwareSchedulingInfo"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.build.engine.config.ResourceAwareSchedulingInfo

::: description
-   

    ------------------------------------------------------------------------

        public abstract class ResourceAwareSchedulingInfo
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type                      Field                         Description
          -------------------------------------- ----------------------------- -------------
          `static ResourceAwareSchedulingInfo`   `NON_AWARE_SCHEDULING_INFO`    

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                       Description
          --------------------------------- -------------
          `ResourceAwareSchedulingInfo()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `WeightedList         | `adjustS              |                       |
        | eningExecutorService` | erviceDefaultWeightsT |                       |
        |                       | o​(ResourceAmounts def |                       |
        |                       | aultAmounts,          |                       |
        |                       |                       |                       |
        |                       | WeightedListeningExec |                       |
        |                       | utorService service)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract             | `get                  | ::: block             |
        | com.google.common.col | AmountsPerRuleType()` | Map from the value of |
        | lect.ImmutableMap<Str |                       | [`HasNameAn           |
        | ing,​ResourceAmounts>` |                       | dType.getType()`](../ |
        |                       |                       | ../../rules/HasNameAn |
        |                       |                       | dType.html#getType()) |
        |                       |                       | to the required       |
        |                       |                       | resources.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `abst                 | `getDefa              |                       |
        | ract ResourceAmounts` | ultResourceAmounts()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `ResourceAmounts`     | `                     |                       |
        |                       | getResourceAmountsFor |                       |
        |                       | Rule​(BuildRule rule)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract boolean`    | `isResourceAwar       |                       |
        |                       | eSchedulingEnabled()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static Resourc       | `of​(boolean resource  |                       |
        | eAwareSchedulingInfo` | AwareSchedulingEnable |                       |
        |                       | d,   ResourceAmounts  |                       |
        |                       | defaultResourceAmount |                       |
        |                       | s,   Map<String,​? ext |                       |
        |                       | ends ResourceAmounts> |                       |
        |                       |  amountsPerRuleType)` |                       |
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

        []{#NON_AWARE_SCHEDULING_INFO}

        -   #### NON_AWARE_SCHEDULING_INFO

                public static final ResourceAwareSchedulingInfo NON_AWARE_SCHEDULING_INFO
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### ResourceAwareSchedulingInfo

                public ResourceAwareSchedulingInfo()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#of(boolean,com.facebook.buck.util.concurrent.ResourceAmounts,java.util.Map)}

        -   #### of

            ``` methodSignature
            public static ResourceAwareSchedulingInfo of​(boolean resourceAwareSchedulingEnabled,
                                                         ResourceAmounts defaultResourceAmounts,
                                                         Map<String,​? extends ResourceAmounts> amountsPerRuleType)
            ```

        []{#isResourceAwareSchedulingEnabled()}

        -   #### isResourceAwareSchedulingEnabled

            ``` methodSignature
            public abstract boolean isResourceAwareSchedulingEnabled()
            ```

        []{#getDefaultResourceAmounts()}

        -   #### getDefaultResourceAmounts

            ``` methodSignature
            public abstract ResourceAmounts getDefaultResourceAmounts()
            ```

        []{#getAmountsPerRuleType()}

        -   #### getAmountsPerRuleType

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableMap<String,​ResourceAmounts> getAmountsPerRuleType()
            ```

            ::: block
            Map from the value of
            [`HasNameAndType.getType()`](../../../rules/HasNameAndType.html#getType())
            to the required resources.
            :::

        []{#getResourceAmountsForRule(com.facebook.buck.core.rules.BuildRule)}

        -   #### getResourceAmountsForRule

            ``` methodSignature
            public ResourceAmounts getResourceAmountsForRule​(BuildRule rule)
            ```

        []{#adjustServiceDefaultWeightsTo(com.facebook.buck.util.concurrent.ResourceAmounts,com.facebook.buck.util.concurrent.WeightedListeningExecutorService)}

        -   #### adjustServiceDefaultWeightsTo

            ``` methodSignature
            public WeightedListeningExecutorService adjustServiceDefaultWeightsTo​(ResourceAmounts defaultAmounts,
                                                                                  WeightedListeningExecutorService service)
            ```
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

-   [Overview](../../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../index-all.html)
-   [Help](../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../allclasses.html)

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
