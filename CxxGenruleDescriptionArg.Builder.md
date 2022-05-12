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
[Package]{.packageLabelInType} [com.facebook.buck.cxx](package-summary.html)
:::

## Class CxxGenruleDescriptionArg.Builder {#class-cxxgenruledescriptionarg.builder .title title="Class CxxGenruleDescriptionArg.Builder"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.cxx.CxxGenruleDescriptionArg.Builder

::: description
-   

    Enclosing class:
    :   [CxxGenruleDescriptionArg](CxxGenruleDescriptionArg.html "class in com.facebook.buck.cxx")

    ------------------------------------------------------------------------

        @NotThreadSafe
        public static final class CxxGenruleDescriptionArg.Builder
        extends Object

    ::: block
    Builds instances of type
    [`CxxGenruleDescriptionArg`](CxxGenruleDescriptionArg.html "class in com.facebook.buck.cxx").
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
        | `CxxGenruleDe         | `addAllCompat         | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Iterable<? e | Adds elements to      |
        |                       | xtends UnconfiguredBu | [`comp                |
        |                       | ildTarget> elements)` | atibleWith`](CxxGenru |
        |                       |                       | leDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxGenruleDe         | `addAllLabels​(Iterab  | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Adds elements to      |
        |                       |                       | [`labels`](           |
        |                       |                       | CxxGenruleDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxGenruleDe         | `addAllLicenses       | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Adds elements to      |
        |                       | ourcePath> elements)` | [`licenses`](Cx       |
        |                       |                       | xGenruleDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxGenruleDe         | `addAllTests​(         | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Adds elements to      |
        |                       | ildTarget> elements)` | [`tests`]             |
        |                       |                       | (CxxGenruleDescriptio |
        |                       |                       | nArg.html#getTests()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxGenruleDe         | `addCompat            | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Unconfigured | Adds one element to   |
        |                       | BuildTarget element)` | [`comp                |
        |                       |                       | atibleWith`](CxxGenru |
        |                       |                       | leDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxGenruleDe         | `addCompatible        | ::: block             |
        | scriptionArg.Builder` | With​(UnconfiguredBuil | Adds elements to      |
        |                       | dTarget... elements)` | [`comp                |
        |                       |                       | atibleWith`](CxxGenru |
        |                       |                       | leDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxGenruleDe         | `addLa                | ::: block             |
        | scriptionArg.Builder` | bels​(String element)` | Adds one element to   |
        |                       |                       | [`labels`](           |
        |                       |                       | CxxGenruleDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxGenruleDe         | `addLabels            | ::: block             |
        | scriptionArg.Builder` | ​(String... elements)` | Adds elements to      |
        |                       |                       | [`labels`](           |
        |                       |                       | CxxGenruleDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxGenruleDe         | `addLicenses          | ::: block             |
        | scriptionArg.Builder` | ​(SourcePath element)` | Adds one element to   |
        |                       |                       | [`licenses`](Cx       |
        |                       |                       | xGenruleDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxGenruleDe         | `addLicenses​(Sou      | ::: block             |
        | scriptionArg.Builder` | rcePath... elements)` | Adds elements to      |
        |                       |                       | [`licenses`](Cx       |
        |                       |                       | xGenruleDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxGenruleDe         | `addTests​(            | ::: block             |
        | scriptionArg.Builder` | BuildTarget element)` | Adds one element to   |
        |                       |                       | [`tests`]             |
        |                       |                       | (CxxGenruleDescriptio |
        |                       |                       | nArg.html#getTests()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxGenruleDe         | `addTests​(Buil        | ::: block             |
        | scriptionArg.Builder` | dTarget... elements)` | Adds elements to      |
        |                       |                       | [`tests`]             |
        |                       |                       | (CxxGenruleDescriptio |
        |                       |                       | nArg.html#getTests()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxG                 | `build()`             | ::: block             |
        | enruleDescriptionArg` |                       | Builds a new          |
        |                       |                       | [`CxxGenr             |
        |                       |                       | uleDescriptionArg`](C |
        |                       |                       | xxGenruleDescriptionA |
        |                       |                       | rg.html "class in com |
        |                       |                       | .facebook.buck.cxx"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxGenruleDe         | `from​(Bu              | ::: block             |
        | scriptionArg.Builder` | ildRuleArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebo           |
        |                       |                       | ok.buck.core.descript |
        |                       |                       | ion.arg.BuildRuleArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxGenruleDe         | `from​(Cons            | ::: block             |
        | scriptionArg.Builder` | tructorArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook         |
        |                       |                       | .buck.core.descriptio |
        |                       |                       | n.arg.ConstructorArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxGenruleDe         | `fro                  | ::: block             |
        | scriptionArg.Builder` | m​(HasTests instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.fa               |
        |                       |                       | cebook.buck.core.desc |
        |                       |                       | ription.arg.HasTests` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxGenruleDe         | `from​(com             | ::: block             |
        | scriptionArg.Builder` | .facebook.buck.cxx.Cx | Copy abstract value   |
        |                       | xGenruleDescription.A | type                  |
        |                       | bstractCxxGenruleDesc | `AbstractCxxG         |
        |                       | riptionArg instance)` | enruleDescriptionArg` |
        |                       |                       | instance into         |
        |                       |                       | builder.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxGenruleDe         | `from​(CxxGenruleDesc  | ::: block             |
        | scriptionArg.Builder` | riptionArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `CxxG                 |
        |                       |                       | enruleDescriptionArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxGenruleDe         | `from​(Abstr           | ::: block             |
        | scriptionArg.Builder` | actGenruleDescription | Fill a builder with   |
        |                       | .CommonArg instance)` | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook.buck.s  |
        |                       |                       | hell.AbstractGenruleD |
        |                       |                       | escription.CommonArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxGenruleDe         | `setBash​(St           | ::: block             |
        | scriptionArg.Builder` | ringWithMacros bash)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`bash`               |
        |                       |                       | ](CxxGenruleDescripti |
        |                       |                       | onArg.html#getBash()) |
        |                       |                       | to bash.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxGenruleDe         | `setBash​(O            | ::: block             |
        | scriptionArg.Builder` | ptional<? extends Str | Initializes the       |
        |                       | ingWithMacros> bash)` | optional value        |
        |                       |                       | [`bash`               |
        |                       |                       | ](CxxGenruleDescripti |
        |                       |                       | onArg.html#getBash()) |
        |                       |                       | to bash.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxGenruleDe         | `setCacheabl          | ::: block             |
        | scriptionArg.Builder` | e​(boolean cacheable)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`cacheable`](Cxx     |
        |                       |                       | GenruleDescriptionArg |
        |                       |                       | .html#getCacheable()) |
        |                       |                       | to cacheable.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxGenruleDe         | `                     | ::: block             |
        | scriptionArg.Builder` | setCacheable​(Optional | Initializes the       |
        |                       | <Boolean> cacheable)` | optional value        |
        |                       |                       | [`cacheable`](Cxx     |
        |                       |                       | GenruleDescriptionArg |
        |                       |                       | .html#getCacheable()) |
        |                       |                       | to cacheable.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxGenruleDe         | `setCmd​(S             | ::: block             |
        | scriptionArg.Builder` | tringWithMacros cmd)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`cmd                 |
        |                       |                       | `](CxxGenruleDescript |
        |                       |                       | ionArg.html#getCmd()) |
        |                       |                       | to cmd.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxGenruleDe         | `setCmd​(              | ::: block             |
        | scriptionArg.Builder` | Optional<? extends St | Initializes the       |
        |                       | ringWithMacros> cmd)` | optional value        |
        |                       |                       | [`cmd                 |
        |                       |                       | `](CxxGenruleDescript |
        |                       |                       | ionArg.html#getCmd()) |
        |                       |                       | to cmd.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxGenruleDe         | `setCmdExe​(Stri       | ::: block             |
        | scriptionArg.Builder` | ngWithMacros cmdExe)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`cmdExe`](           |
        |                       |                       | CxxGenruleDescription |
        |                       |                       | Arg.html#getCmdExe()) |
        |                       |                       | to cmdExe.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxGenruleDe         | `setCmdExe​(Opt        | ::: block             |
        | scriptionArg.Builder` | ional<? extends Strin | Initializes the       |
        |                       | gWithMacros> cmdExe)` | optional value        |
        |                       |                       | [`cmdExe`](           |
        |                       |                       | CxxGenruleDescription |
        |                       |                       | Arg.html#getCmdExe()) |
        |                       |                       | to cmdExe.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxGenruleDe         | `setCompat            | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Iterable<? e | Sets or replaces all  |
        |                       | xtends UnconfiguredBu | elements for          |
        |                       | ildTarget> elements)` | [`comp                |
        |                       |                       | atibleWith`](CxxGenru |
        |                       |                       | leDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxGenruleDe         | `setDefaul            | ::: block             |
        | scriptionArg.Builder` | tTargetPlatform​(Uncon | Initializes the       |
        |                       | figuredBuildTarget de | optional value        |
        |                       | faultTargetPlatform)` | [`defaultTargetPlatf  |
        |                       |                       | orm`](CxxGenruleDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxGenruleDe         | `setDefau             | ::: block             |
        | scriptionArg.Builder` | ltTargetPlatform​(Opti | Initializes the       |
        |                       | onal<? extends Unconf | optional value        |
        |                       | iguredBuildTarget> de | [`defaultTargetPlatf  |
        |                       | faultTargetPlatform)` | orm`](CxxGenruleDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxGenruleDe         | `setEnableSandbox​(bo  | ::: block             |
        | scriptionArg.Builder` | olean enableSandbox)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`en                  |
        |                       |                       | ableSandbox`](CxxGenr |
        |                       |                       | uleDescriptionArg.htm |
        |                       |                       | l#getEnableSandbox()) |
        |                       |                       | to enableSandbox.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxGenruleDe         | `setEnabl             | ::: block             |
        | scriptionArg.Builder` | eSandbox​(Optional<Boo | Initializes the       |
        |                       | lean> enableSandbox)` | optional value        |
        |                       |                       | [`en                  |
        |                       |                       | ableSandbox`](CxxGenr |
        |                       |                       | uleDescriptionArg.htm |
        |                       |                       | l#getEnableSandbox()) |
        |                       |                       | to enableSandbox.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxGenruleDe         | `setEnvir             | ::: block             |
        | scriptionArg.Builder` | onmentExpansionSepara | Initializes the       |
        |                       | tor​(String environmen | optional value        |
        |                       | tExpansionSeparator)` | [`environmentEx       |
        |                       |                       | pansionSeparator`](Cx |
        |                       |                       | xGenruleDescriptionAr |
        |                       |                       | g.html#getEnvironment |
        |                       |                       | ExpansionSeparator()) |
        |                       |                       | to                    |
        |                       |                       | environme             |
        |                       |                       | ntExpansionSeparator. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxGenruleDe         | `setEnvironmentExpa   | ::: block             |
        | scriptionArg.Builder` | nsionSeparator​(Option | Initializes the       |
        |                       | al<String> environmen | optional value        |
        |                       | tExpansionSeparator)` | [`environmentEx       |
        |                       |                       | pansionSeparator`](Cx |
        |                       |                       | xGenruleDescriptionAr |
        |                       |                       | g.html#getEnvironment |
        |                       |                       | ExpansionSeparator()) |
        |                       |                       | to                    |
        |                       |                       | environme             |
        |                       |                       | ntExpansionSeparator. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxGenruleDe         | `setLabels​(Iterab     | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Sets or replaces all  |
        |                       |                       | elements for          |
        |                       |                       | [`labels`](           |
        |                       |                       | CxxGenruleDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxGenruleDe         | `setLicenses          | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Sets or replaces all  |
        |                       | ourcePath> elements)` | elements for          |
        |                       |                       | [`licenses`](Cx       |
        |                       |                       | xGenruleDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxGenruleDe         | `                     | ::: block             |
        | scriptionArg.Builder` | setName​(String name)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`name`               |
        |                       |                       | ](CxxGenruleDescripti |
        |                       |                       | onArg.html#getName()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxGenruleDe         | `setN                 | ::: block             |
        | scriptionArg.Builder` | eedAndroidTools​(boole | Initializes the value |
        |                       | an needAndroidTools)` | for the               |
        |                       |                       | [`needAnd             |
        |                       |                       | roidTools`](CxxGenrul |
        |                       |                       | eDescriptionArg.html# |
        |                       |                       | isNeedAndroidTools()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxGenruleDe         | `setOut​(String out)`  | ::: block             |
        | scriptionArg.Builder` |                       | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`out                 |
        |                       |                       | `](CxxGenruleDescript |
        |                       |                       | ionArg.html#getOut()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxGenruleDe         | `setRe                | ::: block             |
        | scriptionArg.Builder` | mote​(boolean remote)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`remote`](           |
        |                       |                       | CxxGenruleDescription |
        |                       |                       | Arg.html#getRemote()) |
        |                       |                       | to remote.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxGenruleDe         | `setRemote​(Optio      | ::: block             |
        | scriptionArg.Builder` | nal<Boolean> remote)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`remote`](           |
        |                       |                       | CxxGenruleDescription |
        |                       |                       | Arg.html#getRemote()) |
        |                       |                       | to remote.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxGenruleDe         | `set                  | ::: block             |
        | scriptionArg.Builder` | Srcs​(SourceSet srcs)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`srcs`               |
        |                       |                       | ](CxxGenruleDescripti |
        |                       |                       | onArg.html#getSrcs()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxGenruleDe         | `setTests​(            | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Sets or replaces all  |
        |                       | ildTarget> elements)` | elements for          |
        |                       |                       | [`tests`]             |
        |                       |                       | (CxxGenruleDescriptio |
        |                       |                       | nArg.html#getTests()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxGenruleDe         | `                     | ::: block             |
        | scriptionArg.Builder` | setType​(String type)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`type`               |
        |                       |                       | ](CxxGenruleDescripti |
        |                       |                       | onArg.html#getType()) |
        |                       |                       | to type.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `CxxGenruleDe         | `setType​(Op           | ::: block             |
        | scriptionArg.Builder` | tional<String> type)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`type`               |
        |                       |                       | ](CxxGenruleDescripti |
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
            public final CxxGenruleDescriptionArg.Builder from​(HasTests instance)
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
            public final CxxGenruleDescriptionArg.Builder from​(AbstractGenruleDescription.CommonArg instance)
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
            public final CxxGenruleDescriptionArg.Builder from​(BuildRuleArg instance)
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

        []{#from(com.facebook.buck.cxx.CxxGenruleDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final CxxGenruleDescriptionArg.Builder from​(CxxGenruleDescriptionArg instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `CxxGenruleDescriptionArg` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.cxx.CxxGenruleDescription.AbstractCxxGenruleDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final CxxGenruleDescriptionArg.Builder from​(com.facebook.buck.cxx.CxxGenruleDescription.AbstractCxxGenruleDescriptionArg instance)
            ```

            ::: block
            Copy abstract value type `AbstractCxxGenruleDescriptionArg`
            instance into builder.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.core.description.arg.ConstructorArg)}

        -   #### from

            ``` methodSignature
            public final CxxGenruleDescriptionArg.Builder from​(ConstructorArg instance)
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
            public final CxxGenruleDescriptionArg.Builder setOut​(String out)
            ```

            ::: block
            Initializes the value for the
            [`out`](CxxGenruleDescriptionArg.html#getOut()) attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `out` - The value for out

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setBash(com.facebook.buck.rules.macros.StringWithMacros)}

        -   #### setBash

            ``` methodSignature
            public final CxxGenruleDescriptionArg.Builder setBash​(StringWithMacros bash)
            ```

            ::: block
            Initializes the optional value
            [`bash`](CxxGenruleDescriptionArg.html#getBash()) to bash.
            :::

            [Parameters:]{.paramLabel}
            :   `bash` - The value for bash

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setBash(java.util.Optional)}

        -   #### setBash

            ``` methodSignature
            public final CxxGenruleDescriptionArg.Builder setBash​(Optional<? extends StringWithMacros> bash)
            ```

            ::: block
            Initializes the optional value
            [`bash`](CxxGenruleDescriptionArg.html#getBash()) to bash.
            :::

            [Parameters:]{.paramLabel}
            :   `bash` - The value for bash

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCmd(com.facebook.buck.rules.macros.StringWithMacros)}

        -   #### setCmd

            ``` methodSignature
            public final CxxGenruleDescriptionArg.Builder setCmd​(StringWithMacros cmd)
            ```

            ::: block
            Initializes the optional value
            [`cmd`](CxxGenruleDescriptionArg.html#getCmd()) to cmd.
            :::

            [Parameters:]{.paramLabel}
            :   `cmd` - The value for cmd

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setCmd(java.util.Optional)}

        -   #### setCmd

            ``` methodSignature
            public final CxxGenruleDescriptionArg.Builder setCmd​(Optional<? extends StringWithMacros> cmd)
            ```

            ::: block
            Initializes the optional value
            [`cmd`](CxxGenruleDescriptionArg.html#getCmd()) to cmd.
            :::

            [Parameters:]{.paramLabel}
            :   `cmd` - The value for cmd

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCmdExe(com.facebook.buck.rules.macros.StringWithMacros)}

        -   #### setCmdExe

            ``` methodSignature
            public final CxxGenruleDescriptionArg.Builder setCmdExe​(StringWithMacros cmdExe)
            ```

            ::: block
            Initializes the optional value
            [`cmdExe`](CxxGenruleDescriptionArg.html#getCmdExe()) to
            cmdExe.
            :::

            [Parameters:]{.paramLabel}
            :   `cmdExe` - The value for cmdExe

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setCmdExe(java.util.Optional)}

        -   #### setCmdExe

            ``` methodSignature
            public final CxxGenruleDescriptionArg.Builder setCmdExe​(Optional<? extends StringWithMacros> cmdExe)
            ```

            ::: block
            Initializes the optional value
            [`cmdExe`](CxxGenruleDescriptionArg.html#getCmdExe()) to
            cmdExe.
            :::

            [Parameters:]{.paramLabel}
            :   `cmdExe` - The value for cmdExe

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setType(java.lang.String)}

        -   #### setType

            ``` methodSignature
            public final CxxGenruleDescriptionArg.Builder setType​(String type)
            ```

            ::: block
            Initializes the optional value
            [`type`](CxxGenruleDescriptionArg.html#getType()) to type.
            :::

            [Parameters:]{.paramLabel}
            :   `type` - The value for type

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setType(java.util.Optional)}

        -   #### setType

            ``` methodSignature
            public final CxxGenruleDescriptionArg.Builder setType​(Optional<String> type)
            ```

            ::: block
            Initializes the optional value
            [`type`](CxxGenruleDescriptionArg.html#getType()) to type.
            :::

            [Parameters:]{.paramLabel}
            :   `type` - The value for type

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setSrcs(com.facebook.buck.rules.coercer.SourceSet)}

        -   #### setSrcs

            ``` methodSignature
            public final CxxGenruleDescriptionArg.Builder setSrcs​(SourceSet srcs)
            ```

            ::: block
            Initializes the value for the
            [`srcs`](CxxGenruleDescriptionArg.html#getSrcs()) attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`srcs`](CxxGenruleDescriptionArg.html#getSrcs()).*
            :::

            [Parameters:]{.paramLabel}
            :   `srcs` - The value for srcs

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setEnableSandbox(boolean)}

        -   #### setEnableSandbox

            ``` methodSignature
            public final CxxGenruleDescriptionArg.Builder setEnableSandbox​(boolean enableSandbox)
            ```

            ::: block
            Initializes the optional value
            [`enableSandbox`](CxxGenruleDescriptionArg.html#getEnableSandbox())
            to enableSandbox.
            :::

            [Parameters:]{.paramLabel}
            :   `enableSandbox` - The value for enableSandbox

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setEnableSandbox(java.util.Optional)}

        -   #### setEnableSandbox

            ``` methodSignature
            public final CxxGenruleDescriptionArg.Builder setEnableSandbox​(Optional<Boolean> enableSandbox)
            ```

            ::: block
            Initializes the optional value
            [`enableSandbox`](CxxGenruleDescriptionArg.html#getEnableSandbox())
            to enableSandbox.
            :::

            [Parameters:]{.paramLabel}
            :   `enableSandbox` - The value for enableSandbox

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setEnvironmentExpansionSeparator(java.lang.String)}

        -   #### setEnvironmentExpansionSeparator

            ``` methodSignature
            public final CxxGenruleDescriptionArg.Builder setEnvironmentExpansionSeparator​(String environmentExpansionSeparator)
            ```

            ::: block
            Initializes the optional value
            [`environmentExpansionSeparator`](CxxGenruleDescriptionArg.html#getEnvironmentExpansionSeparator())
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
            public final CxxGenruleDescriptionArg.Builder setEnvironmentExpansionSeparator​(Optional<String> environmentExpansionSeparator)
            ```

            ::: block
            Initializes the optional value
            [`environmentExpansionSeparator`](CxxGenruleDescriptionArg.html#getEnvironmentExpansionSeparator())
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
            public final CxxGenruleDescriptionArg.Builder setRemote​(boolean remote)
            ```

            ::: block
            Initializes the optional value
            [`remote`](CxxGenruleDescriptionArg.html#getRemote()) to
            remote.
            :::

            [Parameters:]{.paramLabel}
            :   `remote` - The value for remote

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setRemote(java.util.Optional)}

        -   #### setRemote

            ``` methodSignature
            public final CxxGenruleDescriptionArg.Builder setRemote​(Optional<Boolean> remote)
            ```

            ::: block
            Initializes the optional value
            [`remote`](CxxGenruleDescriptionArg.html#getRemote()) to
            remote.
            :::

            [Parameters:]{.paramLabel}
            :   `remote` - The value for remote

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCacheable(boolean)}

        -   #### setCacheable

            ``` methodSignature
            public final CxxGenruleDescriptionArg.Builder setCacheable​(boolean cacheable)
            ```

            ::: block
            Initializes the optional value
            [`cacheable`](CxxGenruleDescriptionArg.html#getCacheable())
            to cacheable.
            :::

            [Parameters:]{.paramLabel}
            :   `cacheable` - The value for cacheable

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setCacheable(java.util.Optional)}

        -   #### setCacheable

            ``` methodSignature
            public final CxxGenruleDescriptionArg.Builder setCacheable​(Optional<Boolean> cacheable)
            ```

            ::: block
            Initializes the optional value
            [`cacheable`](CxxGenruleDescriptionArg.html#getCacheable())
            to cacheable.
            :::

            [Parameters:]{.paramLabel}
            :   `cacheable` - The value for cacheable

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setNeedAndroidTools(boolean)}

        -   #### setNeedAndroidTools

            ``` methodSignature
            public final CxxGenruleDescriptionArg.Builder setNeedAndroidTools​(boolean needAndroidTools)
            ```

            ::: block
            Initializes the value for the
            [`needAndroidTools`](CxxGenruleDescriptionArg.html#isNeedAndroidTools())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`needAndroidTools`](CxxGenruleDescriptionArg.html#isNeedAndroidTools()).*
            :::

            [Parameters:]{.paramLabel}
            :   `needAndroidTools` - The value for needAndroidTools

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLicenses(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### addLicenses

            ``` methodSignature
            public final CxxGenruleDescriptionArg.Builder addLicenses​(SourcePath element)
            ```

            ::: block
            Adds one element to
            [`licenses`](CxxGenruleDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A licenses element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLicenses(com.facebook.buck.core.sourcepath.SourcePath...)}

        -   #### addLicenses

            ``` methodSignature
            public final CxxGenruleDescriptionArg.Builder addLicenses​(SourcePath... elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](CxxGenruleDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLicenses(java.lang.Iterable)}

        -   #### setLicenses

            ``` methodSignature
            public final CxxGenruleDescriptionArg.Builder setLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`licenses`](CxxGenruleDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLicenses(java.lang.Iterable)}

        -   #### addAllLicenses

            ``` methodSignature
            public final CxxGenruleDescriptionArg.Builder addAllLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](CxxGenruleDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLabels(java.lang.String)}

        -   #### addLabels

            ``` methodSignature
            public final CxxGenruleDescriptionArg.Builder addLabels​(String element)
            ```

            ::: block
            Adds one element to
            [`labels`](CxxGenruleDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A labels element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLabels(java.lang.String...)}

        -   #### addLabels

            ``` methodSignature
            public final CxxGenruleDescriptionArg.Builder addLabels​(String... elements)
            ```

            ::: block
            Adds elements to
            [`labels`](CxxGenruleDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLabels(java.lang.Iterable)}

        -   #### setLabels

            ``` methodSignature
            public final CxxGenruleDescriptionArg.Builder setLabels​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`labels`](CxxGenruleDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLabels(java.lang.Iterable)}

        -   #### addAllLabels

            ``` methodSignature
            public final CxxGenruleDescriptionArg.Builder addAllLabels​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`labels`](CxxGenruleDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDefaultTargetPlatform(com.facebook.buck.core.model.UnconfiguredBuildTarget)}

        -   #### setDefaultTargetPlatform

            ``` methodSignature
            public final CxxGenruleDescriptionArg.Builder setDefaultTargetPlatform​(UnconfiguredBuildTarget defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](CxxGenruleDescriptionArg.html#getDefaultTargetPlatform())
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
            public final CxxGenruleDescriptionArg.Builder setDefaultTargetPlatform​(Optional<? extends UnconfiguredBuildTarget> defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](CxxGenruleDescriptionArg.html#getDefaultTargetPlatform())
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
            public final CxxGenruleDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget element)
            ```

            ::: block
            Adds one element to
            [`compatibleWith`](CxxGenruleDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A compatibleWith element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCompatibleWith(com.facebook.buck.core.model.UnconfiguredBuildTarget...)}

        -   #### addCompatibleWith

            ``` methodSignature
            public final CxxGenruleDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](CxxGenruleDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCompatibleWith(java.lang.Iterable)}

        -   #### setCompatibleWith

            ``` methodSignature
            public final CxxGenruleDescriptionArg.Builder setCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`compatibleWith`](CxxGenruleDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllCompatibleWith(java.lang.Iterable)}

        -   #### addAllCompatibleWith

            ``` methodSignature
            public final CxxGenruleDescriptionArg.Builder addAllCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](CxxGenruleDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setName(java.lang.String)}

        -   #### setName

            ``` methodSignature
            public final CxxGenruleDescriptionArg.Builder setName​(String name)
            ```

            ::: block
            Initializes the value for the
            [`name`](CxxGenruleDescriptionArg.html#getName()) attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `name` - The value for name

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addTests(com.facebook.buck.core.model.BuildTarget)}

        -   #### addTests

            ``` methodSignature
            public final CxxGenruleDescriptionArg.Builder addTests​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`tests`](CxxGenruleDescriptionArg.html#getTests())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A tests element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addTests(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addTests

            ``` methodSignature
            public final CxxGenruleDescriptionArg.Builder addTests​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`tests`](CxxGenruleDescriptionArg.html#getTests())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of tests elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setTests(java.lang.Iterable)}

        -   #### setTests

            ``` methodSignature
            public final CxxGenruleDescriptionArg.Builder setTests​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`tests`](CxxGenruleDescriptionArg.html#getTests())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of tests elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllTests(java.lang.Iterable)}

        -   #### addAllTests

            ``` methodSignature
            public final CxxGenruleDescriptionArg.Builder addAllTests​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`tests`](CxxGenruleDescriptionArg.html#getTests())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of tests elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#build()}

        -   #### build

            ``` methodSignature
            public CxxGenruleDescriptionArg build()
            ```

            ::: block
            Builds a new
            [`CxxGenruleDescriptionArg`](CxxGenruleDescriptionArg.html "class in com.facebook.buck.cxx").
            :::

            [Returns:]{.returnLabel}
            :   An immutable instance of CxxGenruleDescriptionArg

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
