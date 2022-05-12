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
[Package]{.packageLabelInType} [com.facebook.buck.event.listener](package-summary.html)
:::

## Class SuperConsoleConfig {#class-superconsoleconfig .title title="Class SuperConsoleConfig"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.event.listener.SuperConsoleConfig

::: description
-   

    ------------------------------------------------------------------------

        public class SuperConsoleConfig
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                 Description
          ------------------------------------------- -------------
          `SuperConsoleConfig​(BuckConfig delegate)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `long`                | `getBuildRuleMin      |                       |
        |                       | imumDurationMillis()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `getHideSucce         |                       |
        |                       | ededRulesInLogMode()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `getNumbe             |                       |
        |                       | rOfSlowRulesToShow()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `                     |                       |
        |                       | getThreadLineLimit()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `getThre              |                       |
        |                       | adLineLimitOnError()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `getThread            |                       |
        |                       | LineLimitOnWarning()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `OptionalInt`         | `getThreadLi          |                       |
        |                       | neOutputMaxColumns()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isEnabled            | ::: block             |
        |                       | ​(Ansi ansi,           | Whether the           |
        |                       | Verbosity verbosity)` | SuperConsole is       |
        |                       |                       | enabled               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `shouldAlway          |                       |
        |                       | sSortThreadsByTime()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `shouldShow           |                       |
        |                       | SlowRulesInConsole()` |                       |
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

        []{#<init>(com.facebook.buck.core.config.BuckConfig)}

        -   #### SuperConsoleConfig

                public SuperConsoleConfig​(BuckConfig delegate)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getThreadLineLimit()}

        -   #### getThreadLineLimit

            ``` methodSignature
            public int getThreadLineLimit()
            ```

        []{#getThreadLineLimitOnWarning()}

        -   #### getThreadLineLimitOnWarning

            ``` methodSignature
            public int getThreadLineLimitOnWarning()
            ```

        []{#getThreadLineLimitOnError()}

        -   #### getThreadLineLimitOnError

            ``` methodSignature
            public int getThreadLineLimitOnError()
            ```

        []{#shouldAlwaysSortThreadsByTime()}

        -   #### shouldAlwaysSortThreadsByTime

            ``` methodSignature
            public boolean shouldAlwaysSortThreadsByTime()
            ```

        []{#getBuildRuleMinimumDurationMillis()}

        -   #### getBuildRuleMinimumDurationMillis

            ``` methodSignature
            public long getBuildRuleMinimumDurationMillis()
            ```

        []{#getHideSucceededRulesInLogMode()}

        -   #### getHideSucceededRulesInLogMode

            ``` methodSignature
            public boolean getHideSucceededRulesInLogMode()
            ```

        []{#getNumberOfSlowRulesToShow()}

        -   #### getNumberOfSlowRulesToShow

            ``` methodSignature
            public int getNumberOfSlowRulesToShow()
            ```

        []{#shouldShowSlowRulesInConsole()}

        -   #### shouldShowSlowRulesInConsole

            ``` methodSignature
            public boolean shouldShowSlowRulesInConsole()
            ```

        []{#getThreadLineOutputMaxColumns()}

        -   #### getThreadLineOutputMaxColumns

            ``` methodSignature
            public OptionalInt getThreadLineOutputMaxColumns()
            ```

        []{#isEnabled(com.facebook.buck.util.Ansi,com.facebook.buck.util.Verbosity)}

        -   #### isEnabled

            ``` methodSignature
            public boolean isEnabled​(Ansi ansi,
                                     Verbosity verbosity)
            ```

            ::: block
            Whether the SuperConsole is enabled
            :::

            [Returns:]{.returnLabel}
            :   whether the output should be presented using the super
                superConsole style
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
