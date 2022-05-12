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
-   [Nested](#nested.class.summary) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.core.rules.providers.collect](package-summary.html)
:::

## Interface ProviderInfoCollection {#interface-providerinfocollection .title title="Interface ProviderInfoCollection"}
:::

::: contentContainer
::: description
-   

    All Superinterfaces:
    :   `com.google.devtools.build.lib.syntax.SkylarkIndexable`,
        `com.google.devtools.build.lib.syntax.SkylarkQueryable`

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `LegacyProviderInfoCollectionImpl`, `ProviderInfoCollectionImpl`

    ------------------------------------------------------------------------

        public interface ProviderInfoCollection
        extends com.google.devtools.build.lib.syntax.SkylarkIndexable

    ::: block
    Represents a collection of
    [`Provider`](../Provider.html "interface in com.facebook.buck.core.rules.providers")s
    and their corresponding
    [`ProviderInfo`](../ProviderInfo.html "interface in com.facebook.buck.core.rules.providers").
    This is a mapping of the
    [`Provider`](../Provider.html "interface in com.facebook.buck.core.rules.providers")
    via the
    [`Provider.Key`](../Provider.Key.html "interface in com.facebook.buck.core.rules.providers")
    to the corresponding
    [`ProviderInfo`](../ProviderInfo.html "interface in com.facebook.buck.core.rules.providers")
    information that the
    [`Provider`](../Provider.html "interface in com.facebook.buck.core.rules.providers")
    propagates.

    This is `SkylarkIndexable`, so that this can be used to access
    individual provider information from within skylark extension rule
    implementations.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type     Interface                          Description
          --------------------- ---------------------------------- -------------
          `static interface `   `ProviderInfoCollection.Builder`    

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                          Method                             Description
          ------------------------------------------ ---------------------------------- -------------
          `<T extends ProviderInfo<T>>boolean`       `contains​(Provider<T> provider)`    
          `<T extends ProviderInfo<T>>Optional<T>`   `get​(Provider<T> provider)`         
          `DefaultInfo`                              `getDefaultInfo()`                  

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Abstract
          Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}

        -   []{#methods.inherited.from.class.com.google.devtools.build.lib.syntax.SkylarkIndexable}

            ### Methods inherited from interface com.google.devtools.build.lib.syntax.SkylarkIndexable

            `getIndex`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.google.devtools.build.lib.syntax.SkylarkQueryable}

            ### Methods inherited from interface com.google.devtools.build.lib.syntax.SkylarkQueryable

            `containsKey, containsKey`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#get(com.facebook.buck.core.rules.providers.Provider)}

        -   #### get

            ``` methodSignature
            <T extends ProviderInfo<T>> Optional<T> get​(Provider<T> provider)
            ```

            [Returns:]{.returnLabel}
            :   the
                [`ProviderInfo`](../ProviderInfo.html "interface in com.facebook.buck.core.rules.providers")
                of the specific type given the
                [`Provider`](../Provider.html "interface in com.facebook.buck.core.rules.providers")

        []{#contains(com.facebook.buck.core.rules.providers.Provider)}

        -   #### contains

            ``` methodSignature
            <T extends ProviderInfo<T>> boolean contains​(Provider<T> provider)
            ```

            [Returns:]{.returnLabel}
            :   whether collection contains a
                [`ProviderInfo`](../ProviderInfo.html "interface in com.facebook.buck.core.rules.providers")
                of the specific type given by the
                [`Provider`](../Provider.html "interface in com.facebook.buck.core.rules.providers")

        []{#getDefaultInfo()}

        -   #### getDefaultInfo

            ``` methodSignature
            DefaultInfo getDefaultInfo()
            ```

            [Returns:]{.returnLabel}
            :   the
                [`DefaultInfo`](../lib/DefaultInfo.html "class in com.facebook.buck.core.rules.providers.lib")
                contained in this collection
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
-   [Nested](#nested.class.summary) \| 
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
