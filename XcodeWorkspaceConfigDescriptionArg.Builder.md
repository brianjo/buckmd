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

-   [Overview](../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../deprecated-list.html)
-   [Index](../../../../../../index-all.html)
-   [Help](../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.features.apple.common](package-summary.html)
:::

## Class XcodeWorkspaceConfigDescriptionArg.Builder {#class-xcodeworkspaceconfigdescriptionarg.builder .title title="Class XcodeWorkspaceConfigDescriptionArg.Builder"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.features.apple.common.XcodeWorkspaceConfigDescriptionArg.Builder

::: description
-   

    Enclosing class:
    :   [XcodeWorkspaceConfigDescriptionArg](XcodeWorkspaceConfigDescriptionArg.html "class in com.facebook.buck.features.apple.common")

    ------------------------------------------------------------------------

        @NotThreadSafe
        public static final class XcodeWorkspaceConfigDescriptionArg.Builder
        extends Object

    ::: block
    Builds instances of type
    [`XcodeWorkspaceConfigDescriptionArg`](XcodeWorkspaceConfigDescriptionArg.html "class in com.facebook.buck.features.apple.common").
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
        | `X                    | `addAllCompat         | ::: block             |
        | codeWorkspaceConfigDe | ibleWith​(Iterable<? e | Adds elements to      |
        | scriptionArg.Builder` | xtends UnconfiguredBu | [`compatibleWith      |
        |                       | ildTarget> elements)` | `](XcodeWorkspaceConf |
        |                       |                       | igDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `X                    | `addAl                | ::: block             |
        | codeWorkspaceConfigDe | lExtraShallowTargets​( | Adds elements to      |
        | scriptionArg.Builder` | Iterable<? extends Bu | [`ext                 |
        |                       | ildTarget> elements)` | raShallowTargets`](Xc |
        |                       |                       | odeWorkspaceConfigDes |
        |                       |                       | criptionArg.html#getE |
        |                       |                       | xtraShallowTargets()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `X                    | `addAllExtraTargets​(  | ::: block             |
        | codeWorkspaceConfigDe | Iterable<? extends Bu | Adds elements to      |
        | scriptionArg.Builder` | ildTarget> elements)` | [`extraTarge          |
        |                       |                       | ts`](XcodeWorkspaceCo |
        |                       |                       | nfigDescriptionArg.ht |
        |                       |                       | ml#getExtraTargets()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `X                    | `addAllExtraTests​(    | ::: block             |
        | codeWorkspaceConfigDe | Iterable<? extends Bu | Adds elements to      |
        | scriptionArg.Builder` | ildTarget> elements)` | [`extraT              |
        |                       |                       | ests`](XcodeWorkspace |
        |                       |                       | ConfigDescriptionArg. |
        |                       |                       | html#getExtraTests()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `X                    | `addAllLabels​(Iterab  | ::: block             |
        | codeWorkspaceConfigDe | le<String> elements)` | Adds elements to      |
        | scriptionArg.Builder` |                       | [`labels`](XcodeWorks |
        |                       |                       | paceConfigDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `X                    | `addAllLicenses       | ::: block             |
        | codeWorkspaceConfigDe | ​(Iterable<? extends S | Adds elements to      |
        | scriptionArg.Builder` | ourcePath> elements)` | [`li                  |
        |                       |                       | censes`](XcodeWorkspa |
        |                       |                       | ceConfigDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `X                    | `addCompat            | ::: block             |
        | codeWorkspaceConfigDe | ibleWith​(Unconfigured | Adds one element to   |
        | scriptionArg.Builder` | BuildTarget element)` | [`compatibleWith      |
        |                       |                       | `](XcodeWorkspaceConf |
        |                       |                       | igDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `X                    | `addCompatible        | ::: block             |
        | codeWorkspaceConfigDe | With​(UnconfiguredBuil | Adds elements to      |
        | scriptionArg.Builder` | dTarget... elements)` | [`compatibleWith      |
        |                       |                       | `](XcodeWorkspaceConf |
        |                       |                       | igDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `X                    | `ad                   | ::: block             |
        | codeWorkspaceConfigDe | dExtraShallowTargets​( | Adds one element to   |
        | scriptionArg.Builder` | BuildTarget element)` | [`ext                 |
        |                       |                       | raShallowTargets`](Xc |
        |                       |                       | odeWorkspaceConfigDes |
        |                       |                       | criptionArg.html#getE |
        |                       |                       | xtraShallowTargets()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `X                    | `addExt               | ::: block             |
        | codeWorkspaceConfigDe | raShallowTargets​(Buil | Adds elements to      |
        | scriptionArg.Builder` | dTarget... elements)` | [`ext                 |
        |                       |                       | raShallowTargets`](Xc |
        |                       |                       | odeWorkspaceConfigDes |
        |                       |                       | criptionArg.html#getE |
        |                       |                       | xtraShallowTargets()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `X                    | `addExtraTargets​(     | ::: block             |
        | codeWorkspaceConfigDe | BuildTarget element)` | Adds one element to   |
        | scriptionArg.Builder` |                       | [`extraTarge          |
        |                       |                       | ts`](XcodeWorkspaceCo |
        |                       |                       | nfigDescriptionArg.ht |
        |                       |                       | ml#getExtraTargets()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `X                    | `addExtraTargets​(Buil | ::: block             |
        | codeWorkspaceConfigDe | dTarget... elements)` | Adds elements to      |
        | scriptionArg.Builder` |                       | [`extraTarge          |
        |                       |                       | ts`](XcodeWorkspaceCo |
        |                       |                       | nfigDescriptionArg.ht |
        |                       |                       | ml#getExtraTargets()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `X                    | `addExtraTests​(       | ::: block             |
        | codeWorkspaceConfigDe | BuildTarget element)` | Adds one element to   |
        | scriptionArg.Builder` |                       | [`extraT              |
        |                       |                       | ests`](XcodeWorkspace |
        |                       |                       | ConfigDescriptionArg. |
        |                       |                       | html#getExtraTests()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `X                    | `addExtraTests​(Buil   | ::: block             |
        | codeWorkspaceConfigDe | dTarget... elements)` | Adds elements to      |
        | scriptionArg.Builder` |                       | [`extraT              |
        |                       |                       | ests`](XcodeWorkspace |
        |                       |                       | ConfigDescriptionArg. |
        |                       |                       | html#getExtraTests()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `X                    | `addLa                | ::: block             |
        | codeWorkspaceConfigDe | bels​(String element)` | Adds one element to   |
        | scriptionArg.Builder` |                       | [`labels`](XcodeWorks |
        |                       |                       | paceConfigDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `X                    | `addLabels            | ::: block             |
        | codeWorkspaceConfigDe | ​(String... elements)` | Adds elements to      |
        | scriptionArg.Builder` |                       | [`labels`](XcodeWorks |
        |                       |                       | paceConfigDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `X                    | `addLicenses          | ::: block             |
        | codeWorkspaceConfigDe | ​(SourcePath element)` | Adds one element to   |
        | scriptionArg.Builder` |                       | [`li                  |
        |                       |                       | censes`](XcodeWorkspa |
        |                       |                       | ceConfigDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `X                    | `addLicenses​(Sou      | ::: block             |
        | codeWorkspaceConfigDe | rcePath... elements)` | Adds elements to      |
        | scriptionArg.Builder` |                       | [`li                  |
        |                       |                       | censes`](XcodeWorkspa |
        |                       |                       | ceConfigDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `XcodeWorkspace       | `build()`             | ::: block             |
        | ConfigDescriptionArg` |                       | Builds a new          |
        |                       |                       | [`Xco                 |
        |                       |                       | deWorkspaceConfigDesc |
        |                       |                       | riptionArg`](XcodeWor |
        |                       |                       | kspaceConfigDescripti |
        |                       |                       | onArg.html "class in  |
        |                       |                       | com.facebook.buck.fea |
        |                       |                       | tures.apple.common"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `X                    | `from​(Bu              | ::: block             |
        | codeWorkspaceConfigDe | ildRuleArg instance)` | Fill a builder with   |
        | scriptionArg.Builder` |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebo           |
        |                       |                       | ok.buck.core.descript |
        |                       |                       | ion.arg.BuildRuleArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `X                    | `from​(Cons            | ::: block             |
        | codeWorkspaceConfigDe | tructorArg instance)` | Fill a builder with   |
        | scriptionArg.Builder` |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook         |
        |                       |                       | .buck.core.descriptio |
        |                       |                       | n.arg.ConstructorArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `X                    | `from                 | ::: block             |
        | codeWorkspaceConfigDe | ​(com.facebook.buck.fe | Copy abstract value   |
        | scriptionArg.Builder` | atures.apple.common.X | type                  |
        |                       | codeWorkspaceConfigDe | `A                    |
        |                       | scription.AbstractXco | bstractXcodeWorkspace |
        |                       | deWorkspaceConfigDesc | ConfigDescriptionArg` |
        |                       | riptionArg instance)` | instance into         |
        |                       |                       | builder.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `X                    | `from​(Xco             | ::: block             |
        | codeWorkspaceConfigDe | deWorkspaceConfigDesc | Fill a builder with   |
        | scriptionArg.Builder` | riptionArg instance)` | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `XcodeWorkspace       |
        |                       |                       | ConfigDescriptionArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `X                    | `putActionConfi       | ::: block             |
        | codeWorkspaceConfigDe | gNames​(SchemeActionTy | Put one entry to the  |
        | scriptionArg.Builder` | pe key,               | [                     |
        |                       |        String value)` | `actionConfigNames`]( |
        |                       |                       | XcodeWorkspaceConfigD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tActionConfigNames()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `X                    | `putActionC           | ::: block             |
        | codeWorkspaceConfigDe | onfigNames​(Map.Entry< | Put one entry to the  |
        | scriptionArg.Builder` | SchemeActionType,​? ex | [                     |
        |                       | tends String> entry)` | `actionConfigNames`]( |
        |                       |                       | XcodeWorkspaceConfigD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tActionConfigNames()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `X                    | `putAllAct            | ::: block             |
        | codeWorkspaceConfigDe | ionConfigNames​(Map<Sc | Put all mappings from |
        | scriptionArg.Builder` | hemeActionType,​? exte | the specified map as  |
        |                       | nds String> entries)` | entries to            |
        |                       |                       | [                     |
        |                       |                       | `actionConfigNames`]( |
        |                       |                       | XcodeWorkspaceConfigD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tActionConfigNames()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `X                    | `putAllExtraSchemes​(M | ::: block             |
        | codeWorkspaceConfigDe | ap<String,​? extends B | Put all mappings from |
        | scriptionArg.Builder` | uildTarget> entries)` | the specified map as  |
        |                       |                       | entries to            |
        |                       |                       | [`extraSchem          |
        |                       |                       | es`](XcodeWorkspaceCo |
        |                       |                       | nfigDescriptionArg.ht |
        |                       |                       | ml#getExtraSchemes()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `X                    | `putExtraSchemes​(Stri | ::: block             |
        | codeWorkspaceConfigDe | ng key,               | Put one entry to the  |
        | scriptionArg.Builder` |   BuildTarget value)` | [`extraSchem          |
        |                       |                       | es`](XcodeWorkspaceCo |
        |                       |                       | nfigDescriptionArg.ht |
        |                       |                       | ml#getExtraSchemes()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `X                    | `                     | ::: block             |
        | codeWorkspaceConfigDe | putExtraSchemes​(Map.E | Put one entry to the  |
        | scriptionArg.Builder` | ntry<String,​? extends | [`extraSchem          |
        |                       |  BuildTarget> entry)` | es`](XcodeWorkspaceCo |
        |                       |                       | nfigDescriptionArg.ht |
        |                       |                       | ml#getExtraSchemes()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `X                    | `setAct               | ::: block             |
        | codeWorkspaceConfigDe | ionConfigNames​(Map<Sc | Sets or replaces all  |
        | scriptionArg.Builder` | hemeActionType,​? exte | mappings from the     |
        |                       | nds String> entries)` | specified map as      |
        |                       |                       | entries for the       |
        |                       |                       | [                     |
        |                       |                       | `actionConfigNames`]( |
        |                       |                       | XcodeWorkspaceConfigD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tActionConfigNames()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `X                    | `setAdditionalS       | ::: block             |
        | codeWorkspaceConfigDe | chemeActions​(com.goog | Initializes the       |
        | scriptionArg.Builder` | le.common.collect.Imm | optional value        |
        |                       | utableMap<SchemeActio | [`additionalS         |
        |                       | nType,​com.google.comm | chemeActions`](XcodeW |
        |                       | on.collect.ImmutableM | orkspaceConfigDescrip |
        |                       | ap<XCScheme.Additiona | tionArg.html#getAddit |
        |                       | lActions,​com.google.c | ionalSchemeActions()) |
        |                       | ommon.collect.Immutab | to                    |
        |                       | leList<String>>> addi | add                   |
        |                       | tionalSchemeActions)` | itionalSchemeActions. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `X                    | `setAdditional        | ::: block             |
        | codeWorkspaceConfigDe | SchemeActions​(Optiona | Initializes the       |
        | scriptionArg.Builder` | l<? extends com.googl | optional value        |
        |                       | e.common.collect.Immu | [`additionalS         |
        |                       | tableMap<SchemeAction | chemeActions`](XcodeW |
        |                       | Type,​com.google.commo | orkspaceConfigDescrip |
        |                       | n.collect.ImmutableMa | tionArg.html#getAddit |
        |                       | p<XCScheme.Additional | ionalSchemeActions()) |
        |                       | Actions,​com.google.co | to                    |
        |                       | mmon.collect.Immutabl | add                   |
        |                       | eList<String>>>> addi | itionalSchemeActions. |
        |                       | tionalSchemeActions)` | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `X                    | `setApplic            | ::: block             |
        | codeWorkspaceConfigDe | ationLanguage​(String  | Initializes the       |
        | scriptionArg.Builder` | applicationLanguage)` | optional value        |
        |                       |                       | [`app                 |
        |                       |                       | licationLanguage`](Xc |
        |                       |                       | odeWorkspaceConfigDes |
        |                       |                       | criptionArg.html#getA |
        |                       |                       | pplicationLanguage()) |
        |                       |                       | to                    |
        |                       |                       | applicationLanguage.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `X                    | `setApplicationLangu  | ::: block             |
        | codeWorkspaceConfigDe | age​(Optional<String>  | Initializes the       |
        | scriptionArg.Builder` | applicationLanguage)` | optional value        |
        |                       |                       | [`app                 |
        |                       |                       | licationLanguage`](Xc |
        |                       |                       | odeWorkspaceConfigDes |
        |                       |                       | criptionArg.html#getA |
        |                       |                       | pplicationLanguage()) |
        |                       |                       | to                    |
        |                       |                       | applicationLanguage.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `X                    | `setAp                | ::: block             |
        | codeWorkspaceConfigDe | plicationRegion​(Strin | Initializes the       |
        | scriptionArg.Builder` | g applicationRegion)` | optional value        |
        |                       |                       | [                     |
        |                       |                       | `applicationRegion`]( |
        |                       |                       | XcodeWorkspaceConfigD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tApplicationRegion()) |
        |                       |                       | to applicationRegion. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `X                    | `setApplicationR      | ::: block             |
        | codeWorkspaceConfigDe | egion​(Optional<String | Initializes the       |
        | scriptionArg.Builder` | > applicationRegion)` | optional value        |
        |                       |                       | [                     |
        |                       |                       | `applicationRegion`]( |
        |                       |                       | XcodeWorkspaceConfigD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tApplicationRegion()) |
        |                       |                       | to applicationRegion. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `X                    | `setCommand           | ::: block             |
        | codeWorkspaceConfigDe | LineArguments​(com.goo | Initializes the       |
        | scriptionArg.Builder` | gle.common.collect.Im | optional value        |
        |                       | mutableMap<SchemeActi | [`comma               |
        |                       | onType,​com.google.com | ndLineArguments`](Xco |
        |                       | mon.collect.Immutable | deWorkspaceConfigDesc |
        |                       | Map<String,​String>> c | riptionArg.html#getCo |
        |                       | ommandLineArguments)` | mmandLineArguments()) |
        |                       |                       | to                    |
        |                       |                       | commandLineArguments. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `X                    | `setComman            | ::: block             |
        | codeWorkspaceConfigDe | dLineArguments​(Option | Initializes the       |
        | scriptionArg.Builder` | al<? extends com.goog | optional value        |
        |                       | le.common.collect.Imm | [`comma               |
        |                       | utableMap<SchemeActio | ndLineArguments`](Xco |
        |                       | nType,​com.google.comm | deWorkspaceConfigDesc |
        |                       | on.collect.ImmutableM | riptionArg.html#getCo |
        |                       | ap<String,​String>>> c | mmandLineArguments()) |
        |                       | ommandLineArguments)` | to                    |
        |                       |                       | commandLineArguments. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `X                    | `setCompat            | ::: block             |
        | codeWorkspaceConfigDe | ibleWith​(Iterable<? e | Sets or replaces all  |
        | scriptionArg.Builder` | xtends UnconfiguredBu | elements for          |
        |                       | ildTarget> elements)` | [`compatibleWith      |
        |                       |                       | `](XcodeWorkspaceConf |
        |                       |                       | igDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `X                    | `setDefaul            | ::: block             |
        | codeWorkspaceConfigDe | tTargetPlatform​(Uncon | Initializes the       |
        | scriptionArg.Builder` | figuredBuildTarget de | optional value        |
        |                       | faultTargetPlatform)` | [`default             |
        |                       |                       | TargetPlatform`](Xcod |
        |                       |                       | eWorkspaceConfigDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `X                    | `setDefau             | ::: block             |
        | codeWorkspaceConfigDe | ltTargetPlatform​(Opti | Initializes the       |
        | scriptionArg.Builder` | onal<? extends Unconf | optional value        |
        |                       | iguredBuildTarget> de | [`default             |
        |                       | faultTargetPlatform)` | TargetPlatform`](Xcod |
        |                       |                       | eWorkspaceConfigDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `X                    | `setEnviron           | ::: block             |
        | codeWorkspaceConfigDe | mentVariables​(com.goo | Initializes the       |
        | scriptionArg.Builder` | gle.common.collect.Im | optional value        |
        |                       | mutableMap<SchemeActi | [`envir               |
        |                       | onType,​com.google.com | onmentVariables`](Xco |
        |                       | mon.collect.Immutable | deWorkspaceConfigDesc |
        |                       | Map<String,​String>> e | riptionArg.html#getEn |
        |                       | nvironmentVariables)` | vironmentVariables()) |
        |                       |                       | to                    |
        |                       |                       | environmentVariables. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `X                    | `setEnviro            | ::: block             |
        | codeWorkspaceConfigDe | nmentVariables​(Option | Initializes the       |
        | scriptionArg.Builder` | al<? extends com.goog | optional value        |
        |                       | le.common.collect.Imm | [`envir               |
        |                       | utableMap<SchemeActio | onmentVariables`](Xco |
        |                       | nType,​com.google.comm | deWorkspaceConfigDesc |
        |                       | on.collect.ImmutableM | riptionArg.html#getEn |
        |                       | ap<String,​String>>> e | vironmentVariables()) |
        |                       | nvironmentVariables)` | to                    |
        |                       |                       | environmentVariables. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `X                    | `setExpandVaria       | ::: block             |
        | codeWorkspaceConfigDe | blesBasedOn​(com.googl | Initializes the       |
        | scriptionArg.Builder` | e.common.collect.Immu | optional value        |
        |                       | tableMap<SchemeAction | [`expandVar           |
        |                       | Type,​BuildTarget> exp | iablesBasedOn`](Xcode |
        |                       | andVariablesBasedOn)` | WorkspaceConfigDescri |
        |                       |                       | ptionArg.html#getExpa |
        |                       |                       | ndVariablesBasedOn()) |
        |                       |                       | to                    |
        |                       |                       | ex                    |
        |                       |                       | pandVariablesBasedOn. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `X                    | `setExpandVari        | ::: block             |
        | codeWorkspaceConfigDe | ablesBasedOn​(Optional | Initializes the       |
        | scriptionArg.Builder` | <? extends com.google | optional value        |
        |                       | .common.collect.Immut | [`expandVar           |
        |                       | ableMap<SchemeActionT | iablesBasedOn`](Xcode |
        |                       | ype,​BuildTarget>> exp | WorkspaceConfigDescri |
        |                       | andVariablesBasedOn)` | ptionArg.html#getExpa |
        |                       |                       | ndVariablesBasedOn()) |
        |                       |                       | to                    |
        |                       |                       | ex                    |
        |                       |                       | pandVariablesBasedOn. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `X                    | `setExplicit          | ::: block             |
        | codeWorkspaceConfigDe | RunnablePath​(String e | Initializes the       |
        | scriptionArg.Builder` | xplicitRunnablePath)` | optional value        |
        |                       |                       | [`expli               |
        |                       |                       | citRunnablePath`](Xco |
        |                       |                       | deWorkspaceConfigDesc |
        |                       |                       | riptionArg.html#getEx |
        |                       |                       | plicitRunnablePath()) |
        |                       |                       | to                    |
        |                       |                       | explicitRunnablePath. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `X                    | `                     | ::: block             |
        | codeWorkspaceConfigDe | setExplicitRunnablePa | Initializes the       |
        | scriptionArg.Builder` | th​(Optional<String> e | optional value        |
        |                       | xplicitRunnablePath)` | [`expli               |
        |                       |                       | citRunnablePath`](Xco |
        |                       |                       | deWorkspaceConfigDesc |
        |                       |                       | riptionArg.html#getEx |
        |                       |                       | plicitRunnablePath()) |
        |                       |                       | to                    |
        |                       |                       | explicitRunnablePath. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `X                    | `setExtraSchemes​(M    | ::: block             |
        | codeWorkspaceConfigDe | ap<String,​? extends B | Sets or replaces all  |
        | scriptionArg.Builder` | uildTarget> entries)` | mappings from the     |
        |                       |                       | specified map as      |
        |                       |                       | entries for the       |
        |                       |                       | [`extraSchem          |
        |                       |                       | es`](XcodeWorkspaceCo |
        |                       |                       | nfigDescriptionArg.ht |
        |                       |                       | ml#getExtraSchemes()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `X                    | `se                   | ::: block             |
        | codeWorkspaceConfigDe | tExtraShallowTargets​( | Sets or replaces all  |
        | scriptionArg.Builder` | Iterable<? extends Bu | elements for          |
        |                       | ildTarget> elements)` | [`ext                 |
        |                       |                       | raShallowTargets`](Xc |
        |                       |                       | odeWorkspaceConfigDes |
        |                       |                       | criptionArg.html#getE |
        |                       |                       | xtraShallowTargets()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `X                    | `setExtraTargets​(     | ::: block             |
        | codeWorkspaceConfigDe | Iterable<? extends Bu | Sets or replaces all  |
        | scriptionArg.Builder` | ildTarget> elements)` | elements for          |
        |                       |                       | [`extraTarge          |
        |                       |                       | ts`](XcodeWorkspaceCo |
        |                       |                       | nfigDescriptionArg.ht |
        |                       |                       | ml#getExtraTargets()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `X                    | `setExtraTests​(       | ::: block             |
        | codeWorkspaceConfigDe | Iterable<? extends Bu | Sets or replaces all  |
        | scriptionArg.Builder` | ildTarget> elements)` | elements for          |
        |                       |                       | [`extraT              |
        |                       |                       | ests`](XcodeWorkspace |
        |                       |                       | ConfigDescriptionArg. |
        |                       |                       | html#getExtraTests()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `X                    | `setI                 | ::: block             |
        | codeWorkspaceConfigDe | sRemoteRunnable​(boole | Initializes the       |
        | scriptionArg.Builder` | an isRemoteRunnable)` | optional value        |
        |                       |                       | [`isRemoteRunnable`]  |
        |                       |                       | (XcodeWorkspaceConfig |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etIsRemoteRunnable()) |
        |                       |                       | to isRemoteRunnable.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `X                    | `setIsRemoteRun       | ::: block             |
        | codeWorkspaceConfigDe | nable​(Optional<Boolea | Initializes the       |
        | scriptionArg.Builder` | n> isRemoteRunnable)` | optional value        |
        |                       |                       | [`isRemoteRunnable`]  |
        |                       |                       | (XcodeWorkspaceConfig |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etIsRemoteRunnable()) |
        |                       |                       | to isRemoteRunnable.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `X                    | `setLabels​(Iterab     | ::: block             |
        | codeWorkspaceConfigDe | le<String> elements)` | Sets or replaces all  |
        | scriptionArg.Builder` |                       | elements for          |
        |                       |                       | [`labels`](XcodeWorks |
        |                       |                       | paceConfigDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `X                    | `setLaunchStyle​(XCSch | ::: block             |
        | codeWorkspaceConfigDe | eme.LaunchAction.Laun | Initializes the       |
        | scriptionArg.Builder` | chStyle launchStyle)` | optional value        |
        |                       |                       | [`launchSt            |
        |                       |                       | yle`](XcodeWorkspaceC |
        |                       |                       | onfigDescriptionArg.h |
        |                       |                       | tml#getLaunchStyle()) |
        |                       |                       | to launchStyle.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `X                    | `setLaunchStyle​(Opti  | ::: block             |
        | codeWorkspaceConfigDe | onal<? extends XCSche | Initializes the       |
        | scriptionArg.Builder` | me.LaunchAction.Launc | optional value        |
        |                       | hStyle> launchStyle)` | [`launchSt            |
        |                       |                       | yle`](XcodeWorkspaceC |
        |                       |                       | onfigDescriptionArg.h |
        |                       |                       | tml#getLaunchStyle()) |
        |                       |                       | to launchStyle.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `X                    | `setLicenses          | ::: block             |
        | codeWorkspaceConfigDe | ​(Iterable<? extends S | Sets or replaces all  |
        | scriptionArg.Builder` | ourcePath> elements)` | elements for          |
        |                       |                       | [`li                  |
        |                       |                       | censes`](XcodeWorkspa |
        |                       |                       | ceConfigDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `X                    | `                     | ::: block             |
        | codeWorkspaceConfigDe | setName​(String name)` | Initializes the value |
        | scriptionArg.Builder` |                       | for the               |
        |                       |                       | [`name`](XcodeWor     |
        |                       |                       | kspaceConfigDescripti |
        |                       |                       | onArg.html#getName()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `X                    | `setNotificationPa    | ::: block             |
        | codeWorkspaceConfigDe | yloadFile​(String noti | Initializes the       |
        | scriptionArg.Builder` | ficationPayloadFile)` | optional value        |
        |                       |                       | [`notificatio         |
        |                       |                       | nPayloadFile`](XcodeW |
        |                       |                       | orkspaceConfigDescrip |
        |                       |                       | tionArg.html#getNotif |
        |                       |                       | icationPayloadFile()) |
        |                       |                       | to                    |
        |                       |                       | not                   |
        |                       |                       | ificationPayloadFile. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `X                    | `setNot               | ::: block             |
        | codeWorkspaceConfigDe | ificationPayloadFile​( | Initializes the       |
        | scriptionArg.Builder` | Optional<String> noti | optional value        |
        |                       | ficationPayloadFile)` | [`notificatio         |
        |                       |                       | nPayloadFile`](XcodeW |
        |                       |                       | orkspaceConfigDescrip |
        |                       |                       | tionArg.html#getNotif |
        |                       |                       | icationPayloadFile()) |
        |                       |                       | to                    |
        |                       |                       | not                   |
        |                       |                       | ificationPayloadFile. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `X                    | `setSrcTarget​(Bu      | ::: block             |
        | codeWorkspaceConfigDe | ildTarget srcTarget)` | Initializes the       |
        | scriptionArg.Builder` |                       | optional value        |
        |                       |                       | [`srcT                |
        |                       |                       | arget`](XcodeWorkspac |
        |                       |                       | eConfigDescriptionArg |
        |                       |                       | .html#getSrcTarget()) |
        |                       |                       | to srcTarget.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `X                    | `setSrcTarget​(O       | ::: block             |
        | codeWorkspaceConfigDe | ptional<? extends Bui | Initializes the       |
        | scriptionArg.Builder` | ldTarget> srcTarget)` | optional value        |
        |                       |                       | [`srcT                |
        |                       |                       | arget`](XcodeWorkspac |
        |                       |                       | eConfigDescriptionArg |
        |                       |                       | .html#getSrcTarget()) |
        |                       |                       | to srcTarget.         |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `X                    | `s                    | ::: block             |
        | codeWorkspaceConfigDe | etWasCreatedForAppExt | Initializes the       |
        | scriptionArg.Builder` | ension​(boolean wasCre | optional value        |
        |                       | atedForAppExtension)` | [`wasCreatedForAp     |
        |                       |                       | pExtension`](XcodeWor |
        |                       |                       | kspaceConfigDescripti |
        |                       |                       | onArg.html#getWasCrea |
        |                       |                       | tedForAppExtension()) |
        |                       |                       | to                    |
        |                       |                       | wasCr                 |
        |                       |                       | eatedForAppExtension. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `X                    | `setWasCreat          | ::: block             |
        | codeWorkspaceConfigDe | edForAppExtension​(Opt | Initializes the       |
        | scriptionArg.Builder` | ional<Boolean> wasCre | optional value        |
        |                       | atedForAppExtension)` | [`wasCreatedForAp     |
        |                       |                       | pExtension`](XcodeWor |
        |                       |                       | kspaceConfigDescripti |
        |                       |                       | onArg.html#getWasCrea |
        |                       |                       | tedForAppExtension()) |
        |                       |                       | to                    |
        |                       |                       | wasCr                 |
        |                       |                       | eatedForAppExtension. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `X                    | `setWatch             | ::: block             |
        | codeWorkspaceConfigDe | Interface​(XCScheme.La | Initializes the       |
        | scriptionArg.Builder` | unchAction.WatchInter | optional value        |
        |                       | face watchInterface)` | [`watchInterface      |
        |                       |                       | `](XcodeWorkspaceConf |
        |                       |                       | igDescriptionArg.html |
        |                       |                       | #getWatchInterface()) |
        |                       |                       | to watchInterface.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `X                    | `setWatc              | ::: block             |
        | codeWorkspaceConfigDe | hInterface​(Optional<? | Initializes the       |
        | scriptionArg.Builder` |  extends XCScheme.Lau | optional value        |
        |                       | nchAction.WatchInterf | [`watchInterface      |
        |                       | ace> watchInterface)` | `](XcodeWorkspaceConf |
        |                       |                       | igDescriptionArg.html |
        |                       |                       | #getWatchInterface()) |
        |                       |                       | to watchInterface.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `X                    | `setWorkspaceName​(S   | ::: block             |
        | codeWorkspaceConfigDe | tring workspaceName)` | Initializes the       |
        | scriptionArg.Builder` |                       | optional value        |
        |                       |                       | [`workspaceNam        |
        |                       |                       | e`](XcodeWorkspaceCon |
        |                       |                       | figDescriptionArg.htm |
        |                       |                       | l#getWorkspaceName()) |
        |                       |                       | to workspaceName.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `X                    | `setWork              | ::: block             |
        | codeWorkspaceConfigDe | spaceName​(Optional<St | Initializes the       |
        | scriptionArg.Builder` | ring> workspaceName)` | optional value        |
        |                       |                       | [`workspaceNam        |
        |                       |                       | e`](XcodeWorkspaceCon |
        |                       |                       | figDescriptionArg.htm |
        |                       |                       | l#getWorkspaceName()) |
        |                       |                       | to workspaceName.     |
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

        []{#from(com.facebook.buck.features.apple.common.XcodeWorkspaceConfigDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final XcodeWorkspaceConfigDescriptionArg.Builder from​(XcodeWorkspaceConfigDescriptionArg instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `XcodeWorkspaceConfigDescriptionArg` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.features.apple.common.XcodeWorkspaceConfigDescription.AbstractXcodeWorkspaceConfigDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final XcodeWorkspaceConfigDescriptionArg.Builder from​(com.facebook.buck.features.apple.common.XcodeWorkspaceConfigDescription.AbstractXcodeWorkspaceConfigDescriptionArg instance)
            ```

            ::: block
            Copy abstract value type
            `AbstractXcodeWorkspaceConfigDescriptionArg` instance into
            builder.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.core.description.arg.BuildRuleArg)}

        -   #### from

            ``` methodSignature
            public final XcodeWorkspaceConfigDescriptionArg.Builder from​(BuildRuleArg instance)
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
            public final XcodeWorkspaceConfigDescriptionArg.Builder from​(ConstructorArg instance)
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

        []{#setSrcTarget(com.facebook.buck.core.model.BuildTarget)}

        -   #### setSrcTarget

            ``` methodSignature
            public final XcodeWorkspaceConfigDescriptionArg.Builder setSrcTarget​(BuildTarget srcTarget)
            ```

            ::: block
            Initializes the optional value
            [`srcTarget`](XcodeWorkspaceConfigDescriptionArg.html#getSrcTarget())
            to srcTarget.
            :::

            [Parameters:]{.paramLabel}
            :   `srcTarget` - The value for srcTarget

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setSrcTarget(java.util.Optional)}

        -   #### setSrcTarget

            ``` methodSignature
            public final XcodeWorkspaceConfigDescriptionArg.Builder setSrcTarget​(Optional<? extends BuildTarget> srcTarget)
            ```

            ::: block
            Initializes the optional value
            [`srcTarget`](XcodeWorkspaceConfigDescriptionArg.html#getSrcTarget())
            to srcTarget.
            :::

            [Parameters:]{.paramLabel}
            :   `srcTarget` - The value for srcTarget

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addExtraTests(com.facebook.buck.core.model.BuildTarget)}

        -   #### addExtraTests

            ``` methodSignature
            public final XcodeWorkspaceConfigDescriptionArg.Builder addExtraTests​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`extraTests`](XcodeWorkspaceConfigDescriptionArg.html#getExtraTests())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A extraTests element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addExtraTests(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addExtraTests

            ``` methodSignature
            public final XcodeWorkspaceConfigDescriptionArg.Builder addExtraTests​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`extraTests`](XcodeWorkspaceConfigDescriptionArg.html#getExtraTests())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of extraTests elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setExtraTests(java.lang.Iterable)}

        -   #### setExtraTests

            ``` methodSignature
            public final XcodeWorkspaceConfigDescriptionArg.Builder setExtraTests​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`extraTests`](XcodeWorkspaceConfigDescriptionArg.html#getExtraTests())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of extraTests elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllExtraTests(java.lang.Iterable)}

        -   #### addAllExtraTests

            ``` methodSignature
            public final XcodeWorkspaceConfigDescriptionArg.Builder addAllExtraTests​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`extraTests`](XcodeWorkspaceConfigDescriptionArg.html#getExtraTests())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of extraTests elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addExtraTargets(com.facebook.buck.core.model.BuildTarget)}

        -   #### addExtraTargets

            ``` methodSignature
            public final XcodeWorkspaceConfigDescriptionArg.Builder addExtraTargets​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`extraTargets`](XcodeWorkspaceConfigDescriptionArg.html#getExtraTargets())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A extraTargets element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addExtraTargets(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addExtraTargets

            ``` methodSignature
            public final XcodeWorkspaceConfigDescriptionArg.Builder addExtraTargets​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`extraTargets`](XcodeWorkspaceConfigDescriptionArg.html#getExtraTargets())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of extraTargets elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setExtraTargets(java.lang.Iterable)}

        -   #### setExtraTargets

            ``` methodSignature
            public final XcodeWorkspaceConfigDescriptionArg.Builder setExtraTargets​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`extraTargets`](XcodeWorkspaceConfigDescriptionArg.html#getExtraTargets())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of extraTargets elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllExtraTargets(java.lang.Iterable)}

        -   #### addAllExtraTargets

            ``` methodSignature
            public final XcodeWorkspaceConfigDescriptionArg.Builder addAllExtraTargets​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`extraTargets`](XcodeWorkspaceConfigDescriptionArg.html#getExtraTargets())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of extraTargets elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addExtraShallowTargets(com.facebook.buck.core.model.BuildTarget)}

        -   #### addExtraShallowTargets

            ``` methodSignature
            public final XcodeWorkspaceConfigDescriptionArg.Builder addExtraShallowTargets​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`extraShallowTargets`](XcodeWorkspaceConfigDescriptionArg.html#getExtraShallowTargets())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A extraShallowTargets element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addExtraShallowTargets(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addExtraShallowTargets

            ``` methodSignature
            public final XcodeWorkspaceConfigDescriptionArg.Builder addExtraShallowTargets​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`extraShallowTargets`](XcodeWorkspaceConfigDescriptionArg.html#getExtraShallowTargets())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of extraShallowTargets elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setExtraShallowTargets(java.lang.Iterable)}

        -   #### setExtraShallowTargets

            ``` methodSignature
            public final XcodeWorkspaceConfigDescriptionArg.Builder setExtraShallowTargets​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`extraShallowTargets`](XcodeWorkspaceConfigDescriptionArg.html#getExtraShallowTargets())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of extraShallowTargets elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllExtraShallowTargets(java.lang.Iterable)}

        -   #### addAllExtraShallowTargets

            ``` methodSignature
            public final XcodeWorkspaceConfigDescriptionArg.Builder addAllExtraShallowTargets​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`extraShallowTargets`](XcodeWorkspaceConfigDescriptionArg.html#getExtraShallowTargets())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of extraShallowTargets elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setWorkspaceName(java.lang.String)}

        -   #### setWorkspaceName

            ``` methodSignature
            public final XcodeWorkspaceConfigDescriptionArg.Builder setWorkspaceName​(String workspaceName)
            ```

            ::: block
            Initializes the optional value
            [`workspaceName`](XcodeWorkspaceConfigDescriptionArg.html#getWorkspaceName())
            to workspaceName.
            :::

            [Parameters:]{.paramLabel}
            :   `workspaceName` - The value for workspaceName

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setWorkspaceName(java.util.Optional)}

        -   #### setWorkspaceName

            ``` methodSignature
            public final XcodeWorkspaceConfigDescriptionArg.Builder setWorkspaceName​(Optional<String> workspaceName)
            ```

            ::: block
            Initializes the optional value
            [`workspaceName`](XcodeWorkspaceConfigDescriptionArg.html#getWorkspaceName())
            to workspaceName.
            :::

            [Parameters:]{.paramLabel}
            :   `workspaceName` - The value for workspaceName

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putActionConfigNames(com.facebook.buck.features.apple.common.SchemeActionType,java.lang.String)}

        -   #### putActionConfigNames

            ``` methodSignature
            public final XcodeWorkspaceConfigDescriptionArg.Builder putActionConfigNames​(SchemeActionType key,
                                                                                         String value)
            ```

            ::: block
            Put one entry to the
            [`actionConfigNames`](XcodeWorkspaceConfigDescriptionArg.html#getActionConfigNames())
            map.
            :::

            [Parameters:]{.paramLabel}
            :   `key` - The key in the actionConfigNames map
            :   `value` - The associated value in the actionConfigNames
                map

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putActionConfigNames(java.util.Map.Entry)}

        -   #### putActionConfigNames

            ``` methodSignature
            public final XcodeWorkspaceConfigDescriptionArg.Builder putActionConfigNames​(Map.Entry<SchemeActionType,​? extends String> entry)
            ```

            ::: block
            Put one entry to the
            [`actionConfigNames`](XcodeWorkspaceConfigDescriptionArg.html#getActionConfigNames())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entry` - The key and value entry

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setActionConfigNames(java.util.Map)}

        -   #### setActionConfigNames

            ``` methodSignature
            public final XcodeWorkspaceConfigDescriptionArg.Builder setActionConfigNames​(Map<SchemeActionType,​? extends String> entries)
            ```

            ::: block
            Sets or replaces all mappings from the specified map as
            entries for the
            [`actionConfigNames`](XcodeWorkspaceConfigDescriptionArg.html#getActionConfigNames())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entries` - The entries that will be added to the
                actionConfigNames map

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putAllActionConfigNames(java.util.Map)}

        -   #### putAllActionConfigNames

            ``` methodSignature
            public final XcodeWorkspaceConfigDescriptionArg.Builder putAllActionConfigNames​(Map<SchemeActionType,​? extends String> entries)
            ```

            ::: block
            Put all mappings from the specified map as entries to
            [`actionConfigNames`](XcodeWorkspaceConfigDescriptionArg.html#getActionConfigNames())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entries` - The entries that will be added to the
                actionConfigNames map

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putExtraSchemes(java.lang.String,com.facebook.buck.core.model.BuildTarget)}

        -   #### putExtraSchemes

            ``` methodSignature
            public final XcodeWorkspaceConfigDescriptionArg.Builder putExtraSchemes​(String key,
                                                                                    BuildTarget value)
            ```

            ::: block
            Put one entry to the
            [`extraSchemes`](XcodeWorkspaceConfigDescriptionArg.html#getExtraSchemes())
            map.
            :::

            [Parameters:]{.paramLabel}
            :   `key` - The key in the extraSchemes map
            :   `value` - The associated value in the extraSchemes map

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putExtraSchemes(java.util.Map.Entry)}

        -   #### putExtraSchemes

            ``` methodSignature
            public final XcodeWorkspaceConfigDescriptionArg.Builder putExtraSchemes​(Map.Entry<String,​? extends BuildTarget> entry)
            ```

            ::: block
            Put one entry to the
            [`extraSchemes`](XcodeWorkspaceConfigDescriptionArg.html#getExtraSchemes())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entry` - The key and value entry

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setExtraSchemes(java.util.Map)}

        -   #### setExtraSchemes

            ``` methodSignature
            public final XcodeWorkspaceConfigDescriptionArg.Builder setExtraSchemes​(Map<String,​? extends BuildTarget> entries)
            ```

            ::: block
            Sets or replaces all mappings from the specified map as
            entries for the
            [`extraSchemes`](XcodeWorkspaceConfigDescriptionArg.html#getExtraSchemes())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entries` - The entries that will be added to the
                extraSchemes map

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putAllExtraSchemes(java.util.Map)}

        -   #### putAllExtraSchemes

            ``` methodSignature
            public final XcodeWorkspaceConfigDescriptionArg.Builder putAllExtraSchemes​(Map<String,​? extends BuildTarget> entries)
            ```

            ::: block
            Put all mappings from the specified map as entries to
            [`extraSchemes`](XcodeWorkspaceConfigDescriptionArg.html#getExtraSchemes())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entries` - The entries that will be added to the
                extraSchemes map

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setEnvironmentVariables(com.google.common.collect.ImmutableMap)}

        -   #### setEnvironmentVariables

            ``` methodSignature
            public final XcodeWorkspaceConfigDescriptionArg.Builder setEnvironmentVariables​(com.google.common.collect.ImmutableMap<SchemeActionType,​com.google.common.collect.ImmutableMap<String,​String>> environmentVariables)
            ```

            ::: block
            Initializes the optional value
            [`environmentVariables`](XcodeWorkspaceConfigDescriptionArg.html#getEnvironmentVariables())
            to environmentVariables.
            :::

            [Parameters:]{.paramLabel}
            :   `environmentVariables` - The value for
                environmentVariables

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setEnvironmentVariables(java.util.Optional)}

        -   #### setEnvironmentVariables

            ``` methodSignature
            public final XcodeWorkspaceConfigDescriptionArg.Builder setEnvironmentVariables​(Optional<? extends com.google.common.collect.ImmutableMap<SchemeActionType,​com.google.common.collect.ImmutableMap<String,​String>>> environmentVariables)
            ```

            ::: block
            Initializes the optional value
            [`environmentVariables`](XcodeWorkspaceConfigDescriptionArg.html#getEnvironmentVariables())
            to environmentVariables.
            :::

            [Parameters:]{.paramLabel}
            :   `environmentVariables` - The value for
                environmentVariables

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCommandLineArguments(com.google.common.collect.ImmutableMap)}

        -   #### setCommandLineArguments

            ``` methodSignature
            public final XcodeWorkspaceConfigDescriptionArg.Builder setCommandLineArguments​(com.google.common.collect.ImmutableMap<SchemeActionType,​com.google.common.collect.ImmutableMap<String,​String>> commandLineArguments)
            ```

            ::: block
            Initializes the optional value
            [`commandLineArguments`](XcodeWorkspaceConfigDescriptionArg.html#getCommandLineArguments())
            to commandLineArguments.
            :::

            [Parameters:]{.paramLabel}
            :   `commandLineArguments` - The value for
                commandLineArguments

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setCommandLineArguments(java.util.Optional)}

        -   #### setCommandLineArguments

            ``` methodSignature
            public final XcodeWorkspaceConfigDescriptionArg.Builder setCommandLineArguments​(Optional<? extends com.google.common.collect.ImmutableMap<SchemeActionType,​com.google.common.collect.ImmutableMap<String,​String>>> commandLineArguments)
            ```

            ::: block
            Initializes the optional value
            [`commandLineArguments`](XcodeWorkspaceConfigDescriptionArg.html#getCommandLineArguments())
            to commandLineArguments.
            :::

            [Parameters:]{.paramLabel}
            :   `commandLineArguments` - The value for
                commandLineArguments

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setApplicationLanguage(java.lang.String)}

        -   #### setApplicationLanguage

            ``` methodSignature
            public final XcodeWorkspaceConfigDescriptionArg.Builder setApplicationLanguage​(String applicationLanguage)
            ```

            ::: block
            Initializes the optional value
            [`applicationLanguage`](XcodeWorkspaceConfigDescriptionArg.html#getApplicationLanguage())
            to applicationLanguage.
            :::

            [Parameters:]{.paramLabel}
            :   `applicationLanguage` - The value for
                applicationLanguage

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setApplicationLanguage(java.util.Optional)}

        -   #### setApplicationLanguage

            ``` methodSignature
            public final XcodeWorkspaceConfigDescriptionArg.Builder setApplicationLanguage​(Optional<String> applicationLanguage)
            ```

            ::: block
            Initializes the optional value
            [`applicationLanguage`](XcodeWorkspaceConfigDescriptionArg.html#getApplicationLanguage())
            to applicationLanguage.
            :::

            [Parameters:]{.paramLabel}
            :   `applicationLanguage` - The value for
                applicationLanguage

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setApplicationRegion(java.lang.String)}

        -   #### setApplicationRegion

            ``` methodSignature
            public final XcodeWorkspaceConfigDescriptionArg.Builder setApplicationRegion​(String applicationRegion)
            ```

            ::: block
            Initializes the optional value
            [`applicationRegion`](XcodeWorkspaceConfigDescriptionArg.html#getApplicationRegion())
            to applicationRegion.
            :::

            [Parameters:]{.paramLabel}
            :   `applicationRegion` - The value for applicationRegion

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setApplicationRegion(java.util.Optional)}

        -   #### setApplicationRegion

            ``` methodSignature
            public final XcodeWorkspaceConfigDescriptionArg.Builder setApplicationRegion​(Optional<String> applicationRegion)
            ```

            ::: block
            Initializes the optional value
            [`applicationRegion`](XcodeWorkspaceConfigDescriptionArg.html#getApplicationRegion())
            to applicationRegion.
            :::

            [Parameters:]{.paramLabel}
            :   `applicationRegion` - The value for applicationRegion

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setExpandVariablesBasedOn(com.google.common.collect.ImmutableMap)}

        -   #### setExpandVariablesBasedOn

            ``` methodSignature
            public final XcodeWorkspaceConfigDescriptionArg.Builder setExpandVariablesBasedOn​(com.google.common.collect.ImmutableMap<SchemeActionType,​BuildTarget> expandVariablesBasedOn)
            ```

            ::: block
            Initializes the optional value
            [`expandVariablesBasedOn`](XcodeWorkspaceConfigDescriptionArg.html#getExpandVariablesBasedOn())
            to expandVariablesBasedOn.
            :::

            [Parameters:]{.paramLabel}
            :   `expandVariablesBasedOn` - The value for
                expandVariablesBasedOn

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setExpandVariablesBasedOn(java.util.Optional)}

        -   #### setExpandVariablesBasedOn

            ``` methodSignature
            public final XcodeWorkspaceConfigDescriptionArg.Builder setExpandVariablesBasedOn​(Optional<? extends com.google.common.collect.ImmutableMap<SchemeActionType,​BuildTarget>> expandVariablesBasedOn)
            ```

            ::: block
            Initializes the optional value
            [`expandVariablesBasedOn`](XcodeWorkspaceConfigDescriptionArg.html#getExpandVariablesBasedOn())
            to expandVariablesBasedOn.
            :::

            [Parameters:]{.paramLabel}
            :   `expandVariablesBasedOn` - The value for
                expandVariablesBasedOn

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setWasCreatedForAppExtension(boolean)}

        -   #### setWasCreatedForAppExtension

            ``` methodSignature
            public final XcodeWorkspaceConfigDescriptionArg.Builder setWasCreatedForAppExtension​(boolean wasCreatedForAppExtension)
            ```

            ::: block
            Initializes the optional value
            [`wasCreatedForAppExtension`](XcodeWorkspaceConfigDescriptionArg.html#getWasCreatedForAppExtension())
            to wasCreatedForAppExtension.
            :::

            [Parameters:]{.paramLabel}
            :   `wasCreatedForAppExtension` - The value for
                wasCreatedForAppExtension

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setWasCreatedForAppExtension(java.util.Optional)}

        -   #### setWasCreatedForAppExtension

            ``` methodSignature
            public final XcodeWorkspaceConfigDescriptionArg.Builder setWasCreatedForAppExtension​(Optional<Boolean> wasCreatedForAppExtension)
            ```

            ::: block
            Initializes the optional value
            [`wasCreatedForAppExtension`](XcodeWorkspaceConfigDescriptionArg.html#getWasCreatedForAppExtension())
            to wasCreatedForAppExtension.
            :::

            [Parameters:]{.paramLabel}
            :   `wasCreatedForAppExtension` - The value for
                wasCreatedForAppExtension

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setIsRemoteRunnable(boolean)}

        -   #### setIsRemoteRunnable

            ``` methodSignature
            public final XcodeWorkspaceConfigDescriptionArg.Builder setIsRemoteRunnable​(boolean isRemoteRunnable)
            ```

            ::: block
            Initializes the optional value
            [`isRemoteRunnable`](XcodeWorkspaceConfigDescriptionArg.html#getIsRemoteRunnable())
            to isRemoteRunnable.
            :::

            [Parameters:]{.paramLabel}
            :   `isRemoteRunnable` - The value for isRemoteRunnable

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setIsRemoteRunnable(java.util.Optional)}

        -   #### setIsRemoteRunnable

            ``` methodSignature
            public final XcodeWorkspaceConfigDescriptionArg.Builder setIsRemoteRunnable​(Optional<Boolean> isRemoteRunnable)
            ```

            ::: block
            Initializes the optional value
            [`isRemoteRunnable`](XcodeWorkspaceConfigDescriptionArg.html#getIsRemoteRunnable())
            to isRemoteRunnable.
            :::

            [Parameters:]{.paramLabel}
            :   `isRemoteRunnable` - The value for isRemoteRunnable

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setExplicitRunnablePath(java.lang.String)}

        -   #### setExplicitRunnablePath

            ``` methodSignature
            public final XcodeWorkspaceConfigDescriptionArg.Builder setExplicitRunnablePath​(String explicitRunnablePath)
            ```

            ::: block
            Initializes the optional value
            [`explicitRunnablePath`](XcodeWorkspaceConfigDescriptionArg.html#getExplicitRunnablePath())
            to explicitRunnablePath.
            :::

            [Parameters:]{.paramLabel}
            :   `explicitRunnablePath` - The value for
                explicitRunnablePath

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setExplicitRunnablePath(java.util.Optional)}

        -   #### setExplicitRunnablePath

            ``` methodSignature
            public final XcodeWorkspaceConfigDescriptionArg.Builder setExplicitRunnablePath​(Optional<String> explicitRunnablePath)
            ```

            ::: block
            Initializes the optional value
            [`explicitRunnablePath`](XcodeWorkspaceConfigDescriptionArg.html#getExplicitRunnablePath())
            to explicitRunnablePath.
            :::

            [Parameters:]{.paramLabel}
            :   `explicitRunnablePath` - The value for
                explicitRunnablePath

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setNotificationPayloadFile(java.lang.String)}

        -   #### setNotificationPayloadFile

            ``` methodSignature
            public final XcodeWorkspaceConfigDescriptionArg.Builder setNotificationPayloadFile​(String notificationPayloadFile)
            ```

            ::: block
            Initializes the optional value
            [`notificationPayloadFile`](XcodeWorkspaceConfigDescriptionArg.html#getNotificationPayloadFile())
            to notificationPayloadFile.
            :::

            [Parameters:]{.paramLabel}
            :   `notificationPayloadFile` - The value for
                notificationPayloadFile

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setNotificationPayloadFile(java.util.Optional)}

        -   #### setNotificationPayloadFile

            ``` methodSignature
            public final XcodeWorkspaceConfigDescriptionArg.Builder setNotificationPayloadFile​(Optional<String> notificationPayloadFile)
            ```

            ::: block
            Initializes the optional value
            [`notificationPayloadFile`](XcodeWorkspaceConfigDescriptionArg.html#getNotificationPayloadFile())
            to notificationPayloadFile.
            :::

            [Parameters:]{.paramLabel}
            :   `notificationPayloadFile` - The value for
                notificationPayloadFile

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setWatchInterface(com.facebook.buck.apple.xcode.XCScheme.LaunchAction.WatchInterface)}

        -   #### setWatchInterface

            ``` methodSignature
            public final XcodeWorkspaceConfigDescriptionArg.Builder setWatchInterface​(XCScheme.LaunchAction.WatchInterface watchInterface)
            ```

            ::: block
            Initializes the optional value
            [`watchInterface`](XcodeWorkspaceConfigDescriptionArg.html#getWatchInterface())
            to watchInterface.
            :::

            [Parameters:]{.paramLabel}
            :   `watchInterface` - The value for watchInterface

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setWatchInterface(java.util.Optional)}

        -   #### setWatchInterface

            ``` methodSignature
            public final XcodeWorkspaceConfigDescriptionArg.Builder setWatchInterface​(Optional<? extends XCScheme.LaunchAction.WatchInterface> watchInterface)
            ```

            ::: block
            Initializes the optional value
            [`watchInterface`](XcodeWorkspaceConfigDescriptionArg.html#getWatchInterface())
            to watchInterface.
            :::

            [Parameters:]{.paramLabel}
            :   `watchInterface` - The value for watchInterface

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLaunchStyle(com.facebook.buck.apple.xcode.XCScheme.LaunchAction.LaunchStyle)}

        -   #### setLaunchStyle

            ``` methodSignature
            public final XcodeWorkspaceConfigDescriptionArg.Builder setLaunchStyle​(XCScheme.LaunchAction.LaunchStyle launchStyle)
            ```

            ::: block
            Initializes the optional value
            [`launchStyle`](XcodeWorkspaceConfigDescriptionArg.html#getLaunchStyle())
            to launchStyle.
            :::

            [Parameters:]{.paramLabel}
            :   `launchStyle` - The value for launchStyle

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setLaunchStyle(java.util.Optional)}

        -   #### setLaunchStyle

            ``` methodSignature
            public final XcodeWorkspaceConfigDescriptionArg.Builder setLaunchStyle​(Optional<? extends XCScheme.LaunchAction.LaunchStyle> launchStyle)
            ```

            ::: block
            Initializes the optional value
            [`launchStyle`](XcodeWorkspaceConfigDescriptionArg.html#getLaunchStyle())
            to launchStyle.
            :::

            [Parameters:]{.paramLabel}
            :   `launchStyle` - The value for launchStyle

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setAdditionalSchemeActions(com.google.common.collect.ImmutableMap)}

        -   #### setAdditionalSchemeActions

            ``` methodSignature
            public final XcodeWorkspaceConfigDescriptionArg.Builder setAdditionalSchemeActions​(com.google.common.collect.ImmutableMap<SchemeActionType,​com.google.common.collect.ImmutableMap<XCScheme.AdditionalActions,​com.google.common.collect.ImmutableList<String>>> additionalSchemeActions)
            ```

            ::: block
            Initializes the optional value
            [`additionalSchemeActions`](XcodeWorkspaceConfigDescriptionArg.html#getAdditionalSchemeActions())
            to additionalSchemeActions.
            :::

            [Parameters:]{.paramLabel}
            :   `additionalSchemeActions` - The value for
                additionalSchemeActions

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setAdditionalSchemeActions(java.util.Optional)}

        -   #### setAdditionalSchemeActions

            ``` methodSignature
            public final XcodeWorkspaceConfigDescriptionArg.Builder setAdditionalSchemeActions​(Optional<? extends com.google.common.collect.ImmutableMap<SchemeActionType,​com.google.common.collect.ImmutableMap<XCScheme.AdditionalActions,​com.google.common.collect.ImmutableList<String>>>> additionalSchemeActions)
            ```

            ::: block
            Initializes the optional value
            [`additionalSchemeActions`](XcodeWorkspaceConfigDescriptionArg.html#getAdditionalSchemeActions())
            to additionalSchemeActions.
            :::

            [Parameters:]{.paramLabel}
            :   `additionalSchemeActions` - The value for
                additionalSchemeActions

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCompatibleWith(com.facebook.buck.core.model.UnconfiguredBuildTarget)}

        -   #### addCompatibleWith

            ``` methodSignature
            public final XcodeWorkspaceConfigDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget element)
            ```

            ::: block
            Adds one element to
            [`compatibleWith`](XcodeWorkspaceConfigDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A compatibleWith element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCompatibleWith(com.facebook.buck.core.model.UnconfiguredBuildTarget...)}

        -   #### addCompatibleWith

            ``` methodSignature
            public final XcodeWorkspaceConfigDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](XcodeWorkspaceConfigDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCompatibleWith(java.lang.Iterable)}

        -   #### setCompatibleWith

            ``` methodSignature
            public final XcodeWorkspaceConfigDescriptionArg.Builder setCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`compatibleWith`](XcodeWorkspaceConfigDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllCompatibleWith(java.lang.Iterable)}

        -   #### addAllCompatibleWith

            ``` methodSignature
            public final XcodeWorkspaceConfigDescriptionArg.Builder addAllCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](XcodeWorkspaceConfigDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDefaultTargetPlatform(com.facebook.buck.core.model.UnconfiguredBuildTarget)}

        -   #### setDefaultTargetPlatform

            ``` methodSignature
            public final XcodeWorkspaceConfigDescriptionArg.Builder setDefaultTargetPlatform​(UnconfiguredBuildTarget defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](XcodeWorkspaceConfigDescriptionArg.html#getDefaultTargetPlatform())
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
            public final XcodeWorkspaceConfigDescriptionArg.Builder setDefaultTargetPlatform​(Optional<? extends UnconfiguredBuildTarget> defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](XcodeWorkspaceConfigDescriptionArg.html#getDefaultTargetPlatform())
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
            public final XcodeWorkspaceConfigDescriptionArg.Builder addLabels​(String element)
            ```

            ::: block
            Adds one element to
            [`labels`](XcodeWorkspaceConfigDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A labels element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLabels(java.lang.String...)}

        -   #### addLabels

            ``` methodSignature
            public final XcodeWorkspaceConfigDescriptionArg.Builder addLabels​(String... elements)
            ```

            ::: block
            Adds elements to
            [`labels`](XcodeWorkspaceConfigDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLabels(java.lang.Iterable)}

        -   #### setLabels

            ``` methodSignature
            public final XcodeWorkspaceConfigDescriptionArg.Builder setLabels​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`labels`](XcodeWorkspaceConfigDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLabels(java.lang.Iterable)}

        -   #### addAllLabels

            ``` methodSignature
            public final XcodeWorkspaceConfigDescriptionArg.Builder addAllLabels​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`labels`](XcodeWorkspaceConfigDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLicenses(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### addLicenses

            ``` methodSignature
            public final XcodeWorkspaceConfigDescriptionArg.Builder addLicenses​(SourcePath element)
            ```

            ::: block
            Adds one element to
            [`licenses`](XcodeWorkspaceConfigDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A licenses element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLicenses(com.facebook.buck.core.sourcepath.SourcePath...)}

        -   #### addLicenses

            ``` methodSignature
            public final XcodeWorkspaceConfigDescriptionArg.Builder addLicenses​(SourcePath... elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](XcodeWorkspaceConfigDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLicenses(java.lang.Iterable)}

        -   #### setLicenses

            ``` methodSignature
            public final XcodeWorkspaceConfigDescriptionArg.Builder setLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`licenses`](XcodeWorkspaceConfigDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLicenses(java.lang.Iterable)}

        -   #### addAllLicenses

            ``` methodSignature
            public final XcodeWorkspaceConfigDescriptionArg.Builder addAllLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](XcodeWorkspaceConfigDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setName(java.lang.String)}

        -   #### setName

            ``` methodSignature
            public final XcodeWorkspaceConfigDescriptionArg.Builder setName​(String name)
            ```

            ::: block
            Initializes the value for the
            [`name`](XcodeWorkspaceConfigDescriptionArg.html#getName())
            attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `name` - The value for name

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#build()}

        -   #### build

            ``` methodSignature
            public XcodeWorkspaceConfigDescriptionArg build()
            ```

            ::: block
            Builds a new
            [`XcodeWorkspaceConfigDescriptionArg`](XcodeWorkspaceConfigDescriptionArg.html "class in com.facebook.buck.features.apple.common").
            :::

            [Returns:]{.returnLabel}
            :   An immutable instance of
                XcodeWorkspaceConfigDescriptionArg

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

-   [Overview](../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../deprecated-list.html)
-   [Index](../../../../../../index-all.html)
-   [Help](../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../allclasses.html)

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
