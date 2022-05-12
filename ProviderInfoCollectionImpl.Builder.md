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

-   [Overview](../../../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../../index-all.html)
-   [Help](../../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../../allclasses.html)

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
-   [Field](#field.summary) \| 
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.core.rules.providers.collect.impl](package-summary.html)
:::

## Class ProviderInfoCollectionImpl.Builder {#class-providerinfocollectionimpl.builder .title title="Class ProviderInfoCollectionImpl.Builder"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.rules.providers.collect.impl.ProviderInfoCollectionImpl.Builder

::: description
-   

    All Implemented Interfaces:
    :   `ProviderInfoCollection.Builder`

    ```{=html}
    <!-- -->
    ```

    Enclosing class:
    :   [ProviderInfoCollectionImpl](ProviderInfoCollectionImpl.html "class in com.facebook.buck.core.rules.providers.collect.impl")

    ------------------------------------------------------------------------

        public static class ProviderInfoCollectionImpl.Builder
        extends Object
        implements ProviderInfoCollection.Builder
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type                                                                             Field          Description
          --------------------------------------------------------------------------------------------- -------------- -------------
          `protected com.google.common.collect.ImmutableMap.Builder<Provider.Key<?>,​ProviderInfo<?>>`   `mapBuilder`    

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Modifier       Constructor                   Description
          -------------- ----------------------------- -------------
          `protected `   `Builder()`                    
          `protected `   `Builder​(int expectedSize)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `Pr                   | `bui                  | ::: block             |
        | oviderInfoCollection` | ld​(DefaultInfo info)` | Build the             |
        |                       |                       | [`ProviderInfoCo      |
        |                       |                       | llection`](../Provide |
        |                       |                       | rInfoCollection.html  |
        |                       |                       | "interface in com.fac |
        |                       |                       | ebook.buck.core.rules |
        |                       |                       | .providers.collect"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ProviderIn           | `put​(P                | ::: block             |
        | foCollection.Builder` | roviderInfo<?> info)` | Add a new             |
        |                       |                       | [`ProviderI           |
        |                       |                       | nfo`](../../ProviderI |
        |                       |                       | nfo.html "interface i |
        |                       |                       | n com.facebook.buck.c |
        |                       |                       | ore.rules.providers") |
        |                       |                       | to the collection.    |
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
    -   []{#field.detail}

        ### Field Detail

        []{#mapBuilder}

        -   #### mapBuilder

                protected final com.google.common.collect.ImmutableMap.Builder<Provider.Key<?>,​ProviderInfo<?>> mapBuilder
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### Builder

                protected Builder()

        []{#<init>(int)}

        -   #### Builder

                protected Builder​(int expectedSize)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#put(com.facebook.buck.core.rules.providers.ProviderInfo)}

        -   #### put

            ``` methodSignature
            public ProviderInfoCollection.Builder put​(ProviderInfo<?> info)
            ```

            ::: block
            [Description copied from
            interface: `ProviderInfoCollection.Builder`]{.descfrmTypeLabel}
            :::

            ::: block
            Add a new
            [`ProviderInfo`](../../ProviderInfo.html "interface in com.facebook.buck.core.rules.providers")
            to the collection. Multiple
            [`ProviderInfo`](../../ProviderInfo.html "interface in com.facebook.buck.core.rules.providers")
            objects with the same
            [`Provider.Key`](../../Provider.Key.html "interface in com.facebook.buck.core.rules.providers")
            should not be added.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `put` in interface `ProviderInfoCollection.Builder`

        []{#build(com.facebook.buck.core.rules.providers.lib.DefaultInfo)}

        -   #### build

            ``` methodSignature
            public ProviderInfoCollection build​(DefaultInfo info)
            ```

            ::: block
            [Description copied from
            interface: `ProviderInfoCollection.Builder`]{.descfrmTypeLabel}
            :::

            ::: block
            Build the
            [`ProviderInfoCollection`](../ProviderInfoCollection.html "interface in com.facebook.buck.core.rules.providers.collect").
            The
            [`DefaultInfo`](../../lib/DefaultInfo.html "class in com.facebook.buck.core.rules.providers.lib")
            must be specified here.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `build` in interface `ProviderInfoCollection.Builder`
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

-   [Overview](../../../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../../index-all.html)
-   [Help](../../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../../allclasses.html)

<div>

<div>

JavaScript is disabled on your browser.

</div>

</div>

<div>

-   Summary: 
-   Nested \| 
-   [Field](#field.summary) \| 
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
-   [Constr](#constructor.detail) \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
