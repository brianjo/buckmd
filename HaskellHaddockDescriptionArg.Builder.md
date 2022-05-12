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
[Package]{.packageLabelInType} [com.facebook.buck.features.haskell](package-summary.html)
:::

## Class HaskellHaddockDescriptionArg.Builder {#class-haskellhaddockdescriptionarg.builder .title title="Class HaskellHaddockDescriptionArg.Builder"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.features.haskell.HaskellHaddockDescriptionArg.Builder

::: description
-   

    Enclosing class:
    :   [HaskellHaddockDescriptionArg](HaskellHaddockDescriptionArg.html "class in com.facebook.buck.features.haskell")

    ------------------------------------------------------------------------

        @NotThreadSafe
        public static final class HaskellHaddockDescriptionArg.Builder
        extends Object

    ::: block
    Builds instances of type
    [`HaskellHaddockDescriptionArg`](HaskellHaddockDescriptionArg.html "class in com.facebook.buck.features.haskell").
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
        | `HaskellHaddockDe     | `addAllCompat         | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Iterable<? e | Adds elements to      |
        |                       | xtends UnconfiguredBu | [`compatib            |
        |                       | ildTarget> elements)` | leWith`](HaskellHaddo |
        |                       |                       | ckDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellHaddockDe     | `addAllDeps​(          | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Adds elements to      |
        |                       | ildTarget> elements)` | [`deps`](Ha           |
        |                       |                       | skellHaddockDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellHaddockDe     | `addA                 | ::: block             |
        | scriptionArg.Builder` | llHaddockFlags​(Iterab | Adds elements to      |
        |                       | le<String> elements)` | [`hadd                |
        |                       |                       | ockFlags`](HaskellHad |
        |                       |                       | dockDescriptionArg.ht |
        |                       |                       | ml#getHaddockFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellHaddockDe     | `addAllLabels​(Iterab  | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Adds elements to      |
        |                       |                       | [`labels`](Hask       |
        |                       |                       | ellHaddockDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellHaddockDe     | `addAllLicenses       | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Adds elements to      |
        |                       | ourcePath> elements)` | [`licenses`](Haskel   |
        |                       |                       | lHaddockDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellHaddockDe     | `addCompat            | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Unconfigured | Adds one element to   |
        |                       | BuildTarget element)` | [`compatib            |
        |                       |                       | leWith`](HaskellHaddo |
        |                       |                       | ckDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellHaddockDe     | `addCompatible        | ::: block             |
        | scriptionArg.Builder` | With​(UnconfiguredBuil | Adds elements to      |
        |                       | dTarget... elements)` | [`compatib            |
        |                       |                       | leWith`](HaskellHaddo |
        |                       |                       | ckDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellHaddockDe     | `addDeps​(             | ::: block             |
        | scriptionArg.Builder` | BuildTarget element)` | Adds one element to   |
        |                       |                       | [`deps`](Ha           |
        |                       |                       | skellHaddockDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellHaddockDe     | `addDeps​(Buil         | ::: block             |
        | scriptionArg.Builder` | dTarget... elements)` | Adds elements to      |
        |                       |                       | [`deps`](Ha           |
        |                       |                       | skellHaddockDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellHaddockDe     | `addHaddockF          | ::: block             |
        | scriptionArg.Builder` | lags​(String element)` | Adds one element to   |
        |                       |                       | [`hadd                |
        |                       |                       | ockFlags`](HaskellHad |
        |                       |                       | dockDescriptionArg.ht |
        |                       |                       | ml#getHaddockFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellHaddockDe     | `addHaddockFlags      | ::: block             |
        | scriptionArg.Builder` | ​(String... elements)` | Adds elements to      |
        |                       |                       | [`hadd                |
        |                       |                       | ockFlags`](HaskellHad |
        |                       |                       | dockDescriptionArg.ht |
        |                       |                       | ml#getHaddockFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellHaddockDe     | `addLa                | ::: block             |
        | scriptionArg.Builder` | bels​(String element)` | Adds one element to   |
        |                       |                       | [`labels`](Hask       |
        |                       |                       | ellHaddockDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellHaddockDe     | `addLabels            | ::: block             |
        | scriptionArg.Builder` | ​(String... elements)` | Adds elements to      |
        |                       |                       | [`labels`](Hask       |
        |                       |                       | ellHaddockDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellHaddockDe     | `addLicenses          | ::: block             |
        | scriptionArg.Builder` | ​(SourcePath element)` | Adds one element to   |
        |                       |                       | [`licenses`](Haskel   |
        |                       |                       | lHaddockDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellHaddockDe     | `addLicenses​(Sou      | ::: block             |
        | scriptionArg.Builder` | rcePath... elements)` | Adds elements to      |
        |                       |                       | [`licenses`](Haskel   |
        |                       |                       | lHaddockDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellH             | `build()`             | ::: block             |
        | addockDescriptionArg` |                       | Builds a new          |
        |                       |                       | [`Haskell             |
        |                       |                       | HaddockDescriptionArg |
        |                       |                       | `](HaskellHaddockDesc |
        |                       |                       | riptionArg.html "clas |
        |                       |                       | s in com.facebook.buc |
        |                       |                       | k.features.haskell"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellHaddockDe     | `from​(Bu              | ::: block             |
        | scriptionArg.Builder` | ildRuleArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebo           |
        |                       |                       | ok.buck.core.descript |
        |                       |                       | ion.arg.BuildRuleArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellHaddockDe     | `from​(Cons            | ::: block             |
        | scriptionArg.Builder` | tructorArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook         |
        |                       |                       | .buck.core.descriptio |
        |                       |                       | n.arg.ConstructorArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellHaddockDe     | `from​(HasDe           | ::: block             |
        | scriptionArg.Builder` | claredDeps instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook.        |
        |                       |                       | buck.core.description |
        |                       |                       | .arg.HasDeclaredDeps` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellHaddockDe     | `from​(Ha              | ::: block             |
        | scriptionArg.Builder` | sDepsQuery instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebo           |
        |                       |                       | ok.buck.core.descript |
        |                       |                       | ion.arg.HasDepsQuery` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellHaddockDe     | `from​(com             | ::: block             |
        | scriptionArg.Builder` | .facebook.buck.featur | Copy abstract value   |
        |                       | es.haskell.HaskellHad | type                  |
        |                       | dockDescription.Abstr | `AbstractHaskellH     |
        |                       | actHaskellHaddockDesc | addockDescriptionArg` |
        |                       | riptionArg instance)` | instance into         |
        |                       |                       | builder.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellHaddockDe     | `fr                   | ::: block             |
        | scriptionArg.Builder` | om​(HaskellHaddockDesc | Fill a builder with   |
        |                       | riptionArg instance)` | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `HaskellH             |
        |                       |                       | addockDescriptionArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellHaddockDe     | `setCompat            | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Iterable<? e | Sets or replaces all  |
        |                       | xtends UnconfiguredBu | elements for          |
        |                       | ildTarget> elements)` | [`compatib            |
        |                       |                       | leWith`](HaskellHaddo |
        |                       |                       | ckDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellHaddockDe     | `setDefaul            | ::: block             |
        | scriptionArg.Builder` | tTargetPlatform​(Uncon | Initializes the       |
        |                       | figuredBuildTarget de | optional value        |
        |                       | faultTargetPlatform)` | [`d                   |
        |                       |                       | efaultTargetPlatform` |
        |                       |                       | ](HaskellHaddockDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellHaddockDe     | `setDefau             | ::: block             |
        | scriptionArg.Builder` | ltTargetPlatform​(Opti | Initializes the       |
        |                       | onal<? extends Unconf | optional value        |
        |                       | iguredBuildTarget> de | [`d                   |
        |                       | faultTargetPlatform)` | efaultTargetPlatform` |
        |                       |                       | ](HaskellHaddockDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellHaddockDe     | `setDeps​(             | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Sets or replaces all  |
        |                       | ildTarget> elements)` | elements for          |
        |                       |                       | [`deps`](Ha           |
        |                       |                       | skellHaddockDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellHaddockDe     | `setDepsQu            | ::: block             |
        | scriptionArg.Builder` | ery​(Query depsQuery)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`depsQuery`](Haskell |
        |                       |                       | HaddockDescriptionArg |
        |                       |                       | .html#getDepsQuery()) |
        |                       |                       | to depsQuery.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellHaddockDe     | `setDepsQ             | ::: block             |
        | scriptionArg.Builder` | uery​(Optional<? exten | Initializes the       |
        |                       | ds Query> depsQuery)` | optional value        |
        |                       |                       | [`depsQuery`](Haskell |
        |                       |                       | HaddockDescriptionArg |
        |                       |                       | .html#getDepsQuery()) |
        |                       |                       | to depsQuery.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellHaddockDe     | `s                    | ::: block             |
        | scriptionArg.Builder` | etHaddockFlags​(Iterab | Sets or replaces all  |
        |                       | le<String> elements)` | elements for          |
        |                       |                       | [`hadd                |
        |                       |                       | ockFlags`](HaskellHad |
        |                       |                       | dockDescriptionArg.ht |
        |                       |                       | ml#getHaddockFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellHaddockDe     | `setLabels​(Iterab     | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Sets or replaces all  |
        |                       |                       | elements for          |
        |                       |                       | [`labels`](Hask       |
        |                       |                       | ellHaddockDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellHaddockDe     | `setLicenses          | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Sets or replaces all  |
        |                       | ourcePath> elements)` | elements for          |
        |                       |                       | [`licenses`](Haskel   |
        |                       |                       | lHaddockDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellHaddockDe     | `                     | ::: block             |
        | scriptionArg.Builder` | setName​(String name)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`name`](Ha           |
        |                       |                       | skellHaddockDescripti |
        |                       |                       | onArg.html#getName()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellHaddockDe     | `setPlatf             | ::: block             |
        | scriptionArg.Builder` | orm​(Flavor platform)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`platform`](Haskel   |
        |                       |                       | lHaddockDescriptionAr |
        |                       |                       | g.html#getPlatform()) |
        |                       |                       | to platform.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `HaskellHaddockDe     | `setPlat              | ::: block             |
        | scriptionArg.Builder` | form​(Optional<? exten | Initializes the       |
        |                       | ds Flavor> platform)` | optional value        |
        |                       |                       | [`platform`](Haskel   |
        |                       |                       | lHaddockDescriptionAr |
        |                       |                       | g.html#getPlatform()) |
        |                       |                       | to platform.          |
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

        []{#from(com.facebook.buck.features.haskell.HaskellHaddockDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final HaskellHaddockDescriptionArg.Builder from​(HaskellHaddockDescriptionArg instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `HaskellHaddockDescriptionArg` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.features.haskell.HaskellHaddockDescription.AbstractHaskellHaddockDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final HaskellHaddockDescriptionArg.Builder from​(com.facebook.buck.features.haskell.HaskellHaddockDescription.AbstractHaskellHaddockDescriptionArg instance)
            ```

            ::: block
            Copy abstract value type
            `AbstractHaskellHaddockDescriptionArg` instance into
            builder.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.core.description.arg.HasDeclaredDeps)}

        -   #### from

            ``` methodSignature
            public final HaskellHaddockDescriptionArg.Builder from​(HasDeclaredDeps instance)
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

        []{#from(com.facebook.buck.core.description.arg.HasDepsQuery)}

        -   #### from

            ``` methodSignature
            public final HaskellHaddockDescriptionArg.Builder from​(HasDepsQuery instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `com.facebook.buck.core.description.arg.HasDepsQuery`
            instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.core.description.arg.BuildRuleArg)}

        -   #### from

            ``` methodSignature
            public final HaskellHaddockDescriptionArg.Builder from​(BuildRuleArg instance)
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
            public final HaskellHaddockDescriptionArg.Builder from​(ConstructorArg instance)
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

        []{#setPlatform(com.facebook.buck.core.model.Flavor)}

        -   #### setPlatform

            ``` methodSignature
            public final HaskellHaddockDescriptionArg.Builder setPlatform​(Flavor platform)
            ```

            ::: block
            Initializes the optional value
            [`platform`](HaskellHaddockDescriptionArg.html#getPlatform())
            to platform.
            :::

            [Parameters:]{.paramLabel}
            :   `platform` - The value for platform

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setPlatform(java.util.Optional)}

        -   #### setPlatform

            ``` methodSignature
            public final HaskellHaddockDescriptionArg.Builder setPlatform​(Optional<? extends Flavor> platform)
            ```

            ::: block
            Initializes the optional value
            [`platform`](HaskellHaddockDescriptionArg.html#getPlatform())
            to platform.
            :::

            [Parameters:]{.paramLabel}
            :   `platform` - The value for platform

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addHaddockFlags(java.lang.String)}

        -   #### addHaddockFlags

            ``` methodSignature
            public final HaskellHaddockDescriptionArg.Builder addHaddockFlags​(String element)
            ```

            ::: block
            Adds one element to
            [`haddockFlags`](HaskellHaddockDescriptionArg.html#getHaddockFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A haddockFlags element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addHaddockFlags(java.lang.String...)}

        -   #### addHaddockFlags

            ``` methodSignature
            public final HaskellHaddockDescriptionArg.Builder addHaddockFlags​(String... elements)
            ```

            ::: block
            Adds elements to
            [`haddockFlags`](HaskellHaddockDescriptionArg.html#getHaddockFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of haddockFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setHaddockFlags(java.lang.Iterable)}

        -   #### setHaddockFlags

            ``` methodSignature
            public final HaskellHaddockDescriptionArg.Builder setHaddockFlags​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`haddockFlags`](HaskellHaddockDescriptionArg.html#getHaddockFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of haddockFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllHaddockFlags(java.lang.Iterable)}

        -   #### addAllHaddockFlags

            ``` methodSignature
            public final HaskellHaddockDescriptionArg.Builder addAllHaddockFlags​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`haddockFlags`](HaskellHaddockDescriptionArg.html#getHaddockFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of haddockFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCompatibleWith(com.facebook.buck.core.model.UnconfiguredBuildTarget)}

        -   #### addCompatibleWith

            ``` methodSignature
            public final HaskellHaddockDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget element)
            ```

            ::: block
            Adds one element to
            [`compatibleWith`](HaskellHaddockDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A compatibleWith element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCompatibleWith(com.facebook.buck.core.model.UnconfiguredBuildTarget...)}

        -   #### addCompatibleWith

            ``` methodSignature
            public final HaskellHaddockDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](HaskellHaddockDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCompatibleWith(java.lang.Iterable)}

        -   #### setCompatibleWith

            ``` methodSignature
            public final HaskellHaddockDescriptionArg.Builder setCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`compatibleWith`](HaskellHaddockDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllCompatibleWith(java.lang.Iterable)}

        -   #### addAllCompatibleWith

            ``` methodSignature
            public final HaskellHaddockDescriptionArg.Builder addAllCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](HaskellHaddockDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDefaultTargetPlatform(com.facebook.buck.core.model.UnconfiguredBuildTarget)}

        -   #### setDefaultTargetPlatform

            ``` methodSignature
            public final HaskellHaddockDescriptionArg.Builder setDefaultTargetPlatform​(UnconfiguredBuildTarget defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](HaskellHaddockDescriptionArg.html#getDefaultTargetPlatform())
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
            public final HaskellHaddockDescriptionArg.Builder setDefaultTargetPlatform​(Optional<? extends UnconfiguredBuildTarget> defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](HaskellHaddockDescriptionArg.html#getDefaultTargetPlatform())
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
            public final HaskellHaddockDescriptionArg.Builder addLabels​(String element)
            ```

            ::: block
            Adds one element to
            [`labels`](HaskellHaddockDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A labels element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLabels(java.lang.String...)}

        -   #### addLabels

            ``` methodSignature
            public final HaskellHaddockDescriptionArg.Builder addLabels​(String... elements)
            ```

            ::: block
            Adds elements to
            [`labels`](HaskellHaddockDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLabels(java.lang.Iterable)}

        -   #### setLabels

            ``` methodSignature
            public final HaskellHaddockDescriptionArg.Builder setLabels​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`labels`](HaskellHaddockDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLabels(java.lang.Iterable)}

        -   #### addAllLabels

            ``` methodSignature
            public final HaskellHaddockDescriptionArg.Builder addAllLabels​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`labels`](HaskellHaddockDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLicenses(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### addLicenses

            ``` methodSignature
            public final HaskellHaddockDescriptionArg.Builder addLicenses​(SourcePath element)
            ```

            ::: block
            Adds one element to
            [`licenses`](HaskellHaddockDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A licenses element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLicenses(com.facebook.buck.core.sourcepath.SourcePath...)}

        -   #### addLicenses

            ``` methodSignature
            public final HaskellHaddockDescriptionArg.Builder addLicenses​(SourcePath... elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](HaskellHaddockDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLicenses(java.lang.Iterable)}

        -   #### setLicenses

            ``` methodSignature
            public final HaskellHaddockDescriptionArg.Builder setLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`licenses`](HaskellHaddockDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLicenses(java.lang.Iterable)}

        -   #### addAllLicenses

            ``` methodSignature
            public final HaskellHaddockDescriptionArg.Builder addAllLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](HaskellHaddockDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setName(java.lang.String)}

        -   #### setName

            ``` methodSignature
            public final HaskellHaddockDescriptionArg.Builder setName​(String name)
            ```

            ::: block
            Initializes the value for the
            [`name`](HaskellHaddockDescriptionArg.html#getName())
            attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `name` - The value for name

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDepsQuery(com.facebook.buck.rules.query.Query)}

        -   #### setDepsQuery

            ``` methodSignature
            public final HaskellHaddockDescriptionArg.Builder setDepsQuery​(Query depsQuery)
            ```

            ::: block
            Initializes the optional value
            [`depsQuery`](HaskellHaddockDescriptionArg.html#getDepsQuery())
            to depsQuery.
            :::

            [Parameters:]{.paramLabel}
            :   `depsQuery` - The value for depsQuery

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setDepsQuery(java.util.Optional)}

        -   #### setDepsQuery

            ``` methodSignature
            public final HaskellHaddockDescriptionArg.Builder setDepsQuery​(Optional<? extends Query> depsQuery)
            ```

            ::: block
            Initializes the optional value
            [`depsQuery`](HaskellHaddockDescriptionArg.html#getDepsQuery())
            to depsQuery.
            :::

            [Parameters:]{.paramLabel}
            :   `depsQuery` - The value for depsQuery

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addDeps(com.facebook.buck.core.model.BuildTarget)}

        -   #### addDeps

            ``` methodSignature
            public final HaskellHaddockDescriptionArg.Builder addDeps​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`deps`](HaskellHaddockDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A deps element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addDeps(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addDeps

            ``` methodSignature
            public final HaskellHaddockDescriptionArg.Builder addDeps​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`deps`](HaskellHaddockDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDeps(java.lang.Iterable)}

        -   #### setDeps

            ``` methodSignature
            public final HaskellHaddockDescriptionArg.Builder setDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`deps`](HaskellHaddockDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllDeps(java.lang.Iterable)}

        -   #### addAllDeps

            ``` methodSignature
            public final HaskellHaddockDescriptionArg.Builder addAllDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`deps`](HaskellHaddockDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#build()}

        -   #### build

            ``` methodSignature
            public HaskellHaddockDescriptionArg build()
            ```

            ::: block
            Builds a new
            [`HaskellHaddockDescriptionArg`](HaskellHaddockDescriptionArg.html "class in com.facebook.buck.features.haskell").
            :::

            [Returns:]{.returnLabel}
            :   An immutable instance of HaskellHaddockDescriptionArg

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
