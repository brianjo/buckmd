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
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   Constr \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.features.rust](package-summary.html)
:::

## Class ConfigBasedUnresolvedRustPlatform {#class-configbasedunresolvedrustplatform .title title="Class ConfigBasedUnresolvedRustPlatform"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.features.rust.ConfigBasedUnresolvedRustPlatform

::: description
-   

    All Implemented Interfaces:
    :   `FlavorConvertible`, `UnresolvedRustPlatform`

    ------------------------------------------------------------------------

        public class ConfigBasedUnresolvedRustPlatform
        extends Object
        implements UnresolvedRustPlatform

    ::: block
    An
    [`UnresolvedRustPlatform`](UnresolvedRustPlatform.html "interface in com.facebook.buck.features.rust")
    based on .buckconfig values.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `Flavor`              | `getFlavor()`         |                       |
        +-----------------------+-----------------------+-----------------------+
        | `I                    | `getParseTimeDeps     | ::: block             |
        | terable<BuildTarget>` | ​(TargetConfiguration  | Returns the           |
        |                       | targetConfiguration)` | parse-time deps       |
        |                       |                       | required for this     |
        |                       |                       | platform.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com                  | `                     | ::: block             |
        | .facebook.buck.featur | resolve​(BuildRuleReso | Resolves the          |
        | es.rust.RustPlatform` | lver resolver,        | platform.             |
        |                       |  TargetConfiguration  | :::                   |
        |                       | targetConfiguration)` |                       |
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
    -   []{#method.detail}

        ### Method Detail

        []{#resolve(com.facebook.buck.core.rules.BuildRuleResolver,com.facebook.buck.core.model.TargetConfiguration)}

        -   #### resolve

            ``` methodSignature
            public com.facebook.buck.features.rust.RustPlatform resolve​(BuildRuleResolver resolver,
                                                                        TargetConfiguration targetConfiguration)
            ```

            ::: block
            [Description copied from
            interface: `UnresolvedRustPlatform`]{.descfrmTypeLabel}
            :::

            ::: block
            Resolves the platform.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `resolve` in interface `UnresolvedRustPlatform`

        []{#getFlavor()}

        -   #### getFlavor

            ``` methodSignature
            public Flavor getFlavor()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getFlavor` in interface `FlavorConvertible`

            [Specified by:]{.overrideSpecifyLabel}
            :   `getFlavor` in interface `UnresolvedRustPlatform`

        []{#getParseTimeDeps(com.facebook.buck.core.model.TargetConfiguration)}

        -   #### getParseTimeDeps

            ``` methodSignature
            public Iterable<BuildTarget> getParseTimeDeps​(TargetConfiguration targetConfiguration)
            ```

            ::: block
            [Description copied from
            interface: `UnresolvedRustPlatform`]{.descfrmTypeLabel}
            :::

            ::: block
            Returns the parse-time deps required for this platform.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getParseTimeDeps` in interface `UnresolvedRustPlatform`
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
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   Constr \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
