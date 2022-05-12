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
[Package]{.packageLabelInType} [com.facebook.buck.core.model](package-summary.html)
:::

## Class RuleBasedTargetConfiguration {#class-rulebasedtargetconfiguration .title title="Class RuleBasedTargetConfiguration"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.core.model.TargetConfiguration](TargetConfiguration.html "class in com.facebook.buck.core.model")

    -   -   com.facebook.buck.core.model.RuleBasedTargetConfiguration

::: description
-   

    All Implemented Interfaces:
    :   `Comparable<TargetConfiguration>`

    ------------------------------------------------------------------------

        public abstract class RuleBasedTargetConfiguration
        extends TargetConfiguration

    ::: block
    Platform target implementation of
    [`TargetConfiguration`](TargetConfiguration.html "class in com.facebook.buck.core.model").
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                        Description
          ---------------------------------- -------------
          `RuleBasedTargetConfiguration()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `protected void`      | `check()`             |                       |
        +-----------------------+-----------------------+-----------------------+
        | `O                    | `getC                 |                       |
        | ptional<BuildTarget>` | onfigurationTarget()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getTargetPlatform()` |                       |
        | abstract BuildTarget` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static RuleBase      | `of​(BuildTa           |                       |
        | dTargetConfiguration` | rget targetPlatform)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `toString()`          | ::: block             |
        |                       |                       | Build target for rule |
        |                       |                       | based build target or |
        |                       |                       | class name otherwise. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.core.model.TargetConfiguration}

            ### Methods inherited from class com.facebook.buck.core.model.[TargetConfiguration](TargetConfiguration.html "class in com.facebook.buck.core.model")

            `compareTo`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### RuleBasedTargetConfiguration

                public RuleBasedTargetConfiguration()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#check()}

        -   #### check

            ``` methodSignature
            @Check
            protected void check()
            ```

        []{#getTargetPlatform()}

        -   #### getTargetPlatform

            ``` methodSignature
            public abstract BuildTarget getTargetPlatform()
            ```

        []{#getConfigurationTarget()}

        -   #### getConfigurationTarget

            ``` methodSignature
            public Optional<BuildTarget> getConfigurationTarget()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getConfigurationTarget` in class `TargetConfiguration`

        []{#toString()}

        -   #### toString

            ``` methodSignature
            public String toString()
            ```

            ::: block
            [Description copied from
            class: `TargetConfiguration`]{.descfrmTypeLabel}
            :::

            ::: block
            Build target for rule based build target or class name
            otherwise.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `toString` in class `TargetConfiguration`

        []{#of(com.facebook.buck.core.model.BuildTarget)}

        -   #### of

            ``` methodSignature
            public static RuleBasedTargetConfiguration of​(BuildTarget targetPlatform)
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
