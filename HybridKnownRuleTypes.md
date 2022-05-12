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
[Package]{.packageLabelInType} [com.facebook.buck.core.rules.knowntypes](package-summary.html)
:::

## Class HybridKnownRuleTypes {#class-hybridknownruletypes .title title="Class HybridKnownRuleTypes"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.rules.knowntypes.HybridKnownRuleTypes

::: description
-   

    All Implemented Interfaces:
    :   `KnownRuleTypes`

    ------------------------------------------------------------------------

        public class HybridKnownRuleTypes
        extends Object
        implements KnownRuleTypes

    ::: block
    Provides access to rule types and descriptions for both native and
    user defined rules.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                       Description
          ----------------------------------------------------------------------------------------------------------------- -------------
          `HybridKnownRuleTypes​(KnownRuleTypes nativeRuleTypes,                     KnownRuleTypes userDefinedRuleTypes)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `RuleDescriptor<?>`   | `getDescripto         | ::: block             |
        |                       | rByName​(String name)` | Get rule type,        |
        |                       |                       | constructor arg and   |
        |                       |                       | description object    |
        |                       |                       | for by rule name.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.knowntypes.KnownRuleTypes}

            ### Methods inherited from interface com.facebook.buck.core.rules.knowntypes.[KnownRuleTypes](KnownRuleTypes.html "interface in com.facebook.buck.core.rules.knowntypes")

            `getDescriptorByNameChecked`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.core.rules.knowntypes.KnownRuleTypes,com.facebook.buck.core.rules.knowntypes.KnownRuleTypes)}

        -   #### HybridKnownRuleTypes

                public HybridKnownRuleTypes​(KnownRuleTypes nativeRuleTypes,
                                            KnownRuleTypes userDefinedRuleTypes)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getDescriptorByName(java.lang.String)}

        -   #### getDescriptorByName

            ``` methodSignature
            public RuleDescriptor<?> getDescriptorByName​(String name)
            ```

            ::: block
            [Description copied from
            interface: `KnownRuleTypes`]{.descfrmTypeLabel}
            :::

            ::: block
            Get rule type, constructor arg and description object for by
            rule name.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getDescriptorByName` in interface `KnownRuleTypes`
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
