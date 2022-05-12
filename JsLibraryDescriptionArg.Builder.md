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

## Class JsLibraryDescriptionArg.Builder {#class-jslibrarydescriptionarg.builder .title title="Class JsLibraryDescriptionArg.Builder"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.features.js.JsLibraryDescriptionArg.Builder

::: description
-   

    Enclosing class:
    :   [JsLibraryDescriptionArg](JsLibraryDescriptionArg.html "class in com.facebook.buck.features.js")

    ------------------------------------------------------------------------

        @NotThreadSafe
        public static final class JsLibraryDescriptionArg.Builder
        extends Object

    ::: block
    Builds instances of type
    [`JsLibraryDescriptionArg`](JsLibraryDescriptionArg.html "class in com.facebook.buck.features.js").
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
        | `JsLibraryDe          | `addAllCompat         | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Iterable<? e | Adds elements to      |
        |                       | xtends UnconfiguredBu | [`com                 |
        |                       | ildTarget> elements)` | patibleWith`](JsLibra |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsLibraryDe          | `addAllDeps​(          | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Adds elements to      |
        |                       | ildTarget> elements)` | [`deps                |
        |                       |                       | `](JsLibraryDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsLibraryDe          | `addAllLabels​(Iterab  | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Adds elements to      |
        |                       |                       | [`labels`]            |
        |                       |                       | (JsLibraryDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsLibraryDe          | `addAllLicenses       | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Adds elements to      |
        |                       | ourcePath> elements)` | [`licenses`](J        |
        |                       |                       | sLibraryDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsLibraryDe          | `                     | ::: block             |
        | scriptionArg.Builder` | addAllSrcs​(Iterable<? | Adds elements to      |
        |                       |  extends Either<Sourc | [`srcs                |
        |                       | ePath,​Pair<SourcePath | `](JsLibraryDescripti |
        |                       | ,​String>>> elements)` | onArg.html#getSrcs()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsLibraryDe          | `addAllTests​(         | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Adds elements to      |
        |                       | ildTarget> elements)` | [`tests`              |
        |                       |                       | ](JsLibraryDescriptio |
        |                       |                       | nArg.html#getTests()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsLibraryDe          | `addCompat            | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Unconfigured | Adds one element to   |
        |                       | BuildTarget element)` | [`com                 |
        |                       |                       | patibleWith`](JsLibra |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsLibraryDe          | `addCompatible        | ::: block             |
        | scriptionArg.Builder` | With​(UnconfiguredBuil | Adds elements to      |
        |                       | dTarget... elements)` | [`com                 |
        |                       |                       | patibleWith`](JsLibra |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsLibraryDe          | `addDeps​(             | ::: block             |
        | scriptionArg.Builder` | BuildTarget element)` | Adds one element to   |
        |                       |                       | [`deps                |
        |                       |                       | `](JsLibraryDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsLibraryDe          | `addDeps​(Buil         | ::: block             |
        | scriptionArg.Builder` | dTarget... elements)` | Adds elements to      |
        |                       |                       | [`deps                |
        |                       |                       | `](JsLibraryDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsLibraryDe          | `addLa                | ::: block             |
        | scriptionArg.Builder` | bels​(String element)` | Adds one element to   |
        |                       |                       | [`labels`]            |
        |                       |                       | (JsLibraryDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsLibraryDe          | `addLabels            | ::: block             |
        | scriptionArg.Builder` | ​(String... elements)` | Adds elements to      |
        |                       |                       | [`labels`]            |
        |                       |                       | (JsLibraryDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsLibraryDe          | `addLicenses          | ::: block             |
        | scriptionArg.Builder` | ​(SourcePath element)` | Adds one element to   |
        |                       |                       | [`licenses`](J        |
        |                       |                       | sLibraryDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsLibraryDe          | `addLicenses​(Sou      | ::: block             |
        | scriptionArg.Builder` | rcePath... elements)` | Adds elements to      |
        |                       |                       | [`licenses`](J        |
        |                       |                       | sLibraryDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsLibraryDe          | `addSrcs​(Either<Sou   | ::: block             |
        | scriptionArg.Builder` | rcePath,​Pair<SourcePa | Adds one element to   |
        |                       | th,​String>> element)` | [`srcs                |
        |                       |                       | `](JsLibraryDescripti |
        |                       |                       | onArg.html#getSrcs()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsLibraryDe          | `a                    | ::: block             |
        | scriptionArg.Builder` | ddSrcs​(Either<SourceP | Adds elements to      |
        |                       | ath,​Pair<SourcePath,​S | [`srcs                |
        |                       | tring>>... elements)` | `](JsLibraryDescripti |
        |                       |                       | onArg.html#getSrcs()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsLibraryDe          | `addTests​(            | ::: block             |
        | scriptionArg.Builder` | BuildTarget element)` | Adds one element to   |
        |                       |                       | [`tests`              |
        |                       |                       | ](JsLibraryDescriptio |
        |                       |                       | nArg.html#getTests()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsLibraryDe          | `addTests​(Buil        | ::: block             |
        | scriptionArg.Builder` | dTarget... elements)` | Adds elements to      |
        |                       |                       | [`tests`              |
        |                       |                       | ](JsLibraryDescriptio |
        |                       |                       | nArg.html#getTests()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsL                  | `build()`             | ::: block             |
        | ibraryDescriptionArg` |                       | Builds a new          |
        |                       |                       | [`JsLibraryDesc       |
        |                       |                       | riptionArg`](JsLibrar |
        |                       |                       | yDescriptionArg.html  |
        |                       |                       | "class in com.faceboo |
        |                       |                       | k.buck.features.js"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsLibraryDe          | `from​(Bu              | ::: block             |
        | scriptionArg.Builder` | ildRuleArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebo           |
        |                       |                       | ok.buck.core.descript |
        |                       |                       | ion.arg.BuildRuleArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsLibraryDe          | `from​(Cons            | ::: block             |
        | scriptionArg.Builder` | tructorArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook         |
        |                       |                       | .buck.core.descriptio |
        |                       |                       | n.arg.ConstructorArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsLibraryDe          | `from​(HasDe           | ::: block             |
        | scriptionArg.Builder` | claredDeps instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook.        |
        |                       |                       | buck.core.description |
        |                       |                       | .arg.HasDeclaredDeps` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsLibraryDe          | `from​(Ha              | ::: block             |
        | scriptionArg.Builder` | sDepsQuery instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebo           |
        |                       |                       | ok.buck.core.descript |
        |                       |                       | ion.arg.HasDepsQuery` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsLibraryDe          | `fro                  | ::: block             |
        | scriptionArg.Builder` | m​(HasTests instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.fa               |
        |                       |                       | cebook.buck.core.desc |
        |                       |                       | ription.arg.HasTests` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsLibraryDe          | `from​(Ha              | ::: block             |
        | scriptionArg.Builder` | sExtraJson instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `c                    |
        |                       |                       | om.facebook.buck.feat |
        |                       |                       | ures.js.HasExtraJson` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsLibraryDe          | `from​(com.faceb       | ::: block             |
        | scriptionArg.Builder` | ook.buck.features.js. | Copy abstract value   |
        |                       | JsLibraryDescription. | type                  |
        |                       | AbstractJsLibraryDesc | `AbstractJsL          |
        |                       | riptionArg instance)` | ibraryDescriptionArg` |
        |                       |                       | instance into         |
        |                       |                       | builder.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsLibraryDe          | `from​(JsLibraryDesc   | ::: block             |
        | scriptionArg.Builder` | riptionArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `JsL                  |
        |                       |                       | ibraryDescriptionArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsLibraryDe          | `setBaseP             | ::: block             |
        | scriptionArg.Builder` | ath​(String basePath)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`basePath`](J        |
        |                       |                       | sLibraryDescriptionAr |
        |                       |                       | g.html#getBasePath()) |
        |                       |                       | to basePath.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsLibraryDe          | `setBasePath​(Option   | ::: block             |
        | scriptionArg.Builder` | al<String> basePath)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`basePath`](J        |
        |                       |                       | sLibraryDescriptionAr |
        |                       |                       | g.html#getBasePath()) |
        |                       |                       | to basePath.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsLibraryDe          | `setCompat            | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Iterable<? e | Sets or replaces all  |
        |                       | xtends UnconfiguredBu | elements for          |
        |                       | ildTarget> elements)` | [`com                 |
        |                       |                       | patibleWith`](JsLibra |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsLibraryDe          | `setDefaul            | ::: block             |
        | scriptionArg.Builder` | tTargetPlatform​(Uncon | Initializes the       |
        |                       | figuredBuildTarget de | optional value        |
        |                       | faultTargetPlatform)` | [`defaultTargetPlat   |
        |                       |                       | form`](JsLibraryDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsLibraryDe          | `setDefau             | ::: block             |
        | scriptionArg.Builder` | ltTargetPlatform​(Opti | Initializes the       |
        |                       | onal<? extends Unconf | optional value        |
        |                       | iguredBuildTarget> de | [`defaultTargetPlat   |
        |                       | faultTargetPlatform)` | form`](JsLibraryDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsLibraryDe          | `setDeps​(             | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Sets or replaces all  |
        |                       | ildTarget> elements)` | elements for          |
        |                       |                       | [`deps                |
        |                       |                       | `](JsLibraryDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsLibraryDe          | `setDepsQu            | ::: block             |
        | scriptionArg.Builder` | ery​(Query depsQuery)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`depsQuery`](Js      |
        |                       |                       | LibraryDescriptionArg |
        |                       |                       | .html#getDepsQuery()) |
        |                       |                       | to depsQuery.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsLibraryDe          | `setDepsQ             | ::: block             |
        | scriptionArg.Builder` | uery​(Optional<? exten | Initializes the       |
        |                       | ds Query> depsQuery)` | optional value        |
        |                       |                       | [`depsQuery`](Js      |
        |                       |                       | LibraryDescriptionArg |
        |                       |                       | .html#getDepsQuery()) |
        |                       |                       | to depsQuery.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsLibraryDe          | `setExtraJson​(StringW | ::: block             |
        | scriptionArg.Builder` | ithMacros extraJson)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`extraJson`](Js      |
        |                       |                       | LibraryDescriptionArg |
        |                       |                       | .html#getExtraJson()) |
        |                       |                       | to extraJson.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsLibraryDe          | `setExtraJson​(Option  | ::: block             |
        | scriptionArg.Builder` | al<? extends StringWi | Initializes the       |
        |                       | thMacros> extraJson)` | optional value        |
        |                       |                       | [`extraJson`](Js      |
        |                       |                       | LibraryDescriptionArg |
        |                       |                       | .html#getExtraJson()) |
        |                       |                       | to extraJson.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsLibraryDe          | `setLabels​(Iterab     | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Sets or replaces all  |
        |                       |                       | elements for          |
        |                       |                       | [`labels`]            |
        |                       |                       | (JsLibraryDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsLibraryDe          | `setLicenses          | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Sets or replaces all  |
        |                       | ourcePath> elements)` | elements for          |
        |                       |                       | [`licenses`](J        |
        |                       |                       | sLibraryDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsLibraryDe          | `                     | ::: block             |
        | scriptionArg.Builder` | setName​(String name)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`name                |
        |                       |                       | `](JsLibraryDescripti |
        |                       |                       | onArg.html#getName()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsLibraryDe          | `setSrcs​(Iterable<?   | ::: block             |
        | scriptionArg.Builder` |  extends Either<Sourc | Sets or replaces all  |
        |                       | ePath,​Pair<SourcePath | elements for          |
        |                       | ,​String>>> elements)` | [`srcs                |
        |                       |                       | `](JsLibraryDescripti |
        |                       |                       | onArg.html#getSrcs()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsLibraryDe          | `setTests​(            | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Sets or replaces all  |
        |                       | ildTarget> elements)` | elements for          |
        |                       |                       | [`tests`              |
        |                       |                       | ](JsLibraryDescriptio |
        |                       |                       | nArg.html#getTests()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `JsLibraryDe          | `setWorker            | ::: block             |
        | scriptionArg.Builder` | ​(BuildTarget worker)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`worker`]            |
        |                       |                       | (JsLibraryDescription |
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
            public final JsLibraryDescriptionArg.Builder from​(HasDeclaredDeps instance)
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

        []{#from(com.facebook.buck.core.description.arg.HasTests)}

        -   #### from

            ``` methodSignature
            public final JsLibraryDescriptionArg.Builder from​(HasTests instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `com.facebook.buck.core.description.arg.HasTests` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.core.description.arg.HasDepsQuery)}

        -   #### from

            ``` methodSignature
            public final JsLibraryDescriptionArg.Builder from​(HasDepsQuery instance)
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

        []{#from(com.facebook.buck.features.js.HasExtraJson)}

        -   #### from

            ``` methodSignature
            public final JsLibraryDescriptionArg.Builder from​(HasExtraJson instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `com.facebook.buck.features.js.HasExtraJson` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.core.description.arg.BuildRuleArg)}

        -   #### from

            ``` methodSignature
            public final JsLibraryDescriptionArg.Builder from​(BuildRuleArg instance)
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
            public final JsLibraryDescriptionArg.Builder from​(ConstructorArg instance)
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

        []{#from(com.facebook.buck.features.js.JsLibraryDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final JsLibraryDescriptionArg.Builder from​(JsLibraryDescriptionArg instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `JsLibraryDescriptionArg` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.features.js.JsLibraryDescription.AbstractJsLibraryDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final JsLibraryDescriptionArg.Builder from​(com.facebook.buck.features.js.JsLibraryDescription.AbstractJsLibraryDescriptionArg instance)
            ```

            ::: block
            Copy abstract value type `AbstractJsLibraryDescriptionArg`
            instance into builder.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addSrcs(com.facebook.buck.util.types.Either)}

        -   #### addSrcs

            ``` methodSignature
            public final JsLibraryDescriptionArg.Builder addSrcs​(Either<SourcePath,​Pair<SourcePath,​String>> element)
            ```

            ::: block
            Adds one element to
            [`srcs`](JsLibraryDescriptionArg.html#getSrcs()) set.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A srcs element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addSrcs(com.facebook.buck.util.types.Either...)}

        -   #### addSrcs

            ``` methodSignature
            @SafeVarargs
            public final JsLibraryDescriptionArg.Builder addSrcs​(Either<SourcePath,​Pair<SourcePath,​String>>... elements)
            ```

            ::: block
            Adds elements to
            [`srcs`](JsLibraryDescriptionArg.html#getSrcs()) set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of srcs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setSrcs(java.lang.Iterable)}

        -   #### setSrcs

            ``` methodSignature
            public final JsLibraryDescriptionArg.Builder setSrcs​(Iterable<? extends Either<SourcePath,​Pair<SourcePath,​String>>> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`srcs`](JsLibraryDescriptionArg.html#getSrcs()) set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of srcs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllSrcs(java.lang.Iterable)}

        -   #### addAllSrcs

            ``` methodSignature
            public final JsLibraryDescriptionArg.Builder addAllSrcs​(Iterable<? extends Either<SourcePath,​Pair<SourcePath,​String>>> elements)
            ```

            ::: block
            Adds elements to
            [`srcs`](JsLibraryDescriptionArg.html#getSrcs()) set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of srcs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setWorker(com.facebook.buck.core.model.BuildTarget)}

        -   #### setWorker

            ``` methodSignature
            public final JsLibraryDescriptionArg.Builder setWorker​(BuildTarget worker)
            ```

            ::: block
            Initializes the value for the
            [`worker`](JsLibraryDescriptionArg.html#getWorker())
            attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `worker` - The value for worker

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setBasePath(java.lang.String)}

        -   #### setBasePath

            ``` methodSignature
            public final JsLibraryDescriptionArg.Builder setBasePath​(String basePath)
            ```

            ::: block
            Initializes the optional value
            [`basePath`](JsLibraryDescriptionArg.html#getBasePath()) to
            basePath.
            :::

            [Parameters:]{.paramLabel}
            :   `basePath` - The value for basePath

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setBasePath(java.util.Optional)}

        -   #### setBasePath

            ``` methodSignature
            public final JsLibraryDescriptionArg.Builder setBasePath​(Optional<String> basePath)
            ```

            ::: block
            Initializes the optional value
            [`basePath`](JsLibraryDescriptionArg.html#getBasePath()) to
            basePath.
            :::

            [Parameters:]{.paramLabel}
            :   `basePath` - The value for basePath

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCompatibleWith(com.facebook.buck.core.model.UnconfiguredBuildTarget)}

        -   #### addCompatibleWith

            ``` methodSignature
            public final JsLibraryDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget element)
            ```

            ::: block
            Adds one element to
            [`compatibleWith`](JsLibraryDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A compatibleWith element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCompatibleWith(com.facebook.buck.core.model.UnconfiguredBuildTarget...)}

        -   #### addCompatibleWith

            ``` methodSignature
            public final JsLibraryDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](JsLibraryDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCompatibleWith(java.lang.Iterable)}

        -   #### setCompatibleWith

            ``` methodSignature
            public final JsLibraryDescriptionArg.Builder setCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`compatibleWith`](JsLibraryDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllCompatibleWith(java.lang.Iterable)}

        -   #### addAllCompatibleWith

            ``` methodSignature
            public final JsLibraryDescriptionArg.Builder addAllCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](JsLibraryDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDefaultTargetPlatform(com.facebook.buck.core.model.UnconfiguredBuildTarget)}

        -   #### setDefaultTargetPlatform

            ``` methodSignature
            public final JsLibraryDescriptionArg.Builder setDefaultTargetPlatform​(UnconfiguredBuildTarget defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](JsLibraryDescriptionArg.html#getDefaultTargetPlatform())
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
            public final JsLibraryDescriptionArg.Builder setDefaultTargetPlatform​(Optional<? extends UnconfiguredBuildTarget> defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](JsLibraryDescriptionArg.html#getDefaultTargetPlatform())
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
            public final JsLibraryDescriptionArg.Builder addLabels​(String element)
            ```

            ::: block
            Adds one element to
            [`labels`](JsLibraryDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A labels element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLabels(java.lang.String...)}

        -   #### addLabels

            ``` methodSignature
            public final JsLibraryDescriptionArg.Builder addLabels​(String... elements)
            ```

            ::: block
            Adds elements to
            [`labels`](JsLibraryDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLabels(java.lang.Iterable)}

        -   #### setLabels

            ``` methodSignature
            public final JsLibraryDescriptionArg.Builder setLabels​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`labels`](JsLibraryDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLabels(java.lang.Iterable)}

        -   #### addAllLabels

            ``` methodSignature
            public final JsLibraryDescriptionArg.Builder addAllLabels​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`labels`](JsLibraryDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLicenses(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### addLicenses

            ``` methodSignature
            public final JsLibraryDescriptionArg.Builder addLicenses​(SourcePath element)
            ```

            ::: block
            Adds one element to
            [`licenses`](JsLibraryDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A licenses element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLicenses(com.facebook.buck.core.sourcepath.SourcePath...)}

        -   #### addLicenses

            ``` methodSignature
            public final JsLibraryDescriptionArg.Builder addLicenses​(SourcePath... elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](JsLibraryDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLicenses(java.lang.Iterable)}

        -   #### setLicenses

            ``` methodSignature
            public final JsLibraryDescriptionArg.Builder setLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`licenses`](JsLibraryDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLicenses(java.lang.Iterable)}

        -   #### addAllLicenses

            ``` methodSignature
            public final JsLibraryDescriptionArg.Builder addAllLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](JsLibraryDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setName(java.lang.String)}

        -   #### setName

            ``` methodSignature
            public final JsLibraryDescriptionArg.Builder setName​(String name)
            ```

            ::: block
            Initializes the value for the
            [`name`](JsLibraryDescriptionArg.html#getName()) attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `name` - The value for name

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDepsQuery(com.facebook.buck.rules.query.Query)}

        -   #### setDepsQuery

            ``` methodSignature
            public final JsLibraryDescriptionArg.Builder setDepsQuery​(Query depsQuery)
            ```

            ::: block
            Initializes the optional value
            [`depsQuery`](JsLibraryDescriptionArg.html#getDepsQuery())
            to depsQuery.
            :::

            [Parameters:]{.paramLabel}
            :   `depsQuery` - The value for depsQuery

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setDepsQuery(java.util.Optional)}

        -   #### setDepsQuery

            ``` methodSignature
            public final JsLibraryDescriptionArg.Builder setDepsQuery​(Optional<? extends Query> depsQuery)
            ```

            ::: block
            Initializes the optional value
            [`depsQuery`](JsLibraryDescriptionArg.html#getDepsQuery())
            to depsQuery.
            :::

            [Parameters:]{.paramLabel}
            :   `depsQuery` - The value for depsQuery

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addDeps(com.facebook.buck.core.model.BuildTarget)}

        -   #### addDeps

            ``` methodSignature
            public final JsLibraryDescriptionArg.Builder addDeps​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`deps`](JsLibraryDescriptionArg.html#getDeps()) sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A deps element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addDeps(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addDeps

            ``` methodSignature
            public final JsLibraryDescriptionArg.Builder addDeps​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`deps`](JsLibraryDescriptionArg.html#getDeps()) sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDeps(java.lang.Iterable)}

        -   #### setDeps

            ``` methodSignature
            public final JsLibraryDescriptionArg.Builder setDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`deps`](JsLibraryDescriptionArg.html#getDeps()) sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllDeps(java.lang.Iterable)}

        -   #### addAllDeps

            ``` methodSignature
            public final JsLibraryDescriptionArg.Builder addAllDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`deps`](JsLibraryDescriptionArg.html#getDeps()) sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setExtraJson(com.facebook.buck.rules.macros.StringWithMacros)}

        -   #### setExtraJson

            ``` methodSignature
            public final JsLibraryDescriptionArg.Builder setExtraJson​(StringWithMacros extraJson)
            ```

            ::: block
            Initializes the optional value
            [`extraJson`](JsLibraryDescriptionArg.html#getExtraJson())
            to extraJson.
            :::

            [Parameters:]{.paramLabel}
            :   `extraJson` - The value for extraJson

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setExtraJson(java.util.Optional)}

        -   #### setExtraJson

            ``` methodSignature
            public final JsLibraryDescriptionArg.Builder setExtraJson​(Optional<? extends StringWithMacros> extraJson)
            ```

            ::: block
            Initializes the optional value
            [`extraJson`](JsLibraryDescriptionArg.html#getExtraJson())
            to extraJson.
            :::

            [Parameters:]{.paramLabel}
            :   `extraJson` - The value for extraJson

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addTests(com.facebook.buck.core.model.BuildTarget)}

        -   #### addTests

            ``` methodSignature
            public final JsLibraryDescriptionArg.Builder addTests​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`tests`](JsLibraryDescriptionArg.html#getTests())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A tests element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addTests(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addTests

            ``` methodSignature
            public final JsLibraryDescriptionArg.Builder addTests​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`tests`](JsLibraryDescriptionArg.html#getTests())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of tests elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setTests(java.lang.Iterable)}

        -   #### setTests

            ``` methodSignature
            public final JsLibraryDescriptionArg.Builder setTests​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`tests`](JsLibraryDescriptionArg.html#getTests())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of tests elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllTests(java.lang.Iterable)}

        -   #### addAllTests

            ``` methodSignature
            public final JsLibraryDescriptionArg.Builder addAllTests​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`tests`](JsLibraryDescriptionArg.html#getTests())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of tests elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#build()}

        -   #### build

            ``` methodSignature
            public JsLibraryDescriptionArg build()
            ```

            ::: block
            Builds a new
            [`JsLibraryDescriptionArg`](JsLibraryDescriptionArg.html "class in com.facebook.buck.features.js").
            :::

            [Returns:]{.returnLabel}
            :   An immutable instance of JsLibraryDescriptionArg

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
