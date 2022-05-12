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
-   [Nested](#nested.class.summary) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.command.config](package-summary.html)
:::

## Class ConfigDifference {#class-configdifference .title title="Class ConfigDifference"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.command.config.ConfigDifference

::: description
-   

    ------------------------------------------------------------------------

        public class ConfigDifference
        extends Object

    ::: block
    Helper methods for calculating and logging the config differences
    that cause state invalidation
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static interface `   | `ConfigDif            | ::: block             |
        |                       | ference.ConfigChange` | A single changed      |
        |                       |                       | config value          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor            Description
          ---------------------- -------------
          `ConfigDifference()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static               | `compa                | ::: block             |
        | Map<String,​ConfigDiff | re​(Config config1,    | Compares all values   |
        | erence.ConfigChange>` |      Config config2)` | in two sets of        |
        |                       |                       | configs               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static               | `compare​(co           | ::: block             |
        | Map<String,​ConfigDiff | m.google.common.colle | Compares sets of      |
        | erence.ConfigChange>` | ct.ImmutableMap<Strin | config options, and   |
        |                       | g,​com.google.common.c | returns the           |
        |                       | ollect.ImmutableMap<S | difference as a map   |
        |                       | tring,​String>> rawCon | of \'section.key\'    |
        |                       | fig1,        com.goog | strings to pairs      |
        |                       | le.common.collect.Imm | containing the        |
        |                       | utableMap<String,​com. | different values.     |
        |                       | google.common.collect | :::                   |
        |                       | .ImmutableMap<String, |                       |
        |                       | ​String>> rawConfig2)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static               | `compareForCaching​(Bu | ::: block             |
        | Map<String,​ConfigDiff | ckConfig buckConfig1, | Compares only the     |
        | erence.ConfigChange>` |                   Buc | config options that   |
        |                       | kConfig buckConfig2)` | invalidate global     |
        |                       |                       | state                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static String`       | `format               | ::: block             |
        |                       | ConfigChange​(Map.Entr | Format a single       |
        |                       | y<String,​ConfigDiffer | config change         |
        |                       | ence.ConfigChange> ch | :::                   |
        |                       | ange,                 |                       |
        |                       |    boolean truncate)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static String`       | `fo                   | ::: block             |
        |                       | rmatConfigDiff​(Map<St | Format the full set   |
        |                       | ring,​ConfigDifference | of changes between    |
        |                       | .ConfigChange> diff)` | configs to be logged  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static String`       | `                     | ::: block             |
        |                       | formatConfigDiffShort | Format a set of       |
        |                       | ​(Map<String,​ConfigDif | changes between       |
        |                       | ference.ConfigChange> | configs for the       |
        |                       |  diff,                | console               |
        |                       |        int maxLines)` | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
        .tableTab}[[Concrete
        Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>()}

        -   #### ConfigDifference

                public ConfigDifference()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#compare(com.facebook.buck.util.config.Config,com.facebook.buck.util.config.Config)}

        -   #### compare

            ``` methodSignature
            public static Map<String,​ConfigDifference.ConfigChange> compare​(Config config1,
                                                                                  Config config2)
            ```

            ::: block
            Compares all values in two sets of configs
            :::

        []{#compareForCaching(com.facebook.buck.core.config.BuckConfig,com.facebook.buck.core.config.BuckConfig)}

        -   #### compareForCaching

            ``` methodSignature
            public static Map<String,​ConfigDifference.ConfigChange> compareForCaching​(BuckConfig buckConfig1,
                                                                                            BuckConfig buckConfig2)
            ```

            ::: block
            Compares only the config options that invalidate global
            state
            :::

            [Returns:]{.returnLabel}
            :   The difference as a map of \'section.key\' strings to
                changed values

        []{#compare(com.google.common.collect.ImmutableMap,com.google.common.collect.ImmutableMap)}

        -   #### compare

            ``` methodSignature
            public static Map<String,​ConfigDifference.ConfigChange> compare​(com.google.common.collect.ImmutableMap<String,​com.google.common.collect.ImmutableMap<String,​String>> rawConfig1,
                                                                                  com.google.common.collect.ImmutableMap<String,​com.google.common.collect.ImmutableMap<String,​String>> rawConfig2)
            ```

            ::: block
            Compares sets of config options, and returns the difference
            as a map of \'section.key\' strings to pairs containing the
            different values.
            :::

        []{#formatConfigDiffShort(java.util.Map,int)}

        -   #### formatConfigDiffShort

            ``` methodSignature
            public static String formatConfigDiffShort​(Map<String,​ConfigDifference.ConfigChange> diff,
                                                       int maxLines)
            ```

            ::: block
            Format a set of changes between configs for the console
            :::

        []{#formatConfigDiff(java.util.Map)}

        -   #### formatConfigDiff

            ``` methodSignature
            public static String formatConfigDiff​(Map<String,​ConfigDifference.ConfigChange> diff)
            ```

            ::: block
            Format the full set of changes between configs to be logged
            :::

        []{#formatConfigChange(java.util.Map.Entry,boolean)}

        -   #### formatConfigChange

            ``` methodSignature
            public static String formatConfigChange​(Map.Entry<String,​ConfigDifference.ConfigChange> change,
                                                    boolean truncate)
            ```

            ::: block
            Format a single config change
            :::
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
-   [Nested](#nested.class.summary) \| 
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
