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
[Package]{.packageLabelInType} [com.facebook.buck.core.rules.knowntypes](package-summary.html)
:::

## Class KnownNativeRuleTypes {#class-knownnativeruletypes .title title="Class KnownNativeRuleTypes"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.rules.knowntypes.KnownNativeRuleTypes

::: description
-   

    All Implemented Interfaces:
    :   `KnownRuleTypes`

    ------------------------------------------------------------------------

        public abstract class KnownNativeRuleTypes
        extends Object
        implements KnownRuleTypes

    ::: block
    Provides access to rule types.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                Description
          -------------------------- -------------
          `KnownNativeRuleTypes()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `protected void`      | `check()`             |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.common.   | `getDescriptions()`   |                       |
        | collect.ImmutableList |                       |                       |
        | <BaseDescription<?>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `protected com.g      | `get                  |                       |
        | oogle.common.collect. | DescriptionsByRule()` |                       |
        | ImmutableMap<RuleType |                       |                       |
        | ,​BaseDescription<?>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `RuleDescriptor<?>`   | `getDescripto         | ::: block             |
        |                       | rByName​(String name)` | Get rule type,        |
        |                       |                       | constructor arg and   |
        |                       |                       | description object    |
        |                       |                       | for by rule name.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ab                   | `getKnow              |                       |
        | stract com.google.com | nBuildDescriptions()` |                       |
        | mon.collect.Immutable |                       |                       |
        | List<Description<?>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getKnownConfigu      |                       |
        | abstract com.google.c | rationDescriptions()` |                       |
        | ommon.collect.Immutab |                       |                       |
        | leList<ConfigurationR |                       |                       |
        | uleDescription<?,​?>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.com       | `ge                   |                       |
        | mon.collect.Immutable | tNativeTypesByName()` |                       |
        | Map<String,​RuleType>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `abstra               | `getP                 |                       |
        | ct com.google.common. | erFeatureProviders()` |                       |
        | collect.ImmutableList |                       |                       |
        | <BuiltInProvider<?>>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static               | `of                   |                       |
        | KnownNativeRuleTypes` | ​(com.google.common.co |                       |
        |                       | llect.ImmutableList<D |                       |
        |                       | escription<?>> knownB |                       |
        |                       | uildDescriptions,   c |                       |
        |                       | om.google.common.coll |                       |
        |                       | ect.ImmutableList<Con |                       |
        |                       | figurationRuleDescrip |                       |
        |                       | tion<?,​?>> knownConfi |                       |
        |                       | gurationDescriptions, |                       |
        |                       |    com.google.common. |                       |
        |                       | collect.ImmutableList |                       |
        |                       | <BuiltInProvider<?>>  |                       |
        |                       | perFeatureProviders)` |                       |
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
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.knowntypes.KnownRuleTypes}

            ### Methods inherited from interface com.facebook.buck.core.rules.knowntypes.[KnownRuleTypes](KnownRuleTypes.html "interface in com.facebook.buck.core.rules.knowntypes")

            `getDescriptorByNameChecked`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### KnownNativeRuleTypes

                public KnownNativeRuleTypes()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getKnownBuildDescriptions()}

        -   #### getKnownBuildDescriptions

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableList<Description<?>> getKnownBuildDescriptions()
            ```

        []{#getKnownConfigurationDescriptions()}

        -   #### getKnownConfigurationDescriptions

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableList<ConfigurationRuleDescription<?,​?>> getKnownConfigurationDescriptions()
            ```

        []{#getPerFeatureProviders()}

        -   #### getPerFeatureProviders

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableList<BuiltInProvider<?>> getPerFeatureProviders()
            ```

        []{#getNativeTypesByName()}

        -   #### getNativeTypesByName

            ``` methodSignature
            @Lazy
            public com.google.common.collect.ImmutableMap<String,​RuleType> getNativeTypesByName()
            ```

        []{#getDescriptions()}

        -   #### getDescriptions

            ``` methodSignature
            @Lazy
            public com.google.common.collect.ImmutableList<BaseDescription<?>> getDescriptions()
            ```

            [Returns:]{.returnLabel}
            :   all known descriptions

        []{#getDescriptionsByRule()}

        -   #### getDescriptionsByRule

            ``` methodSignature
            @Lazy
            protected com.google.common.collect.ImmutableMap<RuleType,​BaseDescription<?>> getDescriptionsByRule()
            ```

            [Returns:]{.returnLabel}
            :   all descriptions organized by their
                [`RuleType`](../../model/RuleType.html "class in com.facebook.buck.core.model").

        []{#getDescriptorByName(java.lang.String)}

        -   #### getDescriptorByName

            ``` methodSignature
            public RuleDescriptor<?> getDescriptorByName​(String name)
            ```

            ::: block
            [Description copied from
            interface: `KnownRuleTypes`]{.descfrmTypeLabel}
            :::

            ::: block
            Get rule type, constructor arg and description object for by
            rule name.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getDescriptorByName` in interface `KnownRuleTypes`

        []{#check()}

        -   #### check

            ``` methodSignature
            @Check
            protected void check()
            ```

        []{#of(com.google.common.collect.ImmutableList,com.google.common.collect.ImmutableList,com.google.common.collect.ImmutableList)}

        -   #### of

            ``` methodSignature
            public static KnownNativeRuleTypes of​(com.google.common.collect.ImmutableList<Description<?>> knownBuildDescriptions,
                                                  com.google.common.collect.ImmutableList<ConfigurationRuleDescription<?,​?>> knownConfigurationDescriptions,
                                                  com.google.common.collect.ImmutableList<BuiltInProvider<?>> perFeatureProviders)
            ```
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
