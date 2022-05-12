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
-   [Field](#field.summary) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.features.dotnet](package-summary.html)
:::

## Class ImmutableDotnetLibraryProviderInfo {#class-immutabledotnetlibraryproviderinfo .title title="Class ImmutableDotnetLibraryProviderInfo"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.core.starlark.compatible.BuckStarlarkStructObject](../../core/starlark/compatible/BuckStarlarkStructObject.html "class in com.facebook.buck.core.starlark.compatible")

    -   -   [com.facebook.buck.core.rules.providers.impl.BuiltInProviderInfo](../../core/rules/providers/impl/BuiltInProviderInfo.html "class in com.facebook.buck.core.rules.providers.impl")\<[DotnetLibraryProviderInfo](DotnetLibraryProviderInfo.html "class in com.facebook.buck.features.dotnet")\>

        -   -   [com.facebook.buck.features.dotnet.DotnetLibraryProviderInfo](DotnetLibraryProviderInfo.html "class in com.facebook.buck.features.dotnet")

            -   -   com.facebook.buck.features.dotnet.ImmutableDotnetLibraryProviderInfo

::: description
-   

    All Implemented Interfaces:
    :   `ProviderInfo<DotnetLibraryProviderInfo>`,
        `SkylarkProviderInfo`,
        `com.google.devtools.build.lib.skylarkinterface.SkylarkPrintable`,
        `com.google.devtools.build.lib.skylarkinterface.SkylarkValue`,
        `com.google.devtools.build.lib.syntax.ClassObject`

    ------------------------------------------------------------------------

        @ParametersAreNonnullByDefault
        @Generated("org.immutables.processor.ProxyProcessor")
        @Immutable
        @CheckReturnValue
        public final class ImmutableDotnetLibraryProviderInfo
        extends DotnetLibraryProviderInfo

    ::: block
    Immutable implementation of
    [`DotnetLibraryProviderInfo`](DotnetLibraryProviderInfo.html "class in com.facebook.buck.features.dotnet").
    Use the static factory method to create immutable instances:
    `new ImmutableDotnetLibraryProviderInfo()`.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        -   []{#fields.inherited.from.class.com.facebook.buck.features.dotnet.DotnetLibraryProviderInfo}

            ### Fields inherited from class com.facebook.buck.features.dotnet.[DotnetLibraryProviderInfo](DotnetLibraryProviderInfo.html "class in com.facebook.buck.features.dotnet")

            `PROVIDER`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

        +-----------------------------------+-----------------------------------+
        | Constructor                       | Description                       |
        +===================================+===================================+
        | `ImmutableDotnetL                 | ::: block                         |
        | ibraryProviderInfo​(Artifact dll)` | Construct a new immutable         |
        |                                   | `DotnetLibraryProviderInfo`       |
        |                                   | instance.                         |
        |                                   | :::                               |
        +-----------------------------------+-----------------------------------+

        : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `Artifact`            | `dll()`               |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `eq                   | ::: block             |
        |                       | uals​(Object another)` | This instance is      |
        |                       |                       | equal to all          |
        |                       |                       | instances of          |
        |                       |                       | `ImmutableDotne       |
        |                       |                       | tLibraryProviderInfo` |
        |                       |                       | that have equal       |
        |                       |                       | attribute values.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `hashCode()`          | ::: block             |
        |                       |                       | Computes a hash code  |
        |                       |                       | from attributes:      |
        |                       |                       | `dll`.                |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `toString()`          | ::: block             |
        |                       |                       | Prints the immutable  |
        |                       |                       | value                 |
        |                       |                       | `Dotne                |
        |                       |                       | tLibraryProviderInfo` |
        |                       |                       | with attribute        |
        |                       |                       | values.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.providers.impl.BuiltInProviderInfo}

            ### Methods inherited from class com.facebook.buck.core.rules.providers.impl.[BuiltInProviderInfo](../../core/rules/providers/impl/BuiltInProviderInfo.html "class in com.facebook.buck.core.rules.providers.impl")

            `getDeclaredClass, getProvider, getProviderInfo, isImmutable`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.starlark.compatible.BuckStarlarkStructObject}

            ### Methods inherited from class com.facebook.buck.core.starlark.compatible.[BuckStarlarkStructObject](../../core/starlark/compatible/BuckStarlarkStructObject.html "class in com.facebook.buck.core.starlark.compatible")

            `getErrorMessageForUnknownField, getFieldNames, getMethods, getValue, repr`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, finalize, getClass, notify, notifyAll, wait, wait, wait`

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

        []{#<init>(com.facebook.buck.core.artifact.Artifact)}

        -   #### ImmutableDotnetLibraryProviderInfo

                public ImmutableDotnetLibraryProviderInfo​(Artifact dll)

            ::: block
            Construct a new immutable `DotnetLibraryProviderInfo`
            instance.
            :::

            [Parameters:]{.paramLabel}
            :   `dll` - The value for the `dll` attribute
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#dll()}

        -   #### dll

            ``` methodSignature
            public Artifact dll()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `dll` in class `DotnetLibraryProviderInfo`

            [Returns:]{.returnLabel}
            :   The value of the `dll` attribute

        []{#equals(java.lang.Object)}

        -   #### equals

            ``` methodSignature
            public boolean equals​(@Nullable
                                  Object another)
            ```

            ::: block
            This instance is equal to all instances of
            `ImmutableDotnetLibraryProviderInfo` that have equal
            attribute values.
            :::

            [Overrides:]{.overrideSpecifyLabel}
            :   `equals` in class `Object`

            [Returns:]{.returnLabel}
            :   `true` if `this` is equal to `another` instance

        []{#hashCode()}

        -   #### hashCode

            ``` methodSignature
            public int hashCode()
            ```

            ::: block
            Computes a hash code from attributes: `dll`.
            :::

            [Overrides:]{.overrideSpecifyLabel}
            :   `hashCode` in class `Object`

            [Returns:]{.returnLabel}
            :   hashCode value

        []{#toString()}

        -   #### toString

            ``` methodSignature
            public String toString()
            ```

            ::: block
            Prints the immutable value `DotnetLibraryProviderInfo` with
            attribute values.
            :::

            [Overrides:]{.overrideSpecifyLabel}
            :   `toString` in class `Object`

            [Returns:]{.returnLabel}
            :   A string representation of the value
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
-   [Field](#field.summary) \| 
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
