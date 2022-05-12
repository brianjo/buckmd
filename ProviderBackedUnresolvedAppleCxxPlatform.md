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
[Package]{.packageLabelInType} [com.facebook.buck.apple.toolchain.impl](package-summary.html)
:::

## Class ProviderBackedUnresolvedAppleCxxPlatform {#class-providerbackedunresolvedapplecxxplatform .title title="Class ProviderBackedUnresolvedAppleCxxPlatform"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.apple.toolchain.impl.ProviderBackedUnresolvedAppleCxxPlatform

::: description
-   

    All Implemented Interfaces:
    :   `UnresolvedAppleCxxPlatform`, `FlavorConvertible`

    ------------------------------------------------------------------------

        public class ProviderBackedUnresolvedAppleCxxPlatform
        extends Object
        implements UnresolvedAppleCxxPlatform

    ::: block
    Used to provide a
    [`AppleCxxPlatform`](../AppleCxxPlatform.html "class in com.facebook.buck.apple.toolchain")
    that is specified as a apple_toolchain_set build target.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                         Description
          ----------------------------------------------------------------------------------------------------------------------------------- -------------
          `ProviderBackedUnresolvedAppleCxxPlatform​(BuildTarget toolchainSetTarget,                                         Flavor flavor)`    

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
        | `I                    | `getParseTimeDeps     | ::: block             |
        | terable<BuildTarget>` | ​(TargetConfiguration  | Returns the parse     |
        |                       | targetConfiguration)` | time deps of this     |
        |                       |                       | platform.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `U                    | `getUnr               | ::: block             |
        | nresolvedCxxPlatform` | esolvedCxxPlatform()` | Returns the \@{link   |
        |                       |                       | U                     |
        |                       |                       | nresolvedCxxPlatform} |
        |                       |                       | corresponding to the  |
        |                       |                       | resolved              |
        |                       |                       | [`AppleCxx            |
        |                       |                       | Platform`](../AppleCx |
        |                       |                       | xPlatform.html "class |
        |                       |                       |  in com.facebook.buck |
        |                       |                       | .apple.toolchain")\'s |
        |                       |                       | [`CxxPlatform`](../.  |
        |                       |                       | ./../cxx/toolchain/Cx |
        |                       |                       | xPlatform.html "inter |
        |                       |                       | face in com.facebook. |
        |                       |                       | buck.cxx.toolchain"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Unr                  | `getUnres             | ::: block             |
        | esolvedSwiftPlatform` | olvedSwiftPlatform()` | Returns the \@{link   |
        |                       |                       | Unr                   |
        |                       |                       | esolvedSwiftPlatform} |
        |                       |                       | corresponding to the  |
        |                       |                       | resolved              |
        |                       |                       | [`AppleCxx            |
        |                       |                       | Platform`](../AppleCx |
        |                       |                       | xPlatform.html "class |
        |                       |                       |  in com.facebook.buck |
        |                       |                       | .apple.toolchain")\'s |
        |                       |                       | [`CxxPlatform`](../.  |
        |                       |                       | ./../cxx/toolchain/Cx |
        |                       |                       | xPlatform.html "inter |
        |                       |                       | face in com.facebook. |
        |                       |                       | buck.cxx.toolchain"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleCxxPlatform`    | `resolve​(BuildRuleRe  | ::: block             |
        |                       | solver ruleResolver)` | Returns the resolved  |
        |                       |                       | \@{link               |
        |                       |                       | AppleCxxPlatform}.    |
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

        []{#<init>(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.model.Flavor)}

        -   #### ProviderBackedUnresolvedAppleCxxPlatform

                public ProviderBackedUnresolvedAppleCxxPlatform​(BuildTarget toolchainSetTarget,
                                                                Flavor flavor)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getParseTimeDeps(com.facebook.buck.core.model.TargetConfiguration)}

        -   #### getParseTimeDeps

            ``` methodSignature
            public Iterable<BuildTarget> getParseTimeDeps​(TargetConfiguration targetConfiguration)
            ```

            ::: block
            [Description copied from
            interface: `UnresolvedAppleCxxPlatform`]{.descfrmTypeLabel}
            :::

            ::: block
            Returns the parse time deps of this platform.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getParseTimeDeps` in
                interface `UnresolvedAppleCxxPlatform`

        []{#resolve(com.facebook.buck.core.rules.BuildRuleResolver)}

        -   #### resolve

            ``` methodSignature
            public AppleCxxPlatform resolve​(BuildRuleResolver ruleResolver)
            ```

            ::: block
            [Description copied from
            interface: `UnresolvedAppleCxxPlatform`]{.descfrmTypeLabel}
            :::

            ::: block
            Returns the resolved \@{link AppleCxxPlatform}.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `resolve` in interface `UnresolvedAppleCxxPlatform`

        []{#getUnresolvedCxxPlatform()}

        -   #### getUnresolvedCxxPlatform

            ``` methodSignature
            public UnresolvedCxxPlatform getUnresolvedCxxPlatform()
            ```

            ::: block
            [Description copied from
            interface: `UnresolvedAppleCxxPlatform`]{.descfrmTypeLabel}
            :::

            ::: block
            Returns the \@{link UnresolvedCxxPlatform} corresponding to
            the resolved
            [`AppleCxxPlatform`](../AppleCxxPlatform.html "class in com.facebook.buck.apple.toolchain")\'s
            [`CxxPlatform`](../../../cxx/toolchain/CxxPlatform.html "interface in com.facebook.buck.cxx.toolchain").
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getUnresolvedCxxPlatform` in
                interface `UnresolvedAppleCxxPlatform`

        []{#getUnresolvedSwiftPlatform()}

        -   #### getUnresolvedSwiftPlatform

            ``` methodSignature
            public UnresolvedSwiftPlatform getUnresolvedSwiftPlatform()
            ```

            ::: block
            [Description copied from
            interface: `UnresolvedAppleCxxPlatform`]{.descfrmTypeLabel}
            :::

            ::: block
            Returns the \@{link UnresolvedSwiftPlatform} corresponding
            to the resolved
            [`AppleCxxPlatform`](../AppleCxxPlatform.html "class in com.facebook.buck.apple.toolchain")\'s
            [`CxxPlatform`](../../../cxx/toolchain/CxxPlatform.html "interface in com.facebook.buck.cxx.toolchain").
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getUnresolvedSwiftPlatform` in
                interface `UnresolvedAppleCxxPlatform`

        []{#getFlavor()}

        -   #### getFlavor

            ``` methodSignature
            public Flavor getFlavor()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getFlavor` in interface `FlavorConvertible`
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
