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

## Class JsBundleDescriptionArg.Builder {#class-jsbundledescriptionarg.builder .title title="Class JsBundleDescriptionArg.Builder"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.features.js.JsBundleDescriptionArg.Builder

::: description
-   

    Enclosing class:
    :   [JsBundleDescriptionArg](JsBundleDescriptionArg.html "class in com.facebook.buck.features.js")

    ------------------------------------------------------------------------

        @NotThreadSafe
        public static final class JsBundleDescriptionArg.Builder
        extends Object

    ::: block
    Builds instances of type
    [`JsBundleDescriptionArg`](JsBundleDescriptionArg.html "class in com.facebook.buck.features.js").
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
        | `JsBundleDe           | `addAllBundleN        | ::: block             |
        | scriptionArg.Builder` | ameForFlavor​(Iterable | Adds elements to      |
        |                       | <? extends Pair<Flavo | [`bundleNameFo        |
        |                       | r,​String>> elements)` | rFlavor`](JsBundleDes |
        |                       |                       | criptionArg.html#getB |
        |                       |                       | undleNameForFlavor()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsBundleDe           | `addAllCompat         | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Iterable<? e | Adds elements to      |
        |                       | xtends UnconfiguredBu | [`co                  |
        |                       | ildTarget> elements)` | mpatibleWith`](JsBund |
        |                       |                       | leDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsBundleDe           | `addAllDeps​(          | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Adds elements to      |
        |                       | ildTarget> elements)` | [`dep                 |
        |                       |                       | s`](JsBundleDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsBundleDe           | `addAllLabels​(Iterab  | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Adds elements to      |
        |                       |                       | [`labels`             |
        |                       |                       | ](JsBundleDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsBundleDe           | `addAllLicenses       | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Adds elements to      |
        |                       | ourcePath> elements)` | [`licenses`](         |
        |                       |                       | JsBundleDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsBundleDe           | `addBundleN           | ::: block             |
        | scriptionArg.Builder` | ameForFlavor​(Pair<Fla | Adds one element to   |
        |                       | vor,​String> element)` | [`bundleNameFo        |
        |                       |                       | rFlavor`](JsBundleDes |
        |                       |                       | criptionArg.html#getB |
        |                       |                       | undleNameForFlavor()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsBundleDe           | `addBundleNameF       | ::: block             |
        | scriptionArg.Builder` | orFlavor​(Pair<Flavor, | Adds elements to      |
        |                       | ​String>... elements)` | [`bundleNameFo        |
        |                       |                       | rFlavor`](JsBundleDes |
        |                       |                       | criptionArg.html#getB |
        |                       |                       | undleNameForFlavor()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsBundleDe           | `addCompat            | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Unconfigured | Adds one element to   |
        |                       | BuildTarget element)` | [`co                  |
        |                       |                       | mpatibleWith`](JsBund |
        |                       |                       | leDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsBundleDe           | `addCompatible        | ::: block             |
        | scriptionArg.Builder` | With​(UnconfiguredBuil | Adds elements to      |
        |                       | dTarget... elements)` | [`co                  |
        |                       |                       | mpatibleWith`](JsBund |
        |                       |                       | leDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsBundleDe           | `addDeps​(             | ::: block             |
        | scriptionArg.Builder` | BuildTarget element)` | Adds one element to   |
        |                       |                       | [`dep                 |
        |                       |                       | s`](JsBundleDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsBundleDe           | `addDeps​(Buil         | ::: block             |
        | scriptionArg.Builder` | dTarget... elements)` | Adds elements to      |
        |                       |                       | [`dep                 |
        |                       |                       | s`](JsBundleDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsBundleDe           | `addLa                | ::: block             |
        | scriptionArg.Builder` | bels​(String element)` | Adds one element to   |
        |                       |                       | [`labels`             |
        |                       |                       | ](JsBundleDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsBundleDe           | `addLabels            | ::: block             |
        | scriptionArg.Builder` | ​(String... elements)` | Adds elements to      |
        |                       |                       | [`labels`             |
        |                       |                       | ](JsBundleDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsBundleDe           | `addLicenses          | ::: block             |
        | scriptionArg.Builder` | ​(SourcePath element)` | Adds one element to   |
        |                       |                       | [`licenses`](         |
        |                       |                       | JsBundleDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsBundleDe           | `addLicenses​(Sou      | ::: block             |
        | scriptionArg.Builder` | rcePath... elements)` | Adds elements to      |
        |                       |                       | [`licenses`](         |
        |                       |                       | JsBundleDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Js                   | `build()`             | ::: block             |
        | BundleDescriptionArg` |                       | Builds a new          |
        |                       |                       | [`JsBundleDes         |
        |                       |                       | criptionArg`](JsBundl |
        |                       |                       | eDescriptionArg.html  |
        |                       |                       | "class in com.faceboo |
        |                       |                       | k.buck.features.js"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsBundleDe           | `from​(Bu              | ::: block             |
        | scriptionArg.Builder` | ildRuleArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebo           |
        |                       |                       | ok.buck.core.descript |
        |                       |                       | ion.arg.BuildRuleArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsBundleDe           | `from​(Cons            | ::: block             |
        | scriptionArg.Builder` | tructorArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook         |
        |                       |                       | .buck.core.descriptio |
        |                       |                       | n.arg.ConstructorArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsBundleDe           | `from​(HasDe           | ::: block             |
        | scriptionArg.Builder` | claredDeps instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook.        |
        |                       |                       | buck.core.description |
        |                       |                       | .arg.HasDeclaredDeps` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsBundleDe           | `from​(Has             | ::: block             |
        | scriptionArg.Builder` | BundleName instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `co                   |
        |                       |                       | m.facebook.buck.featu |
        |                       |                       | res.js.HasBundleName` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsBundleDe           | `from​(Ha              | ::: block             |
        | scriptionArg.Builder` | sExtraJson instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `c                    |
        |                       |                       | om.facebook.buck.feat |
        |                       |                       | ures.js.HasExtraJson` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsBundleDe           | `from​(com.fac         | ::: block             |
        | scriptionArg.Builder` | ebook.buck.features.j | Copy abstract value   |
        |                       | s.JsBundleDescription | type                  |
        |                       | .AbstractJsBundleDesc | `AbstractJs           |
        |                       | riptionArg instance)` | BundleDescriptionArg` |
        |                       |                       | instance into         |
        |                       |                       | builder.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsBundleDe           | `from​(JsBundleDesc    | ::: block             |
        | scriptionArg.Builder` | riptionArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `Js                   |
        |                       |                       | BundleDescriptionArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsBundleDe           | `setAndroidPackage​(St | ::: block             |
        | scriptionArg.Builder` | ring androidPackage)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`an                  |
        |                       |                       | droidPackage`](JsBund |
        |                       |                       | leDescriptionArg.html |
        |                       |                       | #getAndroidPackage()) |
        |                       |                       | to androidPackage.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsBundleDe           | `setAndroi            | ::: block             |
        | scriptionArg.Builder` | dPackage​(Optional<Str | Initializes the       |
        |                       | ing> androidPackage)` | optional value        |
        |                       |                       | [`an                  |
        |                       |                       | droidPackage`](JsBund |
        |                       |                       | leDescriptionArg.html |
        |                       |                       | #getAndroidPackage()) |
        |                       |                       | to androidPackage.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsBundleDe           | `setBundleNam         | ::: block             |
        | scriptionArg.Builder` | e​(String bundleName)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`bundleName`](Js     |
        |                       |                       | BundleDescriptionArg. |
        |                       |                       | html#getBundleName()) |
        |                       |                       | to bundleName.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsBundleDe           | `s                    | ::: block             |
        | scriptionArg.Builder` | etBundleName​(Optional | Initializes the       |
        |                       | <String> bundleName)` | optional value        |
        |                       |                       | [`bundleName`](Js     |
        |                       |                       | BundleDescriptionArg. |
        |                       |                       | html#getBundleName()) |
        |                       |                       | to bundleName.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsBundleDe           | `setBundleN           | ::: block             |
        | scriptionArg.Builder` | ameForFlavor​(Iterable | Sets or replaces all  |
        |                       | <? extends Pair<Flavo | elements for          |
        |                       | r,​String>> elements)` | [`bundleNameFo        |
        |                       |                       | rFlavor`](JsBundleDes |
        |                       |                       | criptionArg.html#getB |
        |                       |                       | undleNameForFlavor()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsBundleDe           | `setCompat            | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Iterable<? e | Sets or replaces all  |
        |                       | xtends UnconfiguredBu | elements for          |
        |                       | ildTarget> elements)` | [`co                  |
        |                       |                       | mpatibleWith`](JsBund |
        |                       |                       | leDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsBundleDe           | `setDefaul            | ::: block             |
        | scriptionArg.Builder` | tTargetPlatform​(Uncon | Initializes the       |
        |                       | figuredBuildTarget de | optional value        |
        |                       | faultTargetPlatform)` | [`defaultTargetPla    |
        |                       |                       | tform`](JsBundleDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsBundleDe           | `setDefau             | ::: block             |
        | scriptionArg.Builder` | ltTargetPlatform​(Opti | Initializes the       |
        |                       | onal<? extends Unconf | optional value        |
        |                       | iguredBuildTarget> de | [`defaultTargetPla    |
        |                       | faultTargetPlatform)` | tform`](JsBundleDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsBundleDe           | `setDeps​(             | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Sets or replaces all  |
        |                       | ildTarget> elements)` | elements for          |
        |                       |                       | [`dep                 |
        |                       |                       | s`](JsBundleDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsBundleDe           | `setEntry​(Either      | ::: block             |
        | scriptionArg.Builder` | <com.google.common.co | Initializes the value |
        |                       | llect.ImmutableSet<St | for the               |
        |                       | ring>,​String> entry)` | [`entry               |
        |                       |                       | `](JsBundleDescriptio |
        |                       |                       | nArg.html#getEntry()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsBundleDe           | `setExtraJson​(StringW | ::: block             |
        | scriptionArg.Builder` | ithMacros extraJson)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`extraJson`](J       |
        |                       |                       | sBundleDescriptionArg |
        |                       |                       | .html#getExtraJson()) |
        |                       |                       | to extraJson.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsBundleDe           | `setExtraJson​(Option  | ::: block             |
        | scriptionArg.Builder` | al<? extends StringWi | Initializes the       |
        |                       | thMacros> extraJson)` | optional value        |
        |                       |                       | [`extraJson`](J       |
        |                       |                       | sBundleDescriptionArg |
        |                       |                       | .html#getExtraJson()) |
        |                       |                       | to extraJson.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsBundleDe           | `setLabels​(Iterab     | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Sets or replaces all  |
        |                       |                       | elements for          |
        |                       |                       | [`labels`             |
        |                       |                       | ](JsBundleDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsBundleDe           | `setLicenses          | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Sets or replaces all  |
        |                       | ourcePath> elements)` | elements for          |
        |                       |                       | [`licenses`](         |
        |                       |                       | JsBundleDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsBundleDe           | `                     | ::: block             |
        | scriptionArg.Builder` | setName​(String name)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`nam                 |
        |                       |                       | e`](JsBundleDescripti |
        |                       |                       | onArg.html#getName()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsBundleDe           | `setWorker            | ::: block             |
        | scriptionArg.Builder` | ​(BuildTarget worker)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`worker`             |
        |                       |                       | ](JsBundleDescription |
        |                       |                       | Arg.html#getWorker()) |
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

        []{#from(com.facebook.buck.core.description.arg.HasDeclaredDeps)}

        -   #### from

            ``` methodSignature
            public final JsBundleDescriptionArg.Builder from​(HasDeclaredDeps instance)
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

        []{#from(com.facebook.buck.features.js.JsBundleDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final JsBundleDescriptionArg.Builder from​(JsBundleDescriptionArg instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `JsBundleDescriptionArg` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.features.js.JsBundleDescription.AbstractJsBundleDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final JsBundleDescriptionArg.Builder from​(com.facebook.buck.features.js.JsBundleDescription.AbstractJsBundleDescriptionArg instance)
            ```

            ::: block
            Copy abstract value type `AbstractJsBundleDescriptionArg`
            instance into builder.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.features.js.HasExtraJson)}

        -   #### from

            ``` methodSignature
            public final JsBundleDescriptionArg.Builder from​(HasExtraJson instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `com.facebook.buck.features.js.HasExtraJson` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.features.js.HasBundleName)}

        -   #### from

            ``` methodSignature
            public final JsBundleDescriptionArg.Builder from​(HasBundleName instance)
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
            public final JsBundleDescriptionArg.Builder from​(BuildRuleArg instance)
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
            public final JsBundleDescriptionArg.Builder from​(ConstructorArg instance)
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

        []{#setEntry(com.facebook.buck.util.types.Either)}

        -   #### setEntry

            ``` methodSignature
            public final JsBundleDescriptionArg.Builder setEntry​(Either<com.google.common.collect.ImmutableSet<String>,​String> entry)
            ```

            ::: block
            Initializes the value for the
            [`entry`](JsBundleDescriptionArg.html#getEntry()) attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `entry` - The value for entry

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setWorker(com.facebook.buck.core.model.BuildTarget)}

        -   #### setWorker

            ``` methodSignature
            public final JsBundleDescriptionArg.Builder setWorker​(BuildTarget worker)
            ```

            ::: block
            Initializes the value for the
            [`worker`](JsBundleDescriptionArg.html#getWorker())
            attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `worker` - The value for worker

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setAndroidPackage(java.lang.String)}

        -   #### setAndroidPackage

            ``` methodSignature
            public final JsBundleDescriptionArg.Builder setAndroidPackage​(String androidPackage)
            ```

            ::: block
            Initializes the optional value
            [`androidPackage`](JsBundleDescriptionArg.html#getAndroidPackage())
            to androidPackage.
            :::

            [Parameters:]{.paramLabel}
            :   `androidPackage` - The value for androidPackage

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setAndroidPackage(java.util.Optional)}

        -   #### setAndroidPackage

            ``` methodSignature
            public final JsBundleDescriptionArg.Builder setAndroidPackage​(Optional<String> androidPackage)
            ```

            ::: block
            Initializes the optional value
            [`androidPackage`](JsBundleDescriptionArg.html#getAndroidPackage())
            to androidPackage.
            :::

            [Parameters:]{.paramLabel}
            :   `androidPackage` - The value for androidPackage

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCompatibleWith(com.facebook.buck.core.model.UnconfiguredBuildTarget)}

        -   #### addCompatibleWith

            ``` methodSignature
            public final JsBundleDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget element)
            ```

            ::: block
            Adds one element to
            [`compatibleWith`](JsBundleDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A compatibleWith element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCompatibleWith(com.facebook.buck.core.model.UnconfiguredBuildTarget...)}

        -   #### addCompatibleWith

            ``` methodSignature
            public final JsBundleDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](JsBundleDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCompatibleWith(java.lang.Iterable)}

        -   #### setCompatibleWith

            ``` methodSignature
            public final JsBundleDescriptionArg.Builder setCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`compatibleWith`](JsBundleDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllCompatibleWith(java.lang.Iterable)}

        -   #### addAllCompatibleWith

            ``` methodSignature
            public final JsBundleDescriptionArg.Builder addAllCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](JsBundleDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDefaultTargetPlatform(com.facebook.buck.core.model.UnconfiguredBuildTarget)}

        -   #### setDefaultTargetPlatform

            ``` methodSignature
            public final JsBundleDescriptionArg.Builder setDefaultTargetPlatform​(UnconfiguredBuildTarget defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](JsBundleDescriptionArg.html#getDefaultTargetPlatform())
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
            public final JsBundleDescriptionArg.Builder setDefaultTargetPlatform​(Optional<? extends UnconfiguredBuildTarget> defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](JsBundleDescriptionArg.html#getDefaultTargetPlatform())
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
            public final JsBundleDescriptionArg.Builder addLabels​(String element)
            ```

            ::: block
            Adds one element to
            [`labels`](JsBundleDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A labels element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLabels(java.lang.String...)}

        -   #### addLabels

            ``` methodSignature
            public final JsBundleDescriptionArg.Builder addLabels​(String... elements)
            ```

            ::: block
            Adds elements to
            [`labels`](JsBundleDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLabels(java.lang.Iterable)}

        -   #### setLabels

            ``` methodSignature
            public final JsBundleDescriptionArg.Builder setLabels​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`labels`](JsBundleDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLabels(java.lang.Iterable)}

        -   #### addAllLabels

            ``` methodSignature
            public final JsBundleDescriptionArg.Builder addAllLabels​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`labels`](JsBundleDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLicenses(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### addLicenses

            ``` methodSignature
            public final JsBundleDescriptionArg.Builder addLicenses​(SourcePath element)
            ```

            ::: block
            Adds one element to
            [`licenses`](JsBundleDescriptionArg.html#getLicenses()) set.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A licenses element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLicenses(com.facebook.buck.core.sourcepath.SourcePath...)}

        -   #### addLicenses

            ``` methodSignature
            public final JsBundleDescriptionArg.Builder addLicenses​(SourcePath... elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](JsBundleDescriptionArg.html#getLicenses()) set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLicenses(java.lang.Iterable)}

        -   #### setLicenses

            ``` methodSignature
            public final JsBundleDescriptionArg.Builder setLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`licenses`](JsBundleDescriptionArg.html#getLicenses()) set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLicenses(java.lang.Iterable)}

        -   #### addAllLicenses

            ``` methodSignature
            public final JsBundleDescriptionArg.Builder addAllLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](JsBundleDescriptionArg.html#getLicenses()) set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setName(java.lang.String)}

        -   #### setName

            ``` methodSignature
            public final JsBundleDescriptionArg.Builder setName​(String name)
            ```

            ::: block
            Initializes the value for the
            [`name`](JsBundleDescriptionArg.html#getName()) attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `name` - The value for name

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addDeps(com.facebook.buck.core.model.BuildTarget)}

        -   #### addDeps

            ``` methodSignature
            public final JsBundleDescriptionArg.Builder addDeps​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`deps`](JsBundleDescriptionArg.html#getDeps()) sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A deps element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addDeps(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addDeps

            ``` methodSignature
            public final JsBundleDescriptionArg.Builder addDeps​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`deps`](JsBundleDescriptionArg.html#getDeps()) sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDeps(java.lang.Iterable)}

        -   #### setDeps

            ``` methodSignature
            public final JsBundleDescriptionArg.Builder setDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`deps`](JsBundleDescriptionArg.html#getDeps()) sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllDeps(java.lang.Iterable)}

        -   #### addAllDeps

            ``` methodSignature
            public final JsBundleDescriptionArg.Builder addAllDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`deps`](JsBundleDescriptionArg.html#getDeps()) sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setExtraJson(com.facebook.buck.rules.macros.StringWithMacros)}

        -   #### setExtraJson

            ``` methodSignature
            public final JsBundleDescriptionArg.Builder setExtraJson​(StringWithMacros extraJson)
            ```

            ::: block
            Initializes the optional value
            [`extraJson`](JsBundleDescriptionArg.html#getExtraJson()) to
            extraJson.
            :::

            [Parameters:]{.paramLabel}
            :   `extraJson` - The value for extraJson

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setExtraJson(java.util.Optional)}

        -   #### setExtraJson

            ``` methodSignature
            public final JsBundleDescriptionArg.Builder setExtraJson​(Optional<? extends StringWithMacros> extraJson)
            ```

            ::: block
            Initializes the optional value
            [`extraJson`](JsBundleDescriptionArg.html#getExtraJson()) to
            extraJson.
            :::

            [Parameters:]{.paramLabel}
            :   `extraJson` - The value for extraJson

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setBundleName(java.lang.String)}

        -   #### setBundleName

            ``` methodSignature
            public final JsBundleDescriptionArg.Builder setBundleName​(String bundleName)
            ```

            ::: block
            Initializes the optional value
            [`bundleName`](JsBundleDescriptionArg.html#getBundleName())
            to bundleName.
            :::

            [Parameters:]{.paramLabel}
            :   `bundleName` - The value for bundleName

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setBundleName(java.util.Optional)}

        -   #### setBundleName

            ``` methodSignature
            public final JsBundleDescriptionArg.Builder setBundleName​(Optional<String> bundleName)
            ```

            ::: block
            Initializes the optional value
            [`bundleName`](JsBundleDescriptionArg.html#getBundleName())
            to bundleName.
            :::

            [Parameters:]{.paramLabel}
            :   `bundleName` - The value for bundleName

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addBundleNameForFlavor(com.facebook.buck.util.types.Pair)}

        -   #### addBundleNameForFlavor

            ``` methodSignature
            public final JsBundleDescriptionArg.Builder addBundleNameForFlavor​(Pair<Flavor,​String> element)
            ```

            ::: block
            Adds one element to
            [`bundleNameForFlavor`](JsBundleDescriptionArg.html#getBundleNameForFlavor())
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
            public final JsBundleDescriptionArg.Builder addBundleNameForFlavor​(Pair<Flavor,​String>... elements)
            ```

            ::: block
            Adds elements to
            [`bundleNameForFlavor`](JsBundleDescriptionArg.html#getBundleNameForFlavor())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of bundleNameForFlavor elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setBundleNameForFlavor(java.lang.Iterable)}

        -   #### setBundleNameForFlavor

            ``` methodSignature
            public final JsBundleDescriptionArg.Builder setBundleNameForFlavor​(Iterable<? extends Pair<Flavor,​String>> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`bundleNameForFlavor`](JsBundleDescriptionArg.html#getBundleNameForFlavor())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of bundleNameForFlavor elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllBundleNameForFlavor(java.lang.Iterable)}

        -   #### addAllBundleNameForFlavor

            ``` methodSignature
            public final JsBundleDescriptionArg.Builder addAllBundleNameForFlavor​(Iterable<? extends Pair<Flavor,​String>> elements)
            ```

            ::: block
            Adds elements to
            [`bundleNameForFlavor`](JsBundleDescriptionArg.html#getBundleNameForFlavor())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of bundleNameForFlavor elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#build()}

        -   #### build

            ``` methodSignature
            public JsBundleDescriptionArg build()
            ```

            ::: block
            Builds a new
            [`JsBundleDescriptionArg`](JsBundleDescriptionArg.html "class in com.facebook.buck.features.js").
            :::

            [Returns:]{.returnLabel}
            :   An immutable instance of JsBundleDescriptionArg

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
