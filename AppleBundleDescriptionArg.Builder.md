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
[Package]{.packageLabelInType} [com.facebook.buck.apple](package-summary.html)
:::

## Class AppleBundleDescriptionArg.Builder {#class-applebundledescriptionarg.builder .title title="Class AppleBundleDescriptionArg.Builder"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.apple.AppleBundleDescriptionArg.Builder

::: description
-   

    Enclosing class:
    :   [AppleBundleDescriptionArg](AppleBundleDescriptionArg.html "class in com.facebook.buck.apple")

    ------------------------------------------------------------------------

        @NotThreadSafe
        public static final class AppleBundleDescriptionArg.Builder
        extends Object

    ::: block
    Builds instances of type
    [`AppleBundleDescriptionArg`](AppleBundleDescriptionArg.html "class in com.facebook.buck.apple").
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
        | `AppleBundleDe        | `addAl                | ::: block             |
        | scriptionArg.Builder` | lCodesignFlags​(Iterab | Adds elements to      |
        |                       | le<String> elements)` | [`cod                 |
        |                       |                       | esignFlags`](AppleBun |
        |                       |                       | dleDescriptionArg.htm |
        |                       |                       | l#getCodesignFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBundleDe        | `addAllCompat         | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Iterable<? e | Adds elements to      |
        |                       | xtends UnconfiguredBu | [`compa               |
        |                       | ildTarget> elements)` | tibleWith`](AppleBund |
        |                       |                       | leDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBundleDe        | `                     | ::: block             |
        | scriptionArg.Builder` | addAllContacts​(Iterab | Adds elements to      |
        |                       | le<String> elements)` | [`contacts`](App      |
        |                       |                       | leBundleDescriptionAr |
        |                       |                       | g.html#getContacts()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBundleDe        | `addAllDeps​(          | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Adds elements to      |
        |                       | ildTarget> elements)` | [`deps`]              |
        |                       |                       | (AppleBundleDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBundleDe        | `addAllLabels​(Iterab  | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Adds elements to      |
        |                       |                       | [`labels`](A          |
        |                       |                       | ppleBundleDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBundleDe        | `addAllLicenses       | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Adds elements to      |
        |                       | ourcePath> elements)` | [`licenses`](App      |
        |                       |                       | leBundleDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBundleDe        | `addAllTests​(         | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Adds elements to      |
        |                       | ildTarget> elements)` | [`tests`](            |
        |                       |                       | AppleBundleDescriptio |
        |                       |                       | nArg.html#getTests()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBundleDe        | `addCodesignF         | ::: block             |
        | scriptionArg.Builder` | lags​(String element)` | Adds one element to   |
        |                       |                       | [`cod                 |
        |                       |                       | esignFlags`](AppleBun |
        |                       |                       | dleDescriptionArg.htm |
        |                       |                       | l#getCodesignFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBundleDe        | `addCodesignFlags     | ::: block             |
        | scriptionArg.Builder` | ​(String... elements)` | Adds elements to      |
        |                       |                       | [`cod                 |
        |                       |                       | esignFlags`](AppleBun |
        |                       |                       | dleDescriptionArg.htm |
        |                       |                       | l#getCodesignFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBundleDe        | `addCompat            | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Unconfigured | Adds one element to   |
        |                       | BuildTarget element)` | [`compa               |
        |                       |                       | tibleWith`](AppleBund |
        |                       |                       | leDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBundleDe        | `addCompatible        | ::: block             |
        | scriptionArg.Builder` | With​(UnconfiguredBuil | Adds elements to      |
        |                       | dTarget... elements)` | [`compa               |
        |                       |                       | tibleWith`](AppleBund |
        |                       |                       | leDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBundleDe        | `addCont              | ::: block             |
        | scriptionArg.Builder` | acts​(String element)` | Adds one element to   |
        |                       |                       | [`contacts`](App      |
        |                       |                       | leBundleDescriptionAr |
        |                       |                       | g.html#getContacts()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBundleDe        | `addContacts          | ::: block             |
        | scriptionArg.Builder` | ​(String... elements)` | Adds elements to      |
        |                       |                       | [`contacts`](App      |
        |                       |                       | leBundleDescriptionAr |
        |                       |                       | g.html#getContacts()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBundleDe        | `addDeps​(             | ::: block             |
        | scriptionArg.Builder` | BuildTarget element)` | Adds one element to   |
        |                       |                       | [`deps`]              |
        |                       |                       | (AppleBundleDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBundleDe        | `addDeps​(Buil         | ::: block             |
        | scriptionArg.Builder` | dTarget... elements)` | Adds elements to      |
        |                       |                       | [`deps`]              |
        |                       |                       | (AppleBundleDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBundleDe        | `addLa                | ::: block             |
        | scriptionArg.Builder` | bels​(String element)` | Adds one element to   |
        |                       |                       | [`labels`](A          |
        |                       |                       | ppleBundleDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBundleDe        | `addLabels            | ::: block             |
        | scriptionArg.Builder` | ​(String... elements)` | Adds elements to      |
        |                       |                       | [`labels`](A          |
        |                       |                       | ppleBundleDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBundleDe        | `addLicenses          | ::: block             |
        | scriptionArg.Builder` | ​(SourcePath element)` | Adds one element to   |
        |                       |                       | [`licenses`](App      |
        |                       |                       | leBundleDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBundleDe        | `addLicenses​(Sou      | ::: block             |
        | scriptionArg.Builder` | rcePath... elements)` | Adds elements to      |
        |                       |                       | [`licenses`](App      |
        |                       |                       | leBundleDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBundleDe        | `addTests​(            | ::: block             |
        | scriptionArg.Builder` | BuildTarget element)` | Adds one element to   |
        |                       |                       | [`tests`](            |
        |                       |                       | AppleBundleDescriptio |
        |                       |                       | nArg.html#getTests()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBundleDe        | `addTests​(Buil        | ::: block             |
        | scriptionArg.Builder` | dTarget... elements)` | Adds elements to      |
        |                       |                       | [`tests`](            |
        |                       |                       | AppleBundleDescriptio |
        |                       |                       | nArg.html#getTests()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Apple                | `build()`             | ::: block             |
        | BundleDescriptionArg` |                       | Builds a new          |
        |                       |                       | [`AppleBundle         |
        |                       |                       | DescriptionArg`](Appl |
        |                       |                       | eBundleDescriptionArg |
        |                       |                       | .html "class in com.f |
        |                       |                       | acebook.buck.apple"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBundleDe        | `from​(com.fac         | ::: block             |
        | scriptionArg.Builder` | ebook.buck.apple.Appl | Copy abstract value   |
        |                       | eBundleDescription.Ab | type                  |
        |                       | stractAppleBundleDesc | `AbstractApple        |
        |                       | riptionArg instance)` | BundleDescriptionArg` |
        |                       |                       | instance into         |
        |                       |                       | builder.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBundleDe        | `from​(AppleBundleDesc | ::: block             |
        | scriptionArg.Builder` | riptionArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `Apple                |
        |                       |                       | BundleDescriptionArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBundleDe        | `from​(HasAppleBu      | ::: block             |
        | scriptionArg.Builder` | ndleFields instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com                  |
        |                       |                       | .facebook.buck.apple. |
        |                       |                       | HasAppleBundleFields` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBundleDe        | `from​(HasAppleCode    | ::: block             |
        | scriptionArg.Builder` | signFields instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.f                |
        |                       |                       | acebook.buck.apple.Ha |
        |                       |                       | sAppleCodesignFields` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBundleDe        | `from​(Bu              | ::: block             |
        | scriptionArg.Builder` | ildRuleArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebo           |
        |                       |                       | ok.buck.core.descript |
        |                       |                       | ion.arg.BuildRuleArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBundleDe        | `from​(Cons            | ::: block             |
        | scriptionArg.Builder` | tructorArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook         |
        |                       |                       | .buck.core.descriptio |
        |                       |                       | n.arg.ConstructorArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBundleDe        | `from​(H               | ::: block             |
        | scriptionArg.Builder` | asContacts instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.faceb            |
        |                       |                       | ook.buck.core.descrip |
        |                       |                       | tion.arg.HasContacts` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBundleDe        | `from​(HasDe           | ::: block             |
        | scriptionArg.Builder` | claredDeps instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook.        |
        |                       |                       | buck.core.description |
        |                       |                       | .arg.HasDeclaredDeps` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBundleDe        | `from​(HasDefau        | ::: block             |
        | scriptionArg.Builder` | ltPlatform instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook.buc     |
        |                       |                       | k.core.description.ar |
        |                       |                       | g.HasDefaultPlatform` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBundleDe        | `fro                  | ::: block             |
        | scriptionArg.Builder` | m​(HasTests instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.fa               |
        |                       |                       | cebook.buck.core.desc |
        |                       |                       | ription.arg.HasTests` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBundleDe        | `putA                 | ::: block             |
        | scriptionArg.Builder` | llInfoPlistSubstituti | Put all mappings from |
        |                       | ons​(Map<String,​? exte | the specified map as  |
        |                       | nds String> entries)` | entries to            |
        |                       |                       | [`                    |
        |                       |                       | infoPlistSubstitution |
        |                       |                       | s`](AppleBundleDescri |
        |                       |                       | ptionArg.html#getInfo |
        |                       |                       | PlistSubstitutions()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBundleDe        | `putInfoPlistSu       | ::: block             |
        | scriptionArg.Builder` | bstitutions​(String ke | Put one entry to the  |
        |                       | y,                    | [`                    |
        |                       |        String value)` | infoPlistSubstitution |
        |                       |                       | s`](AppleBundleDescri |
        |                       |                       | ptionArg.html#getInfo |
        |                       |                       | PlistSubstitutions()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBundleDe        | `putIn                | ::: block             |
        | scriptionArg.Builder` | foPlistSubstitutions​( | Put one entry to the  |
        |                       | Map.Entry<String,​? ex | [`                    |
        |                       | tends String> entry)` | infoPlistSubstitution |
        |                       |                       | s`](AppleBundleDescri |
        |                       |                       | ptionArg.html#getInfo |
        |                       |                       | PlistSubstitutions()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBundleDe        | `                     | ::: block             |
        | scriptionArg.Builder` | setAssetCatalogsCompi | Initializes the value |
        |                       | lationOptions​(AppleAs | for the               |
        |                       | setCatalogsCompilatio | [`assetCatalogsCompi  |
        |                       | nOptions assetCatalog | lationOptions`](Apple |
        |                       | sCompilationOptions)` | BundleDescriptionArg. |
        |                       |                       | html#getAssetCatalogs |
        |                       |                       | CompilationOptions()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBundleDe        | `setBinary            | ::: block             |
        | scriptionArg.Builder` | ​(BuildTarget binary)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`binary`](A          |
        |                       |                       | ppleBundleDescription |
        |                       |                       | Arg.html#getBinary()) |
        |                       |                       | to binary.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBundleDe        | `setBinar             | ::: block             |
        | scriptionArg.Builder` | y​(Optional<? extends  | Initializes the       |
        |                       | BuildTarget> binary)` | optional value        |
        |                       |                       | [`binary`](A          |
        |                       |                       | ppleBundleDescription |
        |                       |                       | Arg.html#getBinary()) |
        |                       |                       | to binary.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBundleDe        | `se                   | ::: block             |
        | scriptionArg.Builder` | tCodesignFlags​(Iterab | Sets or replaces all  |
        |                       | le<String> elements)` | elements for          |
        |                       |                       | [`cod                 |
        |                       |                       | esignFlags`](AppleBun |
        |                       |                       | dleDescriptionArg.htm |
        |                       |                       | l#getCodesignFlags()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBundleDe        | `set                  | ::: block             |
        | scriptionArg.Builder` | CodesignIdentity​(Stri | Initializes the       |
        |                       | ng codesignIdentity)` | optional value        |
        |                       |                       | [`codesignI           |
        |                       |                       | dentity`](AppleBundle |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etCodesignIdentity()) |
        |                       |                       | to codesignIdentity.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBundleDe        | `setCodesignId        | ::: block             |
        | scriptionArg.Builder` | entity​(Optional<Strin | Initializes the       |
        |                       | g> codesignIdentity)` | optional value        |
        |                       |                       | [`codesignI           |
        |                       |                       | dentity`](AppleBundle |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etCodesignIdentity()) |
        |                       |                       | to codesignIdentity.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBundleDe        | `setCompat            | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Iterable<? e | Sets or replaces all  |
        |                       | xtends UnconfiguredBu | elements for          |
        |                       | ildTarget> elements)` | [`compa               |
        |                       |                       | tibleWith`](AppleBund |
        |                       |                       | leDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBundleDe        | `setContacts​(Iterab   | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Sets or replaces all  |
        |                       |                       | elements for          |
        |                       |                       | [`contacts`](App      |
        |                       |                       | leBundleDescriptionAr |
        |                       |                       | g.html#getContacts()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBundleDe        | `s                    | ::: block             |
        | scriptionArg.Builder` | etDefaultPlatform​(Fla | Initializes the       |
        |                       | vor defaultPlatform)` | optional value        |
        |                       |                       | [`default             |
        |                       |                       | Platform`](AppleBundl |
        |                       |                       | eDescriptionArg.html# |
        |                       |                       | getDefaultPlatform()) |
        |                       |                       | to defaultPlatform.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBundleDe        | `                     | ::: block             |
        | scriptionArg.Builder` | setDefaultPlatform​(Op | Initializes the       |
        |                       | tional<? extends Flav | optional value        |
        |                       | or> defaultPlatform)` | [`default             |
        |                       |                       | Platform`](AppleBundl |
        |                       |                       | eDescriptionArg.html# |
        |                       |                       | getDefaultPlatform()) |
        |                       |                       | to defaultPlatform.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBundleDe        | `setDefaul            | ::: block             |
        | scriptionArg.Builder` | tTargetPlatform​(Uncon | Initializes the       |
        |                       | figuredBuildTarget de | optional value        |
        |                       | faultTargetPlatform)` | [`defaultTargetPlatfo |
        |                       |                       | rm`](AppleBundleDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBundleDe        | `setDefau             | ::: block             |
        | scriptionArg.Builder` | ltTargetPlatform​(Opti | Initializes the       |
        |                       | onal<? extends Unconf | optional value        |
        |                       | iguredBuildTarget> de | [`defaultTargetPlatfo |
        |                       | faultTargetPlatform)` | rm`](AppleBundleDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBundleDe        | `setDeps​(             | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Sets or replaces all  |
        |                       | ildTarget> elements)` | elements for          |
        |                       |                       | [`deps`]              |
        |                       |                       | (AppleBundleDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBundleDe        | `setExtension​(Eithe   | ::: block             |
        | scriptionArg.Builder` | r<AppleBundleExtensio | Initializes the value |
        |                       | n,​String> extension)` | for the               |
        |                       |                       | [`extension`](Appl    |
        |                       |                       | eBundleDescriptionArg |
        |                       |                       | .html#getExtension()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBundleDe        | `setIbtoolFlag        | ::: block             |
        | scriptionArg.Builder` | s​(com.google.common.c | Initializes the       |
        |                       | ollect.ImmutableList< | optional value        |
        |                       | String> ibtoolFlags)` | [                     |
        |                       |                       | `ibtoolFlags`](AppleB |
        |                       |                       | undleDescriptionArg.h |
        |                       |                       | tml#getIbtoolFlags()) |
        |                       |                       | to ibtoolFlags.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBundleDe        | `setIbtoolFla         | ::: block             |
        | scriptionArg.Builder` | gs​(Optional<? extends | Initializes the       |
        |                       |  com.google.common.co | optional value        |
        |                       | llect.ImmutableList<S | [                     |
        |                       | tring>> ibtoolFlags)` | `ibtoolFlags`](AppleB |
        |                       |                       | undleDescriptionArg.h |
        |                       |                       | tml#getIbtoolFlags()) |
        |                       |                       | to ibtoolFlags.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBundleDe        | `setI                 | ::: block             |
        | scriptionArg.Builder` | btoolModuleFlag​(boole | Initializes the       |
        |                       | an ibtoolModuleFlag)` | optional value        |
        |                       |                       | [`ibtoolMod           |
        |                       |                       | uleFlag`](AppleBundle |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etIbtoolModuleFlag()) |
        |                       |                       | to ibtoolModuleFlag.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBundleDe        | `setIbtoolModul       | ::: block             |
        | scriptionArg.Builder` | eFlag​(Optional<Boolea | Initializes the       |
        |                       | n> ibtoolModuleFlag)` | optional value        |
        |                       |                       | [`ibtoolMod           |
        |                       |                       | uleFlag`](AppleBundle |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etIbtoolModuleFlag()) |
        |                       |                       | to ibtoolModuleFlag.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBundleDe        | `setInfoPlist​(S       | ::: block             |
        | scriptionArg.Builder` | ourcePath infoPlist)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`infoPlist`](Appl    |
        |                       |                       | eBundleDescriptionArg |
        |                       |                       | .html#getInfoPlist()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBundleDe        | `s                    | ::: block             |
        | scriptionArg.Builder` | etInfoPlistSubstituti | Sets or replaces all  |
        |                       | ons​(Map<String,​? exte | mappings from the     |
        |                       | nds String> entries)` | specified map as      |
        |                       |                       | entries for the       |
        |                       |                       | [`                    |
        |                       |                       | infoPlistSubstitution |
        |                       |                       | s`](AppleBundleDescri |
        |                       |                       | ptionArg.html#getInfo |
        |                       |                       | PlistSubstitutions()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBundleDe        | `setIsAppCli          | ::: block             |
        | scriptionArg.Builder` | p​(boolean isAppClip)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`isAppClip`](Appl    |
        |                       |                       | eBundleDescriptionArg |
        |                       |                       | .html#getIsAppClip()) |
        |                       |                       | to isAppClip.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBundleDe        | `                     | ::: block             |
        | scriptionArg.Builder` | setIsAppClip​(Optional | Initializes the       |
        |                       | <Boolean> isAppClip)` | optional value        |
        |                       |                       | [`isAppClip`](Appl    |
        |                       |                       | eBundleDescriptionArg |
        |                       |                       | .html#getIsAppClip()) |
        |                       |                       | to isAppClip.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBundleDe        | `setLabels​(Iterab     | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Sets or replaces all  |
        |                       |                       | elements for          |
        |                       |                       | [`labels`](A          |
        |                       |                       | ppleBundleDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBundleDe        | `setLicenses          | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Sets or replaces all  |
        |                       | ourcePath> elements)` | elements for          |
        |                       |                       | [`licenses`](App      |
        |                       |                       | leBundleDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBundleDe        | `                     | ::: block             |
        | scriptionArg.Builder` | setName​(String name)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`name`]              |
        |                       |                       | (AppleBundleDescripti |
        |                       |                       | onArg.html#getName()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBundleDe        | `setPlatfo            | ::: block             |
        | scriptionArg.Builder` | rmBinary​(PatternMatch | Initializes the       |
        |                       | edCollection<BuildTar | optional value        |
        |                       | get> platformBinary)` | [`platf               |
        |                       |                       | ormBinary`](AppleBund |
        |                       |                       | leDescriptionArg.html |
        |                       |                       | #getPlatformBinary()) |
        |                       |                       | to platformBinary.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBundleDe        | `setPlatf             | ::: block             |
        | scriptionArg.Builder` | ormBinary​(Optional<?  | Initializes the       |
        |                       | extends PatternMatche | optional value        |
        |                       | dCollection<BuildTarg | [`platf               |
        |                       | et>> platformBinary)` | ormBinary`](AppleBund |
        |                       |                       | leDescriptionArg.html |
        |                       |                       | #getPlatformBinary()) |
        |                       |                       | to platformBinary.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBundleDe        | `setProductName       | ::: block             |
        | scriptionArg.Builder` | ​(String productName)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [                     |
        |                       |                       | `productName`](AppleB |
        |                       |                       | undleDescriptionArg.h |
        |                       |                       | tml#getProductName()) |
        |                       |                       | to productName.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBundleDe        | `set                  | ::: block             |
        | scriptionArg.Builder` | ProductName​(Optional< | Initializes the       |
        |                       | String> productName)` | optional value        |
        |                       |                       | [                     |
        |                       |                       | `productName`](AppleB |
        |                       |                       | undleDescriptionArg.h |
        |                       |                       | tml#getProductName()) |
        |                       |                       | to productName.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBundleDe        | `setResourceGroup​(S   | ::: block             |
        | scriptionArg.Builder` | tring resourceGroup)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`res                 |
        |                       |                       | ourceGroup`](AppleBun |
        |                       |                       | dleDescriptionArg.htm |
        |                       |                       | l#getResourceGroup()) |
        |                       |                       | to resourceGroup.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBundleDe        | `setReso              | ::: block             |
        | scriptionArg.Builder` | urceGroup​(Optional<St | Initializes the       |
        |                       | ring> resourceGroup)` | optional value        |
        |                       |                       | [`res                 |
        |                       |                       | ourceGroup`](AppleBun |
        |                       |                       | dleDescriptionArg.htm |
        |                       |                       | l#getResourceGroup()) |
        |                       |                       | to resourceGroup.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBundleDe        | `setResourceGrou      | ::: block             |
        | scriptionArg.Builder` | pMap​(com.google.commo | Initializes the       |
        |                       | n.collect.ImmutableLi | optional value        |
        |                       | st<CxxLinkGroupMappin | [`resourceG           |
        |                       | g> resourceGroupMap)` | roupMap`](AppleBundle |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etResourceGroupMap()) |
        |                       |                       | to resourceGroupMap.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBundleDe        | `setResourceGro       | ::: block             |
        | scriptionArg.Builder` | upMap​(Optional<? exte | Initializes the       |
        |                       | nds com.google.common | optional value        |
        |                       | .collect.ImmutableLis | [`resourceG           |
        |                       | t<CxxLinkGroupMapping | roupMap`](AppleBundle |
        |                       | >> resourceGroupMap)` | DescriptionArg.html#g |
        |                       |                       | etResourceGroupMap()) |
        |                       |                       | to resourceGroupMap.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBundleDe        | `setTests​(            | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Sets or replaces all  |
        |                       | ildTarget> elements)` | elements for          |
        |                       |                       | [`tests`](            |
        |                       |                       | AppleBundleDescriptio |
        |                       |                       | nArg.html#getTests()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBundleDe        | `set                  | ::: block             |
        | scriptionArg.Builder` | XcodeProductType​(Stri | Initializes the       |
        |                       | ng xcodeProductType)` | optional value        |
        |                       |                       | [`xcodeProd           |
        |                       |                       | uctType`](AppleBundle |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etXcodeProductType()) |
        |                       |                       | to xcodeProductType.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AppleBundleDe        | `setXcodeProdu        | ::: block             |
        | scriptionArg.Builder` | ctType​(Optional<Strin | Initializes the       |
        |                       | g> xcodeProductType)` | optional value        |
        |                       |                       | [`xcodeProd           |
        |                       |                       | uctType`](AppleBundle |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etXcodeProductType()) |
        |                       |                       | to xcodeProductType.  |
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

        []{#from(com.facebook.buck.apple.HasAppleBundleFields)}

        -   #### from

            ``` methodSignature
            public final AppleBundleDescriptionArg.Builder from​(HasAppleBundleFields instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `com.facebook.buck.apple.HasAppleBundleFields` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.core.description.arg.HasDeclaredDeps)}

        -   #### from

            ``` methodSignature
            public final AppleBundleDescriptionArg.Builder from​(HasDeclaredDeps instance)
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
            public final AppleBundleDescriptionArg.Builder from​(HasTests instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `com.facebook.buck.core.description.arg.HasTests` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.apple.AppleBundleDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final AppleBundleDescriptionArg.Builder from​(AppleBundleDescriptionArg instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `AppleBundleDescriptionArg` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.apple.AppleBundleDescription.AbstractAppleBundleDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final AppleBundleDescriptionArg.Builder from​(com.facebook.buck.apple.AppleBundleDescription.AbstractAppleBundleDescriptionArg instance)
            ```

            ::: block
            Copy abstract value type `AbstractAppleBundleDescriptionArg`
            instance into builder.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.core.description.arg.HasDefaultPlatform)}

        -   #### from

            ``` methodSignature
            public final AppleBundleDescriptionArg.Builder from​(HasDefaultPlatform instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `com.facebook.buck.core.description.arg.HasDefaultPlatform`
            instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.apple.HasAppleCodesignFields)}

        -   #### from

            ``` methodSignature
            public final AppleBundleDescriptionArg.Builder from​(HasAppleCodesignFields instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `com.facebook.buck.apple.HasAppleCodesignFields` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.core.description.arg.BuildRuleArg)}

        -   #### from

            ``` methodSignature
            public final AppleBundleDescriptionArg.Builder from​(BuildRuleArg instance)
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
            public final AppleBundleDescriptionArg.Builder from​(HasContacts instance)
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
            public final AppleBundleDescriptionArg.Builder from​(ConstructorArg instance)
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

        []{#setBinary(com.facebook.buck.core.model.BuildTarget)}

        -   #### setBinary

            ``` methodSignature
            public final AppleBundleDescriptionArg.Builder setBinary​(BuildTarget binary)
            ```

            ::: block
            Initializes the optional value
            [`binary`](AppleBundleDescriptionArg.html#getBinary()) to
            binary.
            :::

            [Parameters:]{.paramLabel}
            :   `binary` - The value for binary

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setBinary(java.util.Optional)}

        -   #### setBinary

            ``` methodSignature
            public final AppleBundleDescriptionArg.Builder setBinary​(Optional<? extends BuildTarget> binary)
            ```

            ::: block
            Initializes the optional value
            [`binary`](AppleBundleDescriptionArg.html#getBinary()) to
            binary.
            :::

            [Parameters:]{.paramLabel}
            :   `binary` - The value for binary

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPlatformBinary(com.facebook.buck.rules.coercer.PatternMatchedCollection)}

        -   #### setPlatformBinary

            ``` methodSignature
            public final AppleBundleDescriptionArg.Builder setPlatformBinary​(PatternMatchedCollection<BuildTarget> platformBinary)
            ```

            ::: block
            Initializes the optional value
            [`platformBinary`](AppleBundleDescriptionArg.html#getPlatformBinary())
            to platformBinary.
            :::

            [Parameters:]{.paramLabel}
            :   `platformBinary` - The value for platformBinary

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setPlatformBinary(java.util.Optional)}

        -   #### setPlatformBinary

            ``` methodSignature
            public final AppleBundleDescriptionArg.Builder setPlatformBinary​(Optional<? extends PatternMatchedCollection<BuildTarget>> platformBinary)
            ```

            ::: block
            Initializes the optional value
            [`platformBinary`](AppleBundleDescriptionArg.html#getPlatformBinary())
            to platformBinary.
            :::

            [Parameters:]{.paramLabel}
            :   `platformBinary` - The value for platformBinary

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setIbtoolModuleFlag(boolean)}

        -   #### setIbtoolModuleFlag

            ``` methodSignature
            public final AppleBundleDescriptionArg.Builder setIbtoolModuleFlag​(boolean ibtoolModuleFlag)
            ```

            ::: block
            Initializes the optional value
            [`ibtoolModuleFlag`](AppleBundleDescriptionArg.html#getIbtoolModuleFlag())
            to ibtoolModuleFlag.
            :::

            [Parameters:]{.paramLabel}
            :   `ibtoolModuleFlag` - The value for ibtoolModuleFlag

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setIbtoolModuleFlag(java.util.Optional)}

        -   #### setIbtoolModuleFlag

            ``` methodSignature
            public final AppleBundleDescriptionArg.Builder setIbtoolModuleFlag​(Optional<Boolean> ibtoolModuleFlag)
            ```

            ::: block
            Initializes the optional value
            [`ibtoolModuleFlag`](AppleBundleDescriptionArg.html#getIbtoolModuleFlag())
            to ibtoolModuleFlag.
            :::

            [Parameters:]{.paramLabel}
            :   `ibtoolModuleFlag` - The value for ibtoolModuleFlag

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setIbtoolFlags(com.google.common.collect.ImmutableList)}

        -   #### setIbtoolFlags

            ``` methodSignature
            public final AppleBundleDescriptionArg.Builder setIbtoolFlags​(com.google.common.collect.ImmutableList<String> ibtoolFlags)
            ```

            ::: block
            Initializes the optional value
            [`ibtoolFlags`](AppleBundleDescriptionArg.html#getIbtoolFlags())
            to ibtoolFlags.
            :::

            [Parameters:]{.paramLabel}
            :   `ibtoolFlags` - The value for ibtoolFlags

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setIbtoolFlags(java.util.Optional)}

        -   #### setIbtoolFlags

            ``` methodSignature
            public final AppleBundleDescriptionArg.Builder setIbtoolFlags​(Optional<? extends com.google.common.collect.ImmutableList<String>> ibtoolFlags)
            ```

            ::: block
            Initializes the optional value
            [`ibtoolFlags`](AppleBundleDescriptionArg.html#getIbtoolFlags())
            to ibtoolFlags.
            :::

            [Parameters:]{.paramLabel}
            :   `ibtoolFlags` - The value for ibtoolFlags

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setResourceGroupMap(com.google.common.collect.ImmutableList)}

        -   #### setResourceGroupMap

            ``` methodSignature
            public final AppleBundleDescriptionArg.Builder setResourceGroupMap​(com.google.common.collect.ImmutableList<CxxLinkGroupMapping> resourceGroupMap)
            ```

            ::: block
            Initializes the optional value
            [`resourceGroupMap`](AppleBundleDescriptionArg.html#getResourceGroupMap())
            to resourceGroupMap.
            :::

            [Parameters:]{.paramLabel}
            :   `resourceGroupMap` - The value for resourceGroupMap

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setResourceGroupMap(java.util.Optional)}

        -   #### setResourceGroupMap

            ``` methodSignature
            public final AppleBundleDescriptionArg.Builder setResourceGroupMap​(Optional<? extends com.google.common.collect.ImmutableList<CxxLinkGroupMapping>> resourceGroupMap)
            ```

            ::: block
            Initializes the optional value
            [`resourceGroupMap`](AppleBundleDescriptionArg.html#getResourceGroupMap())
            to resourceGroupMap.
            :::

            [Parameters:]{.paramLabel}
            :   `resourceGroupMap` - The value for resourceGroupMap

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setResourceGroup(java.lang.String)}

        -   #### setResourceGroup

            ``` methodSignature
            public final AppleBundleDescriptionArg.Builder setResourceGroup​(String resourceGroup)
            ```

            ::: block
            Initializes the optional value
            [`resourceGroup`](AppleBundleDescriptionArg.html#getResourceGroup())
            to resourceGroup.
            :::

            [Parameters:]{.paramLabel}
            :   `resourceGroup` - The value for resourceGroup

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setResourceGroup(java.util.Optional)}

        -   #### setResourceGroup

            ``` methodSignature
            public final AppleBundleDescriptionArg.Builder setResourceGroup​(Optional<String> resourceGroup)
            ```

            ::: block
            Initializes the optional value
            [`resourceGroup`](AppleBundleDescriptionArg.html#getResourceGroup())
            to resourceGroup.
            :::

            [Parameters:]{.paramLabel}
            :   `resourceGroup` - The value for resourceGroup

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addDeps(com.facebook.buck.core.model.BuildTarget)}

        -   #### addDeps

            ``` methodSignature
            public final AppleBundleDescriptionArg.Builder addDeps​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`deps`](AppleBundleDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A deps element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addDeps(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addDeps

            ``` methodSignature
            public final AppleBundleDescriptionArg.Builder addDeps​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`deps`](AppleBundleDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDeps(java.lang.Iterable)}

        -   #### setDeps

            ``` methodSignature
            public final AppleBundleDescriptionArg.Builder setDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`deps`](AppleBundleDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllDeps(java.lang.Iterable)}

        -   #### addAllDeps

            ``` methodSignature
            public final AppleBundleDescriptionArg.Builder addAllDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`deps`](AppleBundleDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLicenses(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### addLicenses

            ``` methodSignature
            public final AppleBundleDescriptionArg.Builder addLicenses​(SourcePath element)
            ```

            ::: block
            Adds one element to
            [`licenses`](AppleBundleDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A licenses element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLicenses(com.facebook.buck.core.sourcepath.SourcePath...)}

        -   #### addLicenses

            ``` methodSignature
            public final AppleBundleDescriptionArg.Builder addLicenses​(SourcePath... elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](AppleBundleDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLicenses(java.lang.Iterable)}

        -   #### setLicenses

            ``` methodSignature
            public final AppleBundleDescriptionArg.Builder setLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`licenses`](AppleBundleDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLicenses(java.lang.Iterable)}

        -   #### addAllLicenses

            ``` methodSignature
            public final AppleBundleDescriptionArg.Builder addAllLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](AppleBundleDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLabels(java.lang.String)}

        -   #### addLabels

            ``` methodSignature
            public final AppleBundleDescriptionArg.Builder addLabels​(String element)
            ```

            ::: block
            Adds one element to
            [`labels`](AppleBundleDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A labels element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLabels(java.lang.String...)}

        -   #### addLabels

            ``` methodSignature
            public final AppleBundleDescriptionArg.Builder addLabels​(String... elements)
            ```

            ::: block
            Adds elements to
            [`labels`](AppleBundleDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLabels(java.lang.Iterable)}

        -   #### setLabels

            ``` methodSignature
            public final AppleBundleDescriptionArg.Builder setLabels​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`labels`](AppleBundleDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLabels(java.lang.Iterable)}

        -   #### addAllLabels

            ``` methodSignature
            public final AppleBundleDescriptionArg.Builder addAllLabels​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`labels`](AppleBundleDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDefaultTargetPlatform(com.facebook.buck.core.model.UnconfiguredBuildTarget)}

        -   #### setDefaultTargetPlatform

            ``` methodSignature
            public final AppleBundleDescriptionArg.Builder setDefaultTargetPlatform​(UnconfiguredBuildTarget defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](AppleBundleDescriptionArg.html#getDefaultTargetPlatform())
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
            public final AppleBundleDescriptionArg.Builder setDefaultTargetPlatform​(Optional<? extends UnconfiguredBuildTarget> defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](AppleBundleDescriptionArg.html#getDefaultTargetPlatform())
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
            public final AppleBundleDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget element)
            ```

            ::: block
            Adds one element to
            [`compatibleWith`](AppleBundleDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A compatibleWith element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCompatibleWith(com.facebook.buck.core.model.UnconfiguredBuildTarget...)}

        -   #### addCompatibleWith

            ``` methodSignature
            public final AppleBundleDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](AppleBundleDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCompatibleWith(java.lang.Iterable)}

        -   #### setCompatibleWith

            ``` methodSignature
            public final AppleBundleDescriptionArg.Builder setCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`compatibleWith`](AppleBundleDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllCompatibleWith(java.lang.Iterable)}

        -   #### addAllCompatibleWith

            ``` methodSignature
            public final AppleBundleDescriptionArg.Builder addAllCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](AppleBundleDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setName(java.lang.String)}

        -   #### setName

            ``` methodSignature
            public final AppleBundleDescriptionArg.Builder setName​(String name)
            ```

            ::: block
            Initializes the value for the
            [`name`](AppleBundleDescriptionArg.html#getName())
            attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `name` - The value for name

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setExtension(com.facebook.buck.util.types.Either)}

        -   #### setExtension

            ``` methodSignature
            public final AppleBundleDescriptionArg.Builder setExtension​(Either<AppleBundleExtension,​String> extension)
            ```

            ::: block
            Initializes the value for the
            [`extension`](AppleBundleDescriptionArg.html#getExtension())
            attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `extension` - The value for extension

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setInfoPlist(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setInfoPlist

            ``` methodSignature
            public final AppleBundleDescriptionArg.Builder setInfoPlist​(SourcePath infoPlist)
            ```

            ::: block
            Initializes the value for the
            [`infoPlist`](AppleBundleDescriptionArg.html#getInfoPlist())
            attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `infoPlist` - The value for infoPlist

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setProductName(java.lang.String)}

        -   #### setProductName

            ``` methodSignature
            public final AppleBundleDescriptionArg.Builder setProductName​(String productName)
            ```

            ::: block
            Initializes the optional value
            [`productName`](AppleBundleDescriptionArg.html#getProductName())
            to productName.
            :::

            [Parameters:]{.paramLabel}
            :   `productName` - The value for productName

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setProductName(java.util.Optional)}

        -   #### setProductName

            ``` methodSignature
            public final AppleBundleDescriptionArg.Builder setProductName​(Optional<String> productName)
            ```

            ::: block
            Initializes the optional value
            [`productName`](AppleBundleDescriptionArg.html#getProductName())
            to productName.
            :::

            [Parameters:]{.paramLabel}
            :   `productName` - The value for productName

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setXcodeProductType(java.lang.String)}

        -   #### setXcodeProductType

            ``` methodSignature
            public final AppleBundleDescriptionArg.Builder setXcodeProductType​(String xcodeProductType)
            ```

            ::: block
            Initializes the optional value
            [`xcodeProductType`](AppleBundleDescriptionArg.html#getXcodeProductType())
            to xcodeProductType.
            :::

            [Parameters:]{.paramLabel}
            :   `xcodeProductType` - The value for xcodeProductType

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setXcodeProductType(java.util.Optional)}

        -   #### setXcodeProductType

            ``` methodSignature
            public final AppleBundleDescriptionArg.Builder setXcodeProductType​(Optional<String> xcodeProductType)
            ```

            ::: block
            Initializes the optional value
            [`xcodeProductType`](AppleBundleDescriptionArg.html#getXcodeProductType())
            to xcodeProductType.
            :::

            [Parameters:]{.paramLabel}
            :   `xcodeProductType` - The value for xcodeProductType

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setIsAppClip(boolean)}

        -   #### setIsAppClip

            ``` methodSignature
            public final AppleBundleDescriptionArg.Builder setIsAppClip​(boolean isAppClip)
            ```

            ::: block
            Initializes the optional value
            [`isAppClip`](AppleBundleDescriptionArg.html#getIsAppClip())
            to isAppClip.
            :::

            [Parameters:]{.paramLabel}
            :   `isAppClip` - The value for isAppClip

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setIsAppClip(java.util.Optional)}

        -   #### setIsAppClip

            ``` methodSignature
            public final AppleBundleDescriptionArg.Builder setIsAppClip​(Optional<Boolean> isAppClip)
            ```

            ::: block
            Initializes the optional value
            [`isAppClip`](AppleBundleDescriptionArg.html#getIsAppClip())
            to isAppClip.
            :::

            [Parameters:]{.paramLabel}
            :   `isAppClip` - The value for isAppClip

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putInfoPlistSubstitutions(java.lang.String,java.lang.String)}

        -   #### putInfoPlistSubstitutions

            ``` methodSignature
            public final AppleBundleDescriptionArg.Builder putInfoPlistSubstitutions​(String key,
                                                                                     String value)
            ```

            ::: block
            Put one entry to the
            [`infoPlistSubstitutions`](AppleBundleDescriptionArg.html#getInfoPlistSubstitutions())
            map.
            :::

            [Parameters:]{.paramLabel}
            :   `key` - The key in the infoPlistSubstitutions map
            :   `value` - The associated value in the
                infoPlistSubstitutions map

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putInfoPlistSubstitutions(java.util.Map.Entry)}

        -   #### putInfoPlistSubstitutions

            ``` methodSignature
            public final AppleBundleDescriptionArg.Builder putInfoPlistSubstitutions​(Map.Entry<String,​? extends String> entry)
            ```

            ::: block
            Put one entry to the
            [`infoPlistSubstitutions`](AppleBundleDescriptionArg.html#getInfoPlistSubstitutions())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entry` - The key and value entry

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setInfoPlistSubstitutions(java.util.Map)}

        -   #### setInfoPlistSubstitutions

            ``` methodSignature
            public final AppleBundleDescriptionArg.Builder setInfoPlistSubstitutions​(Map<String,​? extends String> entries)
            ```

            ::: block
            Sets or replaces all mappings from the specified map as
            entries for the
            [`infoPlistSubstitutions`](AppleBundleDescriptionArg.html#getInfoPlistSubstitutions())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entries` - The entries that will be added to the
                infoPlistSubstitutions map

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putAllInfoPlistSubstitutions(java.util.Map)}

        -   #### putAllInfoPlistSubstitutions

            ``` methodSignature
            public final AppleBundleDescriptionArg.Builder putAllInfoPlistSubstitutions​(Map<String,​? extends String> entries)
            ```

            ::: block
            Put all mappings from the specified map as entries to
            [`infoPlistSubstitutions`](AppleBundleDescriptionArg.html#getInfoPlistSubstitutions())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entries` - The entries that will be added to the
                infoPlistSubstitutions map

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setAssetCatalogsCompilationOptions(com.facebook.buck.apple.AppleAssetCatalogsCompilationOptions)}

        -   #### setAssetCatalogsCompilationOptions

            ``` methodSignature
            public final AppleBundleDescriptionArg.Builder setAssetCatalogsCompilationOptions​(AppleAssetCatalogsCompilationOptions assetCatalogsCompilationOptions)
            ```

            ::: block
            Initializes the value for the
            [`assetCatalogsCompilationOptions`](AppleBundleDescriptionArg.html#getAssetCatalogsCompilationOptions())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`assetCatalogsCompilationOptions`](AppleBundleDescriptionArg.html#getAssetCatalogsCompilationOptions()).*
            :::

            [Parameters:]{.paramLabel}
            :   `assetCatalogsCompilationOptions` - The value for
                assetCatalogsCompilationOptions

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCodesignFlags(java.lang.String)}

        -   #### addCodesignFlags

            ``` methodSignature
            public final AppleBundleDescriptionArg.Builder addCodesignFlags​(String element)
            ```

            ::: block
            Adds one element to
            [`codesignFlags`](AppleBundleDescriptionArg.html#getCodesignFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A codesignFlags element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCodesignFlags(java.lang.String...)}

        -   #### addCodesignFlags

            ``` methodSignature
            public final AppleBundleDescriptionArg.Builder addCodesignFlags​(String... elements)
            ```

            ::: block
            Adds elements to
            [`codesignFlags`](AppleBundleDescriptionArg.html#getCodesignFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of codesignFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCodesignFlags(java.lang.Iterable)}

        -   #### setCodesignFlags

            ``` methodSignature
            public final AppleBundleDescriptionArg.Builder setCodesignFlags​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`codesignFlags`](AppleBundleDescriptionArg.html#getCodesignFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of codesignFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllCodesignFlags(java.lang.Iterable)}

        -   #### addAllCodesignFlags

            ``` methodSignature
            public final AppleBundleDescriptionArg.Builder addAllCodesignFlags​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`codesignFlags`](AppleBundleDescriptionArg.html#getCodesignFlags())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of codesignFlags elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCodesignIdentity(java.lang.String)}

        -   #### setCodesignIdentity

            ``` methodSignature
            public final AppleBundleDescriptionArg.Builder setCodesignIdentity​(String codesignIdentity)
            ```

            ::: block
            Initializes the optional value
            [`codesignIdentity`](AppleBundleDescriptionArg.html#getCodesignIdentity())
            to codesignIdentity.
            :::

            [Parameters:]{.paramLabel}
            :   `codesignIdentity` - The value for codesignIdentity

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setCodesignIdentity(java.util.Optional)}

        -   #### setCodesignIdentity

            ``` methodSignature
            public final AppleBundleDescriptionArg.Builder setCodesignIdentity​(Optional<String> codesignIdentity)
            ```

            ::: block
            Initializes the optional value
            [`codesignIdentity`](AppleBundleDescriptionArg.html#getCodesignIdentity())
            to codesignIdentity.
            :::

            [Parameters:]{.paramLabel}
            :   `codesignIdentity` - The value for codesignIdentity

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addContacts(java.lang.String)}

        -   #### addContacts

            ``` methodSignature
            public final AppleBundleDescriptionArg.Builder addContacts​(String element)
            ```

            ::: block
            Adds one element to
            [`contacts`](AppleBundleDescriptionArg.html#getContacts())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A contacts element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addContacts(java.lang.String...)}

        -   #### addContacts

            ``` methodSignature
            public final AppleBundleDescriptionArg.Builder addContacts​(String... elements)
            ```

            ::: block
            Adds elements to
            [`contacts`](AppleBundleDescriptionArg.html#getContacts())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of contacts elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setContacts(java.lang.Iterable)}

        -   #### setContacts

            ``` methodSignature
            public final AppleBundleDescriptionArg.Builder setContacts​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`contacts`](AppleBundleDescriptionArg.html#getContacts())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of contacts elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllContacts(java.lang.Iterable)}

        -   #### addAllContacts

            ``` methodSignature
            public final AppleBundleDescriptionArg.Builder addAllContacts​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`contacts`](AppleBundleDescriptionArg.html#getContacts())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of contacts elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDefaultPlatform(com.facebook.buck.core.model.Flavor)}

        -   #### setDefaultPlatform

            ``` methodSignature
            public final AppleBundleDescriptionArg.Builder setDefaultPlatform​(Flavor defaultPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultPlatform`](AppleBundleDescriptionArg.html#getDefaultPlatform())
            to defaultPlatform.
            :::

            [Parameters:]{.paramLabel}
            :   `defaultPlatform` - The value for defaultPlatform

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setDefaultPlatform(java.util.Optional)}

        -   #### setDefaultPlatform

            ``` methodSignature
            public final AppleBundleDescriptionArg.Builder setDefaultPlatform​(Optional<? extends Flavor> defaultPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultPlatform`](AppleBundleDescriptionArg.html#getDefaultPlatform())
            to defaultPlatform.
            :::

            [Parameters:]{.paramLabel}
            :   `defaultPlatform` - The value for defaultPlatform

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addTests(com.facebook.buck.core.model.BuildTarget)}

        -   #### addTests

            ``` methodSignature
            public final AppleBundleDescriptionArg.Builder addTests​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`tests`](AppleBundleDescriptionArg.html#getTests())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A tests element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addTests(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addTests

            ``` methodSignature
            public final AppleBundleDescriptionArg.Builder addTests​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`tests`](AppleBundleDescriptionArg.html#getTests())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of tests elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setTests(java.lang.Iterable)}

        -   #### setTests

            ``` methodSignature
            public final AppleBundleDescriptionArg.Builder setTests​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`tests`](AppleBundleDescriptionArg.html#getTests())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of tests elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllTests(java.lang.Iterable)}

        -   #### addAllTests

            ``` methodSignature
            public final AppleBundleDescriptionArg.Builder addAllTests​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`tests`](AppleBundleDescriptionArg.html#getTests())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of tests elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#build()}

        -   #### build

            ``` methodSignature
            public AppleBundleDescriptionArg build()
            ```

            ::: block
            Builds a new
            [`AppleBundleDescriptionArg`](AppleBundleDescriptionArg.html "class in com.facebook.buck.apple").
            :::

            [Returns:]{.returnLabel}
            :   An immutable instance of AppleBundleDescriptionArg

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
