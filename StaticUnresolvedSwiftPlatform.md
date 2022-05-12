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
[Package]{.packageLabelInType} [com.facebook.buck.swift.toolchain.impl](package-summary.html)
:::

## Class StaticUnresolvedSwiftPlatform {#class-staticunresolvedswiftplatform .title title="Class StaticUnresolvedSwiftPlatform"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.swift.toolchain.impl.StaticUnresolvedSwiftPlatform

::: description
-   

    All Implemented Interfaces:
    :   `FlavorConvertible`, `UnresolvedSwiftPlatform`

    ------------------------------------------------------------------------

        public abstract class StaticUnresolvedSwiftPlatform
        extends Object
        implements UnresolvedSwiftPlatform

    ::: block
    Used to provide a
    [`SwiftPlatform`](../SwiftPlatform.html "interface in com.facebook.buck.swift.toolchain")
    that is fully specified before parsing/configuration (specified in
    .buckconfig, for example).
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                         Description
          ----------------------------------- -------------
          `StaticUnresolvedSwiftPlatform()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `abstract Flavor`     | `getFlavor()`         |                       |
        +-----------------------+-----------------------+-----------------------+
        | `I                    | `getParseTimeDeps     | ::: block             |
        | terable<BuildTarget>` | ​(TargetConfiguration  | Returns the parse     |
        |                       | targetConfiguration)` | time deps of this     |
        |                       |                       | platform.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `abstract Opt         | `getStatical          |                       |
        | ional<SwiftPlatform>` | lyResolvedInstance()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static StaticUnr     | `of​(Optional<? exten  |                       |
        | esolvedSwiftPlatform` | ds SwiftPlatform> sta |                       |
        |                       | ticallyResolvedInstan |                       |
        |                       | ce,   Flavor flavor)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Opt                  | `resolve​(BuildRuleRe  | ::: block             |
        | ional<SwiftPlatform>` | solver ruleResolver)` | Returns the resolved  |
        |                       |                       | \@{link               |
        |                       |                       | NdkCxxPlatform}.      |
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

        -   #### StaticUnresolvedSwiftPlatform

                public StaticUnresolvedSwiftPlatform()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getStaticallyResolvedInstance()}

        -   #### getStaticallyResolvedInstance

            ``` methodSignature
            public abstract Optional<SwiftPlatform> getStaticallyResolvedInstance()
            ```

        []{#getFlavor()}

        -   #### getFlavor

            ``` methodSignature
            public abstract Flavor getFlavor()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getFlavor` in interface `FlavorConvertible`

        []{#getParseTimeDeps(com.facebook.buck.core.model.TargetConfiguration)}

        -   #### getParseTimeDeps

            ``` methodSignature
            public Iterable<BuildTarget> getParseTimeDeps​(TargetConfiguration targetConfiguration)
            ```

            ::: block
            [Description copied from
            interface: `UnresolvedSwiftPlatform`]{.descfrmTypeLabel}
            :::

            ::: block
            Returns the parse time deps of this platform.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getParseTimeDeps` in
                interface `UnresolvedSwiftPlatform`

        []{#resolve(com.facebook.buck.core.rules.BuildRuleResolver)}

        -   #### resolve

            ``` methodSignature
            public Optional<SwiftPlatform> resolve​(BuildRuleResolver ruleResolver)
            ```

            ::: block
            [Description copied from
            interface: `UnresolvedSwiftPlatform`]{.descfrmTypeLabel}
            :::

            ::: block
            Returns the resolved \@{link NdkCxxPlatform}.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `resolve` in interface `UnresolvedSwiftPlatform`

        []{#of(java.util.Optional,com.facebook.buck.core.model.Flavor)}

        -   #### of

            ``` methodSignature
            public static StaticUnresolvedSwiftPlatform of​(Optional<? extends SwiftPlatform> staticallyResolvedInstance,
                                                           Flavor flavor)
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
