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
[Package]{.packageLabelInType} [com.facebook.buck.core.starlark.knowntypes](package-summary.html)
:::

## Class KnownUserDefinedRuleTypes {#class-knownuserdefinedruletypes .title title="Class KnownUserDefinedRuleTypes"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.starlark.knowntypes.KnownUserDefinedRuleTypes

::: description
-   

    All Implemented Interfaces:
    :   `KnownRuleTypes`

    ------------------------------------------------------------------------

        public class KnownUserDefinedRuleTypes
        extends Object
        implements KnownRuleTypes

    ::: block
    Maps \`buck.type\` values to
    [`SkylarkUserDefinedRule`](../rule/SkylarkUserDefinedRule.html "class in com.facebook.buck.core.starlark.rule")
    instances. The lifetime of this object is currently global per cell,
    however in the future we may handle invoking the parse pipeline
    multiple times concurrently differently.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                     Description
          ------------------------------- -------------
          `KnownUserDefinedRuleTypes()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `void`                | `addRule​(SkylarkU     | ::: block             |
        |                       | serDefinedRule rule)` | Adds a rule to the    |
        |                       |                       | internal cache        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `RuleDescriptor<?>`   | `getDescripto         | ::: block             |
        |                       | rByName​(String name)` | Get rule type,        |
        |                       |                       | constructor arg and   |
        |                       |                       | description object    |
        |                       |                       | for by rule name.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Sk                   | `getRule​(String ra    | ::: block             |
        | ylarkUserDefinedRule` | wBuckTypeIdentifier)` | Get a rule based on   |
        |                       |                       | its name              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `void`                | `invalidateEx         | ::: block             |
        |                       | tension​(com.google.de | Invalidates all rules |
        |                       | vtools.build.lib.cmdl | found in a specific   |
        |                       | ine.Label extension)` | extension file        |
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
        -   []{#methods.inherited.from.class.com.facebook.buck.core.rules.knowntypes.KnownRuleTypes}

            ### Methods inherited from interface com.facebook.buck.core.rules.knowntypes.[KnownRuleTypes](../../rules/knowntypes/KnownRuleTypes.html "interface in com.facebook.buck.core.rules.knowntypes")

            `getDescriptorByNameChecked`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### KnownUserDefinedRuleTypes

                public KnownUserDefinedRuleTypes()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#addRule(com.facebook.buck.core.starlark.rule.SkylarkUserDefinedRule)}

        -   #### addRule

            ``` methodSignature
            public void addRule​(SkylarkUserDefinedRule rule)
            ```

            ::: block
            Adds a rule to the internal cache
            NOTE: This can only be called on a rule that has been
            exported
            :::

            [Parameters:]{.paramLabel}
            :   `rule` - The rule to cache

        []{#getRule(java.lang.String)}

        -   #### getRule

            ``` methodSignature
            @Nullable
            public SkylarkUserDefinedRule getRule​(String rawBuckTypeIdentifier)
            ```

            ::: block
            Get a rule based on its name
            :::

            [Parameters:]{.paramLabel}
            :   `rawBuckTypeIdentifier` - The name of the rule from
                \`buck.type\` in the parser, or
                [`SkylarkUserDefinedRule.getName()`](../rule/SkylarkUserDefinedRule.html#getName()))

            [Returns:]{.returnLabel}
            :   The rule, or `null` if not found

        []{#invalidateExtension(com.google.devtools.build.lib.cmdline.Label)}

        -   #### invalidateExtension

            ``` methodSignature
            public void invalidateExtension​(com.google.devtools.build.lib.cmdline.Label extension)
            ```

            ::: block
            Invalidates all rules found in a specific extension file
            :::

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
