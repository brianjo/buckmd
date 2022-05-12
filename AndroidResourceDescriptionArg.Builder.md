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

## Class AndroidResourceDescriptionArg.Builder {#class-androidresourcedescriptionarg.builder .title title="Class AndroidResourceDescriptionArg.Builder"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.android.AndroidResourceDescriptionArg.Builder

::: description
-   

    Enclosing class:
    :   [AndroidResourceDescriptionArg](AndroidResourceDescriptionArg.html "class in com.facebook.buck.android")

    ------------------------------------------------------------------------

        @NotThreadSafe
        public static final class AndroidResourceDescriptionArg.Builder
        extends Object

    ::: block
    Builds instances of type
    [`AndroidResourceDescriptionArg`](AndroidResourceDescriptionArg.html "class in com.facebook.buck.android").
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
        | `AndroidResourceDe    | `addAllCompat         | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Iterable<? e | Adds elements to      |
        |                       | xtends UnconfiguredBu | [`compatibl           |
        |                       | ildTarget> elements)` | eWith`](AndroidResour |
        |                       |                       | ceDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidResourceDe    | `addAllDeps​(          | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Adds elements to      |
        |                       | ildTarget> elements)` | [`deps`](And          |
        |                       |                       | roidResourceDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidResourceDe    | `addAllLabels​(Iterab  | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Adds elements to      |
        |                       |                       | [`labels`](Andro      |
        |                       |                       | idResourceDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidResourceDe    | `addAllLicenses       | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Adds elements to      |
        |                       | ourcePath> elements)` | [`licenses`](Android  |
        |                       |                       | ResourceDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidResourceDe    | `addCompat            | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Unconfigured | Adds one element to   |
        |                       | BuildTarget element)` | [`compatibl           |
        |                       |                       | eWith`](AndroidResour |
        |                       |                       | ceDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidResourceDe    | `addCompatible        | ::: block             |
        | scriptionArg.Builder` | With​(UnconfiguredBuil | Adds elements to      |
        |                       | dTarget... elements)` | [`compatibl           |
        |                       |                       | eWith`](AndroidResour |
        |                       |                       | ceDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidResourceDe    | `addDeps​(             | ::: block             |
        | scriptionArg.Builder` | BuildTarget element)` | Adds one element to   |
        |                       |                       | [`deps`](And          |
        |                       |                       | roidResourceDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidResourceDe    | `addDeps​(Buil         | ::: block             |
        | scriptionArg.Builder` | dTarget... elements)` | Adds elements to      |
        |                       |                       | [`deps`](And          |
        |                       |                       | roidResourceDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidResourceDe    | `addLa                | ::: block             |
        | scriptionArg.Builder` | bels​(String element)` | Adds one element to   |
        |                       |                       | [`labels`](Andro      |
        |                       |                       | idResourceDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidResourceDe    | `addLabels            | ::: block             |
        | scriptionArg.Builder` | ​(String... elements)` | Adds elements to      |
        |                       |                       | [`labels`](Andro      |
        |                       |                       | idResourceDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidResourceDe    | `addLicenses          | ::: block             |
        | scriptionArg.Builder` | ​(SourcePath element)` | Adds one element to   |
        |                       |                       | [`licenses`](Android  |
        |                       |                       | ResourceDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidResourceDe    | `addLicenses​(Sou      | ::: block             |
        | scriptionArg.Builder` | rcePath... elements)` | Adds elements to      |
        |                       |                       | [`licenses`](Android  |
        |                       |                       | ResourceDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidRe            | `build()`             | ::: block             |
        | sourceDescriptionArg` |                       | Builds a new          |
        |                       |                       | [`                    |
        |                       |                       | AndroidResourceDescri |
        |                       |                       | ptionArg`](AndroidRes |
        |                       |                       | ourceDescriptionArg.h |
        |                       |                       | tml "class in com.fac |
        |                       |                       | ebook.buck.android"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidResourceDe    | `f                    | ::: block             |
        | scriptionArg.Builder` | rom​(com.facebook.buck | Copy abstract value   |
        |                       | .android.AndroidResou | type                  |
        |                       | rceDescription.Abstra | `AbstractAndroidRe    |
        |                       | ctAndroidResourceDesc | sourceDescriptionArg` |
        |                       | riptionArg instance)` | instance into         |
        |                       |                       | builder.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidResourceDe    | `fro                  | ::: block             |
        | scriptionArg.Builder` | m​(AndroidResourceDesc | Fill a builder with   |
        |                       | riptionArg instance)` | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `AndroidRe            |
        |                       |                       | sourceDescriptionArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidResourceDe    | `from​(Bu              | ::: block             |
        | scriptionArg.Builder` | ildRuleArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebo           |
        |                       |                       | ok.buck.core.descript |
        |                       |                       | ion.arg.BuildRuleArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidResourceDe    | `from​(Cons            | ::: block             |
        | scriptionArg.Builder` | tructorArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook         |
        |                       |                       | .buck.core.descriptio |
        |                       |                       | n.arg.ConstructorArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidResourceDe    | `from​(HasDe           | ::: block             |
        | scriptionArg.Builder` | claredDeps instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook.        |
        |                       |                       | buck.core.description |
        |                       |                       | .arg.HasDeclaredDeps` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidResourceDe    | `setAssets​(Either<    | ::: block             |
        | scriptionArg.Builder` | SourcePath,​com.google | Initializes the       |
        |                       | .common.collect.Immut | optional value        |
        |                       | ableSortedMap<String, | [`assets`](Andro      |
        |                       | ​SourcePath>> assets)` | idResourceDescription |
        |                       |                       | Arg.html#getAssets()) |
        |                       |                       | to assets.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidResourceDe    | `setAssets​(Option     | ::: block             |
        | scriptionArg.Builder` | al<? extends Either<S | Initializes the       |
        |                       | ourcePath,​com.google. | optional value        |
        |                       | common.collect.Immuta | [`assets`](Andro      |
        |                       | bleSortedMap<String,​S | idResourceDescription |
        |                       | ourcePath>>> assets)` | Arg.html#getAssets()) |
        |                       |                       | to assets.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidResourceDe    | `setCompat            | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Iterable<? e | Sets or replaces all  |
        |                       | xtends UnconfiguredBu | elements for          |
        |                       | ildTarget> elements)` | [`compatibl           |
        |                       |                       | eWith`](AndroidResour |
        |                       |                       | ceDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidResourceDe    | `setDefaul            | ::: block             |
        | scriptionArg.Builder` | tTargetPlatform​(Uncon | Initializes the       |
        |                       | figuredBuildTarget de | optional value        |
        |                       | faultTargetPlatform)` | [`de                  |
        |                       |                       | faultTargetPlatform`] |
        |                       |                       | (AndroidResourceDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidResourceDe    | `setDefau             | ::: block             |
        | scriptionArg.Builder` | ltTargetPlatform​(Opti | Initializes the       |
        |                       | onal<? extends Unconf | optional value        |
        |                       | iguredBuildTarget> de | [`de                  |
        |                       | faultTargetPlatform)` | faultTargetPlatform`] |
        |                       |                       | (AndroidResourceDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidResourceDe    | `setDeps​(             | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Sets or replaces all  |
        |                       | ildTarget> elements)` | elements for          |
        |                       |                       | [`deps`](And          |
        |                       |                       | roidResourceDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidResourceDe    | `setHasWhitelis       | ::: block             |
        | scriptionArg.Builder` | tedStrings​(boolean ha | Initializes the value |
        |                       | sWhitelistedStrings)` | for the               |
        |                       |                       | [`ha                  |
        |                       |                       | sWhitelistedStrings`] |
        |                       |                       | (AndroidResourceDescr |
        |                       |                       | iptionArg.html#getHas |
        |                       |                       | WhitelistedStrings()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidResourceDe    | `setLabels​(Iterab     | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Sets or replaces all  |
        |                       |                       | elements for          |
        |                       |                       | [`labels`](Andro      |
        |                       |                       | idResourceDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidResourceDe    | `setLicenses          | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Sets or replaces all  |
        |                       | ourcePath> elements)` | elements for          |
        |                       |                       | [`licenses`](Android  |
        |                       |                       | ResourceDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidResourceDe    | `setManifest​(         | ::: block             |
        | scriptionArg.Builder` | SourcePath manifest)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`manifest`](Android  |
        |                       |                       | ResourceDescriptionAr |
        |                       |                       | g.html#getManifest()) |
        |                       |                       | to manifest.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidResourceDe    | `setManifest          | ::: block             |
        | scriptionArg.Builder` | ​(Optional<? extends S | Initializes the       |
        |                       | ourcePath> manifest)` | optional value        |
        |                       |                       | [`manifest`](Android  |
        |                       |                       | ResourceDescriptionAr |
        |                       |                       | g.html#getManifest()) |
        |                       |                       | to manifest.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidResourceDe    | `                     | ::: block             |
        | scriptionArg.Builder` | setName​(String name)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`name`](And          |
        |                       |                       | roidResourceDescripti |
        |                       |                       | onArg.html#getName()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidResourceDe    | `setPackag            | ::: block             |
        | scriptionArg.Builder` | e​(String getPackage)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`package`](Androi    |
        |                       |                       | dResourceDescriptionA |
        |                       |                       | rg.html#getPackage()) |
        |                       |                       | to getPackage.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidResourceDe    | `setPackage​(Optional  | ::: block             |
        | scriptionArg.Builder` | <String> getPackage)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`package`](Androi    |
        |                       |                       | dResourceDescriptionA |
        |                       |                       | rg.html#getPackage()) |
        |                       |                       | to getPackage.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidResourceDe    | `setProjectAssets     | ::: block             |
        | scriptionArg.Builder` | ​(Path projectAssets)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`project             |
        |                       |                       | Assets`](AndroidResou |
        |                       |                       | rceDescriptionArg.htm |
        |                       |                       | l#getProjectAssets()) |
        |                       |                       | to projectAssets.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidResourceDe    | `setProjectAsset      | ::: block             |
        | scriptionArg.Builder` | s​(Optional<? extends  | Initializes the       |
        |                       | Path> projectAssets)` | optional value        |
        |                       |                       | [`project             |
        |                       |                       | Assets`](AndroidResou |
        |                       |                       | rceDescriptionArg.htm |
        |                       |                       | l#getProjectAssets()) |
        |                       |                       | to projectAssets.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidResourceDe    | `setProject           | ::: block             |
        | scriptionArg.Builder` | Res​(Path projectRes)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`p                   |
        |                       |                       | rojectRes`](AndroidRe |
        |                       |                       | sourceDescriptionArg. |
        |                       |                       | html#getProjectRes()) |
        |                       |                       | to projectRes.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidResourceDe    | `setProjec            | ::: block             |
        | scriptionArg.Builder` | tRes​(Optional<? exten | Initializes the       |
        |                       | ds Path> projectRes)` | optional value        |
        |                       |                       | [`p                   |
        |                       |                       | rojectRes`](AndroidRe |
        |                       |                       | sourceDescriptionArg. |
        |                       |                       | html#getProjectRes()) |
        |                       |                       | to projectRes.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidResourceDe    | `setRes​(Eith          | ::: block             |
        | scriptionArg.Builder` | er<SourcePath,​com.goo | Initializes the       |
        |                       | gle.common.collect.Im | optional value        |
        |                       | mutableSortedMap<Stri | [`res`](An            |
        |                       | ng,​SourcePath>> res)` | droidResourceDescript |
        |                       |                       | ionArg.html#getRes()) |
        |                       |                       | to res.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidResourceDe    | `setRes​(Opt           | ::: block             |
        | scriptionArg.Builder` | ional<? extends Eithe | Initializes the       |
        |                       | r<SourcePath,​com.goog | optional value        |
        |                       | le.common.collect.Imm | [`res`](An            |
        |                       | utableSortedMap<Strin | droidResourceDescript |
        |                       | g,​SourcePath>>> res)` | ionArg.html#getRes()) |
        |                       |                       | to res.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidResourceDe    | `setResourceUnion​(bo  | ::: block             |
        | scriptionArg.Builder` | olean resourceUnion)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`resourc             |
        |                       |                       | eUnion`](AndroidResou |
        |                       |                       | rceDescriptionArg.htm |
        |                       |                       | l#getResourceUnion()) |
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
            public final AndroidResourceDescriptionArg.Builder from​(HasDeclaredDeps instance)
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

        []{#from(com.facebook.buck.android.AndroidResourceDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final AndroidResourceDescriptionArg.Builder from​(AndroidResourceDescriptionArg instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `AndroidResourceDescriptionArg` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.android.AndroidResourceDescription.AbstractAndroidResourceDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final AndroidResourceDescriptionArg.Builder from​(com.facebook.buck.android.AndroidResourceDescription.AbstractAndroidResourceDescriptionArg instance)
            ```

            ::: block
            Copy abstract value type
            `AbstractAndroidResourceDescriptionArg` instance into
            builder.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.core.description.arg.BuildRuleArg)}

        -   #### from

            ``` methodSignature
            public final AndroidResourceDescriptionArg.Builder from​(BuildRuleArg instance)
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
            public final AndroidResourceDescriptionArg.Builder from​(ConstructorArg instance)
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

        []{#setRes(com.facebook.buck.util.types.Either)}

        -   #### setRes

            ``` methodSignature
            public final AndroidResourceDescriptionArg.Builder setRes​(Either<SourcePath,​com.google.common.collect.ImmutableSortedMap<String,​SourcePath>> res)
            ```

            ::: block
            Initializes the optional value
            [`res`](AndroidResourceDescriptionArg.html#getRes()) to res.
            :::

            [Parameters:]{.paramLabel}
            :   `res` - The value for res

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setRes(java.util.Optional)}

        -   #### setRes

            ``` methodSignature
            public final AndroidResourceDescriptionArg.Builder setRes​(Optional<? extends Either<SourcePath,​com.google.common.collect.ImmutableSortedMap<String,​SourcePath>>> res)
            ```

            ::: block
            Initializes the optional value
            [`res`](AndroidResourceDescriptionArg.html#getRes()) to res.
            :::

            [Parameters:]{.paramLabel}
            :   `res` - The value for res

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setAssets(com.facebook.buck.util.types.Either)}

        -   #### setAssets

            ``` methodSignature
            public final AndroidResourceDescriptionArg.Builder setAssets​(Either<SourcePath,​com.google.common.collect.ImmutableSortedMap<String,​SourcePath>> assets)
            ```

            ::: block
            Initializes the optional value
            [`assets`](AndroidResourceDescriptionArg.html#getAssets())
            to assets.
            :::

            [Parameters:]{.paramLabel}
            :   `assets` - The value for assets

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setAssets(java.util.Optional)}

        -   #### setAssets

            ``` methodSignature
            public final AndroidResourceDescriptionArg.Builder setAssets​(Optional<? extends Either<SourcePath,​com.google.common.collect.ImmutableSortedMap<String,​SourcePath>>> assets)
            ```

            ::: block
            Initializes the optional value
            [`assets`](AndroidResourceDescriptionArg.html#getAssets())
            to assets.
            :::

            [Parameters:]{.paramLabel}
            :   `assets` - The value for assets

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setProjectRes(java.nio.file.Path)}

        -   #### setProjectRes

            ``` methodSignature
            public final AndroidResourceDescriptionArg.Builder setProjectRes​(Path projectRes)
            ```

            ::: block
            Initializes the optional value
            [`projectRes`](AndroidResourceDescriptionArg.html#getProjectRes())
            to projectRes.
            :::

            [Parameters:]{.paramLabel}
            :   `projectRes` - The value for projectRes

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setProjectRes(java.util.Optional)}

        -   #### setProjectRes

            ``` methodSignature
            public final AndroidResourceDescriptionArg.Builder setProjectRes​(Optional<? extends Path> projectRes)
            ```

            ::: block
            Initializes the optional value
            [`projectRes`](AndroidResourceDescriptionArg.html#getProjectRes())
            to projectRes.
            :::

            [Parameters:]{.paramLabel}
            :   `projectRes` - The value for projectRes

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setProjectAssets(java.nio.file.Path)}

        -   #### setProjectAssets

            ``` methodSignature
            public final AndroidResourceDescriptionArg.Builder setProjectAssets​(Path projectAssets)
            ```

            ::: block
            Initializes the optional value
            [`projectAssets`](AndroidResourceDescriptionArg.html#getProjectAssets())
            to projectAssets.
            :::

            [Parameters:]{.paramLabel}
            :   `projectAssets` - The value for projectAssets

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setProjectAssets(java.util.Optional)}

        -   #### setProjectAssets

            ``` methodSignature
            public final AndroidResourceDescriptionArg.Builder setProjectAssets​(Optional<? extends Path> projectAssets)
            ```

            ::: block
            Initializes the optional value
            [`projectAssets`](AndroidResourceDescriptionArg.html#getProjectAssets())
            to projectAssets.
            :::

            [Parameters:]{.paramLabel}
            :   `projectAssets` - The value for projectAssets

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setHasWhitelistedStrings(boolean)}

        -   #### setHasWhitelistedStrings

            ``` methodSignature
            public final AndroidResourceDescriptionArg.Builder setHasWhitelistedStrings​(boolean hasWhitelistedStrings)
            ```

            ::: block
            Initializes the value for the
            [`hasWhitelistedStrings`](AndroidResourceDescriptionArg.html#getHasWhitelistedStrings())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`hasWhitelistedStrings`](AndroidResourceDescriptionArg.html#getHasWhitelistedStrings()).*
            :::

            [Parameters:]{.paramLabel}
            :   `hasWhitelistedStrings` - The value for
                hasWhitelistedStrings

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPackage(java.lang.String)}

        -   #### setPackage

            ``` methodSignature
            public final AndroidResourceDescriptionArg.Builder setPackage​(String getPackage)
            ```

            ::: block
            Initializes the optional value
            [`package`](AndroidResourceDescriptionArg.html#getPackage())
            to getPackage.
            :::

            [Parameters:]{.paramLabel}
            :   `getPackage` - The value for getPackage

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setPackage(java.util.Optional)}

        -   #### setPackage

            ``` methodSignature
            public final AndroidResourceDescriptionArg.Builder setPackage​(Optional<String> getPackage)
            ```

            ::: block
            Initializes the optional value
            [`package`](AndroidResourceDescriptionArg.html#getPackage())
            to getPackage.
            :::

            [Parameters:]{.paramLabel}
            :   `getPackage` - The value for getPackage

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setManifest(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setManifest

            ``` methodSignature
            public final AndroidResourceDescriptionArg.Builder setManifest​(SourcePath manifest)
            ```

            ::: block
            Initializes the optional value
            [`manifest`](AndroidResourceDescriptionArg.html#getManifest())
            to manifest.
            :::

            [Parameters:]{.paramLabel}
            :   `manifest` - The value for manifest

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setManifest(java.util.Optional)}

        -   #### setManifest

            ``` methodSignature
            public final AndroidResourceDescriptionArg.Builder setManifest​(Optional<? extends SourcePath> manifest)
            ```

            ::: block
            Initializes the optional value
            [`manifest`](AndroidResourceDescriptionArg.html#getManifest())
            to manifest.
            :::

            [Parameters:]{.paramLabel}
            :   `manifest` - The value for manifest

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setResourceUnion(boolean)}

        -   #### setResourceUnion

            ``` methodSignature
            public final AndroidResourceDescriptionArg.Builder setResourceUnion​(boolean resourceUnion)
            ```

            ::: block
            Initializes the value for the
            [`resourceUnion`](AndroidResourceDescriptionArg.html#getResourceUnion())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`resourceUnion`](AndroidResourceDescriptionArg.html#getResourceUnion()).*
            :::

            [Parameters:]{.paramLabel}
            :   `resourceUnion` - The value for resourceUnion

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLicenses(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### addLicenses

            ``` methodSignature
            public final AndroidResourceDescriptionArg.Builder addLicenses​(SourcePath element)
            ```

            ::: block
            Adds one element to
            [`licenses`](AndroidResourceDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A licenses element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLicenses(com.facebook.buck.core.sourcepath.SourcePath...)}

        -   #### addLicenses

            ``` methodSignature
            public final AndroidResourceDescriptionArg.Builder addLicenses​(SourcePath... elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](AndroidResourceDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLicenses(java.lang.Iterable)}

        -   #### setLicenses

            ``` methodSignature
            public final AndroidResourceDescriptionArg.Builder setLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`licenses`](AndroidResourceDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLicenses(java.lang.Iterable)}

        -   #### addAllLicenses

            ``` methodSignature
            public final AndroidResourceDescriptionArg.Builder addAllLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](AndroidResourceDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLabels(java.lang.String)}

        -   #### addLabels

            ``` methodSignature
            public final AndroidResourceDescriptionArg.Builder addLabels​(String element)
            ```

            ::: block
            Adds one element to
            [`labels`](AndroidResourceDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A labels element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLabels(java.lang.String...)}

        -   #### addLabels

            ``` methodSignature
            public final AndroidResourceDescriptionArg.Builder addLabels​(String... elements)
            ```

            ::: block
            Adds elements to
            [`labels`](AndroidResourceDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLabels(java.lang.Iterable)}

        -   #### setLabels

            ``` methodSignature
            public final AndroidResourceDescriptionArg.Builder setLabels​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`labels`](AndroidResourceDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLabels(java.lang.Iterable)}

        -   #### addAllLabels

            ``` methodSignature
            public final AndroidResourceDescriptionArg.Builder addAllLabels​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`labels`](AndroidResourceDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDefaultTargetPlatform(com.facebook.buck.core.model.UnconfiguredBuildTarget)}

        -   #### setDefaultTargetPlatform

            ``` methodSignature
            public final AndroidResourceDescriptionArg.Builder setDefaultTargetPlatform​(UnconfiguredBuildTarget defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](AndroidResourceDescriptionArg.html#getDefaultTargetPlatform())
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
            public final AndroidResourceDescriptionArg.Builder setDefaultTargetPlatform​(Optional<? extends UnconfiguredBuildTarget> defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](AndroidResourceDescriptionArg.html#getDefaultTargetPlatform())
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
            public final AndroidResourceDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget element)
            ```

            ::: block
            Adds one element to
            [`compatibleWith`](AndroidResourceDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A compatibleWith element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCompatibleWith(com.facebook.buck.core.model.UnconfiguredBuildTarget...)}

        -   #### addCompatibleWith

            ``` methodSignature
            public final AndroidResourceDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](AndroidResourceDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCompatibleWith(java.lang.Iterable)}

        -   #### setCompatibleWith

            ``` methodSignature
            public final AndroidResourceDescriptionArg.Builder setCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`compatibleWith`](AndroidResourceDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllCompatibleWith(java.lang.Iterable)}

        -   #### addAllCompatibleWith

            ``` methodSignature
            public final AndroidResourceDescriptionArg.Builder addAllCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](AndroidResourceDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setName(java.lang.String)}

        -   #### setName

            ``` methodSignature
            public final AndroidResourceDescriptionArg.Builder setName​(String name)
            ```

            ::: block
            Initializes the value for the
            [`name`](AndroidResourceDescriptionArg.html#getName())
            attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `name` - The value for name

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addDeps(com.facebook.buck.core.model.BuildTarget)}

        -   #### addDeps

            ``` methodSignature
            public final AndroidResourceDescriptionArg.Builder addDeps​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`deps`](AndroidResourceDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A deps element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addDeps(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addDeps

            ``` methodSignature
            public final AndroidResourceDescriptionArg.Builder addDeps​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`deps`](AndroidResourceDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDeps(java.lang.Iterable)}

        -   #### setDeps

            ``` methodSignature
            public final AndroidResourceDescriptionArg.Builder setDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`deps`](AndroidResourceDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllDeps(java.lang.Iterable)}

        -   #### addAllDeps

            ``` methodSignature
            public final AndroidResourceDescriptionArg.Builder addAllDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`deps`](AndroidResourceDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#build()}

        -   #### build

            ``` methodSignature
            public AndroidResourceDescriptionArg build()
            ```

            ::: block
            Builds a new
            [`AndroidResourceDescriptionArg`](AndroidResourceDescriptionArg.html "class in com.facebook.buck.android").
            :::

            [Returns:]{.returnLabel}
            :   An immutable instance of AndroidResourceDescriptionArg

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
