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
[Package]{.packageLabelInType} [com.facebook.buck.android.toolchain.ndk.impl](package-summary.html)
:::

## Class ProviderBackedUnresolvedNdkCxxPlatform {#class-providerbackedunresolvedndkcxxplatform .title title="Class ProviderBackedUnresolvedNdkCxxPlatform"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.android.toolchain.ndk.impl.ProviderBackedUnresolvedNdkCxxPlatform

::: description
-   

    All Implemented Interfaces:
    :   `UnresolvedNdkCxxPlatform`, `ProviderBackedCxxPlatform`

    ------------------------------------------------------------------------

        public class ProviderBackedUnresolvedNdkCxxPlatform
        extends Object
        implements ProviderBackedCxxPlatform, UnresolvedNdkCxxPlatform

    ::: block
    Used to provide a
    [`NdkCxxPlatform`](../NdkCxxPlatform.html "interface in com.facebook.buck.android.toolchain.ndk")
    that is specified as a ndk_toolchain build target.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                              Description
          ------------------------------------------------------------------------------------------------------------------------ -------------
          `ProviderBackedUnresolvedNdkCxxPlatform​(BuildTarget buildTarget,                                       Flavor flavor)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `U                    | `getCxxPlatform()`    | ::: block             |
        | nresolvedCxxPlatform` |                       | Returns the \@{link   |
        |                       |                       | U                     |
        |                       |                       | nresolvedCxxPlatform} |
        |                       |                       | corresponding to the  |
        |                       |                       | resolved              |
        |                       |                       | [`NdkCxxPlatform      |
        |                       |                       | `](../NdkCxxPlatform. |
        |                       |                       | html "interface in co |
        |                       |                       | m.facebook.buck.andro |
        |                       |                       | id.toolchain.ndk")\'s |
        |                       |                       | [`                    |
        |                       |                       | CxxPlatform`](../../. |
        |                       |                       | ./../cxx/toolchain/Cx |
        |                       |                       | xPlatform.html "inter |
        |                       |                       | face in com.facebook. |
        |                       |                       | buck.cxx.toolchain"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `I                    | `getParseTimeDeps     | ::: block             |
        | terable<BuildTarget>` | ​(TargetConfiguration  | Returns the parse     |
        |                       | targetConfiguration)` | time deps of this     |
        |                       |                       | platform.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `NdkCxxPlatform`      | `resolve​(BuildRuleRe  | ::: block             |
        |                       | solver ruleResolver)` | Returns the resolved  |
        |                       |                       | \@{link               |
        |                       |                       | NdkCxxPlatform}.      |
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

        -   #### ProviderBackedUnresolvedNdkCxxPlatform

                public ProviderBackedUnresolvedNdkCxxPlatform​(BuildTarget buildTarget,
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
            interface: `UnresolvedNdkCxxPlatform`]{.descfrmTypeLabel}
            :::

            ::: block
            Returns the parse time deps of this platform.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getParseTimeDeps` in
                interface `UnresolvedNdkCxxPlatform`

        []{#resolve(com.facebook.buck.core.rules.BuildRuleResolver)}

        -   #### resolve

            ``` methodSignature
            public NdkCxxPlatform resolve​(BuildRuleResolver ruleResolver)
            ```

            ::: block
            [Description copied from
            interface: `UnresolvedNdkCxxPlatform`]{.descfrmTypeLabel}
            :::

            ::: block
            Returns the resolved \@{link NdkCxxPlatform}.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `resolve` in interface `UnresolvedNdkCxxPlatform`

        []{#getCxxPlatform()}

        -   #### getCxxPlatform

            ``` methodSignature
            public UnresolvedCxxPlatform getCxxPlatform()
            ```

            ::: block
            [Description copied from
            interface: `UnresolvedNdkCxxPlatform`]{.descfrmTypeLabel}
            :::

            ::: block
            Returns the \@{link UnresolvedCxxPlatform} corresponding to
            the resolved
            [`NdkCxxPlatform`](../NdkCxxPlatform.html "interface in com.facebook.buck.android.toolchain.ndk")\'s
            [`CxxPlatform`](../../../../cxx/toolchain/CxxPlatform.html "interface in com.facebook.buck.cxx.toolchain").
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getCxxPlatform` in interface `UnresolvedNdkCxxPlatform`
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
