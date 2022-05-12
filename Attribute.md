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
[Package]{.packageLabelInType} [com.facebook.buck.core.starlark.rule.attr](package-summary.html)
:::

## Class Attribute\<CoercedType\> {#class-attributecoercedtype .title title="Class Attribute"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.starlark.rule.attr.Attribute\<CoercedType\>

::: description
-   

    All Implemented Interfaces:
    :   `AttributeHolder`,
        `com.google.devtools.build.lib.skylarkinterface.SkylarkPrintable`,
        `com.google.devtools.build.lib.skylarkinterface.SkylarkValue`

    ```{=html}
    <!-- -->
    ```

    Direct Known Subclasses:
    :   `BoolAttribute`, `DepAttribute`, `DepListAttribute`,
        `IntAttribute`, `IntListAttribute`, `OutputAttribute`,
        `OutputListAttribute`, `SourceAttribute`, `SourceListAttribute`,
        `SourceSortedSetAttribute`, `StringAttribute`,
        `StringListAttribute`, `StringSortedSetAttribute`,
        `UnconfiguredDepListAttribute`,
        `UnconfiguredOptionalDepAttribute`

    ------------------------------------------------------------------------

        public abstract class Attribute<CoercedType>
        extends Object
        implements AttributeHolder

    ::: block
    Representation of a parameter of a user defined rule
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor     Description
          --------------- -------------
          `Attribute()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `Attribute<?>`        | `getAttribute()`      | ::: block             |
        |                       |                       | Get the actual        |
        |                       |                       | attribute object      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `abstract String`     | `getDoc()`            | ::: block             |
        |                       |                       | The docstring to use  |
        |                       |                       | for this attribute    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Type`                | `getGenericType()`    | ::: block             |
        |                       |                       | Get the generic type  |
        |                       |                       | of `CoercedType`.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `abstract boolean`    | `getMandatory()`      | ::: block             |
        |                       |                       | Whether this          |
        |                       |                       | attribute is          |
        |                       |                       | mandatory or not      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Pos                  | `getPos               |                       |
        | tCoercionTransform<Ru | tCoercionTransform()` |                       |
        | leAnalysisContext,​?>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstract Object`     | `getPreCo             | ::: block             |
        |                       | ercionDefaultValue()` | The default value to  |
        |                       |                       | use if no value is    |
        |                       |                       | provided.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `abstract TypeCo      | `getTypeCoercer()`    | ::: block             |
        | ercer<?,​CoercedType>` |                       | The type coercer to   |
        |                       |                       | use to convert raw    |
        |                       |                       | values from the       |
        |                       |                       | parser into something |
        |                       |                       | usable internally.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CoercedType`         | `getValue​(C           | ::: block             |
        |                       | ellNameResolver cellN | Get the coerced value |
        |                       | ameResolver,          | for this attribute.   |
        |                       | ProjectFilesystem pro | :::                   |
        |                       | jectFilesystem,       |                       |
        |                       |    ForwardRelativePat |                       |
        |                       | h pathRelativeToProje |                       |
        |                       | ctRoot,         Targe |                       |
        |                       | tConfiguration target |                       |
        |                       | Configuration,        |                       |
        |                       |   TargetConfiguration |                       |
        |                       |  hostConfiguration,   |                       |
        |                       |        Object value)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected void`      | `validateCoercedValu  | ::: block             |
        |                       | e​(CoercedType value)` | Validates values      |
        |                       |                       | post-coercion to      |
        |                       |                       | ensure other          |
        |                       |                       | properties besides    |
        |                       |                       | \'type\' are valid    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `p                    | `                     | ::: block             |
        | rotected static void` | validateProvidersPres | Ensures that all of   |
        |                       | ent​(List<Provider<?>> | the                   |
        |                       |  expectedProviders,   | [`                    |
        |                       |                       | Provider`](../../../r |
        |                       |   BuildTarget target, | ules/providers/Provid |
        |                       |                       | er.html "interface in |
        |                       |     ProviderInfoColle |  com.facebook.buck.co |
        |                       | ction providerInfos)` | re.rules.providers")s |
        |                       |                       | in                    |
        |                       |                       | `expectedProviders`   |
        |                       |                       | are present in        |
        |                       |                       | `  providerInfos`     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `protected void`      | `                     | ::: block             |
        |                       | validateValueInList​(L | Helper method to      |
        |                       | ist<CoercedType> valu | validate that a value |
        |                       | es,                   | is in a list and      |
        |                       |   CoercedType value)` | throw a reasonable    |
        |                       |                       | error if not          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Abstract
        Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
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
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### Attribute

                public Attribute()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getAttribute()}

        -   #### getAttribute

            ``` methodSignature
            public Attribute<?> getAttribute()
            ```

            ::: block
            [Description copied from
            interface: `AttributeHolder`]{.descfrmTypeLabel}
            :::

            ::: block
            Get the actual attribute object
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getAttribute` in interface `AttributeHolder`

        []{#getGenericType()}

        -   #### getGenericType

            ``` methodSignature
            @Lazy
            public Type getGenericType()
            ```

            ::: block
            Get the generic type of `CoercedType`.
            :::

        []{#getPreCoercionDefaultValue()}

        -   #### getPreCoercionDefaultValue

            ``` methodSignature
            public abstract Object getPreCoercionDefaultValue()
            ```

            ::: block
            The default value to use if no value is provided.
            This will be validated against
            [`getTypeCoercer()`](#getTypeCoercer()), so may return a
            value whose type does not match
            [`Attribute`](Attribute.html "class in com.facebook.buck.core.starlark.rule.attr")
            (e.g. a list of strings, rather than a list of
            [`SourcePath`](../../../sourcepath/SourcePath.html "interface in com.facebook.buck.core.sourcepath"))
            :::

        []{#getDoc()}

        -   #### getDoc

            ``` methodSignature
            public abstract String getDoc()
            ```

            ::: block
            The docstring to use for this attribute
            :::

        []{#getMandatory()}

        -   #### getMandatory

            ``` methodSignature
            public abstract boolean getMandatory()
            ```

            ::: block
            Whether this attribute is mandatory or not
            :::

        []{#getTypeCoercer()}

        -   #### getTypeCoercer

            ``` methodSignature
            public abstract TypeCoercer<?,​CoercedType> getTypeCoercer()
            ```

            ::: block
            The type coercer to use to convert raw values from the
            parser into something usable internally. This coercer also
            performs validation
            :::

        []{#validateCoercedValue(java.lang.Object)}
        []{#validateCoercedValue(CoercedType)}

        -   #### validateCoercedValue

            ``` methodSignature
            protected void validateCoercedValue​(CoercedType value)
                                         throws CoerceFailedException
            ```

            ::: block
            Validates values post-coercion to ensure other properties
            besides \'type\' are valid
            :::

            [Parameters:]{.paramLabel}
            :   `value` - The value to check

            [Throws:]{.throwsLabel}
            :   `CoerceFailedException` - if the value is invalid (e.g.
                not in a list of pre-approved values)

        []{#getPostCoercionTransform()}

        -   #### getPostCoercionTransform

            ``` methodSignature
            public PostCoercionTransform<RuleAnalysisContext,​?> getPostCoercionTransform()
            ```

            [Returns:]{.returnLabel}
            :   a method that transforms a coerced value into something
                more useful to users, taking into account the rule\'s
                dependencies

        []{#getValue(com.facebook.buck.core.cell.nameresolver.CellNameResolver,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.path.ForwardRelativePath,com.facebook.buck.core.model.TargetConfiguration,com.facebook.buck.core.model.TargetConfiguration,java.lang.Object)}

        -   #### getValue

            ``` methodSignature
            public CoercedType getValue​(CellNameResolver cellNameResolver,
                                        ProjectFilesystem projectFilesystem,
                                        ForwardRelativePath pathRelativeToProjectRoot,
                                        TargetConfiguration targetConfiguration,
                                        TargetConfiguration hostConfiguration,
                                        Object value)
                                 throws CoerceFailedException
            ```

            ::: block
            Get the coerced value for this attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `cellNameResolver` - The cell roots
            :   `projectFilesystem` - The project file system
            :   `pathRelativeToProjectRoot` - The path relative to the
                project root
            :   `targetConfiguration` - The configuration for this
                target
            :   `hostConfiguration` -
            :   `value` - The object that is to be coerced. This
                generally comes directly from the parser.

            [Throws:]{.throwsLabel}
            :   `CoerceFailedException` - if the value could not be
                coerced

        []{#validateValueInList(java.util.List,java.lang.Object)}
        []{#validateValueInList(java.util.List,CoercedType)}

        -   #### validateValueInList

            ``` methodSignature
            protected void validateValueInList​(List<CoercedType> values,
                                               CoercedType value)
                                        throws CoerceFailedException
            ```

            ::: block
            Helper method to validate that a value is in a list and
            throw a reasonable error if not
            :::

            [Throws:]{.throwsLabel}
            :   `CoerceFailedException`

        []{#validateProvidersPresent(java.util.List,com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.rules.providers.collect.ProviderInfoCollection)}

        -   #### validateProvidersPresent

            ``` methodSignature
            protected static void validateProvidersPresent​(List<Provider<?>> expectedProviders,
                                                           BuildTarget target,
                                                           ProviderInfoCollection providerInfos)
            ```

            ::: block
            Ensures that all of the
            [`Provider`](../../../rules/providers/Provider.html "interface in com.facebook.buck.core.rules.providers")s
            in `expectedProviders` are present in `  providerInfos`
            Note that it is enforced that all build rules return at
            least
            [`DefaultInfo`](../../../rules/providers/lib/DefaultInfo.html "class in com.facebook.buck.core.rules.providers.lib"),
            so that is not required to be specified
            :::

            [Parameters:]{.paramLabel}
            :   `expectedProviders` - The providers that ALL MUST be
                present. If empty, no providers are required, and all
                `providerInfos` will be considered valid.
            :   `target` - the target that `providerInfos` is associated
                with. Used in errors.
            :   `providerInfos` - The
                [`ProviderInfo`](../../../rules/providers/ProviderInfo.html "interface in com.facebook.buck.core.rules.providers")s
                for a given dependency

            [Throws:]{.throwsLabel}
            :   `com.google.common.base.VerifyException` - if a provider
                is missing in `      providerInfos`
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
