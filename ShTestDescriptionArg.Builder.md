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

## Class ShTestDescriptionArg.Builder {#class-shtestdescriptionarg.builder .title title="Class ShTestDescriptionArg.Builder"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.shell.ShTestDescriptionArg.Builder

::: description
-   

    Enclosing class:
    :   [ShTestDescriptionArg](ShTestDescriptionArg.html "class in com.facebook.buck.shell")

    ------------------------------------------------------------------------

        @NotThreadSafe
        public static final class ShTestDescriptionArg.Builder
        extends Object

    ::: block
    Builds instances of type
    [`ShTestDescriptionArg`](ShTestDescriptionArg.html "class in com.facebook.buck.shell").
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
        | `ShTestDe             | `addAllArgs​(Itera     | ::: block             |
        | scriptionArg.Builder` | ble<? extends StringW | Adds elements to      |
        |                       | ithMacros> elements)` | [`a                   |
        |                       |                       | rgs`](ShTestDescripti |
        |                       |                       | onArg.html#getArgs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ShTestDe             | `addAllCompat         | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Iterable<? e | Adds elements to      |
        |                       | xtends UnconfiguredBu | [`                    |
        |                       | ildTarget> elements)` | compatibleWith`](ShTe |
        |                       |                       | stDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ShTestDe             | `                     | ::: block             |
        | scriptionArg.Builder` | addAllContacts​(Iterab | Adds elements to      |
        |                       | le<String> elements)` | [`contacts`           |
        |                       |                       | ](ShTestDescriptionAr |
        |                       |                       | g.html#getContacts()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ShTestDe             | `addAllDeps​(          | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Adds elements to      |
        |                       | ildTarget> elements)` | [`d                   |
        |                       |                       | eps`](ShTestDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ShTestDe             | `addAllLabels​(Iterab  | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Adds elements to      |
        |                       |                       | [`label               |
        |                       |                       | s`](ShTestDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ShTestDe             | `addAllLicenses       | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Adds elements to      |
        |                       | ourcePath> elements)` | [`licenses`           |
        |                       |                       | ](ShTestDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ShTestDe             | `addAllResources      | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Adds elements to      |
        |                       | ourcePath> elements)` | [`resources`]         |
        |                       |                       | (ShTestDescriptionArg |
        |                       |                       | .html#getResources()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ShTestDe             | `addArgs​(Strin        | ::: block             |
        | scriptionArg.Builder` | gWithMacros element)` | Adds one element to   |
        |                       |                       | [`a                   |
        |                       |                       | rgs`](ShTestDescripti |
        |                       |                       | onArg.html#getArgs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ShTestDe             | `addArgs​(StringWit    | ::: block             |
        | scriptionArg.Builder` | hMacros... elements)` | Adds elements to      |
        |                       |                       | [`a                   |
        |                       |                       | rgs`](ShTestDescripti |
        |                       |                       | onArg.html#getArgs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ShTestDe             | `addCompat            | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Unconfigured | Adds one element to   |
        |                       | BuildTarget element)` | [`                    |
        |                       |                       | compatibleWith`](ShTe |
        |                       |                       | stDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ShTestDe             | `addCompatible        | ::: block             |
        | scriptionArg.Builder` | With​(UnconfiguredBuil | Adds elements to      |
        |                       | dTarget... elements)` | [`                    |
        |                       |                       | compatibleWith`](ShTe |
        |                       |                       | stDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ShTestDe             | `addCont              | ::: block             |
        | scriptionArg.Builder` | acts​(String element)` | Adds one element to   |
        |                       |                       | [`contacts`           |
        |                       |                       | ](ShTestDescriptionAr |
        |                       |                       | g.html#getContacts()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ShTestDe             | `addContacts          | ::: block             |
        | scriptionArg.Builder` | ​(String... elements)` | Adds elements to      |
        |                       |                       | [`contacts`           |
        |                       |                       | ](ShTestDescriptionAr |
        |                       |                       | g.html#getContacts()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ShTestDe             | `addDeps​(             | ::: block             |
        | scriptionArg.Builder` | BuildTarget element)` | Adds one element to   |
        |                       |                       | [`d                   |
        |                       |                       | eps`](ShTestDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ShTestDe             | `addDeps​(Buil         | ::: block             |
        | scriptionArg.Builder` | dTarget... elements)` | Adds elements to      |
        |                       |                       | [`d                   |
        |                       |                       | eps`](ShTestDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ShTestDe             | `addLa                | ::: block             |
        | scriptionArg.Builder` | bels​(String element)` | Adds one element to   |
        |                       |                       | [`label               |
        |                       |                       | s`](ShTestDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ShTestDe             | `addLabels            | ::: block             |
        | scriptionArg.Builder` | ​(String... elements)` | Adds elements to      |
        |                       |                       | [`label               |
        |                       |                       | s`](ShTestDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ShTestDe             | `addLicenses          | ::: block             |
        | scriptionArg.Builder` | ​(SourcePath element)` | Adds one element to   |
        |                       |                       | [`licenses`           |
        |                       |                       | ](ShTestDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ShTestDe             | `addLicenses​(Sou      | ::: block             |
        | scriptionArg.Builder` | rcePath... elements)` | Adds elements to      |
        |                       |                       | [`licenses`           |
        |                       |                       | ](ShTestDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ShTestDe             | `addResources         | ::: block             |
        | scriptionArg.Builder` | ​(SourcePath element)` | Adds one element to   |
        |                       |                       | [`resources`]         |
        |                       |                       | (ShTestDescriptionArg |
        |                       |                       | .html#getResources()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ShTestDe             | `addResources​(Sou     | ::: block             |
        | scriptionArg.Builder` | rcePath... elements)` | Adds elements to      |
        |                       |                       | [`resources`]         |
        |                       |                       | (ShTestDescriptionArg |
        |                       |                       | .html#getResources()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `build()`             | ::: block             |
        | ShTestDescriptionArg` |                       | Builds a new          |
        |                       |                       | [`S                   |
        |                       |                       | hTestDescriptionArg`] |
        |                       |                       | (ShTestDescriptionArg |
        |                       |                       | .html "class in com.f |
        |                       |                       | acebook.buck.shell"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ShTestDe             | `from​(Bu              | ::: block             |
        | scriptionArg.Builder` | ildRuleArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebo           |
        |                       |                       | ok.buck.core.descript |
        |                       |                       | ion.arg.BuildRuleArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ShTestDe             | `from​(Cons            | ::: block             |
        | scriptionArg.Builder` | tructorArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook         |
        |                       |                       | .buck.core.descriptio |
        |                       |                       | n.arg.ConstructorArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ShTestDe             | `from​(H               | ::: block             |
        | scriptionArg.Builder` | asContacts instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.faceb            |
        |                       |                       | ook.buck.core.descrip |
        |                       |                       | tion.arg.HasContacts` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ShTestDe             | `from​(HasDe           | ::: block             |
        | scriptionArg.Builder` | claredDeps instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook.        |
        |                       |                       | buck.core.description |
        |                       |                       | .arg.HasDeclaredDeps` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ShTestDe             | `from​(HasT            | ::: block             |
        | scriptionArg.Builder` | estTimeout instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook         |
        |                       |                       | .buck.core.descriptio |
        |                       |                       | n.arg.HasTestTimeout` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ShTestDe             | `fr                   | ::: block             |
        | scriptionArg.Builder` | om​(com.facebook.buck. | Copy abstract value   |
        |                       | shell.ShTestDescripti | type                  |
        |                       | on.AbstractShTestDesc | `Abstract             |
        |                       | riptionArg instance)` | ShTestDescriptionArg` |
        |                       |                       | instance into         |
        |                       |                       | builder.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ShTestDe             | `from​(ShTestDesc      | ::: block             |
        | scriptionArg.Builder` | riptionArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `                     |
        |                       |                       | ShTestDescriptionArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ShTestDe             | `putAllEnv​(Map<St     | ::: block             |
        | scriptionArg.Builder` | ring,​? extends String | Put all mappings from |
        |                       | WithMacros> entries)` | the specified map as  |
        |                       |                       | entries to            |
        |                       |                       | [                     |
        |                       |                       | `env`](ShTestDescript |
        |                       |                       | ionArg.html#getEnv()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ShTestDe             | `putEnv​(              | ::: block             |
        | scriptionArg.Builder` | String key,       Str | Put one entry to the  |
        |                       | ingWithMacros value)` | [                     |
        |                       |                       | `env`](ShTestDescript |
        |                       |                       | ionArg.html#getEnv()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ShTestDe             | `putEnv​(Map.Entry<    | ::: block             |
        | scriptionArg.Builder` | String,​? extends Stri | Put one entry to the  |
        |                       | ngWithMacros> entry)` | [                     |
        |                       |                       | `env`](ShTestDescript |
        |                       |                       | ionArg.html#getEnv()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ShTestDe             | `setArgs​(Itera        | ::: block             |
        | scriptionArg.Builder` | ble<? extends StringW | Sets or replaces all  |
        |                       | ithMacros> elements)` | elements for          |
        |                       |                       | [`a                   |
        |                       |                       | rgs`](ShTestDescripti |
        |                       |                       | onArg.html#getArgs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ShTestDe             | `setCompat            | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Iterable<? e | Sets or replaces all  |
        |                       | xtends UnconfiguredBu | elements for          |
        |                       | ildTarget> elements)` | [`                    |
        |                       |                       | compatibleWith`](ShTe |
        |                       |                       | stDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ShTestDe             | `setContacts​(Iterab   | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Sets or replaces all  |
        |                       |                       | elements for          |
        |                       |                       | [`contacts`           |
        |                       |                       | ](ShTestDescriptionAr |
        |                       |                       | g.html#getContacts()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ShTestDe             | `setDefaul            | ::: block             |
        | scriptionArg.Builder` | tTargetPlatform​(Uncon | Initializes the       |
        |                       | figuredBuildTarget de | optional value        |
        |                       | faultTargetPlatform)` | [`defaultTargetP      |
        |                       |                       | latform`](ShTestDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ShTestDe             | `setDefau             | ::: block             |
        | scriptionArg.Builder` | ltTargetPlatform​(Opti | Initializes the       |
        |                       | onal<? extends Unconf | optional value        |
        |                       | iguredBuildTarget> de | [`defaultTargetP      |
        |                       | faultTargetPlatform)` | latform`](ShTestDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ShTestDe             | `setDeps​(             | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Sets or replaces all  |
        |                       | ildTarget> elements)` | elements for          |
        |                       |                       | [`d                   |
        |                       |                       | eps`](ShTestDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ShTestDe             | `setEnv​(Map<St        | ::: block             |
        | scriptionArg.Builder` | ring,​? extends String | Sets or replaces all  |
        |                       | WithMacros> entries)` | mappings from the     |
        |                       |                       | specified map as      |
        |                       |                       | entries for the       |
        |                       |                       | [                     |
        |                       |                       | `env`](ShTestDescript |
        |                       |                       | ionArg.html#getEnv()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ShTestDe             | `setLabels​(Iterab     | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Sets or replaces all  |
        |                       |                       | elements for          |
        |                       |                       | [`label               |
        |                       |                       | s`](ShTestDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ShTestDe             | `setLicenses          | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Sets or replaces all  |
        |                       | ourcePath> elements)` | elements for          |
        |                       |                       | [`licenses`           |
        |                       |                       | ](ShTestDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ShTestDe             | `                     | ::: block             |
        | scriptionArg.Builder` | setName​(String name)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`n                   |
        |                       |                       | ame`](ShTestDescripti |
        |                       |                       | onArg.html#getName()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ShTestDe             | `setResources         | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Sets or replaces all  |
        |                       | ourcePath> elements)` | elements for          |
        |                       |                       | [`resources`]         |
        |                       |                       | (ShTestDescriptionArg |
        |                       |                       | .html#getResources()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ShTestDe             | `setRun               | ::: block             |
        | scriptionArg.Builder` | TestSeparately​(boolea | Initializes the value |
        |                       | n runTestSeparately)` | for the               |
        |                       |                       | [`runTes              |
        |                       |                       | tSeparately`](ShTestD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tRunTestSeparately()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ShTestDe             | `setT                 | ::: block             |
        | scriptionArg.Builder` | est​(SourcePath test)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`t                   |
        |                       |                       | est`](ShTestDescripti |
        |                       |                       | onArg.html#getTest()) |
        |                       |                       | to test.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ShTestDe             | `set                  | ::: block             |
        | scriptionArg.Builder` | Test​(Optional<? exten | Initializes the       |
        |                       | ds SourcePath> test)` | optional value        |
        |                       |                       | [`t                   |
        |                       |                       | est`](ShTestDescripti |
        |                       |                       | onArg.html#getTest()) |
        |                       |                       | to test.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ShTestDe             | `set                  | ::: block             |
        | scriptionArg.Builder` | TestRuleTimeoutMs​(lon | Initializes the       |
        |                       | g testRuleTimeoutMs)` | optional value        |
        |                       |                       | [`testRu              |
        |                       |                       | leTimeoutMs`](ShTestD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tTestRuleTimeoutMs()) |
        |                       |                       | to testRuleTimeoutMs. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ShTestDe             | `setTestRuleTi        | ::: block             |
        | scriptionArg.Builder` | meoutMs​(Optional<Long | Initializes the       |
        |                       | > testRuleTimeoutMs)` | optional value        |
        |                       |                       | [`testRu              |
        |                       |                       | leTimeoutMs`](ShTestD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tTestRuleTimeoutMs()) |
        |                       |                       | to testRuleTimeoutMs. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ShTestDe             | `                     | ::: block             |
        | scriptionArg.Builder` | setType​(String type)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`t                   |
        |                       |                       | ype`](ShTestDescripti |
        |                       |                       | onArg.html#getType()) |
        |                       |                       | to type.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `ShTestDe             | `setType​(Op           | ::: block             |
        | scriptionArg.Builder` | tional<String> type)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`t                   |
        |                       |                       | ype`](ShTestDescripti |
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

        []{#from(com.facebook.buck.core.description.arg.HasDeclaredDeps)}

        -   #### from

            ``` methodSignature
            public final ShTestDescriptionArg.Builder from​(HasDeclaredDeps instance)
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

        []{#from(com.facebook.buck.core.description.arg.HasTestTimeout)}

        -   #### from

            ``` methodSignature
            public final ShTestDescriptionArg.Builder from​(HasTestTimeout instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `com.facebook.buck.core.description.arg.HasTestTimeout`
            instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.core.description.arg.BuildRuleArg)}

        -   #### from

            ``` methodSignature
            public final ShTestDescriptionArg.Builder from​(BuildRuleArg instance)
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

        []{#from(com.facebook.buck.core.description.arg.HasContacts)}

        -   #### from

            ``` methodSignature
            public final ShTestDescriptionArg.Builder from​(HasContacts instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `com.facebook.buck.core.description.arg.HasContacts`
            instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.core.description.arg.ConstructorArg)}

        -   #### from

            ``` methodSignature
            public final ShTestDescriptionArg.Builder from​(ConstructorArg instance)
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

        []{#from(com.facebook.buck.shell.ShTestDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final ShTestDescriptionArg.Builder from​(ShTestDescriptionArg instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `ShTestDescriptionArg` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.shell.ShTestDescription.AbstractShTestDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final ShTestDescriptionArg.Builder from​(com.facebook.buck.shell.ShTestDescription.AbstractShTestDescriptionArg instance)
            ```

            ::: block
            Copy abstract value type `AbstractShTestDescriptionArg`
            instance into builder.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setTest(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setTest

            ``` methodSignature
            public final ShTestDescriptionArg.Builder setTest​(SourcePath test)
            ```

            ::: block
            Initializes the optional value
            [`test`](ShTestDescriptionArg.html#getTest()) to test.
            :::

            [Parameters:]{.paramLabel}
            :   `test` - The value for test

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setTest(java.util.Optional)}

        -   #### setTest

            ``` methodSignature
            public final ShTestDescriptionArg.Builder setTest​(Optional<? extends SourcePath> test)
            ```

            ::: block
            Initializes the optional value
            [`test`](ShTestDescriptionArg.html#getTest()) to test.
            :::

            [Parameters:]{.paramLabel}
            :   `test` - The value for test

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addArgs(com.facebook.buck.rules.macros.StringWithMacros)}

        -   #### addArgs

            ``` methodSignature
            public final ShTestDescriptionArg.Builder addArgs​(StringWithMacros element)
            ```

            ::: block
            Adds one element to
            [`args`](ShTestDescriptionArg.html#getArgs()) list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A args element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addArgs(com.facebook.buck.rules.macros.StringWithMacros...)}

        -   #### addArgs

            ``` methodSignature
            public final ShTestDescriptionArg.Builder addArgs​(StringWithMacros... elements)
            ```

            ::: block
            Adds elements to
            [`args`](ShTestDescriptionArg.html#getArgs()) list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of args elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setArgs(java.lang.Iterable)}

        -   #### setArgs

            ``` methodSignature
            public final ShTestDescriptionArg.Builder setArgs​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`args`](ShTestDescriptionArg.html#getArgs()) list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of args elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllArgs(java.lang.Iterable)}

        -   #### addAllArgs

            ``` methodSignature
            public final ShTestDescriptionArg.Builder addAllArgs​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Adds elements to
            [`args`](ShTestDescriptionArg.html#getArgs()) list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of args elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setType(java.lang.String)}

        -   #### setType

            ``` methodSignature
            public final ShTestDescriptionArg.Builder setType​(String type)
            ```

            ::: block
            Initializes the optional value
            [`type`](ShTestDescriptionArg.html#getType()) to type.
            :::

            [Parameters:]{.paramLabel}
            :   `type` - The value for type

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setType(java.util.Optional)}

        -   #### setType

            ``` methodSignature
            public final ShTestDescriptionArg.Builder setType​(Optional<String> type)
            ```

            ::: block
            Initializes the optional value
            [`type`](ShTestDescriptionArg.html#getType()) to type.
            :::

            [Parameters:]{.paramLabel}
            :   `type` - The value for type

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setRunTestSeparately(boolean)}

        -   #### setRunTestSeparately

            ``` methodSignature
            public final ShTestDescriptionArg.Builder setRunTestSeparately​(boolean runTestSeparately)
            ```

            ::: block
            Initializes the value for the
            [`runTestSeparately`](ShTestDescriptionArg.html#getRunTestSeparately())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`runTestSeparately`](ShTestDescriptionArg.html#getRunTestSeparately()).*
            :::

            [Parameters:]{.paramLabel}
            :   `runTestSeparately` - The value for runTestSeparately

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addResources(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### addResources

            ``` methodSignature
            public final ShTestDescriptionArg.Builder addResources​(SourcePath element)
            ```

            ::: block
            Adds one element to
            [`resources`](ShTestDescriptionArg.html#getResources())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A resources element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addResources(com.facebook.buck.core.sourcepath.SourcePath...)}

        -   #### addResources

            ``` methodSignature
            public final ShTestDescriptionArg.Builder addResources​(SourcePath... elements)
            ```

            ::: block
            Adds elements to
            [`resources`](ShTestDescriptionArg.html#getResources())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of resources elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setResources(java.lang.Iterable)}

        -   #### setResources

            ``` methodSignature
            public final ShTestDescriptionArg.Builder setResources​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`resources`](ShTestDescriptionArg.html#getResources())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of resources elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllResources(java.lang.Iterable)}

        -   #### addAllResources

            ``` methodSignature
            public final ShTestDescriptionArg.Builder addAllResources​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Adds elements to
            [`resources`](ShTestDescriptionArg.html#getResources())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of resources elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putEnv(java.lang.String,com.facebook.buck.rules.macros.StringWithMacros)}

        -   #### putEnv

            ``` methodSignature
            public final ShTestDescriptionArg.Builder putEnv​(String key,
                                                             StringWithMacros value)
            ```

            ::: block
            Put one entry to the
            [`env`](ShTestDescriptionArg.html#getEnv()) map.
            :::

            [Parameters:]{.paramLabel}
            :   `key` - The key in the env map
            :   `value` - The associated value in the env map

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putEnv(java.util.Map.Entry)}

        -   #### putEnv

            ``` methodSignature
            public final ShTestDescriptionArg.Builder putEnv​(Map.Entry<String,​? extends StringWithMacros> entry)
            ```

            ::: block
            Put one entry to the
            [`env`](ShTestDescriptionArg.html#getEnv()) map. Nulls are
            not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entry` - The key and value entry

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setEnv(java.util.Map)}

        -   #### setEnv

            ``` methodSignature
            public final ShTestDescriptionArg.Builder setEnv​(Map<String,​? extends StringWithMacros> entries)
            ```

            ::: block
            Sets or replaces all mappings from the specified map as
            entries for the [`env`](ShTestDescriptionArg.html#getEnv())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entries` - The entries that will be added to the env
                map

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putAllEnv(java.util.Map)}

        -   #### putAllEnv

            ``` methodSignature
            public final ShTestDescriptionArg.Builder putAllEnv​(Map<String,​? extends StringWithMacros> entries)
            ```

            ::: block
            Put all mappings from the specified map as entries to
            [`env`](ShTestDescriptionArg.html#getEnv()) map. Nulls are
            not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entries` - The entries that will be added to the env
                map

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLicenses(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### addLicenses

            ``` methodSignature
            public final ShTestDescriptionArg.Builder addLicenses​(SourcePath element)
            ```

            ::: block
            Adds one element to
            [`licenses`](ShTestDescriptionArg.html#getLicenses()) set.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A licenses element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLicenses(com.facebook.buck.core.sourcepath.SourcePath...)}

        -   #### addLicenses

            ``` methodSignature
            public final ShTestDescriptionArg.Builder addLicenses​(SourcePath... elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](ShTestDescriptionArg.html#getLicenses()) set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLicenses(java.lang.Iterable)}

        -   #### setLicenses

            ``` methodSignature
            public final ShTestDescriptionArg.Builder setLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`licenses`](ShTestDescriptionArg.html#getLicenses()) set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLicenses(java.lang.Iterable)}

        -   #### addAllLicenses

            ``` methodSignature
            public final ShTestDescriptionArg.Builder addAllLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](ShTestDescriptionArg.html#getLicenses()) set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLabels(java.lang.String)}

        -   #### addLabels

            ``` methodSignature
            public final ShTestDescriptionArg.Builder addLabels​(String element)
            ```

            ::: block
            Adds one element to
            [`labels`](ShTestDescriptionArg.html#getLabels()) sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A labels element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLabels(java.lang.String...)}

        -   #### addLabels

            ``` methodSignature
            public final ShTestDescriptionArg.Builder addLabels​(String... elements)
            ```

            ::: block
            Adds elements to
            [`labels`](ShTestDescriptionArg.html#getLabels()) sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLabels(java.lang.Iterable)}

        -   #### setLabels

            ``` methodSignature
            public final ShTestDescriptionArg.Builder setLabels​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`labels`](ShTestDescriptionArg.html#getLabels()) sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLabels(java.lang.Iterable)}

        -   #### addAllLabels

            ``` methodSignature
            public final ShTestDescriptionArg.Builder addAllLabels​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`labels`](ShTestDescriptionArg.html#getLabels()) sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDefaultTargetPlatform(com.facebook.buck.core.model.UnconfiguredBuildTarget)}

        -   #### setDefaultTargetPlatform

            ``` methodSignature
            public final ShTestDescriptionArg.Builder setDefaultTargetPlatform​(UnconfiguredBuildTarget defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](ShTestDescriptionArg.html#getDefaultTargetPlatform())
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
            public final ShTestDescriptionArg.Builder setDefaultTargetPlatform​(Optional<? extends UnconfiguredBuildTarget> defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](ShTestDescriptionArg.html#getDefaultTargetPlatform())
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
            public final ShTestDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget element)
            ```

            ::: block
            Adds one element to
            [`compatibleWith`](ShTestDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A compatibleWith element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCompatibleWith(com.facebook.buck.core.model.UnconfiguredBuildTarget...)}

        -   #### addCompatibleWith

            ``` methodSignature
            public final ShTestDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](ShTestDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCompatibleWith(java.lang.Iterable)}

        -   #### setCompatibleWith

            ``` methodSignature
            public final ShTestDescriptionArg.Builder setCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`compatibleWith`](ShTestDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllCompatibleWith(java.lang.Iterable)}

        -   #### addAllCompatibleWith

            ``` methodSignature
            public final ShTestDescriptionArg.Builder addAllCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](ShTestDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setName(java.lang.String)}

        -   #### setName

            ``` methodSignature
            public final ShTestDescriptionArg.Builder setName​(String name)
            ```

            ::: block
            Initializes the value for the
            [`name`](ShTestDescriptionArg.html#getName()) attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `name` - The value for name

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addContacts(java.lang.String)}

        -   #### addContacts

            ``` methodSignature
            public final ShTestDescriptionArg.Builder addContacts​(String element)
            ```

            ::: block
            Adds one element to
            [`contacts`](ShTestDescriptionArg.html#getContacts())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A contacts element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addContacts(java.lang.String...)}

        -   #### addContacts

            ``` methodSignature
            public final ShTestDescriptionArg.Builder addContacts​(String... elements)
            ```

            ::: block
            Adds elements to
            [`contacts`](ShTestDescriptionArg.html#getContacts())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of contacts elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setContacts(java.lang.Iterable)}

        -   #### setContacts

            ``` methodSignature
            public final ShTestDescriptionArg.Builder setContacts​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`contacts`](ShTestDescriptionArg.html#getContacts())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of contacts elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllContacts(java.lang.Iterable)}

        -   #### addAllContacts

            ``` methodSignature
            public final ShTestDescriptionArg.Builder addAllContacts​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`contacts`](ShTestDescriptionArg.html#getContacts())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of contacts elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addDeps(com.facebook.buck.core.model.BuildTarget)}

        -   #### addDeps

            ``` methodSignature
            public final ShTestDescriptionArg.Builder addDeps​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`deps`](ShTestDescriptionArg.html#getDeps()) sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A deps element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addDeps(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addDeps

            ``` methodSignature
            public final ShTestDescriptionArg.Builder addDeps​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`deps`](ShTestDescriptionArg.html#getDeps()) sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDeps(java.lang.Iterable)}

        -   #### setDeps

            ``` methodSignature
            public final ShTestDescriptionArg.Builder setDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`deps`](ShTestDescriptionArg.html#getDeps()) sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllDeps(java.lang.Iterable)}

        -   #### addAllDeps

            ``` methodSignature
            public final ShTestDescriptionArg.Builder addAllDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`deps`](ShTestDescriptionArg.html#getDeps()) sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setTestRuleTimeoutMs(long)}

        -   #### setTestRuleTimeoutMs

            ``` methodSignature
            public final ShTestDescriptionArg.Builder setTestRuleTimeoutMs​(long testRuleTimeoutMs)
            ```

            ::: block
            Initializes the optional value
            [`testRuleTimeoutMs`](ShTestDescriptionArg.html#getTestRuleTimeoutMs())
            to testRuleTimeoutMs.
            :::

            [Parameters:]{.paramLabel}
            :   `testRuleTimeoutMs` - The value for testRuleTimeoutMs

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setTestRuleTimeoutMs(java.util.Optional)}

        -   #### setTestRuleTimeoutMs

            ``` methodSignature
            public final ShTestDescriptionArg.Builder setTestRuleTimeoutMs​(Optional<Long> testRuleTimeoutMs)
            ```

            ::: block
            Initializes the optional value
            [`testRuleTimeoutMs`](ShTestDescriptionArg.html#getTestRuleTimeoutMs())
            to testRuleTimeoutMs.
            :::

            [Parameters:]{.paramLabel}
            :   `testRuleTimeoutMs` - The value for testRuleTimeoutMs

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#build()}

        -   #### build

            ``` methodSignature
            public ShTestDescriptionArg build()
            ```

            ::: block
            Builds a new
            [`ShTestDescriptionArg`](ShTestDescriptionArg.html "class in com.facebook.buck.shell").
            :::

            [Returns:]{.returnLabel}
            :   An immutable instance of ShTestDescriptionArg

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
