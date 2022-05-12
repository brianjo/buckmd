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

-   [Overview](../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../deprecated-list.html)
-   [Index](../../../../index-all.html)
-   [Help](../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.android](package-summary.html)
:::

## Class AndroidAppModularityDescriptionArg.Builder {#class-androidappmodularitydescriptionarg.builder .title title="Class AndroidAppModularityDescriptionArg.Builder"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.android.AndroidAppModularityDescriptionArg.Builder

::: description
-   

    Enclosing class:
    :   [AndroidAppModularityDescriptionArg](AndroidAppModularityDescriptionArg.html "class in com.facebook.buck.android")

    ------------------------------------------------------------------------

        @NotThreadSafe
        public static final class AndroidAppModularityDescriptionArg.Builder
        extends Object

    ::: block
    Builds instances of type
    [`AndroidAppModularityDescriptionArg`](AndroidAppModularityDescriptionArg.html "class in com.facebook.buck.android").
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
        | `A                    | `addAllCompat         | ::: block             |
        | ndroidAppModularityDe | ibleWith​(Iterable<? e | Adds elements to      |
        | scriptionArg.Builder` | xtends UnconfiguredBu | [`compatibleWith      |
        |                       | ildTarget> elements)` | `](AndroidAppModulari |
        |                       |                       | tyDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `A                    | `addAllDeps​(          | ::: block             |
        | ndroidAppModularityDe | Iterable<? extends Bu | Adds elements to      |
        | scriptionArg.Builder` | ildTarget> elements)` | [`deps`](AndroidA     |
        |                       |                       | ppModularityDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `A                    | `addAllLabels​(Iterab  | ::: block             |
        | ndroidAppModularityDe | le<String> elements)` | Adds elements to      |
        | scriptionArg.Builder` |                       | [`labels`](AndroidApp |
        |                       |                       | ModularityDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `A                    | `addAllLicenses       | ::: block             |
        | ndroidAppModularityDe | ​(Iterable<? extends S | Adds elements to      |
        | scriptionArg.Builder` | ourcePath> elements)` | [`li                  |
        |                       |                       | censes`](AndroidAppMo |
        |                       |                       | dularityDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `A                    | `addAllNoDx​(          | ::: block             |
        | ndroidAppModularityDe | Iterable<? extends Bu | Adds elements to      |
        | scriptionArg.Builder` | ildTarget> elements)` | [`noDx`](AndroidA     |
        |                       |                       | ppModularityDescripti |
        |                       |                       | onArg.html#getNoDx()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `A                    | `addCompat            | ::: block             |
        | ndroidAppModularityDe | ibleWith​(Unconfigured | Adds one element to   |
        | scriptionArg.Builder` | BuildTarget element)` | [`compatibleWith      |
        |                       |                       | `](AndroidAppModulari |
        |                       |                       | tyDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `A                    | `addCompatible        | ::: block             |
        | ndroidAppModularityDe | With​(UnconfiguredBuil | Adds elements to      |
        | scriptionArg.Builder` | dTarget... elements)` | [`compatibleWith      |
        |                       |                       | `](AndroidAppModulari |
        |                       |                       | tyDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `A                    | `addDeps​(             | ::: block             |
        | ndroidAppModularityDe | BuildTarget element)` | Adds one element to   |
        | scriptionArg.Builder` |                       | [`deps`](AndroidA     |
        |                       |                       | ppModularityDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `A                    | `addDeps​(Buil         | ::: block             |
        | ndroidAppModularityDe | dTarget... elements)` | Adds elements to      |
        | scriptionArg.Builder` |                       | [`deps`](AndroidA     |
        |                       |                       | ppModularityDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `A                    | `addLa                | ::: block             |
        | ndroidAppModularityDe | bels​(String element)` | Adds one element to   |
        | scriptionArg.Builder` |                       | [`labels`](AndroidApp |
        |                       |                       | ModularityDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `A                    | `addLabels            | ::: block             |
        | ndroidAppModularityDe | ​(String... elements)` | Adds elements to      |
        | scriptionArg.Builder` |                       | [`labels`](AndroidApp |
        |                       |                       | ModularityDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `A                    | `addLicenses          | ::: block             |
        | ndroidAppModularityDe | ​(SourcePath element)` | Adds one element to   |
        | scriptionArg.Builder` |                       | [`li                  |
        |                       |                       | censes`](AndroidAppMo |
        |                       |                       | dularityDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `A                    | `addLicenses​(Sou      | ::: block             |
        | ndroidAppModularityDe | rcePath... elements)` | Adds elements to      |
        | scriptionArg.Builder` |                       | [`li                  |
        |                       |                       | censes`](AndroidAppMo |
        |                       |                       | dularityDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `A                    | `addNoDx​(             | ::: block             |
        | ndroidAppModularityDe | BuildTarget element)` | Adds one element to   |
        | scriptionArg.Builder` |                       | [`noDx`](AndroidA     |
        |                       |                       | ppModularityDescripti |
        |                       |                       | onArg.html#getNoDx()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `A                    | `addNoDx​(Buil         | ::: block             |
        | ndroidAppModularityDe | dTarget... elements)` | Adds elements to      |
        | scriptionArg.Builder` |                       | [`noDx`](AndroidA     |
        |                       |                       | ppModularityDescripti |
        |                       |                       | onArg.html#getNoDx()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidAppModu       | `build()`             | ::: block             |
        | larityDescriptionArg` |                       | Builds a new          |
        |                       |                       | [`AndroidApp          |
        |                       |                       | ModularityDescription |
        |                       |                       | Arg`](AndroidAppModul |
        |                       |                       | arityDescriptionArg.h |
        |                       |                       | tml "class in com.fac |
        |                       |                       | ebook.buck.android"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `A                    | `from​(com.fa          | ::: block             |
        | ndroidAppModularityDe | cebook.buck.android.A | Copy abstract value   |
        | scriptionArg.Builder` | ndroidAppModularityDe | type                  |
        |                       | scription.AbstractAnd | `A                    |
        |                       | roidAppModularityDesc | bstractAndroidAppModu |
        |                       | riptionArg instance)` | larityDescriptionArg` |
        |                       |                       | instance into         |
        |                       |                       | builder.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `A                    | `from​(And             | ::: block             |
        | ndroidAppModularityDe | roidAppModularityDesc | Fill a builder with   |
        | scriptionArg.Builder` | riptionArg instance)` | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `AndroidAppModu       |
        |                       |                       | larityDescriptionArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `A                    | `from​(Bu              | ::: block             |
        | ndroidAppModularityDe | ildRuleArg instance)` | Fill a builder with   |
        | scriptionArg.Builder` |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebo           |
        |                       |                       | ok.buck.core.descript |
        |                       |                       | ion.arg.BuildRuleArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `A                    | `from​(Cons            | ::: block             |
        | ndroidAppModularityDe | tructorArg instance)` | Fill a builder with   |
        | scriptionArg.Builder` |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook         |
        |                       |                       | .buck.core.descriptio |
        |                       |                       | n.arg.ConstructorArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `A                    | `fro                  | ::: block             |
        | ndroidAppModularityDe | m​(HasApplicationModul | Fill a builder with   |
        | scriptionArg.Builder` | eBlacklist instance)` | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.fa               |
        |                       |                       | cebook.buck.core.desc |
        |                       |                       | ription.arg.HasApplic |
        |                       |                       | ationModuleBlacklist` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `A                    | `from​(HasDe           | ::: block             |
        | ndroidAppModularityDe | claredDeps instance)` | Fill a builder with   |
        | scriptionArg.Builder` |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook.        |
        |                       |                       | buck.core.description |
        |                       |                       | .arg.HasDeclaredDeps` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `A                    | `putAllAppl           | ::: block             |
        | ndroidAppModularityDe | icationModuleConfigs​( | Put all mappings from |
        | scriptionArg.Builder` | Map<String,​? extends  | the specified map as  |
        |                       | com.google.common.col | entries to            |
        |                       | lect.ImmutableList<Bu | [`applicationMo       |
        |                       | ildTarget>> entries)` | duleConfigs`](Android |
        |                       |                       | AppModularityDescript |
        |                       |                       | ionArg.html#getApplic |
        |                       |                       | ationModuleConfigs()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `A                    | `p                    | ::: block             |
        | ndroidAppModularityDe | utApplicationModuleCo | Put one entry to the  |
        | scriptionArg.Builder` | nfigs​(String key,     | [`applicationMo       |
        |                       |                       | duleConfigs`](Android |
        |                       |    com.google.common. | AppModularityDescript |
        |                       | collect.ImmutableList | ionArg.html#getApplic |
        |                       | <BuildTarget> value)` | ationModuleConfigs()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `A                    | `putApplicat          | ::: block             |
        | ndroidAppModularityDe | ionModuleConfigs​(Map. | Put one entry to the  |
        | scriptionArg.Builder` | Entry<String,​? extend | [`applicationMo       |
        |                       | s com.google.common.c | duleConfigs`](Android |
        |                       | ollect.ImmutableList< | AppModularityDescript |
        |                       | BuildTarget>> entry)` | ionArg.html#getApplic |
        |                       |                       | ationModuleConfigs()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `A                    | `setAppl              | ::: block             |
        | ndroidAppModularityDe | icationModuleBlacklis | Initializes the       |
        | scriptionArg.Builder` | t​(List<Query> applica | optional value        |
        |                       | tionModuleBlacklist)` | [`applicationModule   |
        |                       |                       | Blacklist`](AndroidAp |
        |                       |                       | pModularityDescriptio |
        |                       |                       | nArg.html#getApplicat |
        |                       |                       | ionModuleBlacklist()) |
        |                       |                       | to                    |
        |                       |                       | applic                |
        |                       |                       | ationModuleBlacklist. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `A                    | `setApp               | ::: block             |
        | ndroidAppModularityDe | licationModuleBlackli | Initializes the       |
        | scriptionArg.Builder` | st​(Optional<? extends | optional value        |
        |                       |  List<Query>> applica | [`applicationModule   |
        |                       | tionModuleBlacklist)` | Blacklist`](AndroidAp |
        |                       |                       | pModularityDescriptio |
        |                       |                       | nArg.html#getApplicat |
        |                       |                       | ionModuleBlacklist()) |
        |                       |                       | to                    |
        |                       |                       | applic                |
        |                       |                       | ationModuleBlacklist. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `A                    | `setAppl              | ::: block             |
        | ndroidAppModularityDe | icationModuleConfigs​( | Sets or replaces all  |
        | scriptionArg.Builder` | Map<String,​? extends  | mappings from the     |
        |                       | com.google.common.col | specified map as      |
        |                       | lect.ImmutableList<Bu | entries for the       |
        |                       | ildTarget>> entries)` | [`applicationMo       |
        |                       |                       | duleConfigs`](Android |
        |                       |                       | AppModularityDescript |
        |                       |                       | ionArg.html#getApplic |
        |                       |                       | ationModuleConfigs()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `A                    | `setApplicati         | ::: block             |
        | ndroidAppModularityDe | onModuleDependencies​( | Initializes the       |
        | scriptionArg.Builder` | com.google.common.col | optional value        |
        |                       | lect.ImmutableMap<Str | [`ap                  |
        |                       | ing,​com.google.common | plicationModuleDepend |
        |                       | .collect.ImmutableLis | encies`](AndroidAppMo |
        |                       | t<String>> applicatio | dularityDescriptionAr |
        |                       | nModuleDependencies)` | g.html#getApplication |
        |                       |                       | ModuleDependencies()) |
        |                       |                       | to                    |
        |                       |                       | applicati             |
        |                       |                       | onModuleDependencies. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `A                    | `setApplicat          | ::: block             |
        | ndroidAppModularityDe | ionModuleDependencies | Initializes the       |
        | scriptionArg.Builder` | ​(Optional<? extends c | optional value        |
        |                       | om.google.common.coll | [`ap                  |
        |                       | ect.ImmutableMap<Stri | plicationModuleDepend |
        |                       | ng,​com.google.common. | encies`](AndroidAppMo |
        |                       | collect.ImmutableList | dularityDescriptionAr |
        |                       | <String>>> applicatio | g.html#getApplication |
        |                       | nModuleDependencies)` | ModuleDependencies()) |
        |                       |                       | to                    |
        |                       |                       | applicati             |
        |                       |                       | onModuleDependencies. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `A                    | `setCompat            | ::: block             |
        | ndroidAppModularityDe | ibleWith​(Iterable<? e | Sets or replaces all  |
        | scriptionArg.Builder` | xtends UnconfiguredBu | elements for          |
        |                       | ildTarget> elements)` | [`compatibleWith      |
        |                       |                       | `](AndroidAppModulari |
        |                       |                       | tyDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `A                    | `setDefaul            | ::: block             |
        | ndroidAppModularityDe | tTargetPlatform​(Uncon | Initializes the       |
        | scriptionArg.Builder` | figuredBuildTarget de | optional value        |
        |                       | faultTargetPlatform)` | [`default             |
        |                       |                       | TargetPlatform`](Andr |
        |                       |                       | oidAppModularityDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `A                    | `setDefau             | ::: block             |
        | ndroidAppModularityDe | ltTargetPlatform​(Opti | Initializes the       |
        | scriptionArg.Builder` | onal<? extends Unconf | optional value        |
        |                       | iguredBuildTarget> de | [`default             |
        |                       | faultTargetPlatform)` | TargetPlatform`](Andr |
        |                       |                       | oidAppModularityDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `A                    | `setDeps​(             | ::: block             |
        | ndroidAppModularityDe | Iterable<? extends Bu | Sets or replaces all  |
        | scriptionArg.Builder` | ildTarget> elements)` | elements for          |
        |                       |                       | [`deps`](AndroidA     |
        |                       |                       | ppModularityDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `A                    | `setLabels​(Iterab     | ::: block             |
        | ndroidAppModularityDe | le<String> elements)` | Sets or replaces all  |
        | scriptionArg.Builder` |                       | elements for          |
        |                       |                       | [`labels`](AndroidApp |
        |                       |                       | ModularityDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `A                    | `setLicenses          | ::: block             |
        | ndroidAppModularityDe | ​(Iterable<? extends S | Sets or replaces all  |
        | scriptionArg.Builder` | ourcePath> elements)` | elements for          |
        |                       |                       | [`li                  |
        |                       |                       | censes`](AndroidAppMo |
        |                       |                       | dularityDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `A                    | `                     | ::: block             |
        | ndroidAppModularityDe | setName​(String name)` | Initializes the value |
        | scriptionArg.Builder` |                       | for the               |
        |                       |                       | [`name`](AndroidA     |
        |                       |                       | ppModularityDescripti |
        |                       |                       | onArg.html#getName()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `A                    | `setNoDx​(             | ::: block             |
        | ndroidAppModularityDe | Iterable<? extends Bu | Sets or replaces all  |
        | scriptionArg.Builder` | ildTarget> elements)` | elements for          |
        |                       |                       | [`noDx`](AndroidA     |
        |                       |                       | ppModularityDescripti |
        |                       |                       | onArg.html#getNoDx()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `A                    | `setShouldInc         | ::: block             |
        | ndroidAppModularityDe | ludeClasses​(boolean s | Initializes the value |
        | scriptionArg.Builder` | houldIncludeClasses)` | for the               |
        |                       |                       | [`shoul               |
        |                       |                       | dIncludeClasses`](And |
        |                       |                       | roidAppModularityDesc |
        |                       |                       | riptionArg.html#getSh |
        |                       |                       | ouldIncludeClasses()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `A                    | `setShouldInclude     | ::: block             |
        | ndroidAppModularityDe | Libraries​(boolean sho | Initializes the value |
        | scriptionArg.Builder` | uldIncludeLibraries)` | for the               |
        |                       |                       | [`shouldInc           |
        |                       |                       | ludeLibraries`](Andro |
        |                       |                       | idAppModularityDescri |
        |                       |                       | ptionArg.html#getShou |
        |                       |                       | ldIncludeLibraries()) |
        |                       |                       | attribute.            |
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

        []{#from(com.facebook.buck.core.description.arg.HasApplicationModuleBlacklist)}

        -   #### from

            ``` methodSignature
            public final AndroidAppModularityDescriptionArg.Builder from​(HasApplicationModuleBlacklist instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `com.facebook.buck.core.description.arg.HasApplicationModuleBlacklist`
            instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.core.description.arg.HasDeclaredDeps)}

        -   #### from

            ``` methodSignature
            public final AndroidAppModularityDescriptionArg.Builder from​(HasDeclaredDeps instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `com.facebook.buck.core.description.arg.HasDeclaredDeps`
            instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.core.description.arg.BuildRuleArg)}

        -   #### from

            ``` methodSignature
            public final AndroidAppModularityDescriptionArg.Builder from​(BuildRuleArg instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `com.facebook.buck.core.description.arg.BuildRuleArg`
            instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.core.description.arg.ConstructorArg)}

        -   #### from

            ``` methodSignature
            public final AndroidAppModularityDescriptionArg.Builder from​(ConstructorArg instance)
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

        []{#from(com.facebook.buck.android.AndroidAppModularityDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final AndroidAppModularityDescriptionArg.Builder from​(AndroidAppModularityDescriptionArg instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `AndroidAppModularityDescriptionArg` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.android.AndroidAppModularityDescription.AbstractAndroidAppModularityDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final AndroidAppModularityDescriptionArg.Builder from​(com.facebook.buck.android.AndroidAppModularityDescription.AbstractAndroidAppModularityDescriptionArg instance)
            ```

            ::: block
            Copy abstract value type
            `AbstractAndroidAppModularityDescriptionArg` instance into
            builder.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putApplicationModuleConfigs(java.lang.String,com.google.common.collect.ImmutableList)}

        -   #### putApplicationModuleConfigs

            ``` methodSignature
            public final AndroidAppModularityDescriptionArg.Builder putApplicationModuleConfigs​(String key,
                                                                                                com.google.common.collect.ImmutableList<BuildTarget> value)
            ```

            ::: block
            Put one entry to the
            [`applicationModuleConfigs`](AndroidAppModularityDescriptionArg.html#getApplicationModuleConfigs())
            map.
            :::

            [Parameters:]{.paramLabel}
            :   `key` - The key in the applicationModuleConfigs map
            :   `value` - The associated value in the
                applicationModuleConfigs map

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putApplicationModuleConfigs(java.util.Map.Entry)}

        -   #### putApplicationModuleConfigs

            ``` methodSignature
            public final AndroidAppModularityDescriptionArg.Builder putApplicationModuleConfigs​(Map.Entry<String,​? extends com.google.common.collect.ImmutableList<BuildTarget>> entry)
            ```

            ::: block
            Put one entry to the
            [`applicationModuleConfigs`](AndroidAppModularityDescriptionArg.html#getApplicationModuleConfigs())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entry` - The key and value entry

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setApplicationModuleConfigs(java.util.Map)}

        -   #### setApplicationModuleConfigs

            ``` methodSignature
            public final AndroidAppModularityDescriptionArg.Builder setApplicationModuleConfigs​(Map<String,​? extends com.google.common.collect.ImmutableList<BuildTarget>> entries)
            ```

            ::: block
            Sets or replaces all mappings from the specified map as
            entries for the
            [`applicationModuleConfigs`](AndroidAppModularityDescriptionArg.html#getApplicationModuleConfigs())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entries` - The entries that will be added to the
                applicationModuleConfigs map

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putAllApplicationModuleConfigs(java.util.Map)}

        -   #### putAllApplicationModuleConfigs

            ``` methodSignature
            public final AndroidAppModularityDescriptionArg.Builder putAllApplicationModuleConfigs​(Map<String,​? extends com.google.common.collect.ImmutableList<BuildTarget>> entries)
            ```

            ::: block
            Put all mappings from the specified map as entries to
            [`applicationModuleConfigs`](AndroidAppModularityDescriptionArg.html#getApplicationModuleConfigs())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entries` - The entries that will be added to the
                applicationModuleConfigs map

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setApplicationModuleDependencies(com.google.common.collect.ImmutableMap)}

        -   #### setApplicationModuleDependencies

            ``` methodSignature
            public final AndroidAppModularityDescriptionArg.Builder setApplicationModuleDependencies​(com.google.common.collect.ImmutableMap<String,​com.google.common.collect.ImmutableList<String>> applicationModuleDependencies)
            ```

            ::: block
            Initializes the optional value
            [`applicationModuleDependencies`](AndroidAppModularityDescriptionArg.html#getApplicationModuleDependencies())
            to applicationModuleDependencies.
            :::

            [Parameters:]{.paramLabel}
            :   `applicationModuleDependencies` - The value for
                applicationModuleDependencies

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setApplicationModuleDependencies(java.util.Optional)}

        -   #### setApplicationModuleDependencies

            ``` methodSignature
            public final AndroidAppModularityDescriptionArg.Builder setApplicationModuleDependencies​(Optional<? extends com.google.common.collect.ImmutableMap<String,​com.google.common.collect.ImmutableList<String>>> applicationModuleDependencies)
            ```

            ::: block
            Initializes the optional value
            [`applicationModuleDependencies`](AndroidAppModularityDescriptionArg.html#getApplicationModuleDependencies())
            to applicationModuleDependencies.
            :::

            [Parameters:]{.paramLabel}
            :   `applicationModuleDependencies` - The value for
                applicationModuleDependencies

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addNoDx(com.facebook.buck.core.model.BuildTarget)}

        -   #### addNoDx

            ``` methodSignature
            public final AndroidAppModularityDescriptionArg.Builder addNoDx​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`noDx`](AndroidAppModularityDescriptionArg.html#getNoDx())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A noDx element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addNoDx(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addNoDx

            ``` methodSignature
            public final AndroidAppModularityDescriptionArg.Builder addNoDx​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`noDx`](AndroidAppModularityDescriptionArg.html#getNoDx())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of noDx elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setNoDx(java.lang.Iterable)}

        -   #### setNoDx

            ``` methodSignature
            public final AndroidAppModularityDescriptionArg.Builder setNoDx​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`noDx`](AndroidAppModularityDescriptionArg.html#getNoDx())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of noDx elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllNoDx(java.lang.Iterable)}

        -   #### addAllNoDx

            ``` methodSignature
            public final AndroidAppModularityDescriptionArg.Builder addAllNoDx​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`noDx`](AndroidAppModularityDescriptionArg.html#getNoDx())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of noDx elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setShouldIncludeClasses(boolean)}

        -   #### setShouldIncludeClasses

            ``` methodSignature
            public final AndroidAppModularityDescriptionArg.Builder setShouldIncludeClasses​(boolean shouldIncludeClasses)
            ```

            ::: block
            Initializes the value for the
            [`shouldIncludeClasses`](AndroidAppModularityDescriptionArg.html#getShouldIncludeClasses())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`shouldIncludeClasses`](AndroidAppModularityDescriptionArg.html#getShouldIncludeClasses()).*
            :::

            [Parameters:]{.paramLabel}
            :   `shouldIncludeClasses` - The value for
                shouldIncludeClasses

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setShouldIncludeLibraries(boolean)}

        -   #### setShouldIncludeLibraries

            ``` methodSignature
            public final AndroidAppModularityDescriptionArg.Builder setShouldIncludeLibraries​(boolean shouldIncludeLibraries)
            ```

            ::: block
            Initializes the value for the
            [`shouldIncludeLibraries`](AndroidAppModularityDescriptionArg.html#getShouldIncludeLibraries())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`shouldIncludeLibraries`](AndroidAppModularityDescriptionArg.html#getShouldIncludeLibraries()).*
            :::

            [Parameters:]{.paramLabel}
            :   `shouldIncludeLibraries` - The value for
                shouldIncludeLibraries

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLicenses(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### addLicenses

            ``` methodSignature
            public final AndroidAppModularityDescriptionArg.Builder addLicenses​(SourcePath element)
            ```

            ::: block
            Adds one element to
            [`licenses`](AndroidAppModularityDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A licenses element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLicenses(com.facebook.buck.core.sourcepath.SourcePath...)}

        -   #### addLicenses

            ``` methodSignature
            public final AndroidAppModularityDescriptionArg.Builder addLicenses​(SourcePath... elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](AndroidAppModularityDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLicenses(java.lang.Iterable)}

        -   #### setLicenses

            ``` methodSignature
            public final AndroidAppModularityDescriptionArg.Builder setLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`licenses`](AndroidAppModularityDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLicenses(java.lang.Iterable)}

        -   #### addAllLicenses

            ``` methodSignature
            public final AndroidAppModularityDescriptionArg.Builder addAllLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](AndroidAppModularityDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLabels(java.lang.String)}

        -   #### addLabels

            ``` methodSignature
            public final AndroidAppModularityDescriptionArg.Builder addLabels​(String element)
            ```

            ::: block
            Adds one element to
            [`labels`](AndroidAppModularityDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A labels element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLabels(java.lang.String...)}

        -   #### addLabels

            ``` methodSignature
            public final AndroidAppModularityDescriptionArg.Builder addLabels​(String... elements)
            ```

            ::: block
            Adds elements to
            [`labels`](AndroidAppModularityDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLabels(java.lang.Iterable)}

        -   #### setLabels

            ``` methodSignature
            public final AndroidAppModularityDescriptionArg.Builder setLabels​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`labels`](AndroidAppModularityDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLabels(java.lang.Iterable)}

        -   #### addAllLabels

            ``` methodSignature
            public final AndroidAppModularityDescriptionArg.Builder addAllLabels​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`labels`](AndroidAppModularityDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDefaultTargetPlatform(com.facebook.buck.core.model.UnconfiguredBuildTarget)}

        -   #### setDefaultTargetPlatform

            ``` methodSignature
            public final AndroidAppModularityDescriptionArg.Builder setDefaultTargetPlatform​(UnconfiguredBuildTarget defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](AndroidAppModularityDescriptionArg.html#getDefaultTargetPlatform())
            to defaultTargetPlatform.
            :::

            [Parameters:]{.paramLabel}
            :   `defaultTargetPlatform` - The value for
                defaultTargetPlatform

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setDefaultTargetPlatform(java.util.Optional)}

        -   #### setDefaultTargetPlatform

            ``` methodSignature
            public final AndroidAppModularityDescriptionArg.Builder setDefaultTargetPlatform​(Optional<? extends UnconfiguredBuildTarget> defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](AndroidAppModularityDescriptionArg.html#getDefaultTargetPlatform())
            to defaultTargetPlatform.
            :::

            [Parameters:]{.paramLabel}
            :   `defaultTargetPlatform` - The value for
                defaultTargetPlatform

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCompatibleWith(com.facebook.buck.core.model.UnconfiguredBuildTarget)}

        -   #### addCompatibleWith

            ``` methodSignature
            public final AndroidAppModularityDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget element)
            ```

            ::: block
            Adds one element to
            [`compatibleWith`](AndroidAppModularityDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A compatibleWith element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCompatibleWith(com.facebook.buck.core.model.UnconfiguredBuildTarget...)}

        -   #### addCompatibleWith

            ``` methodSignature
            public final AndroidAppModularityDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](AndroidAppModularityDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCompatibleWith(java.lang.Iterable)}

        -   #### setCompatibleWith

            ``` methodSignature
            public final AndroidAppModularityDescriptionArg.Builder setCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`compatibleWith`](AndroidAppModularityDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllCompatibleWith(java.lang.Iterable)}

        -   #### addAllCompatibleWith

            ``` methodSignature
            public final AndroidAppModularityDescriptionArg.Builder addAllCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](AndroidAppModularityDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setName(java.lang.String)}

        -   #### setName

            ``` methodSignature
            public final AndroidAppModularityDescriptionArg.Builder setName​(String name)
            ```

            ::: block
            Initializes the value for the
            [`name`](AndroidAppModularityDescriptionArg.html#getName())
            attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `name` - The value for name

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addDeps(com.facebook.buck.core.model.BuildTarget)}

        -   #### addDeps

            ``` methodSignature
            public final AndroidAppModularityDescriptionArg.Builder addDeps​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`deps`](AndroidAppModularityDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A deps element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addDeps(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addDeps

            ``` methodSignature
            public final AndroidAppModularityDescriptionArg.Builder addDeps​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`deps`](AndroidAppModularityDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDeps(java.lang.Iterable)}

        -   #### setDeps

            ``` methodSignature
            public final AndroidAppModularityDescriptionArg.Builder setDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`deps`](AndroidAppModularityDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllDeps(java.lang.Iterable)}

        -   #### addAllDeps

            ``` methodSignature
            public final AndroidAppModularityDescriptionArg.Builder addAllDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`deps`](AndroidAppModularityDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setApplicationModuleBlacklist(java.util.List)}

        -   #### setApplicationModuleBlacklist

            ``` methodSignature
            public final AndroidAppModularityDescriptionArg.Builder setApplicationModuleBlacklist​(List<Query> applicationModuleBlacklist)
            ```

            ::: block
            Initializes the optional value
            [`applicationModuleBlacklist`](AndroidAppModularityDescriptionArg.html#getApplicationModuleBlacklist())
            to applicationModuleBlacklist.
            :::

            [Parameters:]{.paramLabel}
            :   `applicationModuleBlacklist` - The value for
                applicationModuleBlacklist

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setApplicationModuleBlacklist(java.util.Optional)}

        -   #### setApplicationModuleBlacklist

            ``` methodSignature
            public final AndroidAppModularityDescriptionArg.Builder setApplicationModuleBlacklist​(Optional<? extends List<Query>> applicationModuleBlacklist)
            ```

            ::: block
            Initializes the optional value
            [`applicationModuleBlacklist`](AndroidAppModularityDescriptionArg.html#getApplicationModuleBlacklist())
            to applicationModuleBlacklist.
            :::

            [Parameters:]{.paramLabel}
            :   `applicationModuleBlacklist` - The value for
                applicationModuleBlacklist

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#build()}

        -   #### build

            ``` methodSignature
            public AndroidAppModularityDescriptionArg build()
            ```

            ::: block
            Builds a new
            [`AndroidAppModularityDescriptionArg`](AndroidAppModularityDescriptionArg.html "class in com.facebook.buck.android").
            :::

            [Returns:]{.returnLabel}
            :   An immutable instance of
                AndroidAppModularityDescriptionArg

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

-   [Overview](../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../deprecated-list.html)
-   [Index](../../../../index-all.html)
-   [Help](../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../allclasses.html)

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
