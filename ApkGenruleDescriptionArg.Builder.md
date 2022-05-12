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

## Class ApkGenruleDescriptionArg.Builder {#class-apkgenruledescriptionarg.builder .title title="Class ApkGenruleDescriptionArg.Builder"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.android.ApkGenruleDescriptionArg.Builder

::: description
-   

    Enclosing class:
    :   [ApkGenruleDescriptionArg](ApkGenruleDescriptionArg.html "class in com.facebook.buck.android")

    ------------------------------------------------------------------------

        @NotThreadSafe
        public static final class ApkGenruleDescriptionArg.Builder
        extends Object

    ::: block
    Builds instances of type
    [`ApkGenruleDescriptionArg`](ApkGenruleDescriptionArg.html "class in com.facebook.buck.android").
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
        | `ApkGenruleDe         | `addAllCompat         | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Iterable<? e | Adds elements to      |
        |                       | xtends UnconfiguredBu | [`comp                |
        |                       | ildTarget> elements)` | atibleWith`](ApkGenru |
        |                       |                       | leDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ApkGenruleDe         | `addAllLabels​(Iterab  | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Adds elements to      |
        |                       |                       | [`labels`](           |
        |                       |                       | ApkGenruleDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ApkGenruleDe         | `addAllLicenses       | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Adds elements to      |
        |                       | ourcePath> elements)` | [`licenses`](Ap       |
        |                       |                       | kGenruleDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ApkGenruleDe         | `addAllTests​(         | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Adds elements to      |
        |                       | ildTarget> elements)` | [`tests`]             |
        |                       |                       | (ApkGenruleDescriptio |
        |                       |                       | nArg.html#getTests()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ApkGenruleDe         | `addCompat            | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Unconfigured | Adds one element to   |
        |                       | BuildTarget element)` | [`comp                |
        |                       |                       | atibleWith`](ApkGenru |
        |                       |                       | leDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ApkGenruleDe         | `addCompatible        | ::: block             |
        | scriptionArg.Builder` | With​(UnconfiguredBuil | Adds elements to      |
        |                       | dTarget... elements)` | [`comp                |
        |                       |                       | atibleWith`](ApkGenru |
        |                       |                       | leDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ApkGenruleDe         | `addLa                | ::: block             |
        | scriptionArg.Builder` | bels​(String element)` | Adds one element to   |
        |                       |                       | [`labels`](           |
        |                       |                       | ApkGenruleDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ApkGenruleDe         | `addLabels            | ::: block             |
        | scriptionArg.Builder` | ​(String... elements)` | Adds elements to      |
        |                       |                       | [`labels`](           |
        |                       |                       | ApkGenruleDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ApkGenruleDe         | `addLicenses          | ::: block             |
        | scriptionArg.Builder` | ​(SourcePath element)` | Adds one element to   |
        |                       |                       | [`licenses`](Ap       |
        |                       |                       | kGenruleDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ApkGenruleDe         | `addLicenses​(Sou      | ::: block             |
        | scriptionArg.Builder` | rcePath... elements)` | Adds elements to      |
        |                       |                       | [`licenses`](Ap       |
        |                       |                       | kGenruleDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ApkGenruleDe         | `addTests​(            | ::: block             |
        | scriptionArg.Builder` | BuildTarget element)` | Adds one element to   |
        |                       |                       | [`tests`]             |
        |                       |                       | (ApkGenruleDescriptio |
        |                       |                       | nArg.html#getTests()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ApkGenruleDe         | `addTests​(Buil        | ::: block             |
        | scriptionArg.Builder` | dTarget... elements)` | Adds elements to      |
        |                       |                       | [`tests`]             |
        |                       |                       | (ApkGenruleDescriptio |
        |                       |                       | nArg.html#getTests()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ApkG                 | `build()`             | ::: block             |
        | enruleDescriptionArg` |                       | Builds a new          |
        |                       |                       | [`ApkGenruleD         |
        |                       |                       | escriptionArg`](ApkGe |
        |                       |                       | nruleDescriptionArg.h |
        |                       |                       | tml "class in com.fac |
        |                       |                       | ebook.buck.android"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ApkGenruleDe         | `from​(com.fac         | ::: block             |
        | scriptionArg.Builder` | ebook.buck.android.Ap | Copy abstract value   |
        |                       | kGenruleDescription.A | type                  |
        |                       | bstractApkGenruleDesc | `AbstractApkG         |
        |                       | riptionArg instance)` | enruleDescriptionArg` |
        |                       |                       | instance into         |
        |                       |                       | builder.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ApkGenruleDe         | `from​(ApkGenruleDesc  | ::: block             |
        | scriptionArg.Builder` | riptionArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `ApkG                 |
        |                       |                       | enruleDescriptionArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ApkGenruleDe         | `from​(Bu              | ::: block             |
        | scriptionArg.Builder` | ildRuleArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebo           |
        |                       |                       | ok.buck.core.descript |
        |                       |                       | ion.arg.BuildRuleArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ApkGenruleDe         | `from​(Cons            | ::: block             |
        | scriptionArg.Builder` | tructorArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook         |
        |                       |                       | .buck.core.descriptio |
        |                       |                       | n.arg.ConstructorArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ApkGenruleDe         | `fro                  | ::: block             |
        | scriptionArg.Builder` | m​(HasTests instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.fa               |
        |                       |                       | cebook.buck.core.desc |
        |                       |                       | ription.arg.HasTests` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ApkGenruleDe         | `from​(Abstr           | ::: block             |
        | scriptionArg.Builder` | actGenruleDescription | Fill a builder with   |
        |                       | .CommonArg instance)` | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook.buck.s  |
        |                       |                       | hell.AbstractGenruleD |
        |                       |                       | escription.CommonArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ApkGenruleDe         | `set                  | ::: block             |
        | scriptionArg.Builder` | Apk​(BuildTarget apk)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`apk                 |
        |                       |                       | `](ApkGenruleDescript |
        |                       |                       | ionArg.html#getApk()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ApkGenruleDe         | `setBash​(St           | ::: block             |
        | scriptionArg.Builder` | ringWithMacros bash)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`bash`               |
        |                       |                       | ](ApkGenruleDescripti |
        |                       |                       | onArg.html#getBash()) |
        |                       |                       | to bash.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ApkGenruleDe         | `setBash​(O            | ::: block             |
        | scriptionArg.Builder` | ptional<? extends Str | Initializes the       |
        |                       | ingWithMacros> bash)` | optional value        |
        |                       |                       | [`bash`               |
        |                       |                       | ](ApkGenruleDescripti |
        |                       |                       | onArg.html#getBash()) |
        |                       |                       | to bash.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ApkGenruleDe         | `setCacheabl          | ::: block             |
        | scriptionArg.Builder` | e​(boolean cacheable)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`cacheable`](Apk     |
        |                       |                       | GenruleDescriptionArg |
        |                       |                       | .html#getCacheable()) |
        |                       |                       | to cacheable.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ApkGenruleDe         | `                     | ::: block             |
        | scriptionArg.Builder` | setCacheable​(Optional | Initializes the       |
        |                       | <Boolean> cacheable)` | optional value        |
        |                       |                       | [`cacheable`](Apk     |
        |                       |                       | GenruleDescriptionArg |
        |                       |                       | .html#getCacheable()) |
        |                       |                       | to cacheable.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ApkGenruleDe         | `setCmd​(S             | ::: block             |
        | scriptionArg.Builder` | tringWithMacros cmd)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`cmd                 |
        |                       |                       | `](ApkGenruleDescript |
        |                       |                       | ionArg.html#getCmd()) |
        |                       |                       | to cmd.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ApkGenruleDe         | `setCmd​(              | ::: block             |
        | scriptionArg.Builder` | Optional<? extends St | Initializes the       |
        |                       | ringWithMacros> cmd)` | optional value        |
        |                       |                       | [`cmd                 |
        |                       |                       | `](ApkGenruleDescript |
        |                       |                       | ionArg.html#getCmd()) |
        |                       |                       | to cmd.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ApkGenruleDe         | `setCmdExe​(Stri       | ::: block             |
        | scriptionArg.Builder` | ngWithMacros cmdExe)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`cmdExe`](           |
        |                       |                       | ApkGenruleDescription |
        |                       |                       | Arg.html#getCmdExe()) |
        |                       |                       | to cmdExe.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ApkGenruleDe         | `setCmdExe​(Opt        | ::: block             |
        | scriptionArg.Builder` | ional<? extends Strin | Initializes the       |
        |                       | gWithMacros> cmdExe)` | optional value        |
        |                       |                       | [`cmdExe`](           |
        |                       |                       | ApkGenruleDescription |
        |                       |                       | Arg.html#getCmdExe()) |
        |                       |                       | to cmdExe.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ApkGenruleDe         | `setCompat            | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Iterable<? e | Sets or replaces all  |
        |                       | xtends UnconfiguredBu | elements for          |
        |                       | ildTarget> elements)` | [`comp                |
        |                       |                       | atibleWith`](ApkGenru |
        |                       |                       | leDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ApkGenruleDe         | `setDefaul            | ::: block             |
        | scriptionArg.Builder` | tTargetPlatform​(Uncon | Initializes the       |
        |                       | figuredBuildTarget de | optional value        |
        |                       | faultTargetPlatform)` | [`defaultTargetPlatf  |
        |                       |                       | orm`](ApkGenruleDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ApkGenruleDe         | `setDefau             | ::: block             |
        | scriptionArg.Builder` | ltTargetPlatform​(Opti | Initializes the       |
        |                       | onal<? extends Unconf | optional value        |
        |                       | iguredBuildTarget> de | [`defaultTargetPlatf  |
        |                       | faultTargetPlatform)` | orm`](ApkGenruleDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ApkGenruleDe         | `setEnableSandbox​(bo  | ::: block             |
        | scriptionArg.Builder` | olean enableSandbox)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`en                  |
        |                       |                       | ableSandbox`](ApkGenr |
        |                       |                       | uleDescriptionArg.htm |
        |                       |                       | l#getEnableSandbox()) |
        |                       |                       | to enableSandbox.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ApkGenruleDe         | `setEnabl             | ::: block             |
        | scriptionArg.Builder` | eSandbox​(Optional<Boo | Initializes the       |
        |                       | lean> enableSandbox)` | optional value        |
        |                       |                       | [`en                  |
        |                       |                       | ableSandbox`](ApkGenr |
        |                       |                       | uleDescriptionArg.htm |
        |                       |                       | l#getEnableSandbox()) |
        |                       |                       | to enableSandbox.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ApkGenruleDe         | `setEnvir             | ::: block             |
        | scriptionArg.Builder` | onmentExpansionSepara | Initializes the       |
        |                       | tor​(String environmen | optional value        |
        |                       | tExpansionSeparator)` | [`environmentEx       |
        |                       |                       | pansionSeparator`](Ap |
        |                       |                       | kGenruleDescriptionAr |
        |                       |                       | g.html#getEnvironment |
        |                       |                       | ExpansionSeparator()) |
        |                       |                       | to                    |
        |                       |                       | environme             |
        |                       |                       | ntExpansionSeparator. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ApkGenruleDe         | `setEnvironmentExpa   | ::: block             |
        | scriptionArg.Builder` | nsionSeparator​(Option | Initializes the       |
        |                       | al<String> environmen | optional value        |
        |                       | tExpansionSeparator)` | [`environmentEx       |
        |                       |                       | pansionSeparator`](Ap |
        |                       |                       | kGenruleDescriptionAr |
        |                       |                       | g.html#getEnvironment |
        |                       |                       | ExpansionSeparator()) |
        |                       |                       | to                    |
        |                       |                       | environme             |
        |                       |                       | ntExpansionSeparator. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ApkGenruleDe         | `setIsCacheable​(      | ::: block             |
        | scriptionArg.Builder` | boolean isCacheable)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`isCacheable`](ApkGe |
        |                       |                       | nruleDescriptionArg.h |
        |                       |                       | tml#getIsCacheable()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ApkGenruleDe         | `setLabels​(Iterab     | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Sets or replaces all  |
        |                       |                       | elements for          |
        |                       |                       | [`labels`](           |
        |                       |                       | ApkGenruleDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ApkGenruleDe         | `setLicenses          | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Sets or replaces all  |
        |                       | ourcePath> elements)` | elements for          |
        |                       |                       | [`licenses`](Ap       |
        |                       |                       | kGenruleDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ApkGenruleDe         | `                     | ::: block             |
        | scriptionArg.Builder` | setName​(String name)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`name`               |
        |                       |                       | ](ApkGenruleDescripti |
        |                       |                       | onArg.html#getName()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ApkGenruleDe         | `setN                 | ::: block             |
        | scriptionArg.Builder` | eedAndroidTools​(boole | Initializes the value |
        |                       | an needAndroidTools)` | for the               |
        |                       |                       | [`needAnd             |
        |                       |                       | roidTools`](ApkGenrul |
        |                       |                       | eDescriptionArg.html# |
        |                       |                       | isNeedAndroidTools()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ApkGenruleDe         | `setOut​(String out)`  | ::: block             |
        | scriptionArg.Builder` |                       | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`out                 |
        |                       |                       | `](ApkGenruleDescript |
        |                       |                       | ionArg.html#getOut()) |
        |                       |                       | to out.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ApkGenruleDe         | `setOut​(O             | ::: block             |
        | scriptionArg.Builder` | ptional<String> out)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`out                 |
        |                       |                       | `](ApkGenruleDescript |
        |                       |                       | ionArg.html#getOut()) |
        |                       |                       | to out.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ApkGenruleDe         | `setRe                | ::: block             |
        | scriptionArg.Builder` | mote​(boolean remote)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`remote`](           |
        |                       |                       | ApkGenruleDescription |
        |                       |                       | Arg.html#getRemote()) |
        |                       |                       | to remote.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ApkGenruleDe         | `setRemote​(Optio      | ::: block             |
        | scriptionArg.Builder` | nal<Boolean> remote)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`remote`](           |
        |                       |                       | ApkGenruleDescription |
        |                       |                       | Arg.html#getRemote()) |
        |                       |                       | to remote.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ApkGenruleDe         | `set                  | ::: block             |
        | scriptionArg.Builder` | Srcs​(SourceSet srcs)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`srcs`               |
        |                       |                       | ](ApkGenruleDescripti |
        |                       |                       | onArg.html#getSrcs()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ApkGenruleDe         | `setTests​(            | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Sets or replaces all  |
        |                       | ildTarget> elements)` | elements for          |
        |                       |                       | [`tests`]             |
        |                       |                       | (ApkGenruleDescriptio |
        |                       |                       | nArg.html#getTests()) |
        |                       |                       | sortedSet.            |
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

        []{#from(com.facebook.buck.android.ApkGenruleDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final ApkGenruleDescriptionArg.Builder from​(ApkGenruleDescriptionArg instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `ApkGenruleDescriptionArg` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.android.ApkGenruleDescription.AbstractApkGenruleDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final ApkGenruleDescriptionArg.Builder from​(com.facebook.buck.android.ApkGenruleDescription.AbstractApkGenruleDescriptionArg instance)
            ```

            ::: block
            Copy abstract value type `AbstractApkGenruleDescriptionArg`
            instance into builder.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.core.description.arg.HasTests)}

        -   #### from

            ``` methodSignature
            public final ApkGenruleDescriptionArg.Builder from​(HasTests instance)
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
            public final ApkGenruleDescriptionArg.Builder from​(AbstractGenruleDescription.CommonArg instance)
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
            public final ApkGenruleDescriptionArg.Builder from​(BuildRuleArg instance)
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
            public final ApkGenruleDescriptionArg.Builder from​(ConstructorArg instance)
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
            public final ApkGenruleDescriptionArg.Builder setOut​(String out)
            ```

            ::: block
            Initializes the optional value
            [`out`](ApkGenruleDescriptionArg.html#getOut()) to out.
            :::

            [Parameters:]{.paramLabel}
            :   `out` - The value for out

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setOut(java.util.Optional)}

        -   #### setOut

            ``` methodSignature
            public final ApkGenruleDescriptionArg.Builder setOut​(Optional<String> out)
            ```

            ::: block
            Initializes the optional value
            [`out`](ApkGenruleDescriptionArg.html#getOut()) to out.
            :::

            [Parameters:]{.paramLabel}
            :   `out` - The value for out

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setApk(com.facebook.buck.core.model.BuildTarget)}

        -   #### setApk

            ``` methodSignature
            public final ApkGenruleDescriptionArg.Builder setApk​(BuildTarget apk)
            ```

            ::: block
            Initializes the value for the
            [`apk`](ApkGenruleDescriptionArg.html#getApk()) attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `apk` - The value for apk

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setIsCacheable(boolean)}

        -   #### setIsCacheable

            ``` methodSignature
            public final ApkGenruleDescriptionArg.Builder setIsCacheable​(boolean isCacheable)
            ```

            ::: block
            Initializes the value for the
            [`isCacheable`](ApkGenruleDescriptionArg.html#getIsCacheable())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`isCacheable`](ApkGenruleDescriptionArg.html#getIsCacheable()).*
            :::

            [Parameters:]{.paramLabel}
            :   `isCacheable` - The value for isCacheable

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setBash(com.facebook.buck.rules.macros.StringWithMacros)}

        -   #### setBash

            ``` methodSignature
            public final ApkGenruleDescriptionArg.Builder setBash​(StringWithMacros bash)
            ```

            ::: block
            Initializes the optional value
            [`bash`](ApkGenruleDescriptionArg.html#getBash()) to bash.
            :::

            [Parameters:]{.paramLabel}
            :   `bash` - The value for bash

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setBash(java.util.Optional)}

        -   #### setBash

            ``` methodSignature
            public final ApkGenruleDescriptionArg.Builder setBash​(Optional<? extends StringWithMacros> bash)
            ```

            ::: block
            Initializes the optional value
            [`bash`](ApkGenruleDescriptionArg.html#getBash()) to bash.
            :::

            [Parameters:]{.paramLabel}
            :   `bash` - The value for bash

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCmd(com.facebook.buck.rules.macros.StringWithMacros)}

        -   #### setCmd

            ``` methodSignature
            public final ApkGenruleDescriptionArg.Builder setCmd​(StringWithMacros cmd)
            ```

            ::: block
            Initializes the optional value
            [`cmd`](ApkGenruleDescriptionArg.html#getCmd()) to cmd.
            :::

            [Parameters:]{.paramLabel}
            :   `cmd` - The value for cmd

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setCmd(java.util.Optional)}

        -   #### setCmd

            ``` methodSignature
            public final ApkGenruleDescriptionArg.Builder setCmd​(Optional<? extends StringWithMacros> cmd)
            ```

            ::: block
            Initializes the optional value
            [`cmd`](ApkGenruleDescriptionArg.html#getCmd()) to cmd.
            :::

            [Parameters:]{.paramLabel}
            :   `cmd` - The value for cmd

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCmdExe(com.facebook.buck.rules.macros.StringWithMacros)}

        -   #### setCmdExe

            ``` methodSignature
            public final ApkGenruleDescriptionArg.Builder setCmdExe​(StringWithMacros cmdExe)
            ```

            ::: block
            Initializes the optional value
            [`cmdExe`](ApkGenruleDescriptionArg.html#getCmdExe()) to
            cmdExe.
            :::

            [Parameters:]{.paramLabel}
            :   `cmdExe` - The value for cmdExe

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setCmdExe(java.util.Optional)}

        -   #### setCmdExe

            ``` methodSignature
            public final ApkGenruleDescriptionArg.Builder setCmdExe​(Optional<? extends StringWithMacros> cmdExe)
            ```

            ::: block
            Initializes the optional value
            [`cmdExe`](ApkGenruleDescriptionArg.html#getCmdExe()) to
            cmdExe.
            :::

            [Parameters:]{.paramLabel}
            :   `cmdExe` - The value for cmdExe

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setSrcs(com.facebook.buck.rules.coercer.SourceSet)}

        -   #### setSrcs

            ``` methodSignature
            public final ApkGenruleDescriptionArg.Builder setSrcs​(SourceSet srcs)
            ```

            ::: block
            Initializes the value for the
            [`srcs`](ApkGenruleDescriptionArg.html#getSrcs()) attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`srcs`](ApkGenruleDescriptionArg.html#getSrcs()).*
            :::

            [Parameters:]{.paramLabel}
            :   `srcs` - The value for srcs

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setEnableSandbox(boolean)}

        -   #### setEnableSandbox

            ``` methodSignature
            public final ApkGenruleDescriptionArg.Builder setEnableSandbox​(boolean enableSandbox)
            ```

            ::: block
            Initializes the optional value
            [`enableSandbox`](ApkGenruleDescriptionArg.html#getEnableSandbox())
            to enableSandbox.
            :::

            [Parameters:]{.paramLabel}
            :   `enableSandbox` - The value for enableSandbox

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setEnableSandbox(java.util.Optional)}

        -   #### setEnableSandbox

            ``` methodSignature
            public final ApkGenruleDescriptionArg.Builder setEnableSandbox​(Optional<Boolean> enableSandbox)
            ```

            ::: block
            Initializes the optional value
            [`enableSandbox`](ApkGenruleDescriptionArg.html#getEnableSandbox())
            to enableSandbox.
            :::

            [Parameters:]{.paramLabel}
            :   `enableSandbox` - The value for enableSandbox

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setEnvironmentExpansionSeparator(java.lang.String)}

        -   #### setEnvironmentExpansionSeparator

            ``` methodSignature
            public final ApkGenruleDescriptionArg.Builder setEnvironmentExpansionSeparator​(String environmentExpansionSeparator)
            ```

            ::: block
            Initializes the optional value
            [`environmentExpansionSeparator`](ApkGenruleDescriptionArg.html#getEnvironmentExpansionSeparator())
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
            public final ApkGenruleDescriptionArg.Builder setEnvironmentExpansionSeparator​(Optional<String> environmentExpansionSeparator)
            ```

            ::: block
            Initializes the optional value
            [`environmentExpansionSeparator`](ApkGenruleDescriptionArg.html#getEnvironmentExpansionSeparator())
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
            public final ApkGenruleDescriptionArg.Builder setRemote​(boolean remote)
            ```

            ::: block
            Initializes the optional value
            [`remote`](ApkGenruleDescriptionArg.html#getRemote()) to
            remote.
            :::

            [Parameters:]{.paramLabel}
            :   `remote` - The value for remote

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setRemote(java.util.Optional)}

        -   #### setRemote

            ``` methodSignature
            public final ApkGenruleDescriptionArg.Builder setRemote​(Optional<Boolean> remote)
            ```

            ::: block
            Initializes the optional value
            [`remote`](ApkGenruleDescriptionArg.html#getRemote()) to
            remote.
            :::

            [Parameters:]{.paramLabel}
            :   `remote` - The value for remote

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCacheable(boolean)}

        -   #### setCacheable

            ``` methodSignature
            public final ApkGenruleDescriptionArg.Builder setCacheable​(boolean cacheable)
            ```

            ::: block
            Initializes the optional value
            [`cacheable`](ApkGenruleDescriptionArg.html#getCacheable())
            to cacheable.
            :::

            [Parameters:]{.paramLabel}
            :   `cacheable` - The value for cacheable

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setCacheable(java.util.Optional)}

        -   #### setCacheable

            ``` methodSignature
            public final ApkGenruleDescriptionArg.Builder setCacheable​(Optional<Boolean> cacheable)
            ```

            ::: block
            Initializes the optional value
            [`cacheable`](ApkGenruleDescriptionArg.html#getCacheable())
            to cacheable.
            :::

            [Parameters:]{.paramLabel}
            :   `cacheable` - The value for cacheable

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setNeedAndroidTools(boolean)}

        -   #### setNeedAndroidTools

            ``` methodSignature
            public final ApkGenruleDescriptionArg.Builder setNeedAndroidTools​(boolean needAndroidTools)
            ```

            ::: block
            Initializes the value for the
            [`needAndroidTools`](ApkGenruleDescriptionArg.html#isNeedAndroidTools())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`needAndroidTools`](ApkGenruleDescriptionArg.html#isNeedAndroidTools()).*
            :::

            [Parameters:]{.paramLabel}
            :   `needAndroidTools` - The value for needAndroidTools

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLicenses(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### addLicenses

            ``` methodSignature
            public final ApkGenruleDescriptionArg.Builder addLicenses​(SourcePath element)
            ```

            ::: block
            Adds one element to
            [`licenses`](ApkGenruleDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A licenses element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLicenses(com.facebook.buck.core.sourcepath.SourcePath...)}

        -   #### addLicenses

            ``` methodSignature
            public final ApkGenruleDescriptionArg.Builder addLicenses​(SourcePath... elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](ApkGenruleDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLicenses(java.lang.Iterable)}

        -   #### setLicenses

            ``` methodSignature
            public final ApkGenruleDescriptionArg.Builder setLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`licenses`](ApkGenruleDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLicenses(java.lang.Iterable)}

        -   #### addAllLicenses

            ``` methodSignature
            public final ApkGenruleDescriptionArg.Builder addAllLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](ApkGenruleDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLabels(java.lang.String)}

        -   #### addLabels

            ``` methodSignature
            public final ApkGenruleDescriptionArg.Builder addLabels​(String element)
            ```

            ::: block
            Adds one element to
            [`labels`](ApkGenruleDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A labels element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLabels(java.lang.String...)}

        -   #### addLabels

            ``` methodSignature
            public final ApkGenruleDescriptionArg.Builder addLabels​(String... elements)
            ```

            ::: block
            Adds elements to
            [`labels`](ApkGenruleDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLabels(java.lang.Iterable)}

        -   #### setLabels

            ``` methodSignature
            public final ApkGenruleDescriptionArg.Builder setLabels​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`labels`](ApkGenruleDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLabels(java.lang.Iterable)}

        -   #### addAllLabels

            ``` methodSignature
            public final ApkGenruleDescriptionArg.Builder addAllLabels​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`labels`](ApkGenruleDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDefaultTargetPlatform(com.facebook.buck.core.model.UnconfiguredBuildTarget)}

        -   #### setDefaultTargetPlatform

            ``` methodSignature
            public final ApkGenruleDescriptionArg.Builder setDefaultTargetPlatform​(UnconfiguredBuildTarget defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](ApkGenruleDescriptionArg.html#getDefaultTargetPlatform())
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
            public final ApkGenruleDescriptionArg.Builder setDefaultTargetPlatform​(Optional<? extends UnconfiguredBuildTarget> defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](ApkGenruleDescriptionArg.html#getDefaultTargetPlatform())
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
            public final ApkGenruleDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget element)
            ```

            ::: block
            Adds one element to
            [`compatibleWith`](ApkGenruleDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A compatibleWith element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCompatibleWith(com.facebook.buck.core.model.UnconfiguredBuildTarget...)}

        -   #### addCompatibleWith

            ``` methodSignature
            public final ApkGenruleDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](ApkGenruleDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCompatibleWith(java.lang.Iterable)}

        -   #### setCompatibleWith

            ``` methodSignature
            public final ApkGenruleDescriptionArg.Builder setCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`compatibleWith`](ApkGenruleDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllCompatibleWith(java.lang.Iterable)}

        -   #### addAllCompatibleWith

            ``` methodSignature
            public final ApkGenruleDescriptionArg.Builder addAllCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](ApkGenruleDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setName(java.lang.String)}

        -   #### setName

            ``` methodSignature
            public final ApkGenruleDescriptionArg.Builder setName​(String name)
            ```

            ::: block
            Initializes the value for the
            [`name`](ApkGenruleDescriptionArg.html#getName()) attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `name` - The value for name

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addTests(com.facebook.buck.core.model.BuildTarget)}

        -   #### addTests

            ``` methodSignature
            public final ApkGenruleDescriptionArg.Builder addTests​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`tests`](ApkGenruleDescriptionArg.html#getTests())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A tests element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addTests(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addTests

            ``` methodSignature
            public final ApkGenruleDescriptionArg.Builder addTests​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`tests`](ApkGenruleDescriptionArg.html#getTests())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of tests elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setTests(java.lang.Iterable)}

        -   #### setTests

            ``` methodSignature
            public final ApkGenruleDescriptionArg.Builder setTests​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`tests`](ApkGenruleDescriptionArg.html#getTests())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of tests elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllTests(java.lang.Iterable)}

        -   #### addAllTests

            ``` methodSignature
            public final ApkGenruleDescriptionArg.Builder addAllTests​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`tests`](ApkGenruleDescriptionArg.html#getTests())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of tests elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#build()}

        -   #### build

            ``` methodSignature
            public ApkGenruleDescriptionArg build()
            ```

            ::: block
            Builds a new
            [`ApkGenruleDescriptionArg`](ApkGenruleDescriptionArg.html "class in com.facebook.buck.android").
            :::

            [Returns:]{.returnLabel}
            :   An immutable instance of ApkGenruleDescriptionArg

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
