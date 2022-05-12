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
-   Field \| 
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   Constr \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.core.rules.configsetting](package-summary.html)
:::

## Class ConfigSettingArg.Builder {#class-configsettingarg.builder .title title="Class ConfigSettingArg.Builder"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.rules.configsetting.ConfigSettingArg.Builder

::: description
-   

    Enclosing class:
    :   [ConfigSettingArg](ConfigSettingArg.html "class in com.facebook.buck.core.rules.configsetting")

    ------------------------------------------------------------------------

        @NotThreadSafe
        public static final class ConfigSettingArg.Builder
        extends Object

    ::: block
    Builds instances of type
    [`ConfigSettingArg`](ConfigSettingArg.html "class in com.facebook.buck.core.rules.configsetting").
    Initialize attributes and then invoke the [`build()`](#build())
    method to create an immutable instance.
    *`Builder` is not thread-safe and generally should not be stored in
    a field or collection, but instead used immediately to create
    instances.*
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `Conf                 | `addAllConstrai       | ::: block             |
        | igSettingArg.Builder` | ntValues​(Iterable<? e | Adds elements to      |
        |                       | xtends UnconfiguredBu | [`                    |
        |                       | ildTarget> elements)` | constraintValues`](Co |
        |                       |                       | nfigSettingArg.html#g |
        |                       |                       | etConstraintValues()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Conf                 | `addConstrai          | ::: block             |
        | igSettingArg.Builder` | ntValues​(Unconfigured | Adds one element to   |
        |                       | BuildTarget element)` | [`                    |
        |                       |                       | constraintValues`](Co |
        |                       |                       | nfigSettingArg.html#g |
        |                       |                       | etConstraintValues()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Conf                 | `addConstraintVa      | ::: block             |
        | igSettingArg.Builder` | lues​(UnconfiguredBuil | Adds elements to      |
        |                       | dTarget... elements)` | [`                    |
        |                       |                       | constraintValues`](Co |
        |                       |                       | nfigSettingArg.html#g |
        |                       |                       | etConstraintValues()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ConfigSettingArg`    | `build()`             | ::: block             |
        |                       |                       | Builds a new          |
        |                       |                       | [`ConfigSettin        |
        |                       |                       | gArg`](ConfigSettingA |
        |                       |                       | rg.html "class in com |
        |                       |                       | .facebook.buck.core.r |
        |                       |                       | ules.configsetting"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Conf                 | `from​(Cons            | ::: block             |
        | igSettingArg.Builder` | tructorArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook         |
        |                       |                       | .buck.core.descriptio |
        |                       |                       | n.arg.ConstructorArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Conf                 | `from​(Config          | ::: block             |
        | igSettingArg.Builder` | SettingArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `ConfigSettingArg`    |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Conf                 | `fro                  | ::: block             |
        | igSettingArg.Builder` | m​(com.facebook.buck.c | Copy abstract value   |
        |                       | ore.rules.configsetti | type                  |
        |                       | ng.ConfigSettingDescr | `Abst                 |
        |                       | iption.AbstractConfig | ractConfigSettingArg` |
        |                       | SettingArg instance)` | instance into         |
        |                       |                       | builder.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Conf                 | `putAllVal            | ::: block             |
        | igSettingArg.Builder` | ues​(Map<String,​? exte | Put all mappings from |
        |                       | nds String> entries)` | the specified map as  |
        |                       |                       | entries to            |
        |                       |                       | [`v                   |
        |                       |                       | alues`](ConfigSetting |
        |                       |                       | Arg.html#getValues()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Conf                 | `put                  | ::: block             |
        | igSettingArg.Builder` | Values​(String key,    | Put one entry to the  |
        |                       |        String value)` | [`v                   |
        |                       |                       | alues`](ConfigSetting |
        |                       |                       | Arg.html#getValues()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Conf                 | `putValues​(           | ::: block             |
        | igSettingArg.Builder` | Map.Entry<String,​? ex | Put one entry to the  |
        |                       | tends String> entry)` | [`v                   |
        |                       |                       | alues`](ConfigSetting |
        |                       |                       | Arg.html#getValues()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Conf                 | `setConstrai          | ::: block             |
        | igSettingArg.Builder` | ntValues​(Iterable<? e | Sets or replaces all  |
        |                       | xtends UnconfiguredBu | elements for          |
        |                       | ildTarget> elements)` | [`                    |
        |                       |                       | constraintValues`](Co |
        |                       |                       | nfigSettingArg.html#g |
        |                       |                       | etConstraintValues()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Conf                 | `                     | ::: block             |
        | igSettingArg.Builder` | setName​(String name)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`name`](ConfigSetti  |
        |                       |                       | ngArg.html#getName()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Conf                 | `setVal               | ::: block             |
        | igSettingArg.Builder` | ues​(Map<String,​? exte | Sets or replaces all  |
        |                       | nds String> entries)` | mappings from the     |
        |                       |                       | specified map as      |
        |                       |                       | entries for the       |
        |                       |                       | [`v                   |
        |                       |                       | alues`](ConfigSetting |
        |                       |                       | Arg.html#getValues()) |
        |                       |                       | map.                  |
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
    -   []{#method.detail}

        ### Method Detail

        []{#from(com.facebook.buck.core.rules.configsetting.ConfigSettingArg)}

        -   #### from

            ``` methodSignature
            public final ConfigSettingArg.Builder from​(ConfigSettingArg instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `ConfigSettingArg` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.core.rules.configsetting.ConfigSettingDescription.AbstractConfigSettingArg)}

        -   #### from

            ``` methodSignature
            public final ConfigSettingArg.Builder from​(com.facebook.buck.core.rules.configsetting.ConfigSettingDescription.AbstractConfigSettingArg instance)
            ```

            ::: block
            Copy abstract value type `AbstractConfigSettingArg` instance
            into builder.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.core.description.arg.ConstructorArg)}

        -   #### from

            ``` methodSignature
            public final ConfigSettingArg.Builder from​(ConstructorArg instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `com.facebook.buck.core.description.arg.ConstructorArg`
            instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putValues(java.lang.String,java.lang.String)}

        -   #### putValues

            ``` methodSignature
            public final ConfigSettingArg.Builder putValues​(String key,
                                                            String value)
            ```

            ::: block
            Put one entry to the
            [`values`](ConfigSettingArg.html#getValues()) map.
            :::

            [Parameters:]{.paramLabel}
            :   `key` - The key in the values map
            :   `value` - The associated value in the values map

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putValues(java.util.Map.Entry)}

        -   #### putValues

            ``` methodSignature
            public final ConfigSettingArg.Builder putValues​(Map.Entry<String,​? extends String> entry)
            ```

            ::: block
            Put one entry to the
            [`values`](ConfigSettingArg.html#getValues()) map. Nulls are
            not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entry` - The key and value entry

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setValues(java.util.Map)}

        -   #### setValues

            ``` methodSignature
            public final ConfigSettingArg.Builder setValues​(Map<String,​? extends String> entries)
            ```

            ::: block
            Sets or replaces all mappings from the specified map as
            entries for the
            [`values`](ConfigSettingArg.html#getValues()) map. Nulls are
            not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entries` - The entries that will be added to the values
                map

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putAllValues(java.util.Map)}

        -   #### putAllValues

            ``` methodSignature
            public final ConfigSettingArg.Builder putAllValues​(Map<String,​? extends String> entries)
            ```

            ::: block
            Put all mappings from the specified map as entries to
            [`values`](ConfigSettingArg.html#getValues()) map. Nulls are
            not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entries` - The entries that will be added to the values
                map

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addConstraintValues(com.facebook.buck.core.model.UnconfiguredBuildTarget)}

        -   #### addConstraintValues

            ``` methodSignature
            public final ConfigSettingArg.Builder addConstraintValues​(UnconfiguredBuildTarget element)
            ```

            ::: block
            Adds one element to
            [`constraintValues`](ConfigSettingArg.html#getConstraintValues())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A constraintValues element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addConstraintValues(com.facebook.buck.core.model.UnconfiguredBuildTarget...)}

        -   #### addConstraintValues

            ``` methodSignature
            public final ConfigSettingArg.Builder addConstraintValues​(UnconfiguredBuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`constraintValues`](ConfigSettingArg.html#getConstraintValues())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of constraintValues elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setConstraintValues(java.lang.Iterable)}

        -   #### setConstraintValues

            ``` methodSignature
            public final ConfigSettingArg.Builder setConstraintValues​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`constraintValues`](ConfigSettingArg.html#getConstraintValues())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of constraintValues elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllConstraintValues(java.lang.Iterable)}

        -   #### addAllConstraintValues

            ``` methodSignature
            public final ConfigSettingArg.Builder addAllConstraintValues​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`constraintValues`](ConfigSettingArg.html#getConstraintValues())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of constraintValues elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setName(java.lang.String)}

        -   #### setName

            ``` methodSignature
            public final ConfigSettingArg.Builder setName​(String name)
            ```

            ::: block
            Initializes the value for the
            [`name`](ConfigSettingArg.html#getName()) attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `name` - The value for name

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#build()}

        -   #### build

            ``` methodSignature
            public ConfigSettingArg build()
            ```

            ::: block
            Builds a new
            [`ConfigSettingArg`](ConfigSettingArg.html "class in com.facebook.buck.core.rules.configsetting").
            :::

            [Returns:]{.returnLabel}
            :   An immutable instance of ConfigSettingArg

            [Throws:]{.throwsLabel}
            :   `IllegalStateException` - if any required attributes are
                missing
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
-   Field \| 
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   Constr \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
