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
[Package]{.packageLabelInType} [com.facebook.buck.core.starlark.rule](package-summary.html)
:::

## Class SkylarkDescriptionArg {#class-skylarkdescriptionarg .title title="Class SkylarkDescriptionArg"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.starlark.rule.SkylarkDescriptionArg

::: description
-   

    All Implemented Interfaces:
    :   `BuildRuleArg`, `ConstructorArg`, `DataTransferObject`,
        `SkylarkDescriptionArgBuilder`

    ------------------------------------------------------------------------

        public class SkylarkDescriptionArg
        extends Object
        implements SkylarkDescriptionArgBuilder, BuildRuleArg

    ::: block
    Description arg for user defined rules. Instead of using reflection
    and immutables, this class uses a backing store of attribute names
    -\> coerced values, and makes the user\'s implementation function
    available
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

        -   []{#fields.inherited.from.class.com.facebook.buck.core.description.arg.BuildRuleArg}

            ### Fields inherited from interface com.facebook.buck.core.description.arg.[BuildRuleArg](../../description/arg/BuildRuleArg.html "interface in com.facebook.buck.core.description.arg")

            `DEFAULT_TARGET_PLATFORM_PARAM_NAME`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

        +-----------------------------------+-----------------------------------+
        | Constructor                       | Description                       |
        +===================================+===================================+
        | `SkylarkDescription               | ::: block                         |
        | Arg​(SkylarkUserDefinedRule rule)` | Create an instance of             |
        |                                   | [`                                |
        |                                   | SkylarkDescriptionArg`](SkylarkDe |
        |                                   | scriptionArg.html "class in com.f |
        |                                   | acebook.buck.core.starlark.rule") |
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
        | `void`                | `build()`             | ::: block             |
        |                       |                       | \'Build\' the         |
        |                       |                       | [`SkylarkDescripti    |
        |                       |                       | onArg`](SkylarkDescri |
        |                       |                       | ptionArg.html "class  |
        |                       |                       | in com.facebook.buck. |
        |                       |                       | core.starlark.rule"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.common.   | `getAllParamInfo()`   |                       |
        | collect.ImmutableMap< |                       |                       |
        | String,​ParamInfo<?>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `co                   | `getCompatibleWith()` | ::: block             |
        | m.google.common.colle |                       | A list of             |
        | ct.ImmutableList<Unco |                       | `config_setting` a    |
        | nfiguredBuildTarget>` |                       | target is compatible  |
        |                       |                       | with.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.          | `getContacts()`       |                       |
        | common.collect.Immuta |                       |                       |
        | bleSortedSet<String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `Optional<Unco        | `getDef               | ::: block             |
        | nfiguredBuildTarget>` | aultTargetPlatform()` | The name of build     |
        |                       |                       | target default        |
        |                       |                       | \"new\" platform: it  |
        |                       |                       | is used when a        |
        |                       |                       | platform is not       |
        |                       |                       | specified either      |
        |                       |                       | globally or in a      |
        |                       |                       | target which used     |
        |                       |                       | this target as a      |
        |                       |                       | dependency.           |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `com.goog             | `getImplementation()` |                       |
        | le.devtools.build.lib |                       |                       |
        | .syntax.BaseFunction` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.          | `getLabels()`         |                       |
        | common.collect.Immuta |                       |                       |
        | bleSortedSet<String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.googl            | `getLicenses()`       |                       |
        | e.common.collect.Immu |                       |                       |
        | tableSet<SourcePath>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `String`              | `getName()`           | ::: block             |
        |                       |                       | Each rule has a name  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Object`              | `getPostCoerci        | ::: block             |
        |                       | onValue​(String attr)` | Get an attribute\'s   |
        |                       |                       | value after it was    |
        |                       |                       | set in                |
        |                       |                       | [`S                   |
        |                       |                       | kylarkDescriptionArgB |
        |                       |                       | uilder.setPostCoercio |
        |                       |                       | nValue(String, Object |
        |                       |                       | )`](../coercer/Skylar |
        |                       |                       | kDescriptionArgBuilde |
        |                       |                       | r.html#setPostCoercio |
        |                       |                       | nValue(java.lang.Stri |
        |                       |                       | ng,java.lang.Object)) |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Sk                   | `getRule()`           | ::: block             |
        | ylarkUserDefinedRule` |                       | Get the               |
        |                       |                       | [`SkylarkDescript     |
        |                       |                       | ionArg`](SkylarkDescr |
        |                       |                       | iptionArg.html "class |
        |                       |                       |  in com.facebook.buck |
        |                       |                       | .core.starlark.rule") |
        |                       |                       | that has information  |
        |                       |                       | about parameters and  |
        |                       |                       | the user\'s           |
        |                       |                       | implementation        |
        |                       |                       | function              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `setPo                | ::: block             |
        |                       | stCoercionValue​(Strin | Set the value for a   |
        |                       | g attr,               | specific attribute    |
        |                       |        Object value)` | after it has been     |
        |                       |                       | successfully          |
        |                       |                       | coerced/type checked. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

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
        -   []{#methods.inherited.from.class.com.facebook.buck.core.description.arg.BuildRuleArg}

            ### Methods inherited from interface com.facebook.buck.core.description.arg.[BuildRuleArg](../../description/arg/BuildRuleArg.html "interface in com.facebook.buck.core.description.arg")

            `labelsContainsAnyOf`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.core.starlark.rule.SkylarkUserDefinedRule)}

        -   #### SkylarkDescriptionArg

                public SkylarkDescriptionArg​(SkylarkUserDefinedRule rule)

            ::: block
            Create an instance of
            [`SkylarkDescriptionArg`](SkylarkDescriptionArg.html "class in com.facebook.buck.core.starlark.rule")
            :::

            [Parameters:]{.paramLabel}
            :   `rule` - the rule that should be used to determine
                acceptable attributes for a target, and to provide
                access to the user\'s implementation function
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#setPostCoercionValue(java.lang.String,java.lang.Object)}

        -   #### setPostCoercionValue

            ``` methodSignature
            public void setPostCoercionValue​(String attr,
                                             Object value)
            ```

            ::: block
            [Description copied from
            interface: `SkylarkDescriptionArgBuilder`]{.descfrmTypeLabel}
            :::

            ::: block
            Set the value for a specific attribute after it has been
            successfully coerced/type checked. This attribute must be
            defined in the originally provided
            [`SkylarkUserDefinedRule`](SkylarkUserDefinedRule.html "class in com.facebook.buck.core.starlark.rule")
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `setPostCoercionValue` in
                interface `SkylarkDescriptionArgBuilder`

            [Parameters:]{.paramLabel}
            :   `attr` - The attribute to set the value for
            :   `value` - The value to set. Must not be null.

        []{#getPostCoercionValue(java.lang.String)}

        -   #### getPostCoercionValue

            ``` methodSignature
            public Object getPostCoercionValue​(String attr)
            ```

            ::: block
            [Description copied from
            interface: `SkylarkDescriptionArgBuilder`]{.descfrmTypeLabel}
            :::

            ::: block
            Get an attribute\'s value after it was set in
            [`SkylarkDescriptionArgBuilder.setPostCoercionValue(String, Object)`](../coercer/SkylarkDescriptionArgBuilder.html#setPostCoercionValue(java.lang.String,java.lang.Object))
            It is an error to get an attribute that has not been set.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getPostCoercionValue` in
                interface `SkylarkDescriptionArgBuilder`

            [Parameters:]{.paramLabel}
            :   `attr` - The attribute to get the value for

            [Returns:]{.returnLabel}
            :   The value

        []{#build()}

        -   #### build

            ``` methodSignature
            public void build()
            ```

            ::: block
            \'Build\' the
            [`SkylarkDescriptionArg`](SkylarkDescriptionArg.html "class in com.facebook.buck.core.starlark.rule").
            After this has been called,
            [`setPostCoercionValue(String, Object)`](#setPostCoercionValue(java.lang.String,java.lang.Object))
            may not be called.
            :::

        []{#getRule()}

        -   #### getRule

            ``` methodSignature
            public SkylarkUserDefinedRule getRule()
            ```

            ::: block
            Get the
            [`SkylarkDescriptionArg`](SkylarkDescriptionArg.html "class in com.facebook.buck.core.starlark.rule")
            that has information about parameters and the user\'s
            implementation function
            :::

        []{#getName()}

        -   #### getName

            ``` methodSignature
            public String getName()
            ```

            ::: block
            [Description copied from
            interface: `ConstructorArg`]{.descfrmTypeLabel}
            :::

            ::: block
            Each rule has a name
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getName` in interface `ConstructorArg`

        []{#getDefaultTargetPlatform()}

        -   #### getDefaultTargetPlatform

            ``` methodSignature
            public Optional<UnconfiguredBuildTarget> getDefaultTargetPlatform()
            ```

            ::: block
            [Description copied from
            interface: `BuildRuleArg`]{.descfrmTypeLabel}
            :::

            ::: block
            The name of build target default \"new\" platform: it is
            used when a platform is not specified either globally or in
            a target which used this target as a dependency.
            The value is a build target, but we specify it as string,
            because this function is not actually called, but the attr
            is fetched by name from the raw (unconfigured) target node.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getDefaultTargetPlatform` in interface `BuildRuleArg`

        []{#getAllParamInfo()}

        -   #### getAllParamInfo

            ``` methodSignature
            public com.google.common.collect.ImmutableMap<String,​ParamInfo<?>> getAllParamInfo()
            ```

        []{#getImplementation()}

        -   #### getImplementation

            ``` methodSignature
            public com.google.devtools.build.lib.syntax.BaseFunction getImplementation()
            ```

        []{#getLicenses()}

        -   #### getLicenses

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<SourcePath> getLicenses()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getLicenses` in interface `BuildRuleArg`

        []{#getLabels()}

        -   #### getLabels

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedSet<String> getLabels()
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `getLabels` in interface `BuildRuleArg`

        []{#getContacts()}

        -   #### getContacts

            ``` methodSignature
            public com.google.common.collect.ImmutableSortedSet<String> getContacts()
            ```

            [Returns:]{.returnLabel}
            :   contacts for this rule, or an empty set of \`contacts\`
                was not set

        []{#getCompatibleWith()}

        -   #### getCompatibleWith

            ``` methodSignature
            public com.google.common.collect.ImmutableList<UnconfiguredBuildTarget> getCompatibleWith()
            ```

            ::: block
            [Description copied from
            interface: `BuildRuleArg`]{.descfrmTypeLabel}
            :::

            ::: block
            A list of `config_setting` a target is compatible with.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getCompatibleWith` in interface `BuildRuleArg`
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
