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
[Package]{.packageLabelInType} [com.facebook.buck.core.rules.platform](package-summary.html)
:::

## Class RuleBasedTargetPlatformResolver {#class-rulebasedtargetplatformresolver .title title="Class RuleBasedTargetPlatformResolver"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.rules.platform.RuleBasedTargetPlatformResolver

::: description
-   

    All Implemented Interfaces:
    :   `TargetPlatformResolver`

    ------------------------------------------------------------------------

        public class RuleBasedTargetPlatformResolver
        extends Object
        implements TargetPlatformResolver

    ::: block
    An implementation of
    [`TargetPlatformResolver`](../../model/platform/TargetPlatformResolver.html "interface in com.facebook.buck.core.model.platform")
    that creates
    [`Platform`](../../model/platform/Platform.html "interface in com.facebook.buck.core.model.platform")
    from `PlatformRule` for
    [`RuleBasedTargetConfiguration`](../../model/RuleBasedTargetConfiguration.html "class in com.facebook.buck.core.model").
    Note that the clients of this class need to make sure the queries
    are made with the correct target configuration type.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                            Description
          ---------------------------------------------------------------------- -------------
          `RuleBasedTargetPlatformResolver​(PlatformResolver platformResolver)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                                                                                                           Description
          ------------------- ---------------------------------------------------------------------------------------------------------------- -------------
          `Platform`          `getTargetPlatform​(TargetConfiguration targetConfiguration,                  DependencyStack dependencyStack)`    

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

        []{#<init>(com.facebook.buck.core.model.platform.PlatformResolver)}

        -   #### RuleBasedTargetPlatformResolver

                public RuleBasedTargetPlatformResolver​(PlatformResolver platformResolver)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getTargetPlatform(com.facebook.buck.core.model.TargetConfiguration,com.facebook.buck.core.exceptions.DependencyStack)}

        -   #### getTargetPlatform

            ``` methodSignature
            public Platform getTargetPlatform​(TargetConfiguration targetConfiguration,
                                              DependencyStack dependencyStack)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getTargetPlatform` in
                interface `TargetPlatformResolver`

            [Returns:]{.returnLabel}
            :   [`Platform`](../../model/platform/Platform.html "interface in com.facebook.buck.core.model.platform")
                for a given
                [`TargetConfiguration`](../../model/TargetConfiguration.html "class in com.facebook.buck.core.model").
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
