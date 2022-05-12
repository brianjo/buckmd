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
[Package]{.packageLabelInType} [com.facebook.buck.rules.modern](package-summary.html)
:::

## Interface Serializer.Delegate {#interface-serializer.delegate .title title="Interface Serializer.Delegate"}
:::

::: contentContainer
::: description
-   

    Enclosing class:
    :   [Serializer](Serializer.html "class in com.facebook.buck.rules.modern")

    ------------------------------------------------------------------------

        public static interface Serializer.Delegate

    ::: block
    The first time a \"dynamic\" object is encountered (including
    Buildables themselves), registerNewValue will be called. This should
    return a unique HashCode representation (this hashCode will become
    the serialized representation of that object and deserialization
    will depend on a Deserializer.DataProvider to do the reverse lookup
    back to data/children).
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                   Method                                                                                                                                                                       Description
          ----------------------------------- ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `com.google.common.hash.HashCode`   `registerNewValue​(AddsToRuleKey instance,                 byte[] data,                 com.google.common.collect.ImmutableList<com.google.common.hash.HashCode> children)`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Abstract
          Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#registerNewValue(com.facebook.buck.core.rulekey.AddsToRuleKey,byte[],com.google.common.collect.ImmutableList)}

        -   #### registerNewValue

            ``` methodSignature
            com.google.common.hash.HashCode registerNewValue​(AddsToRuleKey instance,
                                                             byte[] data,
                                                             com.google.common.collect.ImmutableList<com.google.common.hash.HashCode> children)
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
