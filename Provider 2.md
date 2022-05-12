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
[Package]{.packageLabelInType} [com.facebook.buck.core.rules.providers](package-summary.html)
:::

## Interface Provider\<T extends [ProviderInfo](ProviderInfo.html "interface in com.facebook.buck.core.rules.providers")\<T\>\> {#interface-providert-extends-providerinfot .title title="Interface Provider"}
:::

::: contentContainer
::: description
-   

    All Superinterfaces:
    :   `com.google.devtools.build.lib.skylarkinterface.SkylarkPrintable`,
        `com.google.devtools.build.lib.skylarkinterface.SkylarkValue`

    ```{=html}
    <!-- -->
    ```

    All Known Implementing Classes:
    :   `BuiltInProvider`, `UserDefinedProvider`

    ------------------------------------------------------------------------

        public interface Provider<T extends ProviderInfo<T>>
        extends com.google.devtools.build.lib.skylarkinterface.SkylarkValue

    ::: block
    Declared Provider (a constructor for
    [`ProviderInfo`](ProviderInfo.html "interface in com.facebook.buck.core.rules.providers")).
    [`Provider`](Provider.html "interface in com.facebook.buck.core.rules.providers")
    serves both as \"type identifier\" for declared provider instances
    and as a function that can be called to construct an info of a
    provider. To the Skylark user, there are \"providers\" and
    \"provider infos\"; the former is a Java instance of this class, and
    the latter is a Java instance of
    [`ProviderInfo`](ProviderInfo.html "interface in com.facebook.buck.core.rules.providers").
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Interface             | Description           |
        +=======================+=======================+=======================+
        | `static interface `   | `Provider.Key<T>`     | ::: block             |
        |                       |                       | A serializable unique |
        |                       |                       | identifier of a       |
        |                       |                       | [`Provider`](Provid   |
        |                       |                       | er.html "interface in |
        |                       |                       |  com.facebook.buck.co |
        |                       |                       | re.rules.providers"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `Provider.Key<T>`     | `getKey()`            | ::: block             |
        |                       |                       | Returns a             |
        |                       |                       | serializable          |
        |                       |                       | representation of     |
        |                       |                       | this `Provider`.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `toString()`          | ::: block             |
        |                       |                       | Returns a name of     |
        |                       |                       | this `Provider` that  |
        |                       |                       | should be used in     |
        |                       |                       | error messages.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3 .tableTab}

        -   []{#methods.inherited.from.class.com.google.devtools.build.lib.skylarkinterface.SkylarkPrintable}

            ### Methods inherited from interface com.google.devtools.build.lib.skylarkinterface.SkylarkPrintable

            `debugPrint, repr, str`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.google.devtools.build.lib.skylarkinterface.SkylarkValue}

            ### Methods inherited from interface com.google.devtools.build.lib.skylarkinterface.SkylarkValue

            `isHashable, isImmutable`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getKey()}

        -   #### getKey

            ``` methodSignature
            Provider.Key<T> getKey()
            ```

            ::: block
            Returns a serializable representation of this `Provider`.
            :::

        []{#toString()}

        -   #### toString

            ``` methodSignature
            String toString()
            ```

            ::: block
            Returns a name of this `Provider` that should be used in
            error messages.
            :::

            [Overrides:]{.overrideSpecifyLabel}
            :   `toString` in class `Object`
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
