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
-   [Nested](#nested.class.summary) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.core.rules.providers.collect.impl](package-summary.html)
:::

## Class ProviderInfoCollectionImpl {#class-providerinfocollectionimpl .title title="Class ProviderInfoCollectionImpl"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.rules.providers.collect.impl.ProviderInfoCollectionImpl

::: description
-   

    All Implemented Interfaces:
    :   `ProviderInfoCollection`,
        `com.google.devtools.build.lib.syntax.SkylarkIndexable`,
        `com.google.devtools.build.lib.syntax.SkylarkQueryable`

    ------------------------------------------------------------------------

        public class ProviderInfoCollectionImpl
        extends Object
        implements ProviderInfoCollection

    ::: block
    Implementation of
    [`ProviderInfoCollection`](../ProviderInfoCollection.html "interface in com.facebook.buck.core.rules.providers.collect").
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

          Modifier and Type   Class                                  Description
          ------------------- -------------------------------------- -------------
          `static class `     `ProviderInfoCollectionImpl.Builder`    

          : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Modifier       Constructor                                                                                                               Description
          -------------- ------------------------------------------------------------------------------------------------------------------------- -------------
          `protected `   `ProviderInfoCollectionImpl​(com.google.common.collect.ImmutableMap<Provider.Key<?>,​? extends ProviderInfo<?>> infoMap)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                             Method                                                                                                                                                                       Description
          --------------------------------------------- ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `static ProviderInfoCollectionImpl.Builder`   `builder()`                                                                                                                                                                   
          `static ProviderInfoCollectionImpl.Builder`   `builderWithExpectedSize​(int expectedSize)`                                                                                                                                   
          `<T extends ProviderInfo<T>>boolean`          `contains​(Provider<T> provider)`                                                                                                                                              
          `boolean`                                     `containsKey​(Object key,            com.google.devtools.build.lib.events.Location loc,            com.google.devtools.build.lib.skylarkinterface.StarlarkContext context)`    
          `<T extends ProviderInfo<T>>Optional<T>`      `get​(Provider<T> provider)`                                                                                                                                                   
          `DefaultInfo`                                 `getDefaultInfo()`                                                                                                                                                            
          `Object`                                      `getIndex​(Object key,         com.google.devtools.build.lib.events.Location loc,         com.google.devtools.build.lib.skylarkinterface.StarlarkContext context)`             

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
          Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
          .tableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.google.devtools.build.lib.syntax.SkylarkQueryable}

            ### Methods inherited from interface com.google.devtools.build.lib.syntax.SkylarkQueryable

            `containsKey`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.google.common.collect.ImmutableMap)}

        -   #### ProviderInfoCollectionImpl

                protected ProviderInfoCollectionImpl​(com.google.common.collect.ImmutableMap<Provider.Key<?>,​? extends ProviderInfo<?>> infoMap)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getIndex(java.lang.Object,com.google.devtools.build.lib.events.Location,com.google.devtools.build.lib.skylarkinterface.StarlarkContext)}

        -   #### getIndex

            ``` methodSignature
            public Object getIndex​(Object key,
                                   com.google.devtools.build.lib.events.Location loc,
                                   com.google.devtools.build.lib.skylarkinterface.StarlarkContext context)
                            throws com.google.devtools.build.lib.syntax.EvalException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getIndex` in
                interface `com.google.devtools.build.lib.syntax.SkylarkIndexable`

            [Throws:]{.throwsLabel}
            :   `com.google.devtools.build.lib.syntax.EvalException`

        []{#containsKey(java.lang.Object,com.google.devtools.build.lib.events.Location,com.google.devtools.build.lib.skylarkinterface.StarlarkContext)}

        -   #### containsKey

            ``` methodSignature
            public boolean containsKey​(Object key,
                                       com.google.devtools.build.lib.events.Location loc,
                                       com.google.devtools.build.lib.skylarkinterface.StarlarkContext context)
                                throws com.google.devtools.build.lib.syntax.EvalException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `containsKey` in
                interface `com.google.devtools.build.lib.syntax.SkylarkQueryable`

            [Throws:]{.throwsLabel}
            :   `com.google.devtools.build.lib.syntax.EvalException`

        []{#builder()}

        -   #### builder

            ``` methodSignature
            public static ProviderInfoCollectionImpl.Builder builder()
            ```

        []{#builderWithExpectedSize(int)}

        -   #### builderWithExpectedSize

            ``` methodSignature
            public static ProviderInfoCollectionImpl.Builder builderWithExpectedSize​(int expectedSize)
            ```

        []{#get(com.facebook.buck.core.rules.providers.Provider)}

        -   #### get

            ``` methodSignature
            public <T extends ProviderInfo<T>> Optional<T> get​(Provider<T> provider)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `get` in interface `ProviderInfoCollection`

            [Returns:]{.returnLabel}
            :   the
                [`ProviderInfo`](../../ProviderInfo.html "interface in com.facebook.buck.core.rules.providers")
                of the specific type given the
                [`Provider`](../../Provider.html "interface in com.facebook.buck.core.rules.providers")

        []{#contains(com.facebook.buck.core.rules.providers.Provider)}

        -   #### contains

            ``` methodSignature
            public <T extends ProviderInfo<T>> boolean contains​(Provider<T> provider)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `contains` in interface `ProviderInfoCollection`

            [Returns:]{.returnLabel}
            :   whether collection contains a
                [`ProviderInfo`](../../ProviderInfo.html "interface in com.facebook.buck.core.rules.providers")
                of the specific type given by the
                [`Provider`](../../Provider.html "interface in com.facebook.buck.core.rules.providers")

        []{#getDefaultInfo()}

        -   #### getDefaultInfo

            ``` methodSignature
            public DefaultInfo getDefaultInfo()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getDefaultInfo` in interface `ProviderInfoCollection`

            [Returns:]{.returnLabel}
            :   the
                [`DefaultInfo`](../../lib/DefaultInfo.html "class in com.facebook.buck.core.rules.providers.lib")
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
-   [Nested](#nested.class.summary) \| 
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
