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
[Package]{.packageLabelInType} [com.facebook.buck.features.ocaml](package-summary.html)
:::

## Class PrebuiltOcamlLibraryDescriptionArg.Builder {#class-prebuiltocamllibrarydescriptionarg.builder .title title="Class PrebuiltOcamlLibraryDescriptionArg.Builder"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.features.ocaml.PrebuiltOcamlLibraryDescriptionArg.Builder

::: description
-   

    Enclosing class:
    :   [PrebuiltOcamlLibraryDescriptionArg](PrebuiltOcamlLibraryDescriptionArg.html "class in com.facebook.buck.features.ocaml")

    ------------------------------------------------------------------------

        @NotThreadSafe
        public static final class PrebuiltOcamlLibraryDescriptionArg.Builder
        extends Object

    ::: block
    Builds instances of type
    [`PrebuiltOcamlLibraryDescriptionArg`](PrebuiltOcamlLibraryDescriptionArg.html "class in com.facebook.buck.features.ocaml").
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
        | `P                    | `addAl                | ::: block             |
        | rebuiltOcamlLibraryDe | lBytecodeCLibs​(Iterab | Adds elements to      |
        | scriptionArg.Builder` | le<String> elements)` | [`bytecodeCLib        |
        |                       |                       | s`](PrebuiltOcamlLibr |
        |                       |                       | aryDescriptionArg.htm |
        |                       |                       | l#getBytecodeCLibs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `P                    | `addAllCLibs​(Iterab   | ::: block             |
        | rebuiltOcamlLibraryDe | le<String> elements)` | Adds elements to      |
        | scriptionArg.Builder` |                       | [`cLibs`](PrebuiltO   |
        |                       |                       | camlLibraryDescriptio |
        |                       |                       | nArg.html#getCLibs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `P                    | `addAllCompat         | ::: block             |
        | rebuiltOcamlLibraryDe | ibleWith​(Iterable<? e | Adds elements to      |
        | scriptionArg.Builder` | xtends UnconfiguredBu | [`compatibleWith      |
        |                       | ildTarget> elements)` | `](PrebuiltOcamlLibra |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `P                    | `addAllDeps​(          | ::: block             |
        | rebuiltOcamlLibraryDe | Iterable<? extends Bu | Adds elements to      |
        | scriptionArg.Builder` | ildTarget> elements)` | [`deps`](Prebuilt     |
        |                       |                       | OcamlLibraryDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `P                    | `addAllLabels​(Iterab  | ::: block             |
        | rebuiltOcamlLibraryDe | le<String> elements)` | Adds elements to      |
        | scriptionArg.Builder` |                       | [`labels`](PrebuiltOc |
        |                       |                       | amlLibraryDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `P                    | `addAllLicenses       | ::: block             |
        | rebuiltOcamlLibraryDe | ​(Iterable<? extends S | Adds elements to      |
        | scriptionArg.Builder` | ourcePath> elements)` | [`li                  |
        |                       |                       | censes`](PrebuiltOcam |
        |                       |                       | lLibraryDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `P                    | `add                  | ::: block             |
        | rebuiltOcamlLibraryDe | AllNativeCLibs​(Iterab | Adds elements to      |
        | scriptionArg.Builder` | le<String> elements)` | [`nativeCL            |
        |                       |                       | ibs`](PrebuiltOcamlLi |
        |                       |                       | braryDescriptionArg.h |
        |                       |                       | tml#getNativeCLibs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `P                    | `addBytecodeC         | ::: block             |
        | rebuiltOcamlLibraryDe | Libs​(String element)` | Adds one element to   |
        | scriptionArg.Builder` |                       | [`bytecodeCLib        |
        |                       |                       | s`](PrebuiltOcamlLibr |
        |                       |                       | aryDescriptionArg.htm |
        |                       |                       | l#getBytecodeCLibs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `P                    | `addBytecodeCLibs     | ::: block             |
        | rebuiltOcamlLibraryDe | ​(String... elements)` | Adds elements to      |
        | scriptionArg.Builder` |                       | [`bytecodeCLib        |
        |                       |                       | s`](PrebuiltOcamlLibr |
        |                       |                       | aryDescriptionArg.htm |
        |                       |                       | l#getBytecodeCLibs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `P                    | `addC                 | ::: block             |
        | rebuiltOcamlLibraryDe | Libs​(String element)` | Adds one element to   |
        | scriptionArg.Builder` |                       | [`cLibs`](PrebuiltO   |
        |                       |                       | camlLibraryDescriptio |
        |                       |                       | nArg.html#getCLibs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `P                    | `addCLibs             | ::: block             |
        | rebuiltOcamlLibraryDe | ​(String... elements)` | Adds elements to      |
        | scriptionArg.Builder` |                       | [`cLibs`](PrebuiltO   |
        |                       |                       | camlLibraryDescriptio |
        |                       |                       | nArg.html#getCLibs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `P                    | `addCompat            | ::: block             |
        | rebuiltOcamlLibraryDe | ibleWith​(Unconfigured | Adds one element to   |
        | scriptionArg.Builder` | BuildTarget element)` | [`compatibleWith      |
        |                       |                       | `](PrebuiltOcamlLibra |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `P                    | `addCompatible        | ::: block             |
        | rebuiltOcamlLibraryDe | With​(UnconfiguredBuil | Adds elements to      |
        | scriptionArg.Builder` | dTarget... elements)` | [`compatibleWith      |
        |                       |                       | `](PrebuiltOcamlLibra |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `P                    | `addDeps​(             | ::: block             |
        | rebuiltOcamlLibraryDe | BuildTarget element)` | Adds one element to   |
        | scriptionArg.Builder` |                       | [`deps`](Prebuilt     |
        |                       |                       | OcamlLibraryDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `P                    | `addDeps​(Buil         | ::: block             |
        | rebuiltOcamlLibraryDe | dTarget... elements)` | Adds elements to      |
        | scriptionArg.Builder` |                       | [`deps`](Prebuilt     |
        |                       |                       | OcamlLibraryDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `P                    | `addLa                | ::: block             |
        | rebuiltOcamlLibraryDe | bels​(String element)` | Adds one element to   |
        | scriptionArg.Builder` |                       | [`labels`](PrebuiltOc |
        |                       |                       | amlLibraryDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `P                    | `addLabels            | ::: block             |
        | rebuiltOcamlLibraryDe | ​(String... elements)` | Adds elements to      |
        | scriptionArg.Builder` |                       | [`labels`](PrebuiltOc |
        |                       |                       | amlLibraryDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `P                    | `addLicenses          | ::: block             |
        | rebuiltOcamlLibraryDe | ​(SourcePath element)` | Adds one element to   |
        | scriptionArg.Builder` |                       | [`li                  |
        |                       |                       | censes`](PrebuiltOcam |
        |                       |                       | lLibraryDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `P                    | `addLicenses​(Sou      | ::: block             |
        | rebuiltOcamlLibraryDe | rcePath... elements)` | Adds elements to      |
        | scriptionArg.Builder` |                       | [`li                  |
        |                       |                       | censes`](PrebuiltOcam |
        |                       |                       | lLibraryDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `P                    | `addNativeC           | ::: block             |
        | rebuiltOcamlLibraryDe | Libs​(String element)` | Adds one element to   |
        | scriptionArg.Builder` |                       | [`nativeCL            |
        |                       |                       | ibs`](PrebuiltOcamlLi |
        |                       |                       | braryDescriptionArg.h |
        |                       |                       | tml#getNativeCLibs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `P                    | `addNativeCLibs       | ::: block             |
        | rebuiltOcamlLibraryDe | ​(String... elements)` | Adds elements to      |
        | scriptionArg.Builder` |                       | [`nativeCL            |
        |                       |                       | ibs`](PrebuiltOcamlLi |
        |                       |                       | braryDescriptionArg.h |
        |                       |                       | tml#getNativeCLibs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `PrebuiltOcamlL       | `build()`             | ::: block             |
        | ibraryDescriptionArg` |                       | Builds a new          |
        |                       |                       | [`PrebuiltOcamlLibr   |
        |                       |                       | aryDescriptionArg`](P |
        |                       |                       | rebuiltOcamlLibraryDe |
        |                       |                       | scriptionArg.html "cl |
        |                       |                       | ass in com.facebook.b |
        |                       |                       | uck.features.ocaml"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `P                    | `from​(Bu              | ::: block             |
        | rebuiltOcamlLibraryDe | ildRuleArg instance)` | Fill a builder with   |
        | scriptionArg.Builder` |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebo           |
        |                       |                       | ok.buck.core.descript |
        |                       |                       | ion.arg.BuildRuleArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `P                    | `from​(Cons            | ::: block             |
        | rebuiltOcamlLibraryDe | tructorArg instance)` | Fill a builder with   |
        | scriptionArg.Builder` |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook         |
        |                       |                       | .buck.core.descriptio |
        |                       |                       | n.arg.ConstructorArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `P                    | `from​(HasDe           | ::: block             |
        | rebuiltOcamlLibraryDe | claredDeps instance)` | Fill a builder with   |
        | scriptionArg.Builder` |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook.        |
        |                       |                       | buck.core.description |
        |                       |                       | .arg.HasDeclaredDeps` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `P                    | `from​(com.facebook.   | ::: block             |
        | rebuiltOcamlLibraryDe | buck.features.ocaml.P | Copy abstract value   |
        | scriptionArg.Builder` | rebuiltOcamlLibraryDe | type                  |
        |                       | scription.AbstractPre | `A                    |
        |                       | builtOcamlLibraryDesc | bstractPrebuiltOcamlL |
        |                       | riptionArg instance)` | ibraryDescriptionArg` |
        |                       |                       | instance into         |
        |                       |                       | builder.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `P                    | `from​(Pre             | ::: block             |
        | rebuiltOcamlLibraryDe | builtOcamlLibraryDesc | Fill a builder with   |
        | scriptionArg.Builder` | riptionArg instance)` | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `PrebuiltOcamlL       |
        |                       |                       | ibraryDescriptionArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `P                    | `se                   | ::: block             |
        | rebuiltOcamlLibraryDe | tBytecodeCLibs​(Iterab | Sets or replaces all  |
        | scriptionArg.Builder` | le<String> elements)` | elements for          |
        |                       |                       | [`bytecodeCLib        |
        |                       |                       | s`](PrebuiltOcamlLibr |
        |                       |                       | aryDescriptionArg.htm |
        |                       |                       | l#getBytecodeCLibs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `P                    | `setBytecodeLib       | ::: block             |
        | rebuiltOcamlLibraryDe | ​(String bytecodeLib)` | Initializes the value |
        | scriptionArg.Builder` |                       | for the               |
        |                       |                       | [`bytecode            |
        |                       |                       | Lib`](PrebuiltOcamlLi |
        |                       |                       | braryDescriptionArg.h |
        |                       |                       | tml#getBytecodeLib()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `P                    | `setBytecodeOnly​(b    | ::: block             |
        | rebuiltOcamlLibraryDe | oolean bytecodeOnly)` | Initializes the value |
        | scriptionArg.Builder` |                       | for the               |
        |                       |                       | [`bytecodeOn          |
        |                       |                       | ly`](PrebuiltOcamlLib |
        |                       |                       | raryDescriptionArg.ht |
        |                       |                       | ml#getBytecodeOnly()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `P                    | `setCLibs​(Iterab      | ::: block             |
        | rebuiltOcamlLibraryDe | le<String> elements)` | Sets or replaces all  |
        | scriptionArg.Builder` |                       | elements for          |
        |                       |                       | [`cLibs`](PrebuiltO   |
        |                       |                       | camlLibraryDescriptio |
        |                       |                       | nArg.html#getCLibs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `P                    | `setCompat            | ::: block             |
        | rebuiltOcamlLibraryDe | ibleWith​(Iterable<? e | Sets or replaces all  |
        | scriptionArg.Builder` | xtends UnconfiguredBu | elements for          |
        |                       | ildTarget> elements)` | [`compatibleWith      |
        |                       |                       | `](PrebuiltOcamlLibra |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `P                    | `setDefaul            | ::: block             |
        | rebuiltOcamlLibraryDe | tTargetPlatform​(Uncon | Initializes the       |
        | scriptionArg.Builder` | figuredBuildTarget de | optional value        |
        |                       | faultTargetPlatform)` | [`default             |
        |                       |                       | TargetPlatform`](Preb |
        |                       |                       | uiltOcamlLibraryDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `P                    | `setDefau             | ::: block             |
        | rebuiltOcamlLibraryDe | ltTargetPlatform​(Opti | Initializes the       |
        | scriptionArg.Builder` | onal<? extends Unconf | optional value        |
        |                       | iguredBuildTarget> de | [`default             |
        |                       | faultTargetPlatform)` | TargetPlatform`](Preb |
        |                       |                       | uiltOcamlLibraryDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `P                    | `setDeps​(             | ::: block             |
        | rebuiltOcamlLibraryDe | Iterable<? extends Bu | Sets or replaces all  |
        | scriptionArg.Builder` | ildTarget> elements)` | elements for          |
        |                       |                       | [`deps`](Prebuilt     |
        |                       |                       | OcamlLibraryDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `P                    | `setIncludeDi         | ::: block             |
        | rebuiltOcamlLibraryDe | r​(String includeDir)` | Initializes the value |
        | scriptionArg.Builder` |                       | for the               |
        |                       |                       | [`includ              |
        |                       |                       | eDir`](PrebuiltOcamlL |
        |                       |                       | ibraryDescriptionArg. |
        |                       |                       | html#getIncludeDir()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `P                    | `setLabels​(Iterab     | ::: block             |
        | rebuiltOcamlLibraryDe | le<String> elements)` | Sets or replaces all  |
        | scriptionArg.Builder` |                       | elements for          |
        |                       |                       | [`labels`](PrebuiltOc |
        |                       |                       | amlLibraryDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `P                    | `setL                 | ::: block             |
        | rebuiltOcamlLibraryDe | ibDir​(String libDir)` | Initializes the value |
        | scriptionArg.Builder` |                       | for the               |
        |                       |                       | [`libDir`](PrebuiltOc |
        |                       |                       | amlLibraryDescription |
        |                       |                       | Arg.html#getLibDir()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `P                    | `setLib               | ::: block             |
        | rebuiltOcamlLibraryDe | Name​(String libName)` | Initializes the value |
        | scriptionArg.Builder` |                       | for the               |
        |                       |                       | [`                    |
        |                       |                       | libName`](PrebuiltOca |
        |                       |                       | mlLibraryDescriptionA |
        |                       |                       | rg.html#getLibName()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `P                    | `setLicenses          | ::: block             |
        | rebuiltOcamlLibraryDe | ​(Iterable<? extends S | Sets or replaces all  |
        | scriptionArg.Builder` | ourcePath> elements)` | elements for          |
        |                       |                       | [`li                  |
        |                       |                       | censes`](PrebuiltOcam |
        |                       |                       | lLibraryDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `P                    | `                     | ::: block             |
        | rebuiltOcamlLibraryDe | setName​(String name)` | Initializes the value |
        | scriptionArg.Builder` |                       | for the               |
        |                       |                       | [`name`](Prebuilt     |
        |                       |                       | OcamlLibraryDescripti |
        |                       |                       | onArg.html#getName()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `P                    | `                     | ::: block             |
        | rebuiltOcamlLibraryDe | setNativeCLibs​(Iterab | Sets or replaces all  |
        | scriptionArg.Builder` | le<String> elements)` | elements for          |
        |                       |                       | [`nativeCL            |
        |                       |                       | ibs`](PrebuiltOcamlLi |
        |                       |                       | braryDescriptionArg.h |
        |                       |                       | tml#getNativeCLibs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `P                    | `setNativeL           | ::: block             |
        | rebuiltOcamlLibraryDe | ib​(String nativeLib)` | Initializes the value |
        | scriptionArg.Builder` |                       | for the               |
        |                       |                       | [`nati                |
        |                       |                       | veLib`](PrebuiltOcaml |
        |                       |                       | LibraryDescriptionArg |
        |                       |                       | .html#getNativeLib()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `P                    | `setPlatfo            | ::: block             |
        | rebuiltOcamlLibraryDe | rmDeps​(PatternMatched | Initializes the value |
        | scriptionArg.Builder` | Collection<com.google | for the               |
        |                       | .common.collect.Immut | [`platformDe          |
        |                       | ableSortedSet<BuildTa | ps`](PrebuiltOcamlLib |
        |                       | rget>> platformDeps)` | raryDescriptionArg.ht |
        |                       |                       | ml#getPlatformDeps()) |
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

        []{#from(com.facebook.buck.features.ocaml.PrebuiltOcamlLibraryDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final PrebuiltOcamlLibraryDescriptionArg.Builder from​(PrebuiltOcamlLibraryDescriptionArg instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `PrebuiltOcamlLibraryDescriptionArg` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.features.ocaml.PrebuiltOcamlLibraryDescription.AbstractPrebuiltOcamlLibraryDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final PrebuiltOcamlLibraryDescriptionArg.Builder from​(com.facebook.buck.features.ocaml.PrebuiltOcamlLibraryDescription.AbstractPrebuiltOcamlLibraryDescriptionArg instance)
            ```

            ::: block
            Copy abstract value type
            `AbstractPrebuiltOcamlLibraryDescriptionArg` instance into
            builder.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.core.description.arg.HasDeclaredDeps)}

        -   #### from

            ``` methodSignature
            public final PrebuiltOcamlLibraryDescriptionArg.Builder from​(HasDeclaredDeps instance)
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
            public final PrebuiltOcamlLibraryDescriptionArg.Builder from​(BuildRuleArg instance)
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
            public final PrebuiltOcamlLibraryDescriptionArg.Builder from​(ConstructorArg instance)
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

        []{#setLibDir(java.lang.String)}

        -   #### setLibDir

            ``` methodSignature
            public final PrebuiltOcamlLibraryDescriptionArg.Builder setLibDir​(String libDir)
            ```

            ::: block
            Initializes the value for the
            [`libDir`](PrebuiltOcamlLibraryDescriptionArg.html#getLibDir())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`libDir`](PrebuiltOcamlLibraryDescriptionArg.html#getLibDir()).*
            :::

            [Parameters:]{.paramLabel}
            :   `libDir` - The value for libDir

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setIncludeDir(java.lang.String)}

        -   #### setIncludeDir

            ``` methodSignature
            public final PrebuiltOcamlLibraryDescriptionArg.Builder setIncludeDir​(String includeDir)
            ```

            ::: block
            Initializes the value for the
            [`includeDir`](PrebuiltOcamlLibraryDescriptionArg.html#getIncludeDir())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`includeDir`](PrebuiltOcamlLibraryDescriptionArg.html#getIncludeDir()).*
            :::

            [Parameters:]{.paramLabel}
            :   `includeDir` - The value for includeDir

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLibName(java.lang.String)}

        -   #### setLibName

            ``` methodSignature
            public final PrebuiltOcamlLibraryDescriptionArg.Builder setLibName​(String libName)
            ```

            ::: block
            Initializes the value for the
            [`libName`](PrebuiltOcamlLibraryDescriptionArg.html#getLibName())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`libName`](PrebuiltOcamlLibraryDescriptionArg.html#getLibName()).*
            :::

            [Parameters:]{.paramLabel}
            :   `libName` - The value for libName

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setNativeLib(java.lang.String)}

        -   #### setNativeLib

            ``` methodSignature
            public final PrebuiltOcamlLibraryDescriptionArg.Builder setNativeLib​(String nativeLib)
            ```

            ::: block
            Initializes the value for the
            [`nativeLib`](PrebuiltOcamlLibraryDescriptionArg.html#getNativeLib())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`nativeLib`](PrebuiltOcamlLibraryDescriptionArg.html#getNativeLib()).*
            :::

            [Parameters:]{.paramLabel}
            :   `nativeLib` - The value for nativeLib

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setBytecodeLib(java.lang.String)}

        -   #### setBytecodeLib

            ``` methodSignature
            public final PrebuiltOcamlLibraryDescriptionArg.Builder setBytecodeLib​(String bytecodeLib)
            ```

            ::: block
            Initializes the value for the
            [`bytecodeLib`](PrebuiltOcamlLibraryDescriptionArg.html#getBytecodeLib())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`bytecodeLib`](PrebuiltOcamlLibraryDescriptionArg.html#getBytecodeLib()).*
            :::

            [Parameters:]{.paramLabel}
            :   `bytecodeLib` - The value for bytecodeLib

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCLibs(java.lang.String)}

        -   #### addCLibs

            ``` methodSignature
            public final PrebuiltOcamlLibraryDescriptionArg.Builder addCLibs​(String element)
            ```

            ::: block
            Adds one element to
            [`cLibs`](PrebuiltOcamlLibraryDescriptionArg.html#getCLibs())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A cLibs element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCLibs(java.lang.String...)}

        -   #### addCLibs

            ``` methodSignature
            public final PrebuiltOcamlLibraryDescriptionArg.Builder addCLibs​(String... elements)
            ```

            ::: block
            Adds elements to
            [`cLibs`](PrebuiltOcamlLibraryDescriptionArg.html#getCLibs())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of cLibs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCLibs(java.lang.Iterable)}

        -   #### setCLibs

            ``` methodSignature
            public final PrebuiltOcamlLibraryDescriptionArg.Builder setCLibs​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`cLibs`](PrebuiltOcamlLibraryDescriptionArg.html#getCLibs())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of cLibs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllCLibs(java.lang.Iterable)}

        -   #### addAllCLibs

            ``` methodSignature
            public final PrebuiltOcamlLibraryDescriptionArg.Builder addAllCLibs​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`cLibs`](PrebuiltOcamlLibraryDescriptionArg.html#getCLibs())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of cLibs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addNativeCLibs(java.lang.String)}

        -   #### addNativeCLibs

            ``` methodSignature
            public final PrebuiltOcamlLibraryDescriptionArg.Builder addNativeCLibs​(String element)
            ```

            ::: block
            Adds one element to
            [`nativeCLibs`](PrebuiltOcamlLibraryDescriptionArg.html#getNativeCLibs())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A nativeCLibs element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addNativeCLibs(java.lang.String...)}

        -   #### addNativeCLibs

            ``` methodSignature
            public final PrebuiltOcamlLibraryDescriptionArg.Builder addNativeCLibs​(String... elements)
            ```

            ::: block
            Adds elements to
            [`nativeCLibs`](PrebuiltOcamlLibraryDescriptionArg.html#getNativeCLibs())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of nativeCLibs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setNativeCLibs(java.lang.Iterable)}

        -   #### setNativeCLibs

            ``` methodSignature
            public final PrebuiltOcamlLibraryDescriptionArg.Builder setNativeCLibs​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`nativeCLibs`](PrebuiltOcamlLibraryDescriptionArg.html#getNativeCLibs())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of nativeCLibs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllNativeCLibs(java.lang.Iterable)}

        -   #### addAllNativeCLibs

            ``` methodSignature
            public final PrebuiltOcamlLibraryDescriptionArg.Builder addAllNativeCLibs​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`nativeCLibs`](PrebuiltOcamlLibraryDescriptionArg.html#getNativeCLibs())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of nativeCLibs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addBytecodeCLibs(java.lang.String)}

        -   #### addBytecodeCLibs

            ``` methodSignature
            public final PrebuiltOcamlLibraryDescriptionArg.Builder addBytecodeCLibs​(String element)
            ```

            ::: block
            Adds one element to
            [`bytecodeCLibs`](PrebuiltOcamlLibraryDescriptionArg.html#getBytecodeCLibs())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A bytecodeCLibs element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addBytecodeCLibs(java.lang.String...)}

        -   #### addBytecodeCLibs

            ``` methodSignature
            public final PrebuiltOcamlLibraryDescriptionArg.Builder addBytecodeCLibs​(String... elements)
            ```

            ::: block
            Adds elements to
            [`bytecodeCLibs`](PrebuiltOcamlLibraryDescriptionArg.html#getBytecodeCLibs())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of bytecodeCLibs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setBytecodeCLibs(java.lang.Iterable)}

        -   #### setBytecodeCLibs

            ``` methodSignature
            public final PrebuiltOcamlLibraryDescriptionArg.Builder setBytecodeCLibs​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`bytecodeCLibs`](PrebuiltOcamlLibraryDescriptionArg.html#getBytecodeCLibs())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of bytecodeCLibs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllBytecodeCLibs(java.lang.Iterable)}

        -   #### addAllBytecodeCLibs

            ``` methodSignature
            public final PrebuiltOcamlLibraryDescriptionArg.Builder addAllBytecodeCLibs​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`bytecodeCLibs`](PrebuiltOcamlLibraryDescriptionArg.html#getBytecodeCLibs())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of bytecodeCLibs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setBytecodeOnly(boolean)}

        -   #### setBytecodeOnly

            ``` methodSignature
            public final PrebuiltOcamlLibraryDescriptionArg.Builder setBytecodeOnly​(boolean bytecodeOnly)
            ```

            ::: block
            Initializes the value for the
            [`bytecodeOnly`](PrebuiltOcamlLibraryDescriptionArg.html#getBytecodeOnly())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`bytecodeOnly`](PrebuiltOcamlLibraryDescriptionArg.html#getBytecodeOnly()).*
            :::

            [Parameters:]{.paramLabel}
            :   `bytecodeOnly` - The value for bytecodeOnly

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPlatformDeps(com.facebook.buck.rules.coercer.PatternMatchedCollection)}

        -   #### setPlatformDeps

            ``` methodSignature
            public final PrebuiltOcamlLibraryDescriptionArg.Builder setPlatformDeps​(PatternMatchedCollection<com.google.common.collect.ImmutableSortedSet<BuildTarget>> platformDeps)
            ```

            ::: block
            Initializes the value for the
            [`platformDeps`](PrebuiltOcamlLibraryDescriptionArg.html#getPlatformDeps())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`platformDeps`](PrebuiltOcamlLibraryDescriptionArg.html#getPlatformDeps()).*
            :::

            [Parameters:]{.paramLabel}
            :   `platformDeps` - The value for platformDeps

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCompatibleWith(com.facebook.buck.core.model.UnconfiguredBuildTarget)}

        -   #### addCompatibleWith

            ``` methodSignature
            public final PrebuiltOcamlLibraryDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget element)
            ```

            ::: block
            Adds one element to
            [`compatibleWith`](PrebuiltOcamlLibraryDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A compatibleWith element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCompatibleWith(com.facebook.buck.core.model.UnconfiguredBuildTarget...)}

        -   #### addCompatibleWith

            ``` methodSignature
            public final PrebuiltOcamlLibraryDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](PrebuiltOcamlLibraryDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCompatibleWith(java.lang.Iterable)}

        -   #### setCompatibleWith

            ``` methodSignature
            public final PrebuiltOcamlLibraryDescriptionArg.Builder setCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`compatibleWith`](PrebuiltOcamlLibraryDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllCompatibleWith(java.lang.Iterable)}

        -   #### addAllCompatibleWith

            ``` methodSignature
            public final PrebuiltOcamlLibraryDescriptionArg.Builder addAllCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](PrebuiltOcamlLibraryDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDefaultTargetPlatform(com.facebook.buck.core.model.UnconfiguredBuildTarget)}

        -   #### setDefaultTargetPlatform

            ``` methodSignature
            public final PrebuiltOcamlLibraryDescriptionArg.Builder setDefaultTargetPlatform​(UnconfiguredBuildTarget defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](PrebuiltOcamlLibraryDescriptionArg.html#getDefaultTargetPlatform())
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
            public final PrebuiltOcamlLibraryDescriptionArg.Builder setDefaultTargetPlatform​(Optional<? extends UnconfiguredBuildTarget> defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](PrebuiltOcamlLibraryDescriptionArg.html#getDefaultTargetPlatform())
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
            public final PrebuiltOcamlLibraryDescriptionArg.Builder addLabels​(String element)
            ```

            ::: block
            Adds one element to
            [`labels`](PrebuiltOcamlLibraryDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A labels element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLabels(java.lang.String...)}

        -   #### addLabels

            ``` methodSignature
            public final PrebuiltOcamlLibraryDescriptionArg.Builder addLabels​(String... elements)
            ```

            ::: block
            Adds elements to
            [`labels`](PrebuiltOcamlLibraryDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLabels(java.lang.Iterable)}

        -   #### setLabels

            ``` methodSignature
            public final PrebuiltOcamlLibraryDescriptionArg.Builder setLabels​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`labels`](PrebuiltOcamlLibraryDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLabels(java.lang.Iterable)}

        -   #### addAllLabels

            ``` methodSignature
            public final PrebuiltOcamlLibraryDescriptionArg.Builder addAllLabels​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`labels`](PrebuiltOcamlLibraryDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLicenses(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### addLicenses

            ``` methodSignature
            public final PrebuiltOcamlLibraryDescriptionArg.Builder addLicenses​(SourcePath element)
            ```

            ::: block
            Adds one element to
            [`licenses`](PrebuiltOcamlLibraryDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A licenses element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLicenses(com.facebook.buck.core.sourcepath.SourcePath...)}

        -   #### addLicenses

            ``` methodSignature
            public final PrebuiltOcamlLibraryDescriptionArg.Builder addLicenses​(SourcePath... elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](PrebuiltOcamlLibraryDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLicenses(java.lang.Iterable)}

        -   #### setLicenses

            ``` methodSignature
            public final PrebuiltOcamlLibraryDescriptionArg.Builder setLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`licenses`](PrebuiltOcamlLibraryDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLicenses(java.lang.Iterable)}

        -   #### addAllLicenses

            ``` methodSignature
            public final PrebuiltOcamlLibraryDescriptionArg.Builder addAllLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](PrebuiltOcamlLibraryDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setName(java.lang.String)}

        -   #### setName

            ``` methodSignature
            public final PrebuiltOcamlLibraryDescriptionArg.Builder setName​(String name)
            ```

            ::: block
            Initializes the value for the
            [`name`](PrebuiltOcamlLibraryDescriptionArg.html#getName())
            attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `name` - The value for name

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addDeps(com.facebook.buck.core.model.BuildTarget)}

        -   #### addDeps

            ``` methodSignature
            public final PrebuiltOcamlLibraryDescriptionArg.Builder addDeps​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`deps`](PrebuiltOcamlLibraryDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A deps element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addDeps(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addDeps

            ``` methodSignature
            public final PrebuiltOcamlLibraryDescriptionArg.Builder addDeps​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`deps`](PrebuiltOcamlLibraryDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDeps(java.lang.Iterable)}

        -   #### setDeps

            ``` methodSignature
            public final PrebuiltOcamlLibraryDescriptionArg.Builder setDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`deps`](PrebuiltOcamlLibraryDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllDeps(java.lang.Iterable)}

        -   #### addAllDeps

            ``` methodSignature
            public final PrebuiltOcamlLibraryDescriptionArg.Builder addAllDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`deps`](PrebuiltOcamlLibraryDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#build()}

        -   #### build

            ``` methodSignature
            public PrebuiltOcamlLibraryDescriptionArg build()
            ```

            ::: block
            Builds a new
            [`PrebuiltOcamlLibraryDescriptionArg`](PrebuiltOcamlLibraryDescriptionArg.html "class in com.facebook.buck.features.ocaml").
            :::

            [Returns:]{.returnLabel}
            :   An immutable instance of
                PrebuiltOcamlLibraryDescriptionArg

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
