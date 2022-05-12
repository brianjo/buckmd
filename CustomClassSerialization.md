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

## Interface CustomClassSerialization\<T extends [AddsToRuleKey](../../core/rulekey/AddsToRuleKey.html "interface in com.facebook.buck.core.rulekey")\> {#interface-customclassserializationt-extends-addstorulekey .title title="Interface CustomClassSerialization"}
:::

::: contentContainer
::: description
-   

    All Superinterfaces:
    :   `CustomClassBehaviorTag`

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `PythonEnvironment.PythonEnvironmentSerialization`

    ------------------------------------------------------------------------

        public interface CustomClassSerialization<T extends AddsToRuleKey>
        extends CustomClassBehaviorTag

    ::: block
    Allows a class to follow specify its serialization/deserialization
    in terms of calls to the ValueVisitor/ValueCreator.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type             Method                                                         Description
          ----------------------------- -------------------------------------------------------------- -------------
          `<E extends Exception>T`      `deserialize​(ValueCreator<E> deserializer)`                     
          `<E extends Exception>void`   `serialize​(T instance,          ValueVisitor<E> serializer)`    

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

        []{#serialize(com.facebook.buck.core.rulekey.AddsToRuleKey,com.facebook.buck.rules.modern.ValueVisitor)}
        []{#serialize(T,com.facebook.buck.rules.modern.ValueVisitor)}

        -   #### serialize

            ``` methodSignature
            <E extends Exception> void serialize​(T instance,
                                                 ValueVisitor<E> serializer)
                                          throws E extends Exception
            ```

            [Throws:]{.throwsLabel}
            :   `E extends Exception`

        []{#deserialize(com.facebook.buck.rules.modern.ValueCreator)}

        -   #### deserialize

            ``` methodSignature
            <E extends Exception> T deserialize​(ValueCreator<E> deserializer)
                                         throws E extends Exception
            ```

            [Throws:]{.throwsLabel}
            :   `E extends Exception`
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
