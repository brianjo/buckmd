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
[Package]{.packageLabelInType} [com.facebook.buck.core.rules.providers.impl](package-summary.html)
:::

## Class UserDefinedProvider {#class-userdefinedprovider .title title="Class UserDefinedProvider"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.google.devtools.build.lib.syntax.BaseFunction

    -   -   com.facebook.buck.core.rules.providers.impl.UserDefinedProvider

::: description
-   

    All Implemented Interfaces:
    :   `Provider<UserDefinedProviderInfo>`,
        `com.google.devtools.build.lib.packages.SkylarkExportable`,
        `com.google.devtools.build.lib.skylarkinterface.SkylarkPrintable`,
        `com.google.devtools.build.lib.skylarkinterface.SkylarkValue`,
        `com.google.devtools.build.lib.syntax.StarlarkFunction`

    ------------------------------------------------------------------------

        public class UserDefinedProvider
        extends com.google.devtools.build.lib.syntax.BaseFunction
        implements Provider<UserDefinedProviderInfo>, com.google.devtools.build.lib.skylarkinterface.SkylarkValue, com.google.devtools.build.lib.packages.SkylarkExportable

    ::: block
    A
    [`Provider`](../Provider.html "interface in com.facebook.buck.core.rules.providers")
    defined by a user in a build file that creates
    [`UserDefinedProviderInfo`](UserDefinedProviderInfo.html "class in com.facebook.buck.core.rules.providers.impl")
    instances. This is only intended to be used within the context of
    user defined rules, and as such,
    [`UserDefinedProviderInfo`](UserDefinedProviderInfo.html "class in com.facebook.buck.core.rules.providers.impl")
    instances that are created contain skylark-compatible values, rather
    than normal java/guava classes. In the future type restriction may
    also be allowed.
    NOTE: Until
    [`export(Label, String)`](#export(com.google.devtools.build.lib.cmdline.Label,java.lang.String))
    is called, many methods (especially ones that get the user defined
    name of the class) are not safe to call.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        -   []{#fields.inherited.from.class.com.google.devtools.build.lib.syntax.BaseFunction}

            ### Fields inherited from class com.google.devtools.build.lib.syntax.BaseFunction

            `enforcedArgumentTypes, location, objectType, paramDoc, signature`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

        +-----------------------------------+-----------------------------------+
        | Constructor                       | Description                       |
        +===================================+===================================+
        | `UserDefinedProvid                | ::: block                         |
        | er​(com.google.devtools.build.lib. | Create an instance of             |
        | events.Location location,         | [`Use                             |
        |             String[] fieldNames)` | rDefinedProvider`](UserDefinedPro |
        |                                   | vider.html "class in com.facebook |
        |                                   | .buck.core.rules.providers.impl") |
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
        | `protected Object`    | `call​(Object[] ar     |                       |
        |                       | gs,     com.google.de |                       |
        |                       | vtools.build.lib.synt |                       |
        |                       | ax.FuncallExpression  |                       |
        |                       | ast,     com.google.d |                       |
        |                       | evtools.build.lib.syn |                       |
        |                       | tax.Environment env)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `export​(com           |                       |
        |                       | .google.devtools.buil |                       |
        |                       | d.lib.cmdline.Label e |                       |
        |                       | xtensionLabel,        |                       |
        |                       | String exportedName)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Provider.Key<User    | `getKey()`            | ::: block             |
        | DefinedProviderInfo>` |                       | Returns a             |
        |                       |                       | serializable          |
        |                       |                       | representation of     |
        |                       |                       | this `Provider`.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getName()`           |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isExported()`        |                       |
        +-----------------------+-----------------------+-----------------------+
        | `boolean`             | `isImmutable()`       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `repr​(com.goog        |                       |
        |                       | le.devtools.build.lib |                       |
        |                       | .skylarkinterface.Sky |                       |
        |                       | larkPrinter printer)` |                       |
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
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.google.devtools.build.lib.syntax.BaseFunction}

            ### Methods inherited from class com.google.devtools.build.lib.syntax.BaseFunction

            `call, callWithArgArray, canonicalizeArguments, configure, configure, getArgArraySize, getEnforcedArgumentTypes, getFullName, getLocation, getObjectType, getObjectTypeString, getOrCreateChildEnvironment, getParamDoc, getShortSignature, getSignature, hasSelfArgument, isConfigured, printTypeString, processArguments`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, wait, wait, wait`

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

        []{#<init>(com.google.devtools.build.lib.events.Location,java.lang.String[])}

        -   #### UserDefinedProvider

                public UserDefinedProvider​(com.google.devtools.build.lib.events.Location location,
                                           String[] fieldNames)

            ::: block
            Create an instance of
            [`UserDefinedProvider`](UserDefinedProvider.html "class in com.facebook.buck.core.rules.providers.impl")
            :::

            [Parameters:]{.paramLabel}
            :   `location` - The location where the provider was defined
                by the user
            :   `fieldNames` - List of kwargs that will be available
                when
                [`call(Object[],      FuncallExpression, Environment)`](#call(java.lang.Object%5B%5D,com.google.devtools.build.lib.syntax.FuncallExpression,com.google.devtools.build.lib.syntax.Environment))
                is called, and will be available as fields on the
                resulting
                [`UserDefinedProviderInfo`](UserDefinedProviderInfo.html "class in com.facebook.buck.core.rules.providers.impl")
                object
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#isImmutable()}

        -   #### isImmutable

            ``` methodSignature
            public boolean isImmutable()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `isImmutable` in
                interface `com.google.devtools.build.lib.skylarkinterface.SkylarkValue`

            [Overrides:]{.overrideSpecifyLabel}
            :   `isImmutable` in
                class `com.google.devtools.build.lib.syntax.BaseFunction`

        []{#getKey()}

        -   #### getKey

            ``` methodSignature
            public Provider.Key<UserDefinedProviderInfo> getKey()
            ```

            ::: block
            [Description copied from
            interface: `Provider`]{.descfrmTypeLabel}
            :::

            ::: block
            Returns a serializable representation of this `Provider`.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getKey` in
                interface `Provider<UserDefinedProviderInfo>`

        []{#repr(com.google.devtools.build.lib.skylarkinterface.SkylarkPrinter)}

        -   #### repr

            ``` methodSignature
            public void repr​(com.google.devtools.build.lib.skylarkinterface.SkylarkPrinter printer)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `repr` in
                interface `com.google.devtools.build.lib.skylarkinterface.SkylarkPrintable`

            [Overrides:]{.overrideSpecifyLabel}
            :   `repr` in
                class `com.google.devtools.build.lib.syntax.BaseFunction`

        []{#isExported()}

        -   #### isExported

            ``` methodSignature
            public boolean isExported()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `isExported` in
                interface `com.google.devtools.build.lib.packages.SkylarkExportable`

        []{#getName()}

        -   #### getName

            ``` methodSignature
            public String getName()
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `getName` in
                class `com.google.devtools.build.lib.syntax.BaseFunction`

        []{#export(com.google.devtools.build.lib.cmdline.Label,java.lang.String)}

        -   #### export

            ``` methodSignature
            public void export​(com.google.devtools.build.lib.cmdline.Label extensionLabel,
                               String exportedName)
                        throws com.google.devtools.build.lib.syntax.EvalException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `export` in
                interface `com.google.devtools.build.lib.packages.SkylarkExportable`

            [Throws:]{.throwsLabel}
            :   `com.google.devtools.build.lib.syntax.EvalException`

        []{#toString()}

        -   #### toString

            ``` methodSignature
            public String toString()
            ```

            ::: block
            [Description copied from
            interface: `Provider`]{.descfrmTypeLabel}
            :::

            ::: block
            Returns a name of this `Provider` that should be used in
            error messages.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `toString` in
                interface `Provider<UserDefinedProviderInfo>`

            [Overrides:]{.overrideSpecifyLabel}
            :   `toString` in
                class `com.google.devtools.build.lib.syntax.BaseFunction`

        []{#call(java.lang.Object[],com.google.devtools.build.lib.syntax.FuncallExpression,com.google.devtools.build.lib.syntax.Environment)}

        -   #### call

            ``` methodSignature
            protected Object call​(Object[] args,
                                  @Nullable
                                  com.google.devtools.build.lib.syntax.FuncallExpression ast,
                                  com.google.devtools.build.lib.syntax.Environment env)
            ```

            [Overrides:]{.overrideSpecifyLabel}
            :   `call` in
                class `com.google.devtools.build.lib.syntax.BaseFunction`
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
