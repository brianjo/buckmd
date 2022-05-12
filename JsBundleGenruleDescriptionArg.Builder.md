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
[Package]{.packageLabelInType} [com.facebook.buck.features.js](package-summary.html)
:::

## Class JsBundleGenruleDescriptionArg.Builder {#class-jsbundlegenruledescriptionarg.builder .title title="Class JsBundleGenruleDescriptionArg.Builder"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.features.js.JsBundleGenruleDescriptionArg.Builder

::: description
-   

    Enclosing class:
    :   [JsBundleGenruleDescriptionArg](JsBundleGenruleDescriptionArg.html "class in com.facebook.buck.features.js")

    ------------------------------------------------------------------------

        @NotThreadSafe
        public static final class JsBundleGenruleDescriptionArg.Builder
        extends Object

    ::: block
    Builds instances of type
    [`JsBundleGenruleDescriptionArg`](JsBundleGenruleDescriptionArg.html "class in com.facebook.buck.features.js").
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
        | `JsBundleGenruleDe    | `addAllBundleN        | ::: block             |
        | scriptionArg.Builder` | ameForFlavor​(Iterable | Adds elements to      |
        |                       | <? extends Pair<Flavo | [`bundleNameForFlavor |
        |                       | r,​String>> elements)` | `](JsBundleGenruleDes |
        |                       |                       | criptionArg.html#getB |
        |                       |                       | undleNameForFlavor()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsBundleGenruleDe    | `addAllCompat         | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Iterable<? e | Adds elements to      |
        |                       | xtends UnconfiguredBu | [`compatibl           |
        |                       | ildTarget> elements)` | eWith`](JsBundleGenru |
        |                       |                       | leDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsBundleGenruleDe    | `addAllLabels​(Iterab  | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Adds elements to      |
        |                       |                       | [`labels`](JsBun      |
        |                       |                       | dleGenruleDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsBundleGenruleDe    | `addAllLicenses       | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Adds elements to      |
        |                       | ourcePath> elements)` | [`licenses`](JsBundl  |
        |                       |                       | eGenruleDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsBundleGenruleDe    | `addAllTests​(         | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Adds elements to      |
        |                       | ildTarget> elements)` | [`tests`](JsBu        |
        |                       |                       | ndleGenruleDescriptio |
        |                       |                       | nArg.html#getTests()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsBundleGenruleDe    | `addBundleN           | ::: block             |
        | scriptionArg.Builder` | ameForFlavor​(Pair<Fla | Adds one element to   |
        |                       | vor,​String> element)` | [`bundleNameForFlavor |
        |                       |                       | `](JsBundleGenruleDes |
        |                       |                       | criptionArg.html#getB |
        |                       |                       | undleNameForFlavor()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsBundleGenruleDe    | `addBundleNameF       | ::: block             |
        | scriptionArg.Builder` | orFlavor​(Pair<Flavor, | Adds elements to      |
        |                       | ​String>... elements)` | [`bundleNameForFlavor |
        |                       |                       | `](JsBundleGenruleDes |
        |                       |                       | criptionArg.html#getB |
        |                       |                       | undleNameForFlavor()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsBundleGenruleDe    | `addCompat            | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Unconfigured | Adds one element to   |
        |                       | BuildTarget element)` | [`compatibl           |
        |                       |                       | eWith`](JsBundleGenru |
        |                       |                       | leDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsBundleGenruleDe    | `addCompatible        | ::: block             |
        | scriptionArg.Builder` | With​(UnconfiguredBuil | Adds elements to      |
        |                       | dTarget... elements)` | [`compatibl           |
        |                       |                       | eWith`](JsBundleGenru |
        |                       |                       | leDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsBundleGenruleDe    | `addLa                | ::: block             |
        | scriptionArg.Builder` | bels​(String element)` | Adds one element to   |
        |                       |                       | [`labels`](JsBun      |
        |                       |                       | dleGenruleDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsBundleGenruleDe    | `addLabels            | ::: block             |
        | scriptionArg.Builder` | ​(String... elements)` | Adds elements to      |
        |                       |                       | [`labels`](JsBun      |
        |                       |                       | dleGenruleDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsBundleGenruleDe    | `addLicenses          | ::: block             |
        | scriptionArg.Builder` | ​(SourcePath element)` | Adds one element to   |
        |                       |                       | [`licenses`](JsBundl  |
        |                       |                       | eGenruleDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsBundleGenruleDe    | `addLicenses​(Sou      | ::: block             |
        | scriptionArg.Builder` | rcePath... elements)` | Adds elements to      |
        |                       |                       | [`licenses`](JsBundl  |
        |                       |                       | eGenruleDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsBundleGenruleDe    | `addTests​(            | ::: block             |
        | scriptionArg.Builder` | BuildTarget element)` | Adds one element to   |
        |                       |                       | [`tests`](JsBu        |
        |                       |                       | ndleGenruleDescriptio |
        |                       |                       | nArg.html#getTests()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsBundleGenruleDe    | `addTests​(Buil        | ::: block             |
        | scriptionArg.Builder` | dTarget... elements)` | Adds elements to      |
        |                       |                       | [`tests`](JsBu        |
        |                       |                       | ndleGenruleDescriptio |
        |                       |                       | nArg.html#getTests()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsBundleG            | `build()`             | ::: block             |
        | enruleDescriptionArg` |                       | Builds a new          |
        |                       |                       | [`JsBu                |
        |                       |                       | ndleGenruleDescriptio |
        |                       |                       | nArg`](JsBundleGenrul |
        |                       |                       | eDescriptionArg.html  |
        |                       |                       | "class in com.faceboo |
        |                       |                       | k.buck.features.js"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsBundleGenruleDe    | `from​(Bu              | ::: block             |
        | scriptionArg.Builder` | ildRuleArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebo           |
        |                       |                       | ok.buck.core.descript |
        |                       |                       | ion.arg.BuildRuleArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsBundleGenruleDe    | `from​(Cons            | ::: block             |
        | scriptionArg.Builder` | tructorArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook         |
        |                       |                       | .buck.core.descriptio |
        |                       |                       | n.arg.ConstructorArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsBundleGenruleDe    | `fro                  | ::: block             |
        | scriptionArg.Builder` | m​(HasTests instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.fa               |
        |                       |                       | cebook.buck.core.desc |
        |                       |                       | ription.arg.HasTests` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsBundleGenruleDe    | `from​(Has             | ::: block             |
        | scriptionArg.Builder` | BundleName instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `co                   |
        |                       |                       | m.facebook.buck.featu |
        |                       |                       | res.js.HasBundleName` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsBundleGenruleDe    | `from​(                | ::: block             |
        | scriptionArg.Builder` | com.facebook.buck.fea | Copy abstract value   |
        |                       | tures.js.JsBundleGenr | type                  |
        |                       | uleDescription.Abstra | `AbstractJsBundleG    |
        |                       | ctJsBundleGenruleDesc | enruleDescriptionArg` |
        |                       | riptionArg instance)` | instance into         |
        |                       |                       | builder.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsBundleGenruleDe    | `fro                  | ::: block             |
        | scriptionArg.Builder` | m​(JsBundleGenruleDesc | Fill a builder with   |
        |                       | riptionArg instance)` | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `JsBundleG            |
        |                       |                       | enruleDescriptionArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsBundleGenruleDe    | `from​(Abstr           | ::: block             |
        | scriptionArg.Builder` | actGenruleDescription | Fill a builder with   |
        |                       | .CommonArg instance)` | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook.buck.s  |
        |                       |                       | hell.AbstractGenruleD |
        |                       |                       | escription.CommonArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsBundleGenruleDe    | `setBash​(St           | ::: block             |
        | scriptionArg.Builder` | ringWithMacros bash)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`bash`](JsB          |
        |                       |                       | undleGenruleDescripti |
        |                       |                       | onArg.html#getBash()) |
        |                       |                       | to bash.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsBundleGenruleDe    | `setBash​(O            | ::: block             |
        | scriptionArg.Builder` | ptional<? extends Str | Initializes the       |
        |                       | ingWithMacros> bash)` | optional value        |
        |                       |                       | [`bash`](JsB          |
        |                       |                       | undleGenruleDescripti |
        |                       |                       | onArg.html#getBash()) |
        |                       |                       | to bash.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsBundleGenruleDe    | `setBundleNam         | ::: block             |
        | scriptionArg.Builder` | e​(String bundleName)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`b                   |
        |                       |                       | undleName`](JsBundleG |
        |                       |                       | enruleDescriptionArg. |
        |                       |                       | html#getBundleName()) |
        |                       |                       | to bundleName.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsBundleGenruleDe    | `s                    | ::: block             |
        | scriptionArg.Builder` | etBundleName​(Optional | Initializes the       |
        |                       | <String> bundleName)` | optional value        |
        |                       |                       | [`b                   |
        |                       |                       | undleName`](JsBundleG |
        |                       |                       | enruleDescriptionArg. |
        |                       |                       | html#getBundleName()) |
        |                       |                       | to bundleName.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsBundleGenruleDe    | `setBundleN           | ::: block             |
        | scriptionArg.Builder` | ameForFlavor​(Iterable | Sets or replaces all  |
        |                       | <? extends Pair<Flavo | elements for          |
        |                       | r,​String>> elements)` | [`bundleNameForFlavor |
        |                       |                       | `](JsBundleGenruleDes |
        |                       |                       | criptionArg.html#getB |
        |                       |                       | undleNameForFlavor()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsBundleGenruleDe    | `setCacheabl          | ::: block             |
        | scriptionArg.Builder` | e​(boolean cacheable)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [                     |
        |                       |                       | `cacheable`](JsBundle |
        |                       |                       | GenruleDescriptionArg |
        |                       |                       | .html#getCacheable()) |
        |                       |                       | to cacheable.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsBundleGenruleDe    | `                     | ::: block             |
        | scriptionArg.Builder` | setCacheable​(Optional | Initializes the       |
        |                       | <Boolean> cacheable)` | optional value        |
        |                       |                       | [                     |
        |                       |                       | `cacheable`](JsBundle |
        |                       |                       | GenruleDescriptionArg |
        |                       |                       | .html#getCacheable()) |
        |                       |                       | to cacheable.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsBundleGenruleDe    | `setCmd​(S             | ::: block             |
        | scriptionArg.Builder` | tringWithMacros cmd)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`cmd`](Js            |
        |                       |                       | BundleGenruleDescript |
        |                       |                       | ionArg.html#getCmd()) |
        |                       |                       | to cmd.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsBundleGenruleDe    | `setCmd​(              | ::: block             |
        | scriptionArg.Builder` | Optional<? extends St | Initializes the       |
        |                       | ringWithMacros> cmd)` | optional value        |
        |                       |                       | [`cmd`](Js            |
        |                       |                       | BundleGenruleDescript |
        |                       |                       | ionArg.html#getCmd()) |
        |                       |                       | to cmd.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsBundleGenruleDe    | `setCmdExe​(Stri       | ::: block             |
        | scriptionArg.Builder` | ngWithMacros cmdExe)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`cmdExe`](JsBun      |
        |                       |                       | dleGenruleDescription |
        |                       |                       | Arg.html#getCmdExe()) |
        |                       |                       | to cmdExe.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsBundleGenruleDe    | `setCmdExe​(Opt        | ::: block             |
        | scriptionArg.Builder` | ional<? extends Strin | Initializes the       |
        |                       | gWithMacros> cmdExe)` | optional value        |
        |                       |                       | [`cmdExe`](JsBun      |
        |                       |                       | dleGenruleDescription |
        |                       |                       | Arg.html#getCmdExe()) |
        |                       |                       | to cmdExe.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsBundleGenruleDe    | `setCompat            | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Iterable<? e | Sets or replaces all  |
        |                       | xtends UnconfiguredBu | elements for          |
        |                       | ildTarget> elements)` | [`compatibl           |
        |                       |                       | eWith`](JsBundleGenru |
        |                       |                       | leDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsBundleGenruleDe    | `setDefaul            | ::: block             |
        | scriptionArg.Builder` | tTargetPlatform​(Uncon | Initializes the       |
        |                       | figuredBuildTarget de | optional value        |
        |                       | faultTargetPlatform)` | [`de                  |
        |                       |                       | faultTargetPlatform`] |
        |                       |                       | (JsBundleGenruleDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsBundleGenruleDe    | `setDefau             | ::: block             |
        | scriptionArg.Builder` | ltTargetPlatform​(Opti | Initializes the       |
        |                       | onal<? extends Unconf | optional value        |
        |                       | iguredBuildTarget> de | [`de                  |
        |                       | faultTargetPlatform)` | faultTargetPlatform`] |
        |                       |                       | (JsBundleGenruleDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsBundleGenruleDe    | `setEnableSandbox​(bo  | ::: block             |
        | scriptionArg.Builder` | olean enableSandbox)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`enableS             |
        |                       |                       | andbox`](JsBundleGenr |
        |                       |                       | uleDescriptionArg.htm |
        |                       |                       | l#getEnableSandbox()) |
        |                       |                       | to enableSandbox.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsBundleGenruleDe    | `setEnabl             | ::: block             |
        | scriptionArg.Builder` | eSandbox​(Optional<Boo | Initializes the       |
        |                       | lean> enableSandbox)` | optional value        |
        |                       |                       | [`enableS             |
        |                       |                       | andbox`](JsBundleGenr |
        |                       |                       | uleDescriptionArg.htm |
        |                       |                       | l#getEnableSandbox()) |
        |                       |                       | to enableSandbox.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsBundleGenruleDe    | `setEnvir             | ::: block             |
        | scriptionArg.Builder` | onmentExpansionSepara | Initializes the       |
        |                       | tor​(String environmen | optional value        |
        |                       | tExpansionSeparator)` | [`environmentExpansi  |
        |                       |                       | onSeparator`](JsBundl |
        |                       |                       | eGenruleDescriptionAr |
        |                       |                       | g.html#getEnvironment |
        |                       |                       | ExpansionSeparator()) |
        |                       |                       | to                    |
        |                       |                       | environme             |
        |                       |                       | ntExpansionSeparator. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsBundleGenruleDe    | `setEnvironmentExpa   | ::: block             |
        | scriptionArg.Builder` | nsionSeparator​(Option | Initializes the       |
        |                       | al<String> environmen | optional value        |
        |                       | tExpansionSeparator)` | [`environmentExpansi  |
        |                       |                       | onSeparator`](JsBundl |
        |                       |                       | eGenruleDescriptionAr |
        |                       |                       | g.html#getEnvironment |
        |                       |                       | ExpansionSeparator()) |
        |                       |                       | to                    |
        |                       |                       | environme             |
        |                       |                       | ntExpansionSeparator. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsBundleGenruleDe    | `setJsBundle​(B        | ::: block             |
        | scriptionArg.Builder` | uildTarget jsBundle)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`jsBundle`](JsBundl  |
        |                       |                       | eGenruleDescriptionAr |
        |                       |                       | g.html#getJsBundle()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsBundleGenruleDe    | `setLabels​(Iterab     | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Sets or replaces all  |
        |                       |                       | elements for          |
        |                       |                       | [`labels`](JsBun      |
        |                       |                       | dleGenruleDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsBundleGenruleDe    | `setLicenses          | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Sets or replaces all  |
        |                       | ourcePath> elements)` | elements for          |
        |                       |                       | [`licenses`](JsBundl  |
        |                       |                       | eGenruleDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsBundleGenruleDe    | `                     | ::: block             |
        | scriptionArg.Builder` | setName​(String name)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`name`](JsB          |
        |                       |                       | undleGenruleDescripti |
        |                       |                       | onArg.html#getName()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsBundleGenruleDe    | `setN                 | ::: block             |
        | scriptionArg.Builder` | eedAndroidTools​(boole | Initializes the value |
        |                       | an needAndroidTools)` | for the               |
        |                       |                       | [`needAndroidT        |
        |                       |                       | ools`](JsBundleGenrul |
        |                       |                       | eDescriptionArg.html# |
        |                       |                       | isNeedAndroidTools()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsBundleGenruleDe    | `setRe                | ::: block             |
        | scriptionArg.Builder` | mote​(boolean remote)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`remote`](JsBun      |
        |                       |                       | dleGenruleDescription |
        |                       |                       | Arg.html#getRemote()) |
        |                       |                       | to remote.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsBundleGenruleDe    | `setRemote​(Optio      | ::: block             |
        | scriptionArg.Builder` | nal<Boolean> remote)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`remote`](JsBun      |
        |                       |                       | dleGenruleDescription |
        |                       |                       | Arg.html#getRemote()) |
        |                       |                       | to remote.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsBundleGenruleDe    | `se                   | ::: block             |
        | scriptionArg.Builder` | tRewriteDepsFile​(bool | Initializes the value |
        |                       | ean rewriteDepsFile)` | for the               |
        |                       |                       | [`rewriteDeps         |
        |                       |                       | File`](JsBundleGenrul |
        |                       |                       | eDescriptionArg.html# |
        |                       |                       | getRewriteDepsFile()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsBundleGenruleDe    | `setRewriteMisc​(      | ::: block             |
        | scriptionArg.Builder` | boolean rewriteMisc)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`rew                 |
        |                       |                       | riteMisc`](JsBundleGe |
        |                       |                       | nruleDescriptionArg.h |
        |                       |                       | tml#getRewriteMisc()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsBundleGenruleDe    | `setR                 | ::: block             |
        | scriptionArg.Builder` | ewriteSourcemap​(boole | Initializes the value |
        |                       | an rewriteSourcemap)` | for the               |
        |                       |                       | [`rewriteSource       |
        |                       |                       | map`](JsBundleGenrule |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etRewriteSourcemap()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsBundleGenruleDe    | `setSkipResources​(bo  | ::: block             |
        | scriptionArg.Builder` | olean skipResources)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`skipRes             |
        |                       |                       | ources`](JsBundleGenr |
        |                       |                       | uleDescriptionArg.htm |
        |                       |                       | l#getSkipResources()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsBundleGenruleDe    | `set                  | ::: block             |
        | scriptionArg.Builder` | Srcs​(SourceSet srcs)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`srcs`](JsB          |
        |                       |                       | undleGenruleDescripti |
        |                       |                       | onArg.html#getSrcs()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsBundleGenruleDe    | `setTests​(            | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Sets or replaces all  |
        |                       | ildTarget> elements)` | elements for          |
        |                       |                       | [`tests`](JsBu        |
        |                       |                       | ndleGenruleDescriptio |
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

        []{#from(com.facebook.buck.features.js.JsBundleGenruleDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final JsBundleGenruleDescriptionArg.Builder from​(JsBundleGenruleDescriptionArg instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `JsBundleGenruleDescriptionArg` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.features.js.JsBundleGenruleDescription.AbstractJsBundleGenruleDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final JsBundleGenruleDescriptionArg.Builder from​(com.facebook.buck.features.js.JsBundleGenruleDescription.AbstractJsBundleGenruleDescriptionArg instance)
            ```

            ::: block
            Copy abstract value type
            `AbstractJsBundleGenruleDescriptionArg` instance into
            builder.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.core.description.arg.HasTests)}

        -   #### from

            ``` methodSignature
            public final JsBundleGenruleDescriptionArg.Builder from​(HasTests instance)
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
            public final JsBundleGenruleDescriptionArg.Builder from​(AbstractGenruleDescription.CommonArg instance)
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

        []{#from(com.facebook.buck.features.js.HasBundleName)}

        -   #### from

            ``` methodSignature
            public final JsBundleGenruleDescriptionArg.Builder from​(HasBundleName instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `com.facebook.buck.features.js.HasBundleName` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.core.description.arg.BuildRuleArg)}

        -   #### from

            ``` methodSignature
            public final JsBundleGenruleDescriptionArg.Builder from​(BuildRuleArg instance)
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
            public final JsBundleGenruleDescriptionArg.Builder from​(ConstructorArg instance)
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

        []{#setJsBundle(com.facebook.buck.core.model.BuildTarget)}

        -   #### setJsBundle

            ``` methodSignature
            public final JsBundleGenruleDescriptionArg.Builder setJsBundle​(BuildTarget jsBundle)
            ```

            ::: block
            Initializes the value for the
            [`jsBundle`](JsBundleGenruleDescriptionArg.html#getJsBundle())
            attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `jsBundle` - The value for jsBundle

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setRewriteSourcemap(boolean)}

        -   #### setRewriteSourcemap

            ``` methodSignature
            public final JsBundleGenruleDescriptionArg.Builder setRewriteSourcemap​(boolean rewriteSourcemap)
            ```

            ::: block
            Initializes the value for the
            [`rewriteSourcemap`](JsBundleGenruleDescriptionArg.html#getRewriteSourcemap())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`rewriteSourcemap`](JsBundleGenruleDescriptionArg.html#getRewriteSourcemap()).*
            :::

            [Parameters:]{.paramLabel}
            :   `rewriteSourcemap` - The value for rewriteSourcemap

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setRewriteMisc(boolean)}

        -   #### setRewriteMisc

            ``` methodSignature
            public final JsBundleGenruleDescriptionArg.Builder setRewriteMisc​(boolean rewriteMisc)
            ```

            ::: block
            Initializes the value for the
            [`rewriteMisc`](JsBundleGenruleDescriptionArg.html#getRewriteMisc())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`rewriteMisc`](JsBundleGenruleDescriptionArg.html#getRewriteMisc()).*
            :::

            [Parameters:]{.paramLabel}
            :   `rewriteMisc` - The value for rewriteMisc

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setSkipResources(boolean)}

        -   #### setSkipResources

            ``` methodSignature
            public final JsBundleGenruleDescriptionArg.Builder setSkipResources​(boolean skipResources)
            ```

            ::: block
            Initializes the value for the
            [`skipResources`](JsBundleGenruleDescriptionArg.html#getSkipResources())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`skipResources`](JsBundleGenruleDescriptionArg.html#getSkipResources()).*
            :::

            [Parameters:]{.paramLabel}
            :   `skipResources` - The value for skipResources

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setRewriteDepsFile(boolean)}

        -   #### setRewriteDepsFile

            ``` methodSignature
            public final JsBundleGenruleDescriptionArg.Builder setRewriteDepsFile​(boolean rewriteDepsFile)
            ```

            ::: block
            Initializes the value for the
            [`rewriteDepsFile`](JsBundleGenruleDescriptionArg.html#getRewriteDepsFile())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`rewriteDepsFile`](JsBundleGenruleDescriptionArg.html#getRewriteDepsFile()).*
            :::

            [Parameters:]{.paramLabel}
            :   `rewriteDepsFile` - The value for rewriteDepsFile

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setBash(com.facebook.buck.rules.macros.StringWithMacros)}

        -   #### setBash

            ``` methodSignature
            public final JsBundleGenruleDescriptionArg.Builder setBash​(StringWithMacros bash)
            ```

            ::: block
            Initializes the optional value
            [`bash`](JsBundleGenruleDescriptionArg.html#getBash()) to
            bash.
            :::

            [Parameters:]{.paramLabel}
            :   `bash` - The value for bash

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setBash(java.util.Optional)}

        -   #### setBash

            ``` methodSignature
            public final JsBundleGenruleDescriptionArg.Builder setBash​(Optional<? extends StringWithMacros> bash)
            ```

            ::: block
            Initializes the optional value
            [`bash`](JsBundleGenruleDescriptionArg.html#getBash()) to
            bash.
            :::

            [Parameters:]{.paramLabel}
            :   `bash` - The value for bash

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCacheable(boolean)}

        -   #### setCacheable

            ``` methodSignature
            public final JsBundleGenruleDescriptionArg.Builder setCacheable​(boolean cacheable)
            ```

            ::: block
            Initializes the optional value
            [`cacheable`](JsBundleGenruleDescriptionArg.html#getCacheable())
            to cacheable.
            :::

            [Parameters:]{.paramLabel}
            :   `cacheable` - The value for cacheable

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setCacheable(java.util.Optional)}

        -   #### setCacheable

            ``` methodSignature
            public final JsBundleGenruleDescriptionArg.Builder setCacheable​(Optional<Boolean> cacheable)
            ```

            ::: block
            Initializes the optional value
            [`cacheable`](JsBundleGenruleDescriptionArg.html#getCacheable())
            to cacheable.
            :::

            [Parameters:]{.paramLabel}
            :   `cacheable` - The value for cacheable

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCmd(com.facebook.buck.rules.macros.StringWithMacros)}

        -   #### setCmd

            ``` methodSignature
            public final JsBundleGenruleDescriptionArg.Builder setCmd​(StringWithMacros cmd)
            ```

            ::: block
            Initializes the optional value
            [`cmd`](JsBundleGenruleDescriptionArg.html#getCmd()) to cmd.
            :::

            [Parameters:]{.paramLabel}
            :   `cmd` - The value for cmd

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setCmd(java.util.Optional)}

        -   #### setCmd

            ``` methodSignature
            public final JsBundleGenruleDescriptionArg.Builder setCmd​(Optional<? extends StringWithMacros> cmd)
            ```

            ::: block
            Initializes the optional value
            [`cmd`](JsBundleGenruleDescriptionArg.html#getCmd()) to cmd.
            :::

            [Parameters:]{.paramLabel}
            :   `cmd` - The value for cmd

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCmdExe(com.facebook.buck.rules.macros.StringWithMacros)}

        -   #### setCmdExe

            ``` methodSignature
            public final JsBundleGenruleDescriptionArg.Builder setCmdExe​(StringWithMacros cmdExe)
            ```

            ::: block
            Initializes the optional value
            [`cmdExe`](JsBundleGenruleDescriptionArg.html#getCmdExe())
            to cmdExe.
            :::

            [Parameters:]{.paramLabel}
            :   `cmdExe` - The value for cmdExe

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setCmdExe(java.util.Optional)}

        -   #### setCmdExe

            ``` methodSignature
            public final JsBundleGenruleDescriptionArg.Builder setCmdExe​(Optional<? extends StringWithMacros> cmdExe)
            ```

            ::: block
            Initializes the optional value
            [`cmdExe`](JsBundleGenruleDescriptionArg.html#getCmdExe())
            to cmdExe.
            :::

            [Parameters:]{.paramLabel}
            :   `cmdExe` - The value for cmdExe

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setEnableSandbox(boolean)}

        -   #### setEnableSandbox

            ``` methodSignature
            public final JsBundleGenruleDescriptionArg.Builder setEnableSandbox​(boolean enableSandbox)
            ```

            ::: block
            Initializes the optional value
            [`enableSandbox`](JsBundleGenruleDescriptionArg.html#getEnableSandbox())
            to enableSandbox.
            :::

            [Parameters:]{.paramLabel}
            :   `enableSandbox` - The value for enableSandbox

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setEnableSandbox(java.util.Optional)}

        -   #### setEnableSandbox

            ``` methodSignature
            public final JsBundleGenruleDescriptionArg.Builder setEnableSandbox​(Optional<Boolean> enableSandbox)
            ```

            ::: block
            Initializes the optional value
            [`enableSandbox`](JsBundleGenruleDescriptionArg.html#getEnableSandbox())
            to enableSandbox.
            :::

            [Parameters:]{.paramLabel}
            :   `enableSandbox` - The value for enableSandbox

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setEnvironmentExpansionSeparator(java.lang.String)}

        -   #### setEnvironmentExpansionSeparator

            ``` methodSignature
            public final JsBundleGenruleDescriptionArg.Builder setEnvironmentExpansionSeparator​(String environmentExpansionSeparator)
            ```

            ::: block
            Initializes the optional value
            [`environmentExpansionSeparator`](JsBundleGenruleDescriptionArg.html#getEnvironmentExpansionSeparator())
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
            public final JsBundleGenruleDescriptionArg.Builder setEnvironmentExpansionSeparator​(Optional<String> environmentExpansionSeparator)
            ```

            ::: block
            Initializes the optional value
            [`environmentExpansionSeparator`](JsBundleGenruleDescriptionArg.html#getEnvironmentExpansionSeparator())
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
            public final JsBundleGenruleDescriptionArg.Builder setRemote​(boolean remote)
            ```

            ::: block
            Initializes the optional value
            [`remote`](JsBundleGenruleDescriptionArg.html#getRemote())
            to remote.
            :::

            [Parameters:]{.paramLabel}
            :   `remote` - The value for remote

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setRemote(java.util.Optional)}

        -   #### setRemote

            ``` methodSignature
            public final JsBundleGenruleDescriptionArg.Builder setRemote​(Optional<Boolean> remote)
            ```

            ::: block
            Initializes the optional value
            [`remote`](JsBundleGenruleDescriptionArg.html#getRemote())
            to remote.
            :::

            [Parameters:]{.paramLabel}
            :   `remote` - The value for remote

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setSrcs(com.facebook.buck.rules.coercer.SourceSet)}

        -   #### setSrcs

            ``` methodSignature
            public final JsBundleGenruleDescriptionArg.Builder setSrcs​(SourceSet srcs)
            ```

            ::: block
            Initializes the value for the
            [`srcs`](JsBundleGenruleDescriptionArg.html#getSrcs())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`srcs`](JsBundleGenruleDescriptionArg.html#getSrcs()).*
            :::

            [Parameters:]{.paramLabel}
            :   `srcs` - The value for srcs

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setNeedAndroidTools(boolean)}

        -   #### setNeedAndroidTools

            ``` methodSignature
            public final JsBundleGenruleDescriptionArg.Builder setNeedAndroidTools​(boolean needAndroidTools)
            ```

            ::: block
            Initializes the value for the
            [`needAndroidTools`](JsBundleGenruleDescriptionArg.html#isNeedAndroidTools())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`needAndroidTools`](JsBundleGenruleDescriptionArg.html#isNeedAndroidTools()).*
            :::

            [Parameters:]{.paramLabel}
            :   `needAndroidTools` - The value for needAndroidTools

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCompatibleWith(com.facebook.buck.core.model.UnconfiguredBuildTarget)}

        -   #### addCompatibleWith

            ``` methodSignature
            public final JsBundleGenruleDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget element)
            ```

            ::: block
            Adds one element to
            [`compatibleWith`](JsBundleGenruleDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A compatibleWith element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCompatibleWith(com.facebook.buck.core.model.UnconfiguredBuildTarget...)}

        -   #### addCompatibleWith

            ``` methodSignature
            public final JsBundleGenruleDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](JsBundleGenruleDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCompatibleWith(java.lang.Iterable)}

        -   #### setCompatibleWith

            ``` methodSignature
            public final JsBundleGenruleDescriptionArg.Builder setCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`compatibleWith`](JsBundleGenruleDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllCompatibleWith(java.lang.Iterable)}

        -   #### addAllCompatibleWith

            ``` methodSignature
            public final JsBundleGenruleDescriptionArg.Builder addAllCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](JsBundleGenruleDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDefaultTargetPlatform(com.facebook.buck.core.model.UnconfiguredBuildTarget)}

        -   #### setDefaultTargetPlatform

            ``` methodSignature
            public final JsBundleGenruleDescriptionArg.Builder setDefaultTargetPlatform​(UnconfiguredBuildTarget defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](JsBundleGenruleDescriptionArg.html#getDefaultTargetPlatform())
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
            public final JsBundleGenruleDescriptionArg.Builder setDefaultTargetPlatform​(Optional<? extends UnconfiguredBuildTarget> defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](JsBundleGenruleDescriptionArg.html#getDefaultTargetPlatform())
            to defaultTargetPlatform.
            :::

            [Parameters:]{.paramLabel}
            :   `defaultTargetPlatform` - The value for
                defaultTargetPlatform

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLabels(java.lang.String)}

        -   #### addLabels

            ``` methodSignature
            public final JsBundleGenruleDescriptionArg.Builder addLabels​(String element)
            ```

            ::: block
            Adds one element to
            [`labels`](JsBundleGenruleDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A labels element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLabels(java.lang.String...)}

        -   #### addLabels

            ``` methodSignature
            public final JsBundleGenruleDescriptionArg.Builder addLabels​(String... elements)
            ```

            ::: block
            Adds elements to
            [`labels`](JsBundleGenruleDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLabels(java.lang.Iterable)}

        -   #### setLabels

            ``` methodSignature
            public final JsBundleGenruleDescriptionArg.Builder setLabels​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`labels`](JsBundleGenruleDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLabels(java.lang.Iterable)}

        -   #### addAllLabels

            ``` methodSignature
            public final JsBundleGenruleDescriptionArg.Builder addAllLabels​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`labels`](JsBundleGenruleDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLicenses(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### addLicenses

            ``` methodSignature
            public final JsBundleGenruleDescriptionArg.Builder addLicenses​(SourcePath element)
            ```

            ::: block
            Adds one element to
            [`licenses`](JsBundleGenruleDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A licenses element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLicenses(com.facebook.buck.core.sourcepath.SourcePath...)}

        -   #### addLicenses

            ``` methodSignature
            public final JsBundleGenruleDescriptionArg.Builder addLicenses​(SourcePath... elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](JsBundleGenruleDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLicenses(java.lang.Iterable)}

        -   #### setLicenses

            ``` methodSignature
            public final JsBundleGenruleDescriptionArg.Builder setLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`licenses`](JsBundleGenruleDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLicenses(java.lang.Iterable)}

        -   #### addAllLicenses

            ``` methodSignature
            public final JsBundleGenruleDescriptionArg.Builder addAllLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](JsBundleGenruleDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setName(java.lang.String)}

        -   #### setName

            ``` methodSignature
            public final JsBundleGenruleDescriptionArg.Builder setName​(String name)
            ```

            ::: block
            Initializes the value for the
            [`name`](JsBundleGenruleDescriptionArg.html#getName())
            attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `name` - The value for name

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addTests(com.facebook.buck.core.model.BuildTarget)}

        -   #### addTests

            ``` methodSignature
            public final JsBundleGenruleDescriptionArg.Builder addTests​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`tests`](JsBundleGenruleDescriptionArg.html#getTests())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A tests element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addTests(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addTests

            ``` methodSignature
            public final JsBundleGenruleDescriptionArg.Builder addTests​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`tests`](JsBundleGenruleDescriptionArg.html#getTests())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of tests elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setTests(java.lang.Iterable)}

        -   #### setTests

            ``` methodSignature
            public final JsBundleGenruleDescriptionArg.Builder setTests​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`tests`](JsBundleGenruleDescriptionArg.html#getTests())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of tests elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllTests(java.lang.Iterable)}

        -   #### addAllTests

            ``` methodSignature
            public final JsBundleGenruleDescriptionArg.Builder addAllTests​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`tests`](JsBundleGenruleDescriptionArg.html#getTests())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of tests elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setBundleName(java.lang.String)}

        -   #### setBundleName

            ``` methodSignature
            public final JsBundleGenruleDescriptionArg.Builder setBundleName​(String bundleName)
            ```

            ::: block
            Initializes the optional value
            [`bundleName`](JsBundleGenruleDescriptionArg.html#getBundleName())
            to bundleName.
            :::

            [Parameters:]{.paramLabel}
            :   `bundleName` - The value for bundleName

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setBundleName(java.util.Optional)}

        -   #### setBundleName

            ``` methodSignature
            public final JsBundleGenruleDescriptionArg.Builder setBundleName​(Optional<String> bundleName)
            ```

            ::: block
            Initializes the optional value
            [`bundleName`](JsBundleGenruleDescriptionArg.html#getBundleName())
            to bundleName.
            :::

            [Parameters:]{.paramLabel}
            :   `bundleName` - The value for bundleName

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addBundleNameForFlavor(com.facebook.buck.util.types.Pair)}

        -   #### addBundleNameForFlavor

            ``` methodSignature
            public final JsBundleGenruleDescriptionArg.Builder addBundleNameForFlavor​(Pair<Flavor,​String> element)
            ```

            ::: block
            Adds one element to
            [`bundleNameForFlavor`](JsBundleGenruleDescriptionArg.html#getBundleNameForFlavor())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A bundleNameForFlavor element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addBundleNameForFlavor(com.facebook.buck.util.types.Pair...)}

        -   #### addBundleNameForFlavor

            ``` methodSignature
            @SafeVarargs
            public final JsBundleGenruleDescriptionArg.Builder addBundleNameForFlavor​(Pair<Flavor,​String>... elements)
            ```

            ::: block
            Adds elements to
            [`bundleNameForFlavor`](JsBundleGenruleDescriptionArg.html#getBundleNameForFlavor())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of bundleNameForFlavor elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setBundleNameForFlavor(java.lang.Iterable)}

        -   #### setBundleNameForFlavor

            ``` methodSignature
            public final JsBundleGenruleDescriptionArg.Builder setBundleNameForFlavor​(Iterable<? extends Pair<Flavor,​String>> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`bundleNameForFlavor`](JsBundleGenruleDescriptionArg.html#getBundleNameForFlavor())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of bundleNameForFlavor elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllBundleNameForFlavor(java.lang.Iterable)}

        -   #### addAllBundleNameForFlavor

            ``` methodSignature
            public final JsBundleGenruleDescriptionArg.Builder addAllBundleNameForFlavor​(Iterable<? extends Pair<Flavor,​String>> elements)
            ```

            ::: block
            Adds elements to
            [`bundleNameForFlavor`](JsBundleGenruleDescriptionArg.html#getBundleNameForFlavor())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of bundleNameForFlavor elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#build()}

        -   #### build

            ``` methodSignature
            public JsBundleGenruleDescriptionArg build()
            ```

            ::: block
            Builds a new
            [`JsBundleGenruleDescriptionArg`](JsBundleGenruleDescriptionArg.html "class in com.facebook.buck.features.js").
            :::

            [Returns:]{.returnLabel}
            :   An immutable instance of JsBundleGenruleDescriptionArg

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
