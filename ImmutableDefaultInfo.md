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
[Package]{.packageLabelInType} [com.facebook.buck.core.rules.providers.lib](package-summary.html)
:::

## Class ImmutableDefaultInfo {#class-immutabledefaultinfo .title title="Class ImmutableDefaultInfo"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.core.starlark.compatible.BuckStarlarkStructObject](../../../starlark/compatible/BuckStarlarkStructObject.html "class in com.facebook.buck.core.starlark.compatible")

    -   -   [com.facebook.buck.core.rules.providers.impl.BuiltInProviderInfo](../impl/BuiltInProviderInfo.html "class in com.facebook.buck.core.rules.providers.impl")\<[DefaultInfo](DefaultInfo.html "class in com.facebook.buck.core.rules.providers.lib")\>

        -   -   [com.facebook.buck.core.rules.providers.lib.DefaultInfo](DefaultInfo.html "class in com.facebook.buck.core.rules.providers.lib")

            -   -   com.facebook.buck.core.rules.providers.lib.ImmutableDefaultInfo

::: description
-   

    All Implemented Interfaces:
    :   `ProviderInfo<DefaultInfo>`, `SkylarkProviderInfo`,
        `com.google.devtools.build.lib.skylarkinterface.SkylarkPrintable`,
        `com.google.devtools.build.lib.skylarkinterface.SkylarkValue`,
        `com.google.devtools.build.lib.syntax.ClassObject`

    ------------------------------------------------------------------------

        @ParametersAreNonnullByDefault
        @Generated("org.immutables.processor.ProxyProcessor")
        @Immutable
        @CheckReturnValue
        public final class ImmutableDefaultInfo
        extends DefaultInfo

    ::: block
    Immutable implementation of
    [`DefaultInfo`](DefaultInfo.html "class in com.facebook.buck.core.rules.providers.lib").
    Use the static factory method to create immutable instances:
    `new ImmutableDefaultInfo()`.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        -   []{#fields.inherited.from.class.com.facebook.buck.core.rules.providers.lib.DefaultInfo}

            ### Fields inherited from class com.facebook.buck.core.rules.providers.lib.[DefaultInfo](DefaultInfo.html "class in com.facebook.buck.core.rules.providers.lib")

            `PROVIDER`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

        +-----------------------------------+-----------------------------------+
        | Constructor                       | Description                       |
        +===================================+===================================+
        | `Immuta                           | ::: block                         |
        | bleDefaultInfo​(com.google.devtool | Construct a new immutable         |
        | s.build.lib.syntax.SkylarkDict<St | `DefaultInfo` instance.           |
        | ring,​Set<Artifact>> namedOutputs, | :::                               |
        |                      Iterable<? e |                                   |
        | xtends Artifact> defaultOutputs)` |                                   |
        +-----------------------------------+-----------------------------------+

        : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `com.goo              | `defaultOutputs()`    |                       |
        | gle.common.collect.Im |                       |                       |
        | mutableSet<Artifact>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `eq                   | ::: block             |
        |                       | uals​(Object another)` | This instance is      |
        |                       |                       | equal to all          |
        |                       |                       | instances of          |
        |                       |                       | `                     |
        |                       |                       | ImmutableDefaultInfo` |
        |                       |                       | that have equal       |
        |                       |                       | attribute values.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `hashCode()`          | ::: block             |
        |                       |                       | Computes a hash code  |
        |                       |                       | from attributes:      |
        |                       |                       | `namedOutputs`,       |
        |                       |                       | `defaultOutputs`.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.goog             | `namedOutputs()`      | ::: block             |
        | le.devtools.build.lib |                       | These are the named   |
        | .syntax.SkylarkDict<S |                       | outputs of a rule.    |
        | tring,​Set<Artifact>>` |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `toString()`          | ::: block             |
        |                       |                       | Prints the immutable  |
        |                       |                       | value `DefaultInfo`   |
        |                       |                       | with attribute        |
        |                       |                       | values.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.providers.impl.BuiltInProviderInfo}

            ### Methods inherited from class com.facebook.buck.core.rules.providers.impl.[BuiltInProviderInfo](../impl/BuiltInProviderInfo.html "class in com.facebook.buck.core.rules.providers.impl")

            `getDeclaredClass, getProvider, getProviderInfo, isImmutable`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.starlark.compatible.BuckStarlarkStructObject}

            ### Methods inherited from class com.facebook.buck.core.starlark.compatible.[BuckStarlarkStructObject](../../../starlark/compatible/BuckStarlarkStructObject.html "class in com.facebook.buck.core.starlark.compatible")

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

        []{#<init>(com.google.devtools.build.lib.syntax.SkylarkDict,java.lang.Iterable)}

        -   #### ImmutableDefaultInfo

                public ImmutableDefaultInfo​(com.google.devtools.build.lib.syntax.SkylarkDict<String,​Set<Artifact>> namedOutputs,
                                            Iterable<? extends Artifact> defaultOutputs)

            ::: block
            Construct a new immutable `DefaultInfo` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `namedOutputs` - The value for the `namedOutputs`
                attribute
            :   `defaultOutputs` - The value for the `defaultOutputs`
                attribute
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#namedOutputs()}

        -   #### namedOutputs

            ``` methodSignature
            public com.google.devtools.build.lib.syntax.SkylarkDict<String,​Set<Artifact>> namedOutputs()
            ```

            ::: block
            These are the named outputs of a rule. Named outputs are a
            mapping of String identifiers to a set of outputs of the
            rule that the name maps to.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `namedOutputs` in class `DefaultInfo`

            [Returns:]{.returnLabel}
            :   a map of a String, which is the named identifier to a
                set of outputs.

        []{#defaultOutputs()}

        -   #### defaultOutputs

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<Artifact> defaultOutputs()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `defaultOutputs` in class `DefaultInfo`

            [Returns:]{.returnLabel}
            :   the set of default outputs built by the rule if no
                output selection is specified.

        []{#equals(java.lang.Object)}

        -   #### equals

            ``` methodSignature
            public boolean equals​(@Nullable
                                  Object another)
            ```

            ::: block
            This instance is equal to all instances of
            `ImmutableDefaultInfo` that have equal attribute values.
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
            Computes a hash code from attributes: `namedOutputs`,
            `defaultOutputs`.
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
            Prints the immutable value `DefaultInfo` with attribute
            values.
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
