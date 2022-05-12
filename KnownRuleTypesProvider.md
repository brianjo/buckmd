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
[Package]{.packageLabelInType} [com.facebook.buck.core.rules.knowntypes.provider](package-summary.html)
:::

## Class KnownRuleTypesProvider {#class-knownruletypesprovider .title title="Class KnownRuleTypesProvider"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.rules.knowntypes.provider.KnownRuleTypesProvider

::: description
-   

    ------------------------------------------------------------------------

        public class KnownRuleTypesProvider
        extends Object

    ::: block
    Lazily constructs
    [`KnownRuleTypes`](../KnownRuleTypes.html "interface in com.facebook.buck.core.rules.knowntypes")
    for
    [`Cell`](../../../cell/Cell.html "interface in com.facebook.buck.core.cell")s.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                         Description
          ----------------------------------------------------------------------------------- -------------
          `KnownRuleTypesProvider​(KnownNativeRuleTypesFactory knownNativeRuleTypesFactory)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `KnownRuleTypes`      | `get​(Cell cell)`      | ::: block             |
        |                       |                       | Returns               |
        |                       |                       | [`KnownRuleTy         |
        |                       |                       | pes`](../KnownRuleTyp |
        |                       |                       | es.html "interface in |
        |                       |                       |  com.facebook.buck.co |
        |                       |                       | re.rules.knowntypes") |
        |                       |                       | for a given           |
        |                       |                       | [`Cell`](../..        |
        |                       |                       | /../cell/Cell.html "i |
        |                       |                       | nterface in com.faceb |
        |                       |                       | ook.buck.core.cell"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getNative            | ::: block             |
        | KnownNativeRuleTypes` | RuleTypes​(Cell cell)` | Get details for just  |
        |                       |                       | rules implemented in  |
        |                       |                       | Buck itself, rather   |
        |                       |                       | than user defined     |
        |                       |                       | rules                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Known                | `getUserDefined       | ::: block             |
        | UserDefinedRuleTypes` | RuleTypes​(Cell cell)` | Get details for rules |
        |                       |                       | defined by users in   |
        |                       |                       | extension files       |
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

        []{#<init>(com.facebook.buck.core.rules.knowntypes.KnownNativeRuleTypesFactory)}

        -   #### KnownRuleTypesProvider

                public KnownRuleTypesProvider​(KnownNativeRuleTypesFactory knownNativeRuleTypesFactory)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#get(com.facebook.buck.core.cell.Cell)}

        -   #### get

            ``` methodSignature
            public KnownRuleTypes get​(Cell cell)
            ```

            ::: block
            Returns
            [`KnownRuleTypes`](../KnownRuleTypes.html "interface in com.facebook.buck.core.rules.knowntypes")
            for a given
            [`Cell`](../../../cell/Cell.html "interface in com.facebook.buck.core.cell").
            :::

        []{#getNativeRuleTypes(com.facebook.buck.core.cell.Cell)}

        -   #### getNativeRuleTypes

            ``` methodSignature
            public KnownNativeRuleTypes getNativeRuleTypes​(Cell cell)
            ```

            ::: block
            Get details for just rules implemented in Buck itself,
            rather than user defined rules
            :::

        []{#getUserDefinedRuleTypes(com.facebook.buck.core.cell.Cell)}

        -   #### getUserDefinedRuleTypes

            ``` methodSignature
            public KnownUserDefinedRuleTypes getUserDefinedRuleTypes​(Cell cell)
            ```

            ::: block
            Get details for rules defined by users in extension files
            :::
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
