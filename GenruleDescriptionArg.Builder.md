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
[Package]{.packageLabelInType} [com.facebook.buck.shell](package-summary.html)
:::

## Class GenruleDescriptionArg.Builder {#class-genruledescriptionarg.builder .title title="Class GenruleDescriptionArg.Builder"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.shell.GenruleDescriptionArg.Builder

::: description
-   

    Enclosing class:
    :   [GenruleDescriptionArg](GenruleDescriptionArg.html "class in com.facebook.buck.shell")

    ------------------------------------------------------------------------

        @NotThreadSafe
        public static final class GenruleDescriptionArg.Builder
        extends Object

    ::: block
    Builds instances of type
    [`GenruleDescriptionArg`](GenruleDescriptionArg.html "class in com.facebook.buck.shell").
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
        | `GenruleDe            | `addAllCompat         | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Iterable<? e | Adds elements to      |
        |                       | xtends UnconfiguredBu | [`c                   |
        |                       | ildTarget> elements)` | ompatibleWith`](Genru |
        |                       |                       | leDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `GenruleDe            | `addAllLabels​(Iterab  | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Adds elements to      |
        |                       |                       | [`labels              |
        |                       |                       | `](GenruleDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `GenruleDe            | `addAllLicenses       | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Adds elements to      |
        |                       | ourcePath> elements)` | [`licenses`]          |
        |                       |                       | (GenruleDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `GenruleDe            | `addAllTests​(         | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Adds elements to      |
        |                       | ildTarget> elements)` | [`test                |
        |                       |                       | s`](GenruleDescriptio |
        |                       |                       | nArg.html#getTests()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `GenruleDe            | `addCompat            | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Unconfigured | Adds one element to   |
        |                       | BuildTarget element)` | [`c                   |
        |                       |                       | ompatibleWith`](Genru |
        |                       |                       | leDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `GenruleDe            | `addCompatible        | ::: block             |
        | scriptionArg.Builder` | With​(UnconfiguredBuil | Adds elements to      |
        |                       | dTarget... elements)` | [`c                   |
        |                       |                       | ompatibleWith`](Genru |
        |                       |                       | leDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `GenruleDe            | `addLa                | ::: block             |
        | scriptionArg.Builder` | bels​(String element)` | Adds one element to   |
        |                       |                       | [`labels              |
        |                       |                       | `](GenruleDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `GenruleDe            | `addLabels            | ::: block             |
        | scriptionArg.Builder` | ​(String... elements)` | Adds elements to      |
        |                       |                       | [`labels              |
        |                       |                       | `](GenruleDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `GenruleDe            | `addLicenses          | ::: block             |
        | scriptionArg.Builder` | ​(SourcePath element)` | Adds one element to   |
        |                       |                       | [`licenses`]          |
        |                       |                       | (GenruleDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `GenruleDe            | `addLicenses​(Sou      | ::: block             |
        | scriptionArg.Builder` | rcePath... elements)` | Adds elements to      |
        |                       |                       | [`licenses`]          |
        |                       |                       | (GenruleDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `GenruleDe            | `addTests​(            | ::: block             |
        | scriptionArg.Builder` | BuildTarget element)` | Adds one element to   |
        |                       |                       | [`test                |
        |                       |                       | s`](GenruleDescriptio |
        |                       |                       | nArg.html#getTests()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `GenruleDe            | `addTests​(Buil        | ::: block             |
        | scriptionArg.Builder` | dTarget... elements)` | Adds elements to      |
        |                       |                       | [`test                |
        |                       |                       | s`](GenruleDescriptio |
        |                       |                       | nArg.html#getTests()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `G                    | `build()`             | ::: block             |
        | enruleDescriptionArg` |                       | Builds a new          |
        |                       |                       | [`Gen                 |
        |                       |                       | ruleDescriptionArg`]( |
        |                       |                       | GenruleDescriptionArg |
        |                       |                       | .html "class in com.f |
        |                       |                       | acebook.buck.shell"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `GenruleDe            | `from​(Bu              | ::: block             |
        | scriptionArg.Builder` | ildRuleArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebo           |
        |                       |                       | ok.buck.core.descript |
        |                       |                       | ion.arg.BuildRuleArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `GenruleDe            | `from​(Cons            | ::: block             |
        | scriptionArg.Builder` | tructorArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook         |
        |                       |                       | .buck.core.descriptio |
        |                       |                       | n.arg.ConstructorArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `GenruleDe            | `fro                  | ::: block             |
        | scriptionArg.Builder` | m​(HasTests instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.fa               |
        |                       |                       | cebook.buck.core.desc |
        |                       |                       | ription.arg.HasTests` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `GenruleDe            | `from​(Abstr           | ::: block             |
        | scriptionArg.Builder` | actGenruleDescription | Fill a builder with   |
        |                       | .CommonArg instance)` | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook.buck.s  |
        |                       |                       | hell.AbstractGenruleD |
        |                       |                       | escription.CommonArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `GenruleDe            | `from                 | ::: block             |
        | scriptionArg.Builder` | ​(com.facebook.buck.sh | Copy abstract value   |
        |                       | ell.GenruleDescriptio | type                  |
        |                       | n.AbstractGenruleDesc | `AbstractG            |
        |                       | riptionArg instance)` | enruleDescriptionArg` |
        |                       |                       | instance into         |
        |                       |                       | builder.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `GenruleDe            | `from​(GenruleDesc     | ::: block             |
        | scriptionArg.Builder` | riptionArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `G                    |
        |                       |                       | enruleDescriptionArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `GenruleDe            | `setBash​(St           | ::: block             |
        | scriptionArg.Builder` | ringWithMacros bash)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`ba                  |
        |                       |                       | sh`](GenruleDescripti |
        |                       |                       | onArg.html#getBash()) |
        |                       |                       | to bash.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `GenruleDe            | `setBash​(O            | ::: block             |
        | scriptionArg.Builder` | ptional<? extends Str | Initializes the       |
        |                       | ingWithMacros> bash)` | optional value        |
        |                       |                       | [`ba                  |
        |                       |                       | sh`](GenruleDescripti |
        |                       |                       | onArg.html#getBash()) |
        |                       |                       | to bash.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `GenruleDe            | `setCacheabl          | ::: block             |
        | scriptionArg.Builder` | e​(boolean cacheable)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`cacheable`](        |
        |                       |                       | GenruleDescriptionArg |
        |                       |                       | .html#getCacheable()) |
        |                       |                       | to cacheable.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `GenruleDe            | `                     | ::: block             |
        | scriptionArg.Builder` | setCacheable​(Optional | Initializes the       |
        |                       | <Boolean> cacheable)` | optional value        |
        |                       |                       | [`cacheable`](        |
        |                       |                       | GenruleDescriptionArg |
        |                       |                       | .html#getCacheable()) |
        |                       |                       | to cacheable.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `GenruleDe            | `setCmd​(S             | ::: block             |
        | scriptionArg.Builder` | tringWithMacros cmd)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`                    |
        |                       |                       | cmd`](GenruleDescript |
        |                       |                       | ionArg.html#getCmd()) |
        |                       |                       | to cmd.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `GenruleDe            | `setCmd​(              | ::: block             |
        | scriptionArg.Builder` | Optional<? extends St | Initializes the       |
        |                       | ringWithMacros> cmd)` | optional value        |
        |                       |                       | [`                    |
        |                       |                       | cmd`](GenruleDescript |
        |                       |                       | ionArg.html#getCmd()) |
        |                       |                       | to cmd.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `GenruleDe            | `setCmdExe​(Stri       | ::: block             |
        | scriptionArg.Builder` | ngWithMacros cmdExe)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`cmdExe              |
        |                       |                       | `](GenruleDescription |
        |                       |                       | Arg.html#getCmdExe()) |
        |                       |                       | to cmdExe.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `GenruleDe            | `setCmdExe​(Opt        | ::: block             |
        | scriptionArg.Builder` | ional<? extends Strin | Initializes the       |
        |                       | gWithMacros> cmdExe)` | optional value        |
        |                       |                       | [`cmdExe              |
        |                       |                       | `](GenruleDescription |
        |                       |                       | Arg.html#getCmdExe()) |
        |                       |                       | to cmdExe.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `GenruleDe            | `setCompat            | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Iterable<? e | Sets or replaces all  |
        |                       | xtends UnconfiguredBu | elements for          |
        |                       | ildTarget> elements)` | [`c                   |
        |                       |                       | ompatibleWith`](Genru |
        |                       |                       | leDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `GenruleDe            | `setDefaul            | ::: block             |
        | scriptionArg.Builder` | tTargetPlatform​(Uncon | Initializes the       |
        |                       | figuredBuildTarget de | optional value        |
        |                       | faultTargetPlatform)` | [`defaultTargetPl     |
        |                       |                       | atform`](GenruleDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `GenruleDe            | `setDefau             | ::: block             |
        | scriptionArg.Builder` | ltTargetPlatform​(Opti | Initializes the       |
        |                       | onal<? extends Unconf | optional value        |
        |                       | iguredBuildTarget> de | [`defaultTargetPl     |
        |                       | faultTargetPlatform)` | atform`](GenruleDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `GenruleDe            | `setEnableSandbox​(bo  | ::: block             |
        | scriptionArg.Builder` | olean enableSandbox)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [                     |
        |                       |                       | `enableSandbox`](Genr |
        |                       |                       | uleDescriptionArg.htm |
        |                       |                       | l#getEnableSandbox()) |
        |                       |                       | to enableSandbox.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `GenruleDe            | `setEnabl             | ::: block             |
        | scriptionArg.Builder` | eSandbox​(Optional<Boo | Initializes the       |
        |                       | lean> enableSandbox)` | optional value        |
        |                       |                       | [                     |
        |                       |                       | `enableSandbox`](Genr |
        |                       |                       | uleDescriptionArg.htm |
        |                       |                       | l#getEnableSandbox()) |
        |                       |                       | to enableSandbox.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `GenruleDe            | `setEnvir             | ::: block             |
        | scriptionArg.Builder` | onmentExpansionSepara | Initializes the       |
        |                       | tor​(String environmen | optional value        |
        |                       | tExpansionSeparator)` | [`environmen          |
        |                       |                       | tExpansionSeparator`] |
        |                       |                       | (GenruleDescriptionAr |
        |                       |                       | g.html#getEnvironment |
        |                       |                       | ExpansionSeparator()) |
        |                       |                       | to                    |
        |                       |                       | environme             |
        |                       |                       | ntExpansionSeparator. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `GenruleDe            | `setEnvironmentExpa   | ::: block             |
        | scriptionArg.Builder` | nsionSeparator​(Option | Initializes the       |
        |                       | al<String> environmen | optional value        |
        |                       | tExpansionSeparator)` | [`environmen          |
        |                       |                       | tExpansionSeparator`] |
        |                       |                       | (GenruleDescriptionAr |
        |                       |                       | g.html#getEnvironment |
        |                       |                       | ExpansionSeparator()) |
        |                       |                       | to                    |
        |                       |                       | environme             |
        |                       |                       | ntExpansionSeparator. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `GenruleDe            | `setExecutable        | ::: block             |
        | scriptionArg.Builder` | ​(boolean executable)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`executable`](G      |
        |                       |                       | enruleDescriptionArg. |
        |                       |                       | html#getExecutable()) |
        |                       |                       | to executable.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `GenruleDe            | `se                   | ::: block             |
        | scriptionArg.Builder` | tExecutable​(Optional< | Initializes the       |
        |                       | Boolean> executable)` | optional value        |
        |                       |                       | [`executable`](G      |
        |                       |                       | enruleDescriptionArg. |
        |                       |                       | html#getExecutable()) |
        |                       |                       | to executable.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `GenruleDe            | `setLabels​(Iterab     | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Sets or replaces all  |
        |                       |                       | elements for          |
        |                       |                       | [`labels              |
        |                       |                       | `](GenruleDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `GenruleDe            | `setLicenses          | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Sets or replaces all  |
        |                       | ourcePath> elements)` | elements for          |
        |                       |                       | [`licenses`]          |
        |                       |                       | (GenruleDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `GenruleDe            | `                     | ::: block             |
        | scriptionArg.Builder` | setName​(String name)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`na                  |
        |                       |                       | me`](GenruleDescripti |
        |                       |                       | onArg.html#getName()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `GenruleDe            | `setN                 | ::: block             |
        | scriptionArg.Builder` | eedAndroidTools​(boole | Initializes the value |
        |                       | an needAndroidTools)` | for the               |
        |                       |                       | [`need                |
        |                       |                       | AndroidTools`](Genrul |
        |                       |                       | eDescriptionArg.html# |
        |                       |                       | isNeedAndroidTools()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `GenruleDe            | `setOut​(String out)`  | ::: block             |
        | scriptionArg.Builder` |                       | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`                    |
        |                       |                       | out`](GenruleDescript |
        |                       |                       | ionArg.html#getOut()) |
        |                       |                       | to out.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `GenruleDe            | `setOut​(O             | ::: block             |
        | scriptionArg.Builder` | ptional<String> out)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`                    |
        |                       |                       | out`](GenruleDescript |
        |                       |                       | ionArg.html#getOut()) |
        |                       |                       | to out.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `GenruleDe            | `set                  | ::: block             |
        | scriptionArg.Builder` | Outs​(com.google.commo | Initializes the       |
        |                       | n.collect.ImmutableMa | optional value        |
        |                       | p<String,​com.google.c | [`ou                  |
        |                       | ommon.collect.Immutab | ts`](GenruleDescripti |
        |                       | leSet<String>> outs)` | onArg.html#getOuts()) |
        |                       |                       | to outs.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `GenruleDe            | `se                   | ::: block             |
        | scriptionArg.Builder` | tOuts​(Optional<? exte | Initializes the       |
        |                       | nds com.google.common | optional value        |
        |                       | .collect.ImmutableMap | [`ou                  |
        |                       | <String,​com.google.co | ts`](GenruleDescripti |
        |                       | mmon.collect.Immutabl | onArg.html#getOuts()) |
        |                       | eSet<String>>> outs)` | to outs.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `GenruleDe            | `setRe                | ::: block             |
        | scriptionArg.Builder` | mote​(boolean remote)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`remote              |
        |                       |                       | `](GenruleDescription |
        |                       |                       | Arg.html#getRemote()) |
        |                       |                       | to remote.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `GenruleDe            | `setRemote​(Optio      | ::: block             |
        | scriptionArg.Builder` | nal<Boolean> remote)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`remote              |
        |                       |                       | `](GenruleDescription |
        |                       |                       | Arg.html#getRemote()) |
        |                       |                       | to remote.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `GenruleDe            | `set                  | ::: block             |
        | scriptionArg.Builder` | Srcs​(SourceSet srcs)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`sr                  |
        |                       |                       | cs`](GenruleDescripti |
        |                       |                       | onArg.html#getSrcs()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `GenruleDe            | `setTests​(            | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Sets or replaces all  |
        |                       | ildTarget> elements)` | elements for          |
        |                       |                       | [`test                |
        |                       |                       | s`](GenruleDescriptio |
        |                       |                       | nArg.html#getTests()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `GenruleDe            | `                     | ::: block             |
        | scriptionArg.Builder` | setType​(String type)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`ty                  |
        |                       |                       | pe`](GenruleDescripti |
        |                       |                       | onArg.html#getType()) |
        |                       |                       | to type.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `GenruleDe            | `setType​(Op           | ::: block             |
        | scriptionArg.Builder` | tional<String> type)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`ty                  |
        |                       |                       | pe`](GenruleDescripti |
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

        []{#from(com.facebook.buck.shell.GenruleDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final GenruleDescriptionArg.Builder from​(GenruleDescriptionArg instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `GenruleDescriptionArg` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.shell.GenruleDescription.AbstractGenruleDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final GenruleDescriptionArg.Builder from​(com.facebook.buck.shell.GenruleDescription.AbstractGenruleDescriptionArg instance)
            ```

            ::: block
            Copy abstract value type `AbstractGenruleDescriptionArg`
            instance into builder.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.core.description.arg.HasTests)}

        -   #### from

            ``` methodSignature
            public final GenruleDescriptionArg.Builder from​(HasTests instance)
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
            public final GenruleDescriptionArg.Builder from​(AbstractGenruleDescription.CommonArg instance)
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
            public final GenruleDescriptionArg.Builder from​(BuildRuleArg instance)
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
            public final GenruleDescriptionArg.Builder from​(ConstructorArg instance)
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

        []{#setOut(java.lang.String)}

        -   #### setOut

            ``` methodSignature
            public final GenruleDescriptionArg.Builder setOut​(String out)
            ```

            ::: block
            Initializes the optional value
            [`out`](GenruleDescriptionArg.html#getOut()) to out.
            :::

            [Parameters:]{.paramLabel}
            :   `out` - The value for out

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setOut(java.util.Optional)}

        -   #### setOut

            ``` methodSignature
            public final GenruleDescriptionArg.Builder setOut​(Optional<String> out)
            ```

            ::: block
            Initializes the optional value
            [`out`](GenruleDescriptionArg.html#getOut()) to out.
            :::

            [Parameters:]{.paramLabel}
            :   `out` - The value for out

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setOuts(com.google.common.collect.ImmutableMap)}

        -   #### setOuts

            ``` methodSignature
            public final GenruleDescriptionArg.Builder setOuts​(com.google.common.collect.ImmutableMap<String,​com.google.common.collect.ImmutableSet<String>> outs)
            ```

            ::: block
            Initializes the optional value
            [`outs`](GenruleDescriptionArg.html#getOuts()) to outs.
            :::

            [Parameters:]{.paramLabel}
            :   `outs` - The value for outs

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setOuts(java.util.Optional)}

        -   #### setOuts

            ``` methodSignature
            public final GenruleDescriptionArg.Builder setOuts​(Optional<? extends com.google.common.collect.ImmutableMap<String,​com.google.common.collect.ImmutableSet<String>>> outs)
            ```

            ::: block
            Initializes the optional value
            [`outs`](GenruleDescriptionArg.html#getOuts()) to outs.
            :::

            [Parameters:]{.paramLabel}
            :   `outs` - The value for outs

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setExecutable(boolean)}

        -   #### setExecutable

            ``` methodSignature
            public final GenruleDescriptionArg.Builder setExecutable​(boolean executable)
            ```

            ::: block
            Initializes the optional value
            [`executable`](GenruleDescriptionArg.html#getExecutable())
            to executable.
            :::

            [Parameters:]{.paramLabel}
            :   `executable` - The value for executable

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setExecutable(java.util.Optional)}

        -   #### setExecutable

            ``` methodSignature
            public final GenruleDescriptionArg.Builder setExecutable​(Optional<Boolean> executable)
            ```

            ::: block
            Initializes the optional value
            [`executable`](GenruleDescriptionArg.html#getExecutable())
            to executable.
            :::

            [Parameters:]{.paramLabel}
            :   `executable` - The value for executable

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setBash(com.facebook.buck.rules.macros.StringWithMacros)}

        -   #### setBash

            ``` methodSignature
            public final GenruleDescriptionArg.Builder setBash​(StringWithMacros bash)
            ```

            ::: block
            Initializes the optional value
            [`bash`](GenruleDescriptionArg.html#getBash()) to bash.
            :::

            [Parameters:]{.paramLabel}
            :   `bash` - The value for bash

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setBash(java.util.Optional)}

        -   #### setBash

            ``` methodSignature
            public final GenruleDescriptionArg.Builder setBash​(Optional<? extends StringWithMacros> bash)
            ```

            ::: block
            Initializes the optional value
            [`bash`](GenruleDescriptionArg.html#getBash()) to bash.
            :::

            [Parameters:]{.paramLabel}
            :   `bash` - The value for bash

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCmd(com.facebook.buck.rules.macros.StringWithMacros)}

        -   #### setCmd

            ``` methodSignature
            public final GenruleDescriptionArg.Builder setCmd​(StringWithMacros cmd)
            ```

            ::: block
            Initializes the optional value
            [`cmd`](GenruleDescriptionArg.html#getCmd()) to cmd.
            :::

            [Parameters:]{.paramLabel}
            :   `cmd` - The value for cmd

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setCmd(java.util.Optional)}

        -   #### setCmd

            ``` methodSignature
            public final GenruleDescriptionArg.Builder setCmd​(Optional<? extends StringWithMacros> cmd)
            ```

            ::: block
            Initializes the optional value
            [`cmd`](GenruleDescriptionArg.html#getCmd()) to cmd.
            :::

            [Parameters:]{.paramLabel}
            :   `cmd` - The value for cmd

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCmdExe(com.facebook.buck.rules.macros.StringWithMacros)}

        -   #### setCmdExe

            ``` methodSignature
            public final GenruleDescriptionArg.Builder setCmdExe​(StringWithMacros cmdExe)
            ```

            ::: block
            Initializes the optional value
            [`cmdExe`](GenruleDescriptionArg.html#getCmdExe()) to
            cmdExe.
            :::

            [Parameters:]{.paramLabel}
            :   `cmdExe` - The value for cmdExe

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setCmdExe(java.util.Optional)}

        -   #### setCmdExe

            ``` methodSignature
            public final GenruleDescriptionArg.Builder setCmdExe​(Optional<? extends StringWithMacros> cmdExe)
            ```

            ::: block
            Initializes the optional value
            [`cmdExe`](GenruleDescriptionArg.html#getCmdExe()) to
            cmdExe.
            :::

            [Parameters:]{.paramLabel}
            :   `cmdExe` - The value for cmdExe

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setType(java.lang.String)}

        -   #### setType

            ``` methodSignature
            public final GenruleDescriptionArg.Builder setType​(String type)
            ```

            ::: block
            Initializes the optional value
            [`type`](GenruleDescriptionArg.html#getType()) to type.
            :::

            [Parameters:]{.paramLabel}
            :   `type` - The value for type

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setType(java.util.Optional)}

        -   #### setType

            ``` methodSignature
            public final GenruleDescriptionArg.Builder setType​(Optional<String> type)
            ```

            ::: block
            Initializes the optional value
            [`type`](GenruleDescriptionArg.html#getType()) to type.
            :::

            [Parameters:]{.paramLabel}
            :   `type` - The value for type

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setSrcs(com.facebook.buck.rules.coercer.SourceSet)}

        -   #### setSrcs

            ``` methodSignature
            public final GenruleDescriptionArg.Builder setSrcs​(SourceSet srcs)
            ```

            ::: block
            Initializes the value for the
            [`srcs`](GenruleDescriptionArg.html#getSrcs()) attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`srcs`](GenruleDescriptionArg.html#getSrcs()).*
            :::

            [Parameters:]{.paramLabel}
            :   `srcs` - The value for srcs

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setEnableSandbox(boolean)}

        -   #### setEnableSandbox

            ``` methodSignature
            public final GenruleDescriptionArg.Builder setEnableSandbox​(boolean enableSandbox)
            ```

            ::: block
            Initializes the optional value
            [`enableSandbox`](GenruleDescriptionArg.html#getEnableSandbox())
            to enableSandbox.
            :::

            [Parameters:]{.paramLabel}
            :   `enableSandbox` - The value for enableSandbox

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setEnableSandbox(java.util.Optional)}

        -   #### setEnableSandbox

            ``` methodSignature
            public final GenruleDescriptionArg.Builder setEnableSandbox​(Optional<Boolean> enableSandbox)
            ```

            ::: block
            Initializes the optional value
            [`enableSandbox`](GenruleDescriptionArg.html#getEnableSandbox())
            to enableSandbox.
            :::

            [Parameters:]{.paramLabel}
            :   `enableSandbox` - The value for enableSandbox

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setEnvironmentExpansionSeparator(java.lang.String)}

        -   #### setEnvironmentExpansionSeparator

            ``` methodSignature
            public final GenruleDescriptionArg.Builder setEnvironmentExpansionSeparator​(String environmentExpansionSeparator)
            ```

            ::: block
            Initializes the optional value
            [`environmentExpansionSeparator`](GenruleDescriptionArg.html#getEnvironmentExpansionSeparator())
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
            public final GenruleDescriptionArg.Builder setEnvironmentExpansionSeparator​(Optional<String> environmentExpansionSeparator)
            ```

            ::: block
            Initializes the optional value
            [`environmentExpansionSeparator`](GenruleDescriptionArg.html#getEnvironmentExpansionSeparator())
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
            public final GenruleDescriptionArg.Builder setRemote​(boolean remote)
            ```

            ::: block
            Initializes the optional value
            [`remote`](GenruleDescriptionArg.html#getRemote()) to
            remote.
            :::

            [Parameters:]{.paramLabel}
            :   `remote` - The value for remote

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setRemote(java.util.Optional)}

        -   #### setRemote

            ``` methodSignature
            public final GenruleDescriptionArg.Builder setRemote​(Optional<Boolean> remote)
            ```

            ::: block
            Initializes the optional value
            [`remote`](GenruleDescriptionArg.html#getRemote()) to
            remote.
            :::

            [Parameters:]{.paramLabel}
            :   `remote` - The value for remote

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCacheable(boolean)}

        -   #### setCacheable

            ``` methodSignature
            public final GenruleDescriptionArg.Builder setCacheable​(boolean cacheable)
            ```

            ::: block
            Initializes the optional value
            [`cacheable`](GenruleDescriptionArg.html#getCacheable()) to
            cacheable.
            :::

            [Parameters:]{.paramLabel}
            :   `cacheable` - The value for cacheable

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setCacheable(java.util.Optional)}

        -   #### setCacheable

            ``` methodSignature
            public final GenruleDescriptionArg.Builder setCacheable​(Optional<Boolean> cacheable)
            ```

            ::: block
            Initializes the optional value
            [`cacheable`](GenruleDescriptionArg.html#getCacheable()) to
            cacheable.
            :::

            [Parameters:]{.paramLabel}
            :   `cacheable` - The value for cacheable

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setNeedAndroidTools(boolean)}

        -   #### setNeedAndroidTools

            ``` methodSignature
            public final GenruleDescriptionArg.Builder setNeedAndroidTools​(boolean needAndroidTools)
            ```

            ::: block
            Initializes the value for the
            [`needAndroidTools`](GenruleDescriptionArg.html#isNeedAndroidTools())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`needAndroidTools`](GenruleDescriptionArg.html#isNeedAndroidTools()).*
            :::

            [Parameters:]{.paramLabel}
            :   `needAndroidTools` - The value for needAndroidTools

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLicenses(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### addLicenses

            ``` methodSignature
            public final GenruleDescriptionArg.Builder addLicenses​(SourcePath element)
            ```

            ::: block
            Adds one element to
            [`licenses`](GenruleDescriptionArg.html#getLicenses()) set.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A licenses element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLicenses(com.facebook.buck.core.sourcepath.SourcePath...)}

        -   #### addLicenses

            ``` methodSignature
            public final GenruleDescriptionArg.Builder addLicenses​(SourcePath... elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](GenruleDescriptionArg.html#getLicenses()) set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLicenses(java.lang.Iterable)}

        -   #### setLicenses

            ``` methodSignature
            public final GenruleDescriptionArg.Builder setLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`licenses`](GenruleDescriptionArg.html#getLicenses()) set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLicenses(java.lang.Iterable)}

        -   #### addAllLicenses

            ``` methodSignature
            public final GenruleDescriptionArg.Builder addAllLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](GenruleDescriptionArg.html#getLicenses()) set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLabels(java.lang.String)}

        -   #### addLabels

            ``` methodSignature
            public final GenruleDescriptionArg.Builder addLabels​(String element)
            ```

            ::: block
            Adds one element to
            [`labels`](GenruleDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A labels element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLabels(java.lang.String...)}

        -   #### addLabels

            ``` methodSignature
            public final GenruleDescriptionArg.Builder addLabels​(String... elements)
            ```

            ::: block
            Adds elements to
            [`labels`](GenruleDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLabels(java.lang.Iterable)}

        -   #### setLabels

            ``` methodSignature
            public final GenruleDescriptionArg.Builder setLabels​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`labels`](GenruleDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLabels(java.lang.Iterable)}

        -   #### addAllLabels

            ``` methodSignature
            public final GenruleDescriptionArg.Builder addAllLabels​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`labels`](GenruleDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDefaultTargetPlatform(com.facebook.buck.core.model.UnconfiguredBuildTarget)}

        -   #### setDefaultTargetPlatform

            ``` methodSignature
            public final GenruleDescriptionArg.Builder setDefaultTargetPlatform​(UnconfiguredBuildTarget defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](GenruleDescriptionArg.html#getDefaultTargetPlatform())
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
            public final GenruleDescriptionArg.Builder setDefaultTargetPlatform​(Optional<? extends UnconfiguredBuildTarget> defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](GenruleDescriptionArg.html#getDefaultTargetPlatform())
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
            public final GenruleDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget element)
            ```

            ::: block
            Adds one element to
            [`compatibleWith`](GenruleDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A compatibleWith element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCompatibleWith(com.facebook.buck.core.model.UnconfiguredBuildTarget...)}

        -   #### addCompatibleWith

            ``` methodSignature
            public final GenruleDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](GenruleDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCompatibleWith(java.lang.Iterable)}

        -   #### setCompatibleWith

            ``` methodSignature
            public final GenruleDescriptionArg.Builder setCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`compatibleWith`](GenruleDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllCompatibleWith(java.lang.Iterable)}

        -   #### addAllCompatibleWith

            ``` methodSignature
            public final GenruleDescriptionArg.Builder addAllCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](GenruleDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setName(java.lang.String)}

        -   #### setName

            ``` methodSignature
            public final GenruleDescriptionArg.Builder setName​(String name)
            ```

            ::: block
            Initializes the value for the
            [`name`](GenruleDescriptionArg.html#getName()) attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `name` - The value for name

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addTests(com.facebook.buck.core.model.BuildTarget)}

        -   #### addTests

            ``` methodSignature
            public final GenruleDescriptionArg.Builder addTests​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`tests`](GenruleDescriptionArg.html#getTests()) sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A tests element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addTests(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addTests

            ``` methodSignature
            public final GenruleDescriptionArg.Builder addTests​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`tests`](GenruleDescriptionArg.html#getTests()) sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of tests elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setTests(java.lang.Iterable)}

        -   #### setTests

            ``` methodSignature
            public final GenruleDescriptionArg.Builder setTests​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`tests`](GenruleDescriptionArg.html#getTests()) sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of tests elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllTests(java.lang.Iterable)}

        -   #### addAllTests

            ``` methodSignature
            public final GenruleDescriptionArg.Builder addAllTests​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`tests`](GenruleDescriptionArg.html#getTests()) sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of tests elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#build()}

        -   #### build

            ``` methodSignature
            public GenruleDescriptionArg build()
            ```

            ::: block
            Builds a new
            [`GenruleDescriptionArg`](GenruleDescriptionArg.html "class in com.facebook.buck.shell").
            :::

            [Returns:]{.returnLabel}
            :   An immutable instance of GenruleDescriptionArg

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
