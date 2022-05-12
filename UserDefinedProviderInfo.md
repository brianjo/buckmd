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
[Package]{.packageLabelInType} [com.facebook.buck.core.rules.providers.impl](package-summary.html)
:::

## Class UserDefinedProviderInfo {#class-userdefinedproviderinfo .title title="Class UserDefinedProviderInfo"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.rules.providers.impl.UserDefinedProviderInfo

::: description
-   

    All Implemented Interfaces:
    :   `ProviderInfo<UserDefinedProviderInfo>`, `SkylarkProviderInfo`,
        `com.google.devtools.build.lib.skylarkinterface.SkylarkPrintable`,
        `com.google.devtools.build.lib.skylarkinterface.SkylarkValue`,
        `com.google.devtools.build.lib.syntax.ClassObject`

    ------------------------------------------------------------------------

        public class UserDefinedProviderInfo
        extends Object
        implements ProviderInfo<UserDefinedProviderInfo>, com.google.devtools.build.lib.skylarkinterface.SkylarkValue, com.google.devtools.build.lib.syntax.ClassObject

    ::: block
    [`ProviderInfo`](../ProviderInfo.html "interface in com.facebook.buck.core.rules.providers")
    that is created by a
    [`Provider`](../Provider.html "interface in com.facebook.buck.core.rules.providers")
    that is defined at runtime by a user. e.g.
    `FooInfo = provider(fields=["foo"]); info = FooInfo(foo="bar")` in a
    build file
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

        +-----------------------------------+-----------------------------------+
        | Constructor                       | Description                       |
        +===================================+===================================+
        | `UserDefinedProviderInfo​(Pr       | ::: block                         |
        | ovider<UserDefinedProviderInfo> p | Create an instance of             |
        | rovider,                        c | [`UserDefined                     |
        | om.google.common.collect.Immutabl | ProviderInfo`](UserDefinedProvide |
        | eMap<String,​Object> fieldValues)` | rInfo.html "class in com.facebook |
        |                                   | .buck.core.rules.providers.impl") |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+

        : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                         Method                                                                          Description
          --------------------------------------------------------- ------------------------------------------------------------------------------- -------------
          `String`                                                  `getErrorMessageForUnknownField​(String field)`                                   
          `com.google.common.collect.ImmutableCollection<String>`   `getFieldNames()`                                                                
          `Provider<UserDefinedProviderInfo>`                       `getProvider()`                                                                  
          `ProviderInfo<?>`                                         `getProviderInfo()`                                                              
          `Object`                                                  `getValue​(String name)`                                                          
          `boolean`                                                 `isImmutable()`                                                                  
          `void`                                                    `repr​(com.google.devtools.build.lib.skylarkinterface.SkylarkPrinter printer)`    

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
        -   []{#methods.inherited.from.class.com.google.devtools.build.lib.skylarkinterface.SkylarkPrintable}

            ### Methods inherited from interface com.google.devtools.build.lib.skylarkinterface.SkylarkPrintable

            `debugPrint, str`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.google.devtools.build.lib.skylarkinterface.SkylarkValue}

            ### Methods inherited from interface com.google.devtools.build.lib.skylarkinterface.SkylarkValue

            `isHashable`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.core.rules.providers.Provider,com.google.common.collect.ImmutableMap)}

        -   #### UserDefinedProviderInfo

                public UserDefinedProviderInfo​(Provider<UserDefinedProviderInfo> provider,
                                               com.google.common.collect.ImmutableMap<String,​Object> fieldValues)

            ::: block
            Create an instance of
            [`UserDefinedProviderInfo`](UserDefinedProviderInfo.html "class in com.facebook.buck.core.rules.providers.impl")
            :::

            [Parameters:]{.paramLabel}
            :   `provider` - The provider that created this
                [`UserDefinedProviderInfo`](UserDefinedProviderInfo.html "class in com.facebook.buck.core.rules.providers.impl")
                object
            :   `fieldValues` - A mapping of field names to their
                values. Note that the names must be valid skylark
                identifiers as they are accessed via
                `info_instance.<field>`. The values must be valid when
                used in the Skylark interpreter. That is, either
                primitives, or instances of `SkylarkValue`
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getProvider()}

        -   #### getProvider

            ``` methodSignature
            public Provider<UserDefinedProviderInfo> getProvider()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getProvider` in
                interface `ProviderInfo<UserDefinedProviderInfo>`

            [Returns:]{.returnLabel}
            :   the
                [`Provider`](../Provider.html "interface in com.facebook.buck.core.rules.providers")
                instance that constructs instances of this info.

        []{#getProviderInfo()}

        -   #### getProviderInfo

            ``` methodSignature
            public ProviderInfo<?> getProviderInfo()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getProviderInfo` in interface `SkylarkProviderInfo`

            [Returns:]{.returnLabel}
            :   The original provider info

        []{#repr(com.google.devtools.build.lib.skylarkinterface.SkylarkPrinter)}

        -   #### repr

            ``` methodSignature
            public void repr​(com.google.devtools.build.lib.skylarkinterface.SkylarkPrinter printer)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `repr` in
                interface `com.google.devtools.build.lib.skylarkinterface.SkylarkPrintable`

        []{#getValue(java.lang.String)}

        -   #### getValue

            ``` methodSignature
            @Nullable
            public Object getValue​(String name)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getValue` in
                interface `com.google.devtools.build.lib.syntax.ClassObject`

        []{#getFieldNames()}

        -   #### getFieldNames

            ``` methodSignature
            public com.google.common.collect.ImmutableCollection<String> getFieldNames()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getFieldNames` in
                interface `com.google.devtools.build.lib.syntax.ClassObject`

        []{#getErrorMessageForUnknownField(java.lang.String)}

        -   #### getErrorMessageForUnknownField

            ``` methodSignature
            @Nullable
            public String getErrorMessageForUnknownField​(String field)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getErrorMessageForUnknownField` in
                interface `com.google.devtools.build.lib.syntax.ClassObject`

        []{#isImmutable()}

        -   #### isImmutable

            ``` methodSignature
            public boolean isImmutable()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `isImmutable` in
                interface `com.google.devtools.build.lib.skylarkinterface.SkylarkValue`
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
