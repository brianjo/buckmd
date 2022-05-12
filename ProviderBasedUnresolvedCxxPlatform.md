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
[Package]{.packageLabelInType} [com.facebook.buck.cxx.toolchain](package-summary.html)
:::

## Class ProviderBasedUnresolvedCxxPlatform {#class-providerbasedunresolvedcxxplatform .title title="Class ProviderBasedUnresolvedCxxPlatform"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.cxx.toolchain.ProviderBasedUnresolvedCxxPlatform

::: description
-   

    All Implemented Interfaces:
    :   `FlavorConvertible`, `ProviderBackedCxxPlatform`,
        `UnresolvedCxxPlatform`

    ------------------------------------------------------------------------

        public class ProviderBasedUnresolvedCxxPlatform
        extends Object
        implements UnresolvedCxxPlatform, ProviderBackedCxxPlatform

    ::: block
    Used to provide a
    [`CxxPlatform`](CxxPlatform.html "interface in com.facebook.buck.cxx.toolchain")
    that is specified as a cxx_toolchain build target.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                              Description
          ---------------------------------------------------------------------------------------------------------------------------------------- -------------
          `ProviderBasedUnresolvedCxxPlatform​(UnconfiguredBuildTarget unconfiguredBuildTarget,                                   Flavor flavor)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `Flavor`              | `getFlavor()`         |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Iterable<?           | `g                    | ::: block             |
        | extends BuildTarget>` | etLinkerParseTimeDeps | This probably         |
        |                       | ​(TargetConfiguration  | shouldn\'t exist.     |
        |                       | targetConfiguration)` | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `I                    | `getParseTimeDeps     | ::: block             |
        | terable<BuildTarget>` | ​(TargetConfiguration  | Returns the           |
        |                       | targetConfiguration)` | parse-time deps       |
        |                       |                       | required for this     |
        |                       |                       | platform.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxPlatform`         | `                     | ::: block             |
        |                       | resolve​(BuildRuleReso | Resolves the          |
        |                       | lver resolver,        | platform.             |
        |                       |  TargetConfiguration  | :::                   |
        |                       | targetConfiguration)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `U                    | `withFlavo            | ::: block             |
        | nresolvedCxxPlatform` | r​(Flavor hostFlavor)` | Returns this provider |
        |                       |                       | as a different        |
        |                       |                       | flavor.               |
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

        []{#<init>(com.facebook.buck.core.model.UnconfiguredBuildTarget,com.facebook.buck.core.model.Flavor)}

        -   #### ProviderBasedUnresolvedCxxPlatform

                public ProviderBasedUnresolvedCxxPlatform​(UnconfiguredBuildTarget unconfiguredBuildTarget,
                                                          Flavor flavor)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#resolve(com.facebook.buck.core.rules.BuildRuleResolver,com.facebook.buck.core.model.TargetConfiguration)}

        -   #### resolve

            ``` methodSignature
            public CxxPlatform resolve​(BuildRuleResolver resolver,
                                       TargetConfiguration targetConfiguration)
            ```

            ::: block
            [Description copied from
            interface: `UnresolvedCxxPlatform`]{.descfrmTypeLabel}
            :::

            ::: block
            Resolves the platform.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `resolve` in interface `UnresolvedCxxPlatform`

        []{#getFlavor()}

        -   #### getFlavor

            ``` methodSignature
            public Flavor getFlavor()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getFlavor` in interface `FlavorConvertible`

            [Specified by:]{.overrideSpecifyLabel}
            :   `getFlavor` in interface `UnresolvedCxxPlatform`

        []{#withFlavor(com.facebook.buck.core.model.Flavor)}

        -   #### withFlavor

            ``` methodSignature
            public UnresolvedCxxPlatform withFlavor​(Flavor hostFlavor)
            ```

            ::: block
            [Description copied from
            interface: `UnresolvedCxxPlatform`]{.descfrmTypeLabel}
            :::

            ::: block
            Returns this provider as a different flavor. This might only
            make sense for .buckconfig-configured cxx platforms and be
            removed in the future.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `withFlavor` in interface `UnresolvedCxxPlatform`

        []{#getParseTimeDeps(com.facebook.buck.core.model.TargetConfiguration)}

        -   #### getParseTimeDeps

            ``` methodSignature
            public Iterable<BuildTarget> getParseTimeDeps​(TargetConfiguration targetConfiguration)
            ```

            ::: block
            [Description copied from
            interface: `UnresolvedCxxPlatform`]{.descfrmTypeLabel}
            :::

            ::: block
            Returns the parse-time deps required for this platform.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getParseTimeDeps` in interface `UnresolvedCxxPlatform`

        []{#getLinkerParseTimeDeps(com.facebook.buck.core.model.TargetConfiguration)}

        -   #### getLinkerParseTimeDeps

            ``` methodSignature
            public Iterable<? extends BuildTarget> getLinkerParseTimeDeps​(TargetConfiguration targetConfiguration)
            ```

            ::: block
            [Description copied from
            interface: `UnresolvedCxxPlatform`]{.descfrmTypeLabel}
            :::

            ::: block
            This probably shouldn\'t exist. Users probably shouldn\'t be
            able to specify specific individual pieces of the platform
            that they want to use. If you\'re tempted to use this, use
            getParseTimeDeps() instead or update this comment with your
            valid use case.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getLinkerParseTimeDeps` in
                interface `UnresolvedCxxPlatform`
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
