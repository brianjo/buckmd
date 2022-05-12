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
[Package]{.packageLabelInType} [com.facebook.buck.support.cli.config](package-summary.html)
:::

## Class AliasConfig {#class-aliasconfig .title title="Class AliasConfig"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.support.cli.config.AliasConfig

::: description
-   

    All Implemented Interfaces:
    :   `ConfigView<BuckConfig>`

    ------------------------------------------------------------------------

        public abstract class AliasConfig
        extends Object
        implements ConfigView<BuckConfig>

    ::: block
    Contains the logic for handling the \[alias\] section of
    .buckconfig.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor       Description
          ----------------- -------------
          `AliasConfig()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static AliasConfig`  | `fro                  |                       |
        |                       | m​(BuckConfig config)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.commo     | `getAliases()`        |                       |
        | n.collect.ImmutableSe |                       |                       |
        | tMultimap<String,​Unco |                       |                       |
        | nfiguredBuildTarget>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.g                | `getBuildTargetForAl  |                       |
        | oogle.common.collect. | iasAsString​(String po |                       |
        | ImmutableSet<String>` | ssiblyFlavoredAlias)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `c                    | `getBui               |                       |
        | om.google.common.coll | ldTargetsForAlias​(Str |                       |
        | ect.ImmutableSet<Unco | ing unflavoredAlias)` |                       |
        | nfiguredBuildTarget>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.google.c         | `getEntries()`        |                       |
        | ommon.collect.Immutab |                       |                       |
        | leMap<String,​String>` |                       |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static AliasConfig`  | `of​(                  |                       |
        |                       | BuckConfig delegate)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `com.go               | `resolveAliases​(Ite   | ::: block             |
        | ogle.common.collect.I | rable<String> input)` | Accept a list of      |
        | mmutableList<String>` |                       | strings and for those |
        |                       |                       | of them which are     |
        |                       |                       | configured aliases,   |
        |                       |                       | convert them to       |
        |                       |                       | appropriate aliased   |
        |                       |                       | values.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static void`         | `validateAliasNa      |                       |
        |                       | me​(String aliasName)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static void`         | `validateLabelNa      |                       |
        |                       | me​(String aliasName)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Instance
        Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.core.config.ConfigView}

            ### Methods inherited from interface com.facebook.buck.core.config.[ConfigView](../../../core/config/ConfigView.html "interface in com.facebook.buck.core.config")

            `getDelegate`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### AliasConfig

                public AliasConfig()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#from(com.facebook.buck.core.config.BuckConfig)}

        -   #### from

            ``` methodSignature
            public static AliasConfig from​(BuckConfig config)
            ```

        []{#of(com.facebook.buck.core.config.BuckConfig)}

        -   #### of

            ``` methodSignature
            public static AliasConfig of​(BuckConfig delegate)
            ```

        []{#getEntries()}

        -   #### getEntries

            ``` methodSignature
            public com.google.common.collect.ImmutableMap<String,​String> getEntries()
            ```

        []{#resolveAliases(java.lang.Iterable)}

        -   #### resolveAliases

            ``` methodSignature
            public com.google.common.collect.ImmutableList<String> resolveAliases​(Iterable<String> input)
            ```

            ::: block
            Accept a list of strings and for those of them which are
            configured aliases, convert them to appropriate aliased
            values. The order of the resulting list does not change.
            :::

        []{#getAliases()}

        -   #### getAliases

            ``` methodSignature
            @Lazy
            public com.google.common.collect.ImmutableSetMultimap<String,​UnconfiguredBuildTarget> getAliases()
            ```

        []{#getBuildTargetForAliasAsString(java.lang.String)}

        -   #### getBuildTargetForAliasAsString

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<String> getBuildTargetForAliasAsString​(String possiblyFlavoredAlias)
            ```

        []{#getBuildTargetsForAlias(java.lang.String)}

        -   #### getBuildTargetsForAlias

            ``` methodSignature
            public com.google.common.collect.ImmutableSet<UnconfiguredBuildTarget> getBuildTargetsForAlias​(String unflavoredAlias)
            ```

        []{#validateAliasName(java.lang.String)}

        -   #### validateAliasName

            ``` methodSignature
            public static void validateAliasName​(String aliasName)
                                          throws HumanReadableException
            ```

            [Throws:]{.throwsLabel}
            :   `HumanReadableException`

        []{#validateLabelName(java.lang.String)}

        -   #### validateLabelName

            ``` methodSignature
            public static void validateLabelName​(String aliasName)
                                          throws HumanReadableException
            ```

            [Throws:]{.throwsLabel}
            :   `HumanReadableException`
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
