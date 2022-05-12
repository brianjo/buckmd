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
-   [Package](package-summary.html)
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
[Package]{.packageLabelInType} [com.facebook.buck.rules.keys.config](package-summary.html)
:::

## Class RuleKeyConfiguration {#class-rulekeyconfiguration .title title="Class RuleKeyConfiguration"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.rules.keys.config.RuleKeyConfiguration

::: description
-   

    ------------------------------------------------------------------------

        public abstract class RuleKeyConfiguration
        extends Object

    ::: block
    Provides rule key configuration options.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                Description
          -------------------------- -------------
          `RuleKeyConfiguration()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `abstract Bu          | `getBuck              |                       |
        | ckModuleHashStrategy` | ModuleHashStrategy()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract long`       | `getBuildInputRu      |                       |
        |                       | leKeyFileSizeLimit()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract String`     | `getCoreKey()`        |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract int`        | `getSeed()`           | ::: block             |
        |                       |                       | The seed of all rule  |
        |                       |                       | keys.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static               | `of​(int seed,         |                       |
        | RuleKeyConfiguration` |  String coreKey,   lo |                       |
        |                       | ng buildInputRuleKeyF |                       |
        |                       | ileSizeLimit,   BuckM |                       |
        |                       | oduleHashStrategy buc |                       |
        |                       | kModuleHashStrategy)` |                       |
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
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### RuleKeyConfiguration

                public RuleKeyConfiguration()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getSeed()}

        -   #### getSeed

            ``` methodSignature
            public abstract int getSeed()
            ```

            ::: block
            The seed of all rule keys.
            :::

        []{#getCoreKey()}

        -   #### getCoreKey

            ``` methodSignature
            public abstract String getCoreKey()
            ```

        []{#getBuildInputRuleKeyFileSizeLimit()}

        -   #### getBuildInputRuleKeyFileSizeLimit

            ``` methodSignature
            public abstract long getBuildInputRuleKeyFileSizeLimit()
            ```

        []{#getBuckModuleHashStrategy()}

        -   #### getBuckModuleHashStrategy

            ``` methodSignature
            public abstract BuckModuleHashStrategy getBuckModuleHashStrategy()
            ```

        []{#of(int,java.lang.String,long,com.facebook.buck.core.module.BuckModuleHashStrategy)}

        -   #### of

            ``` methodSignature
            public static RuleKeyConfiguration of​(int seed,
                                                  String coreKey,
                                                  long buildInputRuleKeyFileSizeLimit,
                                                  BuckModuleHashStrategy buckModuleHashStrategy)
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

-   [Overview](../../../../../../index.html)
-   [Package](package-summary.html)
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
