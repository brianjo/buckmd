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
[Package]{.packageLabelInType} [com.facebook.buck.jvm.java](package-summary.html)
:::

## Class JarGenruleDescriptionArg.Builder {#class-jargenruledescriptionarg.builder .title title="Class JarGenruleDescriptionArg.Builder"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.jvm.java.JarGenruleDescriptionArg.Builder

::: description
-   

    Enclosing class:
    :   [JarGenruleDescriptionArg](JarGenruleDescriptionArg.html "class in com.facebook.buck.jvm.java")

    ------------------------------------------------------------------------

        @NotThreadSafe
        public static final class JarGenruleDescriptionArg.Builder
        extends Object

    ::: block
    Builds instances of type
    [`JarGenruleDescriptionArg`](JarGenruleDescriptionArg.html "class in com.facebook.buck.jvm.java").
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
        | `JarGenruleDe         | `addAllCompat         | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Iterable<? e | Adds elements to      |
        |                       | xtends UnconfiguredBu | [`comp                |
        |                       | ildTarget> elements)` | atibleWith`](JarGenru |
        |                       |                       | leDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JarGenruleDe         | `addAllLabels​(Iterab  | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Adds elements to      |
        |                       |                       | [`labels`](           |
        |                       |                       | JarGenruleDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JarGenruleDe         | `addAllLicenses       | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Adds elements to      |
        |                       | ourcePath> elements)` | [`licenses`](Ja       |
        |                       |                       | rGenruleDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JarGenruleDe         | `addAllTests​(         | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Adds elements to      |
        |                       | ildTarget> elements)` | [`tests`]             |
        |                       |                       | (JarGenruleDescriptio |
        |                       |                       | nArg.html#getTests()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JarGenruleDe         | `addCompat            | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Unconfigured | Adds one element to   |
        |                       | BuildTarget element)` | [`comp                |
        |                       |                       | atibleWith`](JarGenru |
        |                       |                       | leDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JarGenruleDe         | `addCompatible        | ::: block             |
        | scriptionArg.Builder` | With​(UnconfiguredBuil | Adds elements to      |
        |                       | dTarget... elements)` | [`comp                |
        |                       |                       | atibleWith`](JarGenru |
        |                       |                       | leDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JarGenruleDe         | `addLa                | ::: block             |
        | scriptionArg.Builder` | bels​(String element)` | Adds one element to   |
        |                       |                       | [`labels`](           |
        |                       |                       | JarGenruleDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JarGenruleDe         | `addLabels            | ::: block             |
        | scriptionArg.Builder` | ​(String... elements)` | Adds elements to      |
        |                       |                       | [`labels`](           |
        |                       |                       | JarGenruleDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JarGenruleDe         | `addLicenses          | ::: block             |
        | scriptionArg.Builder` | ​(SourcePath element)` | Adds one element to   |
        |                       |                       | [`licenses`](Ja       |
        |                       |                       | rGenruleDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JarGenruleDe         | `addLicenses​(Sou      | ::: block             |
        | scriptionArg.Builder` | rcePath... elements)` | Adds elements to      |
        |                       |                       | [`licenses`](Ja       |
        |                       |                       | rGenruleDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JarGenruleDe         | `addTests​(            | ::: block             |
        | scriptionArg.Builder` | BuildTarget element)` | Adds one element to   |
        |                       |                       | [`tests`]             |
        |                       |                       | (JarGenruleDescriptio |
        |                       |                       | nArg.html#getTests()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JarGenruleDe         | `addTests​(Buil        | ::: block             |
        | scriptionArg.Builder` | dTarget... elements)` | Adds elements to      |
        |                       |                       | [`tests`]             |
        |                       |                       | (JarGenruleDescriptio |
        |                       |                       | nArg.html#getTests()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JarG                 | `build()`             | ::: block             |
        | enruleDescriptionArg` |                       | Builds a new          |
        |                       |                       | [`JarGenruleDe        |
        |                       |                       | scriptionArg`](JarGen |
        |                       |                       | ruleDescriptionArg.ht |
        |                       |                       | ml "class in com.face |
        |                       |                       | book.buck.jvm.java"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JarGenruleDe         | `from​(Bu              | ::: block             |
        | scriptionArg.Builder` | ildRuleArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebo           |
        |                       |                       | ok.buck.core.descript |
        |                       |                       | ion.arg.BuildRuleArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JarGenruleDe         | `from​(Cons            | ::: block             |
        | scriptionArg.Builder` | tructorArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook         |
        |                       |                       | .buck.core.descriptio |
        |                       |                       | n.arg.ConstructorArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JarGenruleDe         | `fro                  | ::: block             |
        | scriptionArg.Builder` | m​(HasTests instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.fa               |
        |                       |                       | cebook.buck.core.desc |
        |                       |                       | ription.arg.HasTests` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JarGenruleDe         | `from​(com.face        | ::: block             |
        | scriptionArg.Builder` | book.buck.jvm.java.Ja | Copy abstract value   |
        |                       | rGenruleDescription.A | type                  |
        |                       | bstractJarGenruleDesc | `AbstractJarG         |
        |                       | riptionArg instance)` | enruleDescriptionArg` |
        |                       |                       | instance into         |
        |                       |                       | builder.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JarGenruleDe         | `from​(JarGenruleDesc  | ::: block             |
        | scriptionArg.Builder` | riptionArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `JarG                 |
        |                       |                       | enruleDescriptionArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JarGenruleDe         | `from​(Abstr           | ::: block             |
        | scriptionArg.Builder` | actGenruleDescription | Fill a builder with   |
        |                       | .CommonArg instance)` | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook.buck.s  |
        |                       |                       | hell.AbstractGenruleD |
        |                       |                       | escription.CommonArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JarGenruleDe         | `setBash​(St           | ::: block             |
        | scriptionArg.Builder` | ringWithMacros bash)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`bash`               |
        |                       |                       | ](JarGenruleDescripti |
        |                       |                       | onArg.html#getBash()) |
        |                       |                       | to bash.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JarGenruleDe         | `setBash​(O            | ::: block             |
        | scriptionArg.Builder` | ptional<? extends Str | Initializes the       |
        |                       | ingWithMacros> bash)` | optional value        |
        |                       |                       | [`bash`               |
        |                       |                       | ](JarGenruleDescripti |
        |                       |                       | onArg.html#getBash()) |
        |                       |                       | to bash.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JarGenruleDe         | `setCacheabl          | ::: block             |
        | scriptionArg.Builder` | e​(boolean cacheable)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`cacheable`](Jar     |
        |                       |                       | GenruleDescriptionArg |
        |                       |                       | .html#getCacheable()) |
        |                       |                       | to cacheable.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JarGenruleDe         | `                     | ::: block             |
        | scriptionArg.Builder` | setCacheable​(Optional | Initializes the       |
        |                       | <Boolean> cacheable)` | optional value        |
        |                       |                       | [`cacheable`](Jar     |
        |                       |                       | GenruleDescriptionArg |
        |                       |                       | .html#getCacheable()) |
        |                       |                       | to cacheable.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JarGenruleDe         | `setCmd​(S             | ::: block             |
        | scriptionArg.Builder` | tringWithMacros cmd)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`cmd                 |
        |                       |                       | `](JarGenruleDescript |
        |                       |                       | ionArg.html#getCmd()) |
        |                       |                       | to cmd.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JarGenruleDe         | `setCmd​(              | ::: block             |
        | scriptionArg.Builder` | Optional<? extends St | Initializes the       |
        |                       | ringWithMacros> cmd)` | optional value        |
        |                       |                       | [`cmd                 |
        |                       |                       | `](JarGenruleDescript |
        |                       |                       | ionArg.html#getCmd()) |
        |                       |                       | to cmd.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JarGenruleDe         | `setCmdExe​(Stri       | ::: block             |
        | scriptionArg.Builder` | ngWithMacros cmdExe)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`cmdExe`](           |
        |                       |                       | JarGenruleDescription |
        |                       |                       | Arg.html#getCmdExe()) |
        |                       |                       | to cmdExe.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JarGenruleDe         | `setCmdExe​(Opt        | ::: block             |
        | scriptionArg.Builder` | ional<? extends Strin | Initializes the       |
        |                       | gWithMacros> cmdExe)` | optional value        |
        |                       |                       | [`cmdExe`](           |
        |                       |                       | JarGenruleDescription |
        |                       |                       | Arg.html#getCmdExe()) |
        |                       |                       | to cmdExe.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JarGenruleDe         | `setCompat            | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Iterable<? e | Sets or replaces all  |
        |                       | xtends UnconfiguredBu | elements for          |
        |                       | ildTarget> elements)` | [`comp                |
        |                       |                       | atibleWith`](JarGenru |
        |                       |                       | leDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JarGenruleDe         | `setDefaul            | ::: block             |
        | scriptionArg.Builder` | tTargetPlatform​(Uncon | Initializes the       |
        |                       | figuredBuildTarget de | optional value        |
        |                       | faultTargetPlatform)` | [`defaultTargetPlatf  |
        |                       |                       | orm`](JarGenruleDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JarGenruleDe         | `setDefau             | ::: block             |
        | scriptionArg.Builder` | ltTargetPlatform​(Opti | Initializes the       |
        |                       | onal<? extends Unconf | optional value        |
        |                       | iguredBuildTarget> de | [`defaultTargetPlatf  |
        |                       | faultTargetPlatform)` | orm`](JarGenruleDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JarGenruleDe         | `setEnableSandbox​(bo  | ::: block             |
        | scriptionArg.Builder` | olean enableSandbox)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`en                  |
        |                       |                       | ableSandbox`](JarGenr |
        |                       |                       | uleDescriptionArg.htm |
        |                       |                       | l#getEnableSandbox()) |
        |                       |                       | to enableSandbox.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JarGenruleDe         | `setEnabl             | ::: block             |
        | scriptionArg.Builder` | eSandbox​(Optional<Boo | Initializes the       |
        |                       | lean> enableSandbox)` | optional value        |
        |                       |                       | [`en                  |
        |                       |                       | ableSandbox`](JarGenr |
        |                       |                       | uleDescriptionArg.htm |
        |                       |                       | l#getEnableSandbox()) |
        |                       |                       | to enableSandbox.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JarGenruleDe         | `setEnvir             | ::: block             |
        | scriptionArg.Builder` | onmentExpansionSepara | Initializes the       |
        |                       | tor​(String environmen | optional value        |
        |                       | tExpansionSeparator)` | [`environmentEx       |
        |                       |                       | pansionSeparator`](Ja |
        |                       |                       | rGenruleDescriptionAr |
        |                       |                       | g.html#getEnvironment |
        |                       |                       | ExpansionSeparator()) |
        |                       |                       | to                    |
        |                       |                       | environme             |
        |                       |                       | ntExpansionSeparator. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JarGenruleDe         | `setEnvironmentExpa   | ::: block             |
        | scriptionArg.Builder` | nsionSeparator​(Option | Initializes the       |
        |                       | al<String> environmen | optional value        |
        |                       | tExpansionSeparator)` | [`environmentEx       |
        |                       |                       | pansionSeparator`](Ja |
        |                       |                       | rGenruleDescriptionAr |
        |                       |                       | g.html#getEnvironment |
        |                       |                       | ExpansionSeparator()) |
        |                       |                       | to                    |
        |                       |                       | environme             |
        |                       |                       | ntExpansionSeparator. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JarGenruleDe         | `setLabels​(Iterab     | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Sets or replaces all  |
        |                       |                       | elements for          |
        |                       |                       | [`labels`](           |
        |                       |                       | JarGenruleDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JarGenruleDe         | `setLicenses          | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Sets or replaces all  |
        |                       | ourcePath> elements)` | elements for          |
        |                       |                       | [`licenses`](Ja       |
        |                       |                       | rGenruleDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JarGenruleDe         | `                     | ::: block             |
        | scriptionArg.Builder` | setName​(String name)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`name`               |
        |                       |                       | ](JarGenruleDescripti |
        |                       |                       | onArg.html#getName()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JarGenruleDe         | `setN                 | ::: block             |
        | scriptionArg.Builder` | eedAndroidTools​(boole | Initializes the value |
        |                       | an needAndroidTools)` | for the               |
        |                       |                       | [`needAnd             |
        |                       |                       | roidTools`](JarGenrul |
        |                       |                       | eDescriptionArg.html# |
        |                       |                       | isNeedAndroidTools()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JarGenruleDe         | `setRe                | ::: block             |
        | scriptionArg.Builder` | mote​(boolean remote)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`remote`](           |
        |                       |                       | JarGenruleDescription |
        |                       |                       | Arg.html#getRemote()) |
        |                       |                       | to remote.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JarGenruleDe         | `setRemote​(Optio      | ::: block             |
        | scriptionArg.Builder` | nal<Boolean> remote)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`remote`](           |
        |                       |                       | JarGenruleDescription |
        |                       |                       | Arg.html#getRemote()) |
        |                       |                       | to remote.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JarGenruleDe         | `set                  | ::: block             |
        | scriptionArg.Builder` | Srcs​(SourceSet srcs)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`srcs`               |
        |                       |                       | ](JarGenruleDescripti |
        |                       |                       | onArg.html#getSrcs()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JarGenruleDe         | `setTests​(            | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Sets or replaces all  |
        |                       | ildTarget> elements)` | elements for          |
        |                       |                       | [`tests`]             |
        |                       |                       | (JarGenruleDescriptio |
        |                       |                       | nArg.html#getTests()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JarGenruleDe         | `                     | ::: block             |
        | scriptionArg.Builder` | setType​(String type)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`type`               |
        |                       |                       | ](JarGenruleDescripti |
        |                       |                       | onArg.html#getType()) |
        |                       |                       | to type.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JarGenruleDe         | `setType​(Op           | ::: block             |
        | scriptionArg.Builder` | tional<String> type)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`type`               |
        |                       |                       | ](JarGenruleDescripti |
        |                       |                       | onArg.html#getType()) |
        |                       |                       | to type.              |
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

        []{#from(com.facebook.buck.core.description.arg.HasTests)}

        -   #### from

            ``` methodSignature
            public final JarGenruleDescriptionArg.Builder from​(HasTests instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `com.facebook.buck.core.description.arg.HasTests` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.shell.AbstractGenruleDescription.CommonArg)}

        -   #### from

            ``` methodSignature
            public final JarGenruleDescriptionArg.Builder from​(AbstractGenruleDescription.CommonArg instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `com.facebook.buck.shell.AbstractGenruleDescription.CommonArg`
            instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.core.description.arg.BuildRuleArg)}

        -   #### from

            ``` methodSignature
            public final JarGenruleDescriptionArg.Builder from​(BuildRuleArg instance)
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
            public final JarGenruleDescriptionArg.Builder from​(ConstructorArg instance)
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

        []{#from(com.facebook.buck.jvm.java.JarGenruleDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final JarGenruleDescriptionArg.Builder from​(JarGenruleDescriptionArg instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `JarGenruleDescriptionArg` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.jvm.java.JarGenruleDescription.AbstractJarGenruleDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final JarGenruleDescriptionArg.Builder from​(com.facebook.buck.jvm.java.JarGenruleDescription.AbstractJarGenruleDescriptionArg instance)
            ```

            ::: block
            Copy abstract value type `AbstractJarGenruleDescriptionArg`
            instance into builder.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setBash(com.facebook.buck.rules.macros.StringWithMacros)}

        -   #### setBash

            ``` methodSignature
            public final JarGenruleDescriptionArg.Builder setBash​(StringWithMacros bash)
            ```

            ::: block
            Initializes the optional value
            [`bash`](JarGenruleDescriptionArg.html#getBash()) to bash.
            :::

            [Parameters:]{.paramLabel}
            :   `bash` - The value for bash

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setBash(java.util.Optional)}

        -   #### setBash

            ``` methodSignature
            public final JarGenruleDescriptionArg.Builder setBash​(Optional<? extends StringWithMacros> bash)
            ```

            ::: block
            Initializes the optional value
            [`bash`](JarGenruleDescriptionArg.html#getBash()) to bash.
            :::

            [Parameters:]{.paramLabel}
            :   `bash` - The value for bash

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCmd(com.facebook.buck.rules.macros.StringWithMacros)}

        -   #### setCmd

            ``` methodSignature
            public final JarGenruleDescriptionArg.Builder setCmd​(StringWithMacros cmd)
            ```

            ::: block
            Initializes the optional value
            [`cmd`](JarGenruleDescriptionArg.html#getCmd()) to cmd.
            :::

            [Parameters:]{.paramLabel}
            :   `cmd` - The value for cmd

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setCmd(java.util.Optional)}

        -   #### setCmd

            ``` methodSignature
            public final JarGenruleDescriptionArg.Builder setCmd​(Optional<? extends StringWithMacros> cmd)
            ```

            ::: block
            Initializes the optional value
            [`cmd`](JarGenruleDescriptionArg.html#getCmd()) to cmd.
            :::

            [Parameters:]{.paramLabel}
            :   `cmd` - The value for cmd

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCmdExe(com.facebook.buck.rules.macros.StringWithMacros)}

        -   #### setCmdExe

            ``` methodSignature
            public final JarGenruleDescriptionArg.Builder setCmdExe​(StringWithMacros cmdExe)
            ```

            ::: block
            Initializes the optional value
            [`cmdExe`](JarGenruleDescriptionArg.html#getCmdExe()) to
            cmdExe.
            :::

            [Parameters:]{.paramLabel}
            :   `cmdExe` - The value for cmdExe

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setCmdExe(java.util.Optional)}

        -   #### setCmdExe

            ``` methodSignature
            public final JarGenruleDescriptionArg.Builder setCmdExe​(Optional<? extends StringWithMacros> cmdExe)
            ```

            ::: block
            Initializes the optional value
            [`cmdExe`](JarGenruleDescriptionArg.html#getCmdExe()) to
            cmdExe.
            :::

            [Parameters:]{.paramLabel}
            :   `cmdExe` - The value for cmdExe

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setType(java.lang.String)}

        -   #### setType

            ``` methodSignature
            public final JarGenruleDescriptionArg.Builder setType​(String type)
            ```

            ::: block
            Initializes the optional value
            [`type`](JarGenruleDescriptionArg.html#getType()) to type.
            :::

            [Parameters:]{.paramLabel}
            :   `type` - The value for type

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setType(java.util.Optional)}

        -   #### setType

            ``` methodSignature
            public final JarGenruleDescriptionArg.Builder setType​(Optional<String> type)
            ```

            ::: block
            Initializes the optional value
            [`type`](JarGenruleDescriptionArg.html#getType()) to type.
            :::

            [Parameters:]{.paramLabel}
            :   `type` - The value for type

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setSrcs(com.facebook.buck.rules.coercer.SourceSet)}

        -   #### setSrcs

            ``` methodSignature
            public final JarGenruleDescriptionArg.Builder setSrcs​(SourceSet srcs)
            ```

            ::: block
            Initializes the value for the
            [`srcs`](JarGenruleDescriptionArg.html#getSrcs()) attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`srcs`](JarGenruleDescriptionArg.html#getSrcs()).*
            :::

            [Parameters:]{.paramLabel}
            :   `srcs` - The value for srcs

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setEnableSandbox(boolean)}

        -   #### setEnableSandbox

            ``` methodSignature
            public final JarGenruleDescriptionArg.Builder setEnableSandbox​(boolean enableSandbox)
            ```

            ::: block
            Initializes the optional value
            [`enableSandbox`](JarGenruleDescriptionArg.html#getEnableSandbox())
            to enableSandbox.
            :::

            [Parameters:]{.paramLabel}
            :   `enableSandbox` - The value for enableSandbox

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setEnableSandbox(java.util.Optional)}

        -   #### setEnableSandbox

            ``` methodSignature
            public final JarGenruleDescriptionArg.Builder setEnableSandbox​(Optional<Boolean> enableSandbox)
            ```

            ::: block
            Initializes the optional value
            [`enableSandbox`](JarGenruleDescriptionArg.html#getEnableSandbox())
            to enableSandbox.
            :::

            [Parameters:]{.paramLabel}
            :   `enableSandbox` - The value for enableSandbox

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setEnvironmentExpansionSeparator(java.lang.String)}

        -   #### setEnvironmentExpansionSeparator

            ``` methodSignature
            public final JarGenruleDescriptionArg.Builder setEnvironmentExpansionSeparator​(String environmentExpansionSeparator)
            ```

            ::: block
            Initializes the optional value
            [`environmentExpansionSeparator`](JarGenruleDescriptionArg.html#getEnvironmentExpansionSeparator())
            to environmentExpansionSeparator.
            :::

            [Parameters:]{.paramLabel}
            :   `environmentExpansionSeparator` - The value for
                environmentExpansionSeparator

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setEnvironmentExpansionSeparator(java.util.Optional)}

        -   #### setEnvironmentExpansionSeparator

            ``` methodSignature
            public final JarGenruleDescriptionArg.Builder setEnvironmentExpansionSeparator​(Optional<String> environmentExpansionSeparator)
            ```

            ::: block
            Initializes the optional value
            [`environmentExpansionSeparator`](JarGenruleDescriptionArg.html#getEnvironmentExpansionSeparator())
            to environmentExpansionSeparator.
            :::

            [Parameters:]{.paramLabel}
            :   `environmentExpansionSeparator` - The value for
                environmentExpansionSeparator

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setRemote(boolean)}

        -   #### setRemote

            ``` methodSignature
            public final JarGenruleDescriptionArg.Builder setRemote​(boolean remote)
            ```

            ::: block
            Initializes the optional value
            [`remote`](JarGenruleDescriptionArg.html#getRemote()) to
            remote.
            :::

            [Parameters:]{.paramLabel}
            :   `remote` - The value for remote

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setRemote(java.util.Optional)}

        -   #### setRemote

            ``` methodSignature
            public final JarGenruleDescriptionArg.Builder setRemote​(Optional<Boolean> remote)
            ```

            ::: block
            Initializes the optional value
            [`remote`](JarGenruleDescriptionArg.html#getRemote()) to
            remote.
            :::

            [Parameters:]{.paramLabel}
            :   `remote` - The value for remote

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCacheable(boolean)}

        -   #### setCacheable

            ``` methodSignature
            public final JarGenruleDescriptionArg.Builder setCacheable​(boolean cacheable)
            ```

            ::: block
            Initializes the optional value
            [`cacheable`](JarGenruleDescriptionArg.html#getCacheable())
            to cacheable.
            :::

            [Parameters:]{.paramLabel}
            :   `cacheable` - The value for cacheable

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setCacheable(java.util.Optional)}

        -   #### setCacheable

            ``` methodSignature
            public final JarGenruleDescriptionArg.Builder setCacheable​(Optional<Boolean> cacheable)
            ```

            ::: block
            Initializes the optional value
            [`cacheable`](JarGenruleDescriptionArg.html#getCacheable())
            to cacheable.
            :::

            [Parameters:]{.paramLabel}
            :   `cacheable` - The value for cacheable

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setNeedAndroidTools(boolean)}

        -   #### setNeedAndroidTools

            ``` methodSignature
            public final JarGenruleDescriptionArg.Builder setNeedAndroidTools​(boolean needAndroidTools)
            ```

            ::: block
            Initializes the value for the
            [`needAndroidTools`](JarGenruleDescriptionArg.html#isNeedAndroidTools())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`needAndroidTools`](JarGenruleDescriptionArg.html#isNeedAndroidTools()).*
            :::

            [Parameters:]{.paramLabel}
            :   `needAndroidTools` - The value for needAndroidTools

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLicenses(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### addLicenses

            ``` methodSignature
            public final JarGenruleDescriptionArg.Builder addLicenses​(SourcePath element)
            ```

            ::: block
            Adds one element to
            [`licenses`](JarGenruleDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A licenses element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLicenses(com.facebook.buck.core.sourcepath.SourcePath...)}

        -   #### addLicenses

            ``` methodSignature
            public final JarGenruleDescriptionArg.Builder addLicenses​(SourcePath... elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](JarGenruleDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLicenses(java.lang.Iterable)}

        -   #### setLicenses

            ``` methodSignature
            public final JarGenruleDescriptionArg.Builder setLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`licenses`](JarGenruleDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLicenses(java.lang.Iterable)}

        -   #### addAllLicenses

            ``` methodSignature
            public final JarGenruleDescriptionArg.Builder addAllLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](JarGenruleDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLabels(java.lang.String)}

        -   #### addLabels

            ``` methodSignature
            public final JarGenruleDescriptionArg.Builder addLabels​(String element)
            ```

            ::: block
            Adds one element to
            [`labels`](JarGenruleDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A labels element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLabels(java.lang.String...)}

        -   #### addLabels

            ``` methodSignature
            public final JarGenruleDescriptionArg.Builder addLabels​(String... elements)
            ```

            ::: block
            Adds elements to
            [`labels`](JarGenruleDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLabels(java.lang.Iterable)}

        -   #### setLabels

            ``` methodSignature
            public final JarGenruleDescriptionArg.Builder setLabels​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`labels`](JarGenruleDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLabels(java.lang.Iterable)}

        -   #### addAllLabels

            ``` methodSignature
            public final JarGenruleDescriptionArg.Builder addAllLabels​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`labels`](JarGenruleDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDefaultTargetPlatform(com.facebook.buck.core.model.UnconfiguredBuildTarget)}

        -   #### setDefaultTargetPlatform

            ``` methodSignature
            public final JarGenruleDescriptionArg.Builder setDefaultTargetPlatform​(UnconfiguredBuildTarget defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](JarGenruleDescriptionArg.html#getDefaultTargetPlatform())
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
            public final JarGenruleDescriptionArg.Builder setDefaultTargetPlatform​(Optional<? extends UnconfiguredBuildTarget> defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](JarGenruleDescriptionArg.html#getDefaultTargetPlatform())
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
            public final JarGenruleDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget element)
            ```

            ::: block
            Adds one element to
            [`compatibleWith`](JarGenruleDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A compatibleWith element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCompatibleWith(com.facebook.buck.core.model.UnconfiguredBuildTarget...)}

        -   #### addCompatibleWith

            ``` methodSignature
            public final JarGenruleDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](JarGenruleDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCompatibleWith(java.lang.Iterable)}

        -   #### setCompatibleWith

            ``` methodSignature
            public final JarGenruleDescriptionArg.Builder setCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`compatibleWith`](JarGenruleDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllCompatibleWith(java.lang.Iterable)}

        -   #### addAllCompatibleWith

            ``` methodSignature
            public final JarGenruleDescriptionArg.Builder addAllCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](JarGenruleDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setName(java.lang.String)}

        -   #### setName

            ``` methodSignature
            public final JarGenruleDescriptionArg.Builder setName​(String name)
            ```

            ::: block
            Initializes the value for the
            [`name`](JarGenruleDescriptionArg.html#getName()) attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `name` - The value for name

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addTests(com.facebook.buck.core.model.BuildTarget)}

        -   #### addTests

            ``` methodSignature
            public final JarGenruleDescriptionArg.Builder addTests​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`tests`](JarGenruleDescriptionArg.html#getTests())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A tests element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addTests(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addTests

            ``` methodSignature
            public final JarGenruleDescriptionArg.Builder addTests​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`tests`](JarGenruleDescriptionArg.html#getTests())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of tests elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setTests(java.lang.Iterable)}

        -   #### setTests

            ``` methodSignature
            public final JarGenruleDescriptionArg.Builder setTests​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`tests`](JarGenruleDescriptionArg.html#getTests())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of tests elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllTests(java.lang.Iterable)}

        -   #### addAllTests

            ``` methodSignature
            public final JarGenruleDescriptionArg.Builder addAllTests​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`tests`](JarGenruleDescriptionArg.html#getTests())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of tests elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#build()}

        -   #### build

            ``` methodSignature
            public JarGenruleDescriptionArg build()
            ```

            ::: block
            Builds a new
            [`JarGenruleDescriptionArg`](JarGenruleDescriptionArg.html "class in com.facebook.buck.jvm.java").
            :::

            [Returns:]{.returnLabel}
            :   An immutable instance of JarGenruleDescriptionArg

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
