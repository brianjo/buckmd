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
[Package]{.packageLabelInType} [com.facebook.buck.features.lua](package-summary.html)
:::

## Class LuaBinaryDescriptionArg.Builder {#class-luabinarydescriptionarg.builder .title title="Class LuaBinaryDescriptionArg.Builder"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.features.lua.LuaBinaryDescriptionArg.Builder

::: description
-   

    Enclosing class:
    :   [LuaBinaryDescriptionArg](LuaBinaryDescriptionArg.html "class in com.facebook.buck.features.lua")

    ------------------------------------------------------------------------

        @NotThreadSafe
        public static final class LuaBinaryDescriptionArg.Builder
        extends Object

    ::: block
    Builds instances of type
    [`LuaBinaryDescriptionArg`](LuaBinaryDescriptionArg.html "class in com.facebook.buck.features.lua").
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
        | `LuaBinaryDe          | `addAllCompat         | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Iterable<? e | Adds elements to      |
        |                       | xtends UnconfiguredBu | [`com                 |
        |                       | ildTarget> elements)` | patibleWith`](LuaBina |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `LuaBinaryDe          | `addAllDeps​(          | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Adds elements to      |
        |                       | ildTarget> elements)` | [`deps                |
        |                       |                       | `](LuaBinaryDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `LuaBinaryDe          | `addAllLabels​(Iterab  | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Adds elements to      |
        |                       |                       | [`labels`]            |
        |                       |                       | (LuaBinaryDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `LuaBinaryDe          | `addAllLicenses       | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Adds elements to      |
        |                       | ourcePath> elements)` | [`licenses`](L        |
        |                       |                       | uaBinaryDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `LuaBinaryDe          | `addCompat            | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Unconfigured | Adds one element to   |
        |                       | BuildTarget element)` | [`com                 |
        |                       |                       | patibleWith`](LuaBina |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `LuaBinaryDe          | `addCompatible        | ::: block             |
        | scriptionArg.Builder` | With​(UnconfiguredBuil | Adds elements to      |
        |                       | dTarget... elements)` | [`com                 |
        |                       |                       | patibleWith`](LuaBina |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `LuaBinaryDe          | `addDeps​(             | ::: block             |
        | scriptionArg.Builder` | BuildTarget element)` | Adds one element to   |
        |                       |                       | [`deps                |
        |                       |                       | `](LuaBinaryDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `LuaBinaryDe          | `addDeps​(Buil         | ::: block             |
        | scriptionArg.Builder` | dTarget... elements)` | Adds elements to      |
        |                       |                       | [`deps                |
        |                       |                       | `](LuaBinaryDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `LuaBinaryDe          | `addLa                | ::: block             |
        | scriptionArg.Builder` | bels​(String element)` | Adds one element to   |
        |                       |                       | [`labels`]            |
        |                       |                       | (LuaBinaryDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `LuaBinaryDe          | `addLabels            | ::: block             |
        | scriptionArg.Builder` | ​(String... elements)` | Adds elements to      |
        |                       |                       | [`labels`]            |
        |                       |                       | (LuaBinaryDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `LuaBinaryDe          | `addLicenses          | ::: block             |
        | scriptionArg.Builder` | ​(SourcePath element)` | Adds one element to   |
        |                       |                       | [`licenses`](L        |
        |                       |                       | uaBinaryDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `LuaBinaryDe          | `addLicenses​(Sou      | ::: block             |
        | scriptionArg.Builder` | rcePath... elements)` | Adds elements to      |
        |                       |                       | [`licenses`](L        |
        |                       |                       | uaBinaryDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Lua                  | `build()`             | ::: block             |
        | BinaryDescriptionArg` |                       | Builds a new          |
        |                       |                       | [`LuaBinaryDescr      |
        |                       |                       | iptionArg`](LuaBinary |
        |                       |                       | DescriptionArg.html " |
        |                       |                       | class in com.facebook |
        |                       |                       | .buck.features.lua"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `LuaBinaryDe          | `from​(Bu              | ::: block             |
        | scriptionArg.Builder` | ildRuleArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebo           |
        |                       |                       | ok.buck.core.descript |
        |                       |                       | ion.arg.BuildRuleArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `LuaBinaryDe          | `from​(Cons            | ::: block             |
        | scriptionArg.Builder` | tructorArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook         |
        |                       |                       | .buck.core.descriptio |
        |                       |                       | n.arg.ConstructorArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `LuaBinaryDe          | `from​(HasDe           | ::: block             |
        | scriptionArg.Builder` | claredDeps instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook.        |
        |                       |                       | buck.core.description |
        |                       |                       | .arg.HasDeclaredDeps` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `LuaBinaryDe          | `from​(com.facebo      | ::: block             |
        | scriptionArg.Builder` | ok.buck.features.lua. | Copy abstract value   |
        |                       | LuaBinaryDescription. | type                  |
        |                       | AbstractLuaBinaryDesc | `AbstractLua          |
        |                       | riptionArg instance)` | BinaryDescriptionArg` |
        |                       |                       | instance into         |
        |                       |                       | builder.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `LuaBinaryDe          | `from​(LuaBinaryDesc   | ::: block             |
        | scriptionArg.Builder` | riptionArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `Lua                  |
        |                       |                       | BinaryDescriptionArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `LuaBinaryDe          | `setCompat            | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Iterable<? e | Sets or replaces all  |
        |                       | xtends UnconfiguredBu | elements for          |
        |                       | ildTarget> elements)` | [`com                 |
        |                       |                       | patibleWith`](LuaBina |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `LuaBinaryDe          | `setDefaul            | ::: block             |
        | scriptionArg.Builder` | tTargetPlatform​(Uncon | Initializes the       |
        |                       | figuredBuildTarget de | optional value        |
        |                       | faultTargetPlatform)` | [`defaultTargetPlat   |
        |                       |                       | form`](LuaBinaryDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `LuaBinaryDe          | `setDefau             | ::: block             |
        | scriptionArg.Builder` | ltTargetPlatform​(Opti | Initializes the       |
        |                       | onal<? extends Unconf | optional value        |
        |                       | iguredBuildTarget> de | [`defaultTargetPlat   |
        |                       | faultTargetPlatform)` | form`](LuaBinaryDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `LuaBinaryDe          | `setDeps​(             | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Sets or replaces all  |
        |                       | ildTarget> elements)` | elements for          |
        |                       |                       | [`deps                |
        |                       |                       | `](LuaBinaryDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `LuaBinaryDe          | `setLabels​(Iterab     | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Sets or replaces all  |
        |                       |                       | elements for          |
        |                       |                       | [`labels`]            |
        |                       |                       | (LuaBinaryDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `LuaBinaryDe          | `setLicenses          | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Sets or replaces all  |
        |                       | ourcePath> elements)` | elements for          |
        |                       |                       | [`licenses`](L        |
        |                       |                       | uaBinaryDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `LuaBinaryDe          | `setMainModul         | ::: block             |
        | scriptionArg.Builder` | e​(String mainModule)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`mainModule`](Lua    |
        |                       |                       | BinaryDescriptionArg. |
        |                       |                       | html#getMainModule()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `LuaBinaryDe          | `                     | ::: block             |
        | scriptionArg.Builder` | setName​(String name)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`name                |
        |                       |                       | `](LuaBinaryDescripti |
        |                       |                       | onArg.html#getName()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `LuaBinaryDe          | `setNativeStarter     | ::: block             |
        | scriptionArg.Builder` | Library​(BuildTarget n | Initializes the       |
        |                       | ativeStarterLibrary)` | optional value        |
        |                       |                       | [`nativeStarterLi     |
        |                       |                       | brary`](LuaBinaryDesc |
        |                       |                       | riptionArg.html#getNa |
        |                       |                       | tiveStarterLibrary()) |
        |                       |                       | to                    |
        |                       |                       | nativeStarterLibrary. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `LuaBinaryDe          | `setNativeStarte      | ::: block             |
        | scriptionArg.Builder` | rLibrary​(Optional<? e | Initializes the       |
        |                       | xtends BuildTarget> n | optional value        |
        |                       | ativeStarterLibrary)` | [`nativeStarterLi     |
        |                       |                       | brary`](LuaBinaryDesc |
        |                       |                       | riptionArg.html#getNa |
        |                       |                       | tiveStarterLibrary()) |
        |                       |                       | to                    |
        |                       |                       | nativeStarterLibrary. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `LuaBinaryDe          | `setPackageSty        | ::: block             |
        | scriptionArg.Builder` | le​(LuaPlatform.Packag | Initializes the       |
        |                       | eStyle packageStyle)` | optional value        |
        |                       |                       | [                     |
        |                       |                       | `packageStyle`](LuaBi |
        |                       |                       | naryDescriptionArg.ht |
        |                       |                       | ml#getPackageStyle()) |
        |                       |                       | to packageStyle.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `LuaBinaryDe          | `setPackageSt         | ::: block             |
        | scriptionArg.Builder` | yle​(Optional<? extend | Initializes the       |
        |                       | s LuaPlatform.Package | optional value        |
        |                       | Style> packageStyle)` | [                     |
        |                       |                       | `packageStyle`](LuaBi |
        |                       |                       | naryDescriptionArg.ht |
        |                       |                       | ml#getPackageStyle()) |
        |                       |                       | to packageStyle.      |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `LuaBinaryDe          | `setPlatf             | ::: block             |
        | scriptionArg.Builder` | orm​(Flavor platform)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`platform`](L        |
        |                       |                       | uaBinaryDescriptionAr |
        |                       |                       | g.html#getPlatform()) |
        |                       |                       | to platform.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `LuaBinaryDe          | `setPlat              | ::: block             |
        | scriptionArg.Builder` | form​(Optional<? exten | Initializes the       |
        |                       | ds Flavor> platform)` | optional value        |
        |                       |                       | [`platform`](L        |
        |                       |                       | uaBinaryDescriptionAr |
        |                       |                       | g.html#getPlatform()) |
        |                       |                       | to platform.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `LuaBinaryDe          | `setPlatfo            | ::: block             |
        | scriptionArg.Builder` | rmDeps​(PatternMatched | Initializes the value |
        |                       | Collection<com.google | for the               |
        |                       | .common.collect.Immut | [                     |
        |                       | ableSortedSet<BuildTa | `platformDeps`](LuaBi |
        |                       | rget>> platformDeps)` | naryDescriptionArg.ht |
        |                       |                       | ml#getPlatformDeps()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `LuaBinaryDe          | `setPythonPlatform​(St | ::: block             |
        | scriptionArg.Builder` | ring pythonPlatform)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`pyt                 |
        |                       |                       | honPlatform`](LuaBina |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getPythonPlatform()) |
        |                       |                       | to pythonPlatform.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `LuaBinaryDe          | `setPython            | ::: block             |
        | scriptionArg.Builder` | Platform​(Optional<Str | Initializes the       |
        |                       | ing> pythonPlatform)` | optional value        |
        |                       |                       | [`pyt                 |
        |                       |                       | honPlatform`](LuaBina |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getPythonPlatform()) |
        |                       |                       | to pythonPlatform.    |
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
            public final LuaBinaryDescriptionArg.Builder from​(HasDeclaredDeps instance)
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
            public final LuaBinaryDescriptionArg.Builder from​(BuildRuleArg instance)
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
            public final LuaBinaryDescriptionArg.Builder from​(ConstructorArg instance)
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

        []{#from(com.facebook.buck.features.lua.LuaBinaryDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final LuaBinaryDescriptionArg.Builder from​(LuaBinaryDescriptionArg instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `LuaBinaryDescriptionArg` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.features.lua.LuaBinaryDescription.AbstractLuaBinaryDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final LuaBinaryDescriptionArg.Builder from​(com.facebook.buck.features.lua.LuaBinaryDescription.AbstractLuaBinaryDescriptionArg instance)
            ```

            ::: block
            Copy abstract value type `AbstractLuaBinaryDescriptionArg`
            instance into builder.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setMainModule(java.lang.String)}

        -   #### setMainModule

            ``` methodSignature
            public final LuaBinaryDescriptionArg.Builder setMainModule​(String mainModule)
            ```

            ::: block
            Initializes the value for the
            [`mainModule`](LuaBinaryDescriptionArg.html#getMainModule())
            attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `mainModule` - The value for mainModule

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setNativeStarterLibrary(com.facebook.buck.core.model.BuildTarget)}

        -   #### setNativeStarterLibrary

            ``` methodSignature
            public final LuaBinaryDescriptionArg.Builder setNativeStarterLibrary​(BuildTarget nativeStarterLibrary)
            ```

            ::: block
            Initializes the optional value
            [`nativeStarterLibrary`](LuaBinaryDescriptionArg.html#getNativeStarterLibrary())
            to nativeStarterLibrary.
            :::

            [Parameters:]{.paramLabel}
            :   `nativeStarterLibrary` - The value for
                nativeStarterLibrary

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setNativeStarterLibrary(java.util.Optional)}

        -   #### setNativeStarterLibrary

            ``` methodSignature
            public final LuaBinaryDescriptionArg.Builder setNativeStarterLibrary​(Optional<? extends BuildTarget> nativeStarterLibrary)
            ```

            ::: block
            Initializes the optional value
            [`nativeStarterLibrary`](LuaBinaryDescriptionArg.html#getNativeStarterLibrary())
            to nativeStarterLibrary.
            :::

            [Parameters:]{.paramLabel}
            :   `nativeStarterLibrary` - The value for
                nativeStarterLibrary

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPythonPlatform(java.lang.String)}

        -   #### setPythonPlatform

            ``` methodSignature
            public final LuaBinaryDescriptionArg.Builder setPythonPlatform​(String pythonPlatform)
            ```

            ::: block
            Initializes the optional value
            [`pythonPlatform`](LuaBinaryDescriptionArg.html#getPythonPlatform())
            to pythonPlatform.
            :::

            [Parameters:]{.paramLabel}
            :   `pythonPlatform` - The value for pythonPlatform

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setPythonPlatform(java.util.Optional)}

        -   #### setPythonPlatform

            ``` methodSignature
            public final LuaBinaryDescriptionArg.Builder setPythonPlatform​(Optional<String> pythonPlatform)
            ```

            ::: block
            Initializes the optional value
            [`pythonPlatform`](LuaBinaryDescriptionArg.html#getPythonPlatform())
            to pythonPlatform.
            :::

            [Parameters:]{.paramLabel}
            :   `pythonPlatform` - The value for pythonPlatform

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPlatform(com.facebook.buck.core.model.Flavor)}

        -   #### setPlatform

            ``` methodSignature
            public final LuaBinaryDescriptionArg.Builder setPlatform​(Flavor platform)
            ```

            ::: block
            Initializes the optional value
            [`platform`](LuaBinaryDescriptionArg.html#getPlatform()) to
            platform.
            :::

            [Parameters:]{.paramLabel}
            :   `platform` - The value for platform

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setPlatform(java.util.Optional)}

        -   #### setPlatform

            ``` methodSignature
            public final LuaBinaryDescriptionArg.Builder setPlatform​(Optional<? extends Flavor> platform)
            ```

            ::: block
            Initializes the optional value
            [`platform`](LuaBinaryDescriptionArg.html#getPlatform()) to
            platform.
            :::

            [Parameters:]{.paramLabel}
            :   `platform` - The value for platform

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPackageStyle(com.facebook.buck.features.lua.LuaPlatform.PackageStyle)}

        -   #### setPackageStyle

            ``` methodSignature
            public final LuaBinaryDescriptionArg.Builder setPackageStyle​(LuaPlatform.PackageStyle packageStyle)
            ```

            ::: block
            Initializes the optional value
            [`packageStyle`](LuaBinaryDescriptionArg.html#getPackageStyle())
            to packageStyle.
            :::

            [Parameters:]{.paramLabel}
            :   `packageStyle` - The value for packageStyle

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setPackageStyle(java.util.Optional)}

        -   #### setPackageStyle

            ``` methodSignature
            public final LuaBinaryDescriptionArg.Builder setPackageStyle​(Optional<? extends LuaPlatform.PackageStyle> packageStyle)
            ```

            ::: block
            Initializes the optional value
            [`packageStyle`](LuaBinaryDescriptionArg.html#getPackageStyle())
            to packageStyle.
            :::

            [Parameters:]{.paramLabel}
            :   `packageStyle` - The value for packageStyle

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPlatformDeps(com.facebook.buck.rules.coercer.PatternMatchedCollection)}

        -   #### setPlatformDeps

            ``` methodSignature
            public final LuaBinaryDescriptionArg.Builder setPlatformDeps​(PatternMatchedCollection<com.google.common.collect.ImmutableSortedSet<BuildTarget>> platformDeps)
            ```

            ::: block
            Initializes the value for the
            [`platformDeps`](LuaBinaryDescriptionArg.html#getPlatformDeps())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`platformDeps`](LuaBinaryDescriptionArg.html#getPlatformDeps()).*
            :::

            [Parameters:]{.paramLabel}
            :   `platformDeps` - The value for platformDeps

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCompatibleWith(com.facebook.buck.core.model.UnconfiguredBuildTarget)}

        -   #### addCompatibleWith

            ``` methodSignature
            public final LuaBinaryDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget element)
            ```

            ::: block
            Adds one element to
            [`compatibleWith`](LuaBinaryDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A compatibleWith element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCompatibleWith(com.facebook.buck.core.model.UnconfiguredBuildTarget...)}

        -   #### addCompatibleWith

            ``` methodSignature
            public final LuaBinaryDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](LuaBinaryDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCompatibleWith(java.lang.Iterable)}

        -   #### setCompatibleWith

            ``` methodSignature
            public final LuaBinaryDescriptionArg.Builder setCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`compatibleWith`](LuaBinaryDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllCompatibleWith(java.lang.Iterable)}

        -   #### addAllCompatibleWith

            ``` methodSignature
            public final LuaBinaryDescriptionArg.Builder addAllCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](LuaBinaryDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDefaultTargetPlatform(com.facebook.buck.core.model.UnconfiguredBuildTarget)}

        -   #### setDefaultTargetPlatform

            ``` methodSignature
            public final LuaBinaryDescriptionArg.Builder setDefaultTargetPlatform​(UnconfiguredBuildTarget defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](LuaBinaryDescriptionArg.html#getDefaultTargetPlatform())
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
            public final LuaBinaryDescriptionArg.Builder setDefaultTargetPlatform​(Optional<? extends UnconfiguredBuildTarget> defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](LuaBinaryDescriptionArg.html#getDefaultTargetPlatform())
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
            public final LuaBinaryDescriptionArg.Builder addLabels​(String element)
            ```

            ::: block
            Adds one element to
            [`labels`](LuaBinaryDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A labels element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLabels(java.lang.String...)}

        -   #### addLabels

            ``` methodSignature
            public final LuaBinaryDescriptionArg.Builder addLabels​(String... elements)
            ```

            ::: block
            Adds elements to
            [`labels`](LuaBinaryDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLabels(java.lang.Iterable)}

        -   #### setLabels

            ``` methodSignature
            public final LuaBinaryDescriptionArg.Builder setLabels​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`labels`](LuaBinaryDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLabels(java.lang.Iterable)}

        -   #### addAllLabels

            ``` methodSignature
            public final LuaBinaryDescriptionArg.Builder addAllLabels​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`labels`](LuaBinaryDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLicenses(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### addLicenses

            ``` methodSignature
            public final LuaBinaryDescriptionArg.Builder addLicenses​(SourcePath element)
            ```

            ::: block
            Adds one element to
            [`licenses`](LuaBinaryDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A licenses element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLicenses(com.facebook.buck.core.sourcepath.SourcePath...)}

        -   #### addLicenses

            ``` methodSignature
            public final LuaBinaryDescriptionArg.Builder addLicenses​(SourcePath... elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](LuaBinaryDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLicenses(java.lang.Iterable)}

        -   #### setLicenses

            ``` methodSignature
            public final LuaBinaryDescriptionArg.Builder setLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`licenses`](LuaBinaryDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLicenses(java.lang.Iterable)}

        -   #### addAllLicenses

            ``` methodSignature
            public final LuaBinaryDescriptionArg.Builder addAllLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](LuaBinaryDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setName(java.lang.String)}

        -   #### setName

            ``` methodSignature
            public final LuaBinaryDescriptionArg.Builder setName​(String name)
            ```

            ::: block
            Initializes the value for the
            [`name`](LuaBinaryDescriptionArg.html#getName()) attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `name` - The value for name

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addDeps(com.facebook.buck.core.model.BuildTarget)}

        -   #### addDeps

            ``` methodSignature
            public final LuaBinaryDescriptionArg.Builder addDeps​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`deps`](LuaBinaryDescriptionArg.html#getDeps()) sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A deps element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addDeps(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addDeps

            ``` methodSignature
            public final LuaBinaryDescriptionArg.Builder addDeps​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`deps`](LuaBinaryDescriptionArg.html#getDeps()) sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDeps(java.lang.Iterable)}

        -   #### setDeps

            ``` methodSignature
            public final LuaBinaryDescriptionArg.Builder setDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`deps`](LuaBinaryDescriptionArg.html#getDeps()) sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllDeps(java.lang.Iterable)}

        -   #### addAllDeps

            ``` methodSignature
            public final LuaBinaryDescriptionArg.Builder addAllDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`deps`](LuaBinaryDescriptionArg.html#getDeps()) sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#build()}

        -   #### build

            ``` methodSignature
            public LuaBinaryDescriptionArg build()
            ```

            ::: block
            Builds a new
            [`LuaBinaryDescriptionArg`](LuaBinaryDescriptionArg.html "class in com.facebook.buck.features.lua").
            :::

            [Returns:]{.returnLabel}
            :   An immutable instance of LuaBinaryDescriptionArg

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
