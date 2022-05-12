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

## Interface ClassInfo\<T extends [AddsToRuleKey](../../core/rulekey/AddsToRuleKey.html "interface in com.facebook.buck.core.rulekey")\> {#interface-classinfot-extends-addstorulekey .title title="Interface ClassInfo"}
:::

::: contentContainer
::: description
-   

    All Known Implementing Classes:
    :   `DefaultClassInfo`

    ------------------------------------------------------------------------

        public interface ClassInfo<T extends AddsToRuleKey>

    ::: block
    ClassInfo is used by ModernBuildRule to extract information from an
    AddsToRuleKey instance. It computes various things (rulekeys, deps,
    etc) by iterating over all the fields of the AddsToRuleKey.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `com.google.common.   | `getFieldInfos()`     |                       |
        | collect.ImmutableColl |                       |                       |
        | ection<FieldInfo<?>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<C           | `getSuperInfo()`      |                       |
        | lassInfo<? super T>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getType()`           | ::: block             |
        |                       |                       | Returns a lower       |
        |                       |                       | underscore name for   |
        |                       |                       | this type.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `<E ex                | `vis                  |                       |
        | tends Exception>void` | it​(T value,      Valu |                       |
        |                       | eVisitor<E> visitor)` |                       |
        +-----------------------+-----------------------+-----------------------+

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

        []{#getType()}

        -   #### getType

            ``` methodSignature
            String getType()
            ```

            ::: block
            Returns a lower underscore name for this type.
            :::

        []{#visit(com.facebook.buck.core.rulekey.AddsToRuleKey,com.facebook.buck.rules.modern.ValueVisitor)}
        []{#visit(T,com.facebook.buck.rules.modern.ValueVisitor)}

        -   #### visit

            ``` methodSignature
            <E extends Exception> void visit​(T value,
                                             ValueVisitor<E> visitor)
                                      throws E extends Exception
            ```

            [Throws:]{.throwsLabel}
            :   `E extends Exception`

        []{#getSuperInfo()}

        -   #### getSuperInfo

            ``` methodSignature
            Optional<ClassInfo<? super T>> getSuperInfo()
            ```

        []{#getFieldInfos()}

        -   #### getFieldInfos

            ``` methodSignature
            com.google.common.collect.ImmutableCollection<FieldInfo<?>> getFieldInfos()
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
