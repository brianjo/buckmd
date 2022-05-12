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

## Class BuiltInProviderInfo\<T extends BuiltInProviderInfo\<T\>\> {#class-builtinproviderinfot-extends-builtinproviderinfot .title title="Class BuiltInProviderInfo"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.core.starlark.compatible.BuckStarlarkStructObject](../../../starlark/compatible/BuckStarlarkStructObject.html "class in com.facebook.buck.core.starlark.compatible")

    -   -   com.facebook.buck.core.rules.providers.impl.BuiltInProviderInfo\<T\>

::: description
-   

    [Type Parameters:]{.paramLabel}
    :   `T` - the specific type of the
        [`BuiltInProviderInfo`](BuiltInProviderInfo.html "class in com.facebook.buck.core.rules.providers.impl")

    ```{=html}
    <!-- -->
    ```

    All Implemented Interfaces:
    :   `ProviderInfo<T>`, `SkylarkProviderInfo`,
        `com.google.devtools.build.lib.skylarkinterface.SkylarkPrintable`,
        `com.google.devtools.build.lib.skylarkinterface.SkylarkValue`,
        `com.google.devtools.build.lib.syntax.ClassObject`

    ```{=html}
    <!-- -->
    ```

    Direct Known Subclasses:
    :   `DefaultInfo`, `DotnetLegacyToolchainInfo`,
        `DotnetLibraryProviderInfo`, `RunInfo`, `TestInfo`

    ------------------------------------------------------------------------

        public abstract class BuiltInProviderInfo<T extends BuiltInProviderInfo<T>>
        extends BuckStarlarkStructObject
        implements ProviderInfo<T>

    ::: block
    Represents a
    [`ProviderInfo`](../ProviderInfo.html "interface in com.facebook.buck.core.rules.providers")
    that is defined in Java. The corresponding
    [`Provider`](../Provider.html "interface in com.facebook.buck.core.rules.providers")
    is automatically generated from the this class.
    The specific provider implementation should use the
    [`ImmutableInfo`](../annotations/ImmutableInfo.html "annotation in com.facebook.buck.core.rules.providers.annotations")
    annotation, and be an abstract class that contains only methods that
    act as accessors of the struct. The method name will be equivalent
    to the struct field name. The methods should only return Skylark
    compatible types.

    One additional public static method may be declared, named
    `instantiateFromSkylark`. This method can take skylark compatible
    values, and must return an instance of this
    [`BuiltInProviderInfo`](BuiltInProviderInfo.html "class in com.facebook.buck.core.rules.providers.impl").
    The number of arguments to this method must match the names
    specified in
    [`ImmutableInfo`](../annotations/ImmutableInfo.html "annotation in com.facebook.buck.core.rules.providers.annotations"),
    and is mostly used to convert types, ensure that structures are
    immutable, etc.

    An immutable implementation will be generated for the info.

    The
    [`BuiltInProviderInfo`](BuiltInProviderInfo.html "class in com.facebook.buck.core.rules.providers.impl")
    should have a public static field containing the
    [`BuiltInProvider`](BuiltInProvider.html "class in com.facebook.buck.core.rules.providers.impl")
    for the class. That provider can be created with
    `  BuiltInProvider.of(ImmutableSomeClass.class`.

    TODO(bobyf): support map/list/set types better
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Modifier       Constructor               Description
          -------------- ------------------------- -------------
          `protected `   `BuiltInProviderInfo()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type      Method                 Description
          ---------------------- ---------------------- -------------
          `protected Class<?>`   `getDeclaredClass()`    
          `BuiltInProvider<T>`   `getProvider()`         
          `ProviderInfo<?>`      `getProviderInfo()`     
          `boolean`              `isImmutable()`         

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.core.starlark.compatible.BuckStarlarkStructObject}

            ### Methods inherited from class com.facebook.buck.core.starlark.compatible.[BuckStarlarkStructObject](../../../starlark/compatible/BuckStarlarkStructObject.html "class in com.facebook.buck.core.starlark.compatible")

            `getErrorMessageForUnknownField, getFieldNames, getMethods, getValue, repr`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.google.devtools.build.lib.skylarkinterface.SkylarkPrintable}

            ### Methods inherited from interface com.google.devtools.build.lib.skylarkinterface.SkylarkPrintable

            `debugPrint, repr, str`

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

        []{#<init>()}

        -   #### BuiltInProviderInfo

                protected BuiltInProviderInfo()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getProvider()}

        -   #### getProvider

            ``` methodSignature
            public BuiltInProvider<T> getProvider()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getProvider` in
                interface `ProviderInfo<T extends BuiltInProviderInfo<T>>`

            [Returns:]{.returnLabel}
            :   the
                [`Provider`](../Provider.html "interface in com.facebook.buck.core.rules.providers")
                instance that constructs instances of this info.

        []{#getDeclaredClass()}

        -   #### getDeclaredClass

            ``` methodSignature
            protected Class<?> getDeclaredClass()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getDeclaredClass` in class `BuckStarlarkStructObject`

            [Returns:]{.returnLabel}
            :   the class for which all declared methods on it are
                considered skylark accessible.

        []{#getProviderInfo()}

        -   #### getProviderInfo

            ``` methodSignature
            public ProviderInfo<?> getProviderInfo()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getProviderInfo` in interface `SkylarkProviderInfo`

            [Returns:]{.returnLabel}
            :   The original provider info

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
