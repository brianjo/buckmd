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

## Class ImmutableTestInfo {#class-immutabletestinfo .title title="Class ImmutableTestInfo"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.core.starlark.compatible.BuckStarlarkStructObject](../../../starlark/compatible/BuckStarlarkStructObject.html "class in com.facebook.buck.core.starlark.compatible")

    -   -   [com.facebook.buck.core.rules.providers.impl.BuiltInProviderInfo](../impl/BuiltInProviderInfo.html "class in com.facebook.buck.core.rules.providers.impl")\<[TestInfo](TestInfo.html "class in com.facebook.buck.core.rules.providers.lib")\>

        -   -   [com.facebook.buck.core.rules.providers.lib.TestInfo](TestInfo.html "class in com.facebook.buck.core.rules.providers.lib")

            -   -   com.facebook.buck.core.rules.providers.lib.ImmutableTestInfo

::: description
-   

    All Implemented Interfaces:
    :   `ProviderInfo<TestInfo>`, `SkylarkProviderInfo`,
        `com.google.devtools.build.lib.skylarkinterface.SkylarkPrintable`,
        `com.google.devtools.build.lib.skylarkinterface.SkylarkValue`,
        `com.google.devtools.build.lib.syntax.ClassObject`

    ------------------------------------------------------------------------

        @ParametersAreNonnullByDefault
        @Generated("org.immutables.processor.ProxyProcessor")
        @Immutable
        @CheckReturnValue
        public final class ImmutableTestInfo
        extends TestInfo

    ::: block
    Immutable implementation of
    [`TestInfo`](TestInfo.html "class in com.facebook.buck.core.rules.providers.lib").
    Use the static factory method to create immutable instances:
    `new ImmutableTestInfo()`.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        -   []{#fields.inherited.from.class.com.facebook.buck.core.rules.providers.lib.TestInfo}

            ### Fields inherited from class com.facebook.buck.core.rules.providers.lib.[TestInfo](TestInfo.html "class in com.facebook.buck.core.rules.providers.lib")

            `PROVIDER`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

        +-----------------------------------+-----------------------------------+
        | Constructor                       | Description                       |
        +===================================+===================================+
        | `Immut                            | ::: block                         |
        | ableTestInfo​(String testName,     | Construct a new immutable         |
        |               String testCaseName | `TestInfo` instance.              |
        | ,                  Iterable<Strin | :::                               |
        | g> labels,                  Itera |                                   |
        | ble<String> contacts,             |                                   |
        |       Object timeoutMs,           |                                   |
        |         boolean runTestsSeparatel |                                   |
        | y,                  String type)` |                                   |
        +-----------------------------------+-----------------------------------+

        : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `com.g                | `contacts()`          |                       |
        | oogle.common.collect. |                       |                       |
        | ImmutableSet<String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `eq                   | ::: block             |
        |                       | uals​(Object another)` | This instance is      |
        |                       |                       | equal to all          |
        |                       |                       | instances of          |
        |                       |                       | `ImmutableTestInfo`   |
        |                       |                       | that have equal       |
        |                       |                       | attribute values.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `int`                 | `hashCode()`          | ::: block             |
        |                       |                       | Computes a hash code  |
        |                       |                       | from attributes:      |
        |                       |                       | `testName`,           |
        |                       |                       | `testCaseName`,       |
        |                       |                       | `labels`, `contacts`, |
        |                       |                       | `timeoutMs`,          |
        |                       |                       | `runTestsSeparately`, |
        |                       |                       | `type`.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.g                | `labels()`            |                       |
        | oogle.common.collect. |                       |                       |
        | ImmutableSet<String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `                     |                       |
        |                       | runTestsSeparately()` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `testCaseName()`      |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `testName()`          |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Object`              | `timeoutMs()`         |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `toString()`          | ::: block             |
        |                       |                       | Prints the immutable  |
        |                       |                       | value `TestInfo` with |
        |                       |                       | attribute values.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `type()`              |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Long>`      | `typedTimeoutMs()`    |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.providers.lib.TestInfo}

            ### Methods inherited from class com.facebook.buck.core.rules.providers.lib.[TestInfo](TestInfo.html "class in com.facebook.buck.core.rules.providers.lib")

            `instantiateFromSkylark, of`

        ```{=html}
        <!-- -->
        ```
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

        []{#<init>(java.lang.String,java.lang.String,java.lang.Iterable,java.lang.Iterable,java.lang.Object,boolean,java.lang.String)}

        -   #### ImmutableTestInfo

                public ImmutableTestInfo​(String testName,
                                         String testCaseName,
                                         Iterable<String> labels,
                                         Iterable<String> contacts,
                                         Object timeoutMs,
                                         boolean runTestsSeparately,
                                         String type)

            ::: block
            Construct a new immutable `TestInfo` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `testName` - The value for the `testName` attribute
            :   `testCaseName` - The value for the `testCaseName`
                attribute
            :   `labels` - The value for the `labels` attribute
            :   `contacts` - The value for the `contacts` attribute
            :   `timeoutMs` - The value for the `timeoutMs` attribute
            :   `runTestsSeparately` - The value for the
                `runTestsSeparately` attribute
            :   `type` - The value for the `type` attribute
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#testName()}

        -   #### testName

            ``` methodSignature
            public String testName()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `testName` in class `TestInfo`

            [Returns:]{.returnLabel}
            :   the type of test. This should generally be the rule name

        []{#testCaseName()}

        -   #### testCaseName

            ``` methodSignature
            public String testCaseName()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `testCaseName` in class `TestInfo`

            [Returns:]{.returnLabel}
            :   the name of the test case

        []{#labels()}

        -   #### labels

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<String> labels()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `labels` in class `TestInfo`

        []{#contacts()}

        -   #### contacts

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<String> contacts()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `contacts` in class `TestInfo`

        []{#timeoutMs()}

        -   #### timeoutMs

            ``` methodSignature
            public Object timeoutMs()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `timeoutMs` in class `TestInfo`

        []{#runTestsSeparately()}

        -   #### runTestsSeparately

            ``` methodSignature
            public boolean runTestsSeparately()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `runTestsSeparately` in class `TestInfo`

        []{#type()}

        -   #### type

            ``` methodSignature
            public String type()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `type` in class `TestInfo`

            [Returns:]{.returnLabel}
            :   the \'type\' to pass to the external test runner

        []{#equals(java.lang.Object)}

        -   #### equals

            ``` methodSignature
            public boolean equals​(@Nullable
                                  Object another)
            ```

            ::: block
            This instance is equal to all instances of
            `ImmutableTestInfo` that have equal attribute values.
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
            Computes a hash code from attributes: `testName`,
            `testCaseName`, `labels`, `contacts`, `timeoutMs`,
            `runTestsSeparately`, `type`.
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
            Prints the immutable value `TestInfo` with attribute values.
            :::

            [Overrides:]{.overrideSpecifyLabel}
            :   `toString` in class `Object`

            [Returns:]{.returnLabel}
            :   A string representation of the value

        []{#typedTimeoutMs()}

        -   #### typedTimeoutMs

            ``` methodSignature
            public Optional<Long> typedTimeoutMs()
            ```

            ::: block
            Returns a lazily initialized value of the
            [`typedTimeoutMs`](TestInfo.html#typedTimeoutMs())
            attribute. Initialized once and only once and stored for
            subsequent access with proper synchronization.
            :::

            [Overrides:]{.overrideSpecifyLabel}
            :   `typedTimeoutMs` in class `TestInfo`

            [Returns:]{.returnLabel}
            :   A lazily initialized value of the `typedTimeoutMs`
                attribute
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
