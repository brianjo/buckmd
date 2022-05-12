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

## Class AndroidBinaryDescriptionArg.Builder {#class-androidbinarydescriptionarg.builder .title title="Class AndroidBinaryDescriptionArg.Builder"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.android.AndroidBinaryDescriptionArg.Builder

::: description
-   

    Enclosing class:
    :   [AndroidBinaryDescriptionArg](AndroidBinaryDescriptionArg.html "class in com.facebook.buck.android")

    ------------------------------------------------------------------------

        @NotThreadSafe
        public static final class AndroidBinaryDescriptionArg.Builder
        extends Object

    ::: block
    Builds instances of type
    [`AndroidBinaryDescriptionArg`](AndroidBinaryDescriptionArg.html "class in com.facebook.buck.android").
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
        | `AndroidBinaryDe      | `addAdditionalAaptPa  | ::: block             |
        | scriptionArg.Builder` | rams​(String element)` | Adds one element to   |
        |                       |                       | [`additionalAaptParam |
        |                       |                       | s`](AndroidBinaryDesc |
        |                       |                       | riptionArg.html#getAd |
        |                       |                       | ditionalAaptParams()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `ad                   | ::: block             |
        | scriptionArg.Builder` | dAdditionalAaptParams | Adds elements to      |
        |                       | ​(String... elements)` | [`additionalAaptParam |
        |                       |                       | s`](AndroidBinaryDesc |
        |                       |                       | riptionArg.html#getAd |
        |                       |                       | ditionalAaptParams()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `addAllAdditi         | ::: block             |
        | scriptionArg.Builder` | onalAaptParams​(Iterab | Adds elements to      |
        |                       | le<String> elements)` | [`additionalAaptParam |
        |                       |                       | s`](AndroidBinaryDesc |
        |                       |                       | riptionArg.html#getAd |
        |                       |                       | ditionalAaptParams()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `addAllAllowe         | ::: block             |
        | scriptionArg.Builder` | dDuplicateResourceTyp | Adds elements to      |
        |                       | es​(Iterable<RDotTxtEn | [`allowedDuplicate    |
        |                       | try.RType> elements)` | ResourceTypes`](Andro |
        |                       |                       | idBinaryDescriptionAr |
        |                       |                       | g.html#getAllowedDupl |
        |                       |                       | icateResourceTypes()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `a                    | ::: block             |
        | scriptionArg.Builder` | ddAllApplicationModul | Adds elements to      |
        |                       | esWithManifest​(Iterab | [`applicationModules  |
        |                       | le<String> elements)` | WithManifest`](Androi |
        |                       |                       | dBinaryDescriptionArg |
        |                       |                       | .html#getApplicationM |
        |                       |                       | odulesWithManifest()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `ad                   | ::: block             |
        | scriptionArg.Builder` | dAllApplicationModule | Adds elements to      |
        |                       | sWithResources​(Iterab | [                     |
        |                       | le<String> elements)` | `applicationModulesWi |
        |                       |                       | thResources`](Android |
        |                       |                       | BinaryDescriptionArg. |
        |                       |                       | html#getApplicationMo |
        |                       |                       | dulesWithResources()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `addAllAppl           | ::: block             |
        | scriptionArg.Builder` | icationModuleTargets​( | Adds elements to      |
        |                       | Iterable<? extends Bu | [`applic              |
        |                       | ildTarget> elements)` | ationModuleTargets`]( |
        |                       |                       | AndroidBinaryDescript |
        |                       |                       | ionArg.html#getApplic |
        |                       |                       | ationModuleTargets()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `addAllBanne          | ::: block             |
        | scriptionArg.Builder` | dDuplicateResourceTyp | Adds elements to      |
        |                       | es​(Iterable<RDotTxtEn | [`bannedDuplicat      |
        |                       | try.RType> elements)` | eResourceTypes`](Andr |
        |                       |                       | oidBinaryDescriptionA |
        |                       |                       | rg.html#getBannedDupl |
        |                       |                       | icateResourceTypes()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `addAllCompat         | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Iterable<? e | Adds elements to      |
        |                       | xtends UnconfiguredBu | [`compati             |
        |                       | ildTarget> elements)` | bleWith`](AndroidBina |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `addAllCpu            | ::: block             |
        | scriptionArg.Builder` | Filters​(Iterable<Targ | Adds elements to      |
        |                       | etCpuType> elements)` | [                     |
        |                       |                       | `cpuFilters`](Android |
        |                       |                       | BinaryDescriptionArg. |
        |                       |                       | html#getCpuFilters()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `addAllDeps​(          | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Adds elements to      |
        |                       | ildTarget> elements)` | [`deps`](A            |
        |                       |                       | ndroidBinaryDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `addAllExopackag      | ::: block             |
        | scriptionArg.Builder` | eModes​(Iterable<Exopa | Adds elements to      |
        |                       | ckageMode> elements)` | [`exopackag           |
        |                       |                       | eModes`](AndroidBinar |
        |                       |                       | yDescriptionArg.html# |
        |                       |                       | getExopackageModes()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `addAllExtraFil       | ::: block             |
        | scriptionArg.Builder` | teredResources​(Iterab | Adds elements to      |
        |                       | le<String> elements)` | [`ex                  |
        |                       |                       | traFilteredResources` |
        |                       |                       | ](AndroidBinaryDescri |
        |                       |                       | ptionArg.html#getExtr |
        |                       |                       | aFilteredResources()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `addAllLabels​(Iterab  | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Adds elements to      |
        |                       |                       | [`labels`](And        |
        |                       |                       | roidBinaryDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `addAllLicenses       | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Adds elements to      |
        |                       | ourcePath> elements)` | [`licenses`](Andro    |
        |                       |                       | idBinaryDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `addAllLocales​(Iterab | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Adds elements to      |
        |                       |                       | [`locales`](Andr      |
        |                       |                       | oidBinaryDescriptionA |
        |                       |                       | rg.html#getLocales()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `addAllNoDx​(          | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Adds elements to      |
        |                       | ildTarget> elements)` | [`noDx`](A            |
        |                       |                       | ndroidBinaryDescripti |
        |                       |                       | onArg.html#getNoDx()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `addAllowedDuplicate  | ::: block             |
        | scriptionArg.Builder` | ResourceTypes​(RDotTxt | Adds one element to   |
        |                       | Entry.RType element)` | [`allowedDuplicate    |
        |                       |                       | ResourceTypes`](Andro |
        |                       |                       | idBinaryDescriptionAr |
        |                       |                       | g.html#getAllowedDupl |
        |                       |                       | icateResourceTypes()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `ad                   | ::: block             |
        | scriptionArg.Builder` | dAllowedDuplicateReso | Adds elements to      |
        |                       | urceTypes​(RDotTxtEntr | [`allowedDuplicate    |
        |                       | y.RType... elements)` | ResourceTypes`](Andro |
        |                       |                       | idBinaryDescriptionAr |
        |                       |                       | g.html#getAllowedDupl |
        |                       |                       | icateResourceTypes()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `addAllPrepr          | ::: block             |
        | scriptionArg.Builder` | ocessJavaClassesDeps​( | Adds elements to      |
        |                       | Iterable<? extends Bu | [`preproce            |
        |                       | ildTarget> elements)` | ssJavaClassesDeps`](A |
        |                       |                       | ndroidBinaryDescripti |
        |                       |                       | onArg.html#getPreproc |
        |                       |                       | essJavaClassesDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `addAllPrim           | ::: block             |
        | scriptionArg.Builder` | aryDexPatterns​(Iterab | Adds elements to      |
        |                       | le<String> elements)` | [`primaryDexPatte     |
        |                       |                       | rns`](AndroidBinaryDe |
        |                       |                       | scriptionArg.html#get |
        |                       |                       | PrimaryDexPatterns()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `addAllP              | ::: block             |
        | scriptionArg.Builder` | roguardJvmArgs​(Iterab | Adds elements to      |
        |                       | le<String> elements)` | [`proguardJ           |
        |                       |                       | vmArgs`](AndroidBinar |
        |                       |                       | yDescriptionArg.html# |
        |                       |                       | getProguardJvmArgs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `addAl                | ::: block             |
        | scriptionArg.Builder` | lRedexExtraArgs​(Itera | Adds elements to      |
        |                       | ble<? extends StringW | [`redexEx             |
        |                       | ithMacros> elements)` | traArgs`](AndroidBina |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getRedexExtraArgs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `addAllRelinkerWhitel | ::: block             |
        | scriptionArg.Builder` | ist​(Iterable<? extend | Adds elements to      |
        |                       | s Pattern> elements)` | [`relinkerWhite       |
        |                       |                       | list`](AndroidBinaryD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tRelinkerWhitelist()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `addAll               | ::: block             |
        | scriptionArg.Builder` | ResourceFilter​(Iterab | Adds elements to      |
        |                       | le<String> elements)` | [`resourc             |
        |                       |                       | eFilter`](AndroidBina |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getResourceFilter()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `addAllTests​(         | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Adds elements to      |
        |                       | ildTarget> elements)` | [`tests`](An          |
        |                       |                       | droidBinaryDescriptio |
        |                       |                       | nArg.html#getTests()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `addAppli             | ::: block             |
        | scriptionArg.Builder` | cationModulesWithMani | Adds one element to   |
        |                       | fest​(String element)` | [`applicationModules  |
        |                       |                       | WithManifest`](Androi |
        |                       |                       | dBinaryDescriptionArg |
        |                       |                       | .html#getApplicationM |
        |                       |                       | odulesWithManifest()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `addApplicati         | ::: block             |
        | scriptionArg.Builder` | onModulesWithManifest | Adds elements to      |
        |                       | ​(String... elements)` | [`applicationModules  |
        |                       |                       | WithManifest`](Androi |
        |                       |                       | dBinaryDescriptionArg |
        |                       |                       | .html#getApplicationM |
        |                       |                       | odulesWithManifest()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `addApplic            | ::: block             |
        | scriptionArg.Builder` | ationModulesWithResou | Adds one element to   |
        |                       | rces​(String element)` | [                     |
        |                       |                       | `applicationModulesWi |
        |                       |                       | thResources`](Android |
        |                       |                       | BinaryDescriptionArg. |
        |                       |                       | html#getApplicationMo |
        |                       |                       | dulesWithResources()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `addApplicatio        | ::: block             |
        | scriptionArg.Builder` | nModulesWithResources | Adds elements to      |
        |                       | ​(String... elements)` | [                     |
        |                       |                       | `applicationModulesWi |
        |                       |                       | thResources`](Android |
        |                       |                       | BinaryDescriptionArg. |
        |                       |                       | html#getApplicationMo |
        |                       |                       | dulesWithResources()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `addAppl              | ::: block             |
        | scriptionArg.Builder` | icationModuleTargets​( | Adds one element to   |
        |                       | BuildTarget element)` | [`applic              |
        |                       |                       | ationModuleTargets`]( |
        |                       |                       | AndroidBinaryDescript |
        |                       |                       | ionArg.html#getApplic |
        |                       |                       | ationModuleTargets()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `addApplicat          | ::: block             |
        | scriptionArg.Builder` | ionModuleTargets​(Buil | Adds elements to      |
        |                       | dTarget... elements)` | [`applic              |
        |                       |                       | ationModuleTargets`]( |
        |                       |                       | AndroidBinaryDescript |
        |                       |                       | ionArg.html#getApplic |
        |                       |                       | ationModuleTargets()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `addBannedDuplicate   | ::: block             |
        | scriptionArg.Builder` | ResourceTypes​(RDotTxt | Adds one element to   |
        |                       | Entry.RType element)` | [`bannedDuplicat      |
        |                       |                       | eResourceTypes`](Andr |
        |                       |                       | oidBinaryDescriptionA |
        |                       |                       | rg.html#getBannedDupl |
        |                       |                       | icateResourceTypes()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `a                    | ::: block             |
        | scriptionArg.Builder` | ddBannedDuplicateReso | Adds elements to      |
        |                       | urceTypes​(RDotTxtEntr | [`bannedDuplicat      |
        |                       | y.RType... elements)` | eResourceTypes`](Andr |
        |                       |                       | oidBinaryDescriptionA |
        |                       |                       | rg.html#getBannedDupl |
        |                       |                       | icateResourceTypes()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `addCompat            | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Unconfigured | Adds one element to   |
        |                       | BuildTarget element)` | [`compati             |
        |                       |                       | bleWith`](AndroidBina |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `addCompatible        | ::: block             |
        | scriptionArg.Builder` | With​(UnconfiguredBuil | Adds elements to      |
        |                       | dTarget... elements)` | [`compati             |
        |                       |                       | bleWith`](AndroidBina |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `addCpuFilters​(Ta     | ::: block             |
        | scriptionArg.Builder` | rgetCpuType element)` | Adds one element to   |
        |                       |                       | [                     |
        |                       |                       | `cpuFilters`](Android |
        |                       |                       | BinaryDescriptionArg. |
        |                       |                       | html#getCpuFilters()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `addCpuFilters​(Target | ::: block             |
        | scriptionArg.Builder` | CpuType... elements)` | Adds elements to      |
        |                       |                       | [                     |
        |                       |                       | `cpuFilters`](Android |
        |                       |                       | BinaryDescriptionArg. |
        |                       |                       | html#getCpuFilters()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `addDeps​(             | ::: block             |
        | scriptionArg.Builder` | BuildTarget element)` | Adds one element to   |
        |                       |                       | [`deps`](A            |
        |                       |                       | ndroidBinaryDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `addDeps​(Buil         | ::: block             |
        | scriptionArg.Builder` | dTarget... elements)` | Adds elements to      |
        |                       |                       | [`deps`](A            |
        |                       |                       | ndroidBinaryDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `a                    | ::: block             |
        | scriptionArg.Builder` | ddExopackageModes​(Exo | Adds one element to   |
        |                       | packageMode element)` | [`exopackag           |
        |                       |                       | eModes`](AndroidBinar |
        |                       |                       | yDescriptionArg.html# |
        |                       |                       | getExopackageModes()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `addEx                | ::: block             |
        | scriptionArg.Builder` | opackageModes​(Exopack | Adds elements to      |
        |                       | ageMode... elements)` | [`exopackag           |
        |                       |                       | eModes`](AndroidBinar |
        |                       |                       | yDescriptionArg.html# |
        |                       |                       | getExopackageModes()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `                     | ::: block             |
        | scriptionArg.Builder` | addExtraFilteredResou | Adds one element to   |
        |                       | rces​(String element)` | [`ex                  |
        |                       |                       | traFilteredResources` |
        |                       |                       | ](AndroidBinaryDescri |
        |                       |                       | ptionArg.html#getExtr |
        |                       |                       | aFilteredResources()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `addE                 | ::: block             |
        | scriptionArg.Builder` | xtraFilteredResources | Adds elements to      |
        |                       | ​(String... elements)` | [`ex                  |
        |                       |                       | traFilteredResources` |
        |                       |                       | ](AndroidBinaryDescri |
        |                       |                       | ptionArg.html#getExtr |
        |                       |                       | aFilteredResources()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `addLa                | ::: block             |
        | scriptionArg.Builder` | bels​(String element)` | Adds one element to   |
        |                       |                       | [`labels`](And        |
        |                       |                       | roidBinaryDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `addLabels            | ::: block             |
        | scriptionArg.Builder` | ​(String... elements)` | Adds elements to      |
        |                       |                       | [`labels`](And        |
        |                       |                       | roidBinaryDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `addLicenses          | ::: block             |
        | scriptionArg.Builder` | ​(SourcePath element)` | Adds one element to   |
        |                       |                       | [`licenses`](Andro    |
        |                       |                       | idBinaryDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `addLicenses​(Sou      | ::: block             |
        | scriptionArg.Builder` | rcePath... elements)` | Adds elements to      |
        |                       |                       | [`licenses`](Andro    |
        |                       |                       | idBinaryDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `addLoc               | ::: block             |
        | scriptionArg.Builder` | ales​(String element)` | Adds one element to   |
        |                       |                       | [`locales`](Andr      |
        |                       |                       | oidBinaryDescriptionA |
        |                       |                       | rg.html#getLocales()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `addLocales           | ::: block             |
        | scriptionArg.Builder` | ​(String... elements)` | Adds elements to      |
        |                       |                       | [`locales`](Andr      |
        |                       |                       | oidBinaryDescriptionA |
        |                       |                       | rg.html#getLocales()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `addNoDx​(             | ::: block             |
        | scriptionArg.Builder` | BuildTarget element)` | Adds one element to   |
        |                       |                       | [`noDx`](A            |
        |                       |                       | ndroidBinaryDescripti |
        |                       |                       | onArg.html#getNoDx()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `addNoDx​(Buil         | ::: block             |
        | scriptionArg.Builder` | dTarget... elements)` | Adds elements to      |
        |                       |                       | [`noDx`](A            |
        |                       |                       | ndroidBinaryDescripti |
        |                       |                       | onArg.html#getNoDx()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `addPrepr             | ::: block             |
        | scriptionArg.Builder` | ocessJavaClassesDeps​( | Adds one element to   |
        |                       | BuildTarget element)` | [`preproce            |
        |                       |                       | ssJavaClassesDeps`](A |
        |                       |                       | ndroidBinaryDescripti |
        |                       |                       | onArg.html#getPreproc |
        |                       |                       | essJavaClassesDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `addPreproces         | ::: block             |
        | scriptionArg.Builder` | sJavaClassesDeps​(Buil | Adds elements to      |
        |                       | dTarget... elements)` | [`preproce            |
        |                       |                       | ssJavaClassesDeps`](A |
        |                       |                       | ndroidBinaryDescripti |
        |                       |                       | onArg.html#getPreproc |
        |                       |                       | essJavaClassesDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `addPrimaryDexPatt    | ::: block             |
        | scriptionArg.Builder` | erns​(String element)` | Adds one element to   |
        |                       |                       | [`primaryDexPatte     |
        |                       |                       | rns`](AndroidBinaryDe |
        |                       |                       | scriptionArg.html#get |
        |                       |                       | PrimaryDexPatterns()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `                     | ::: block             |
        | scriptionArg.Builder` | addPrimaryDexPatterns | Adds elements to      |
        |                       | ​(String... elements)` | [`primaryDexPatte     |
        |                       |                       | rns`](AndroidBinaryDe |
        |                       |                       | scriptionArg.html#get |
        |                       |                       | PrimaryDexPatterns()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `addProguardJvm       | ::: block             |
        | scriptionArg.Builder` | Args​(String element)` | Adds one element to   |
        |                       |                       | [`proguardJ           |
        |                       |                       | vmArgs`](AndroidBinar |
        |                       |                       | yDescriptionArg.html# |
        |                       |                       | getProguardJvmArgs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `addProguardJvmArgs   | ::: block             |
        | scriptionArg.Builder` | ​(String... elements)` | Adds elements to      |
        |                       |                       | [`proguardJ           |
        |                       |                       | vmArgs`](AndroidBinar |
        |                       |                       | yDescriptionArg.html# |
        |                       |                       | getProguardJvmArgs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `ad                   | ::: block             |
        | scriptionArg.Builder` | dRedexExtraArgs​(Strin | Adds one element to   |
        |                       | gWithMacros element)` | [`redexEx             |
        |                       |                       | traArgs`](AndroidBina |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getRedexExtraArgs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `addRed               | ::: block             |
        | scriptionArg.Builder` | exExtraArgs​(StringWit | Adds elements to      |
        |                       | hMacros... elements)` | [`redexEx             |
        |                       |                       | traArgs`](AndroidBina |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getRedexExtraArgs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `addRelinkerWhitel    | ::: block             |
        | scriptionArg.Builder` | ist​(Pattern element)` | Adds one element to   |
        |                       |                       | [`relinkerWhite       |
        |                       |                       | list`](AndroidBinaryD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tRelinkerWhitelist()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `                     | ::: block             |
        | scriptionArg.Builder` | addRelinkerWhitelist​( | Adds elements to      |
        |                       | Pattern... elements)` | [`relinkerWhite       |
        |                       |                       | list`](AndroidBinaryD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tRelinkerWhitelist()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `addResourceFi        | ::: block             |
        | scriptionArg.Builder` | lter​(String element)` | Adds one element to   |
        |                       |                       | [`resourc             |
        |                       |                       | eFilter`](AndroidBina |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getResourceFilter()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `addResourceFilter    | ::: block             |
        | scriptionArg.Builder` | ​(String... elements)` | Adds elements to      |
        |                       |                       | [`resourc             |
        |                       |                       | eFilter`](AndroidBina |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getResourceFilter()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `addTests​(            | ::: block             |
        | scriptionArg.Builder` | BuildTarget element)` | Adds one element to   |
        |                       |                       | [`tests`](An          |
        |                       |                       | droidBinaryDescriptio |
        |                       |                       | nArg.html#getTests()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `addTests​(Buil        | ::: block             |
        | scriptionArg.Builder` | dTarget... elements)` | Adds elements to      |
        |                       |                       | [`tests`](An          |
        |                       |                       | droidBinaryDescriptio |
        |                       |                       | nArg.html#getTests()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Android              | `build()`             | ::: block             |
        | BinaryDescriptionArg` |                       | Builds a new          |
        |                       |                       | [`AndroidBinaryDesc   |
        |                       |                       | riptionArg`](AndroidB |
        |                       |                       | inaryDescriptionArg.h |
        |                       |                       | tml "class in com.fac |
        |                       |                       | ebook.buck.android"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `from​(com.facebook.   | ::: block             |
        | scriptionArg.Builder` | buck.android.AndroidB | Copy abstract value   |
        |                       | inaryDescription.Abst | type                  |
        |                       | ractAndroidBinaryDesc | `AbstractAndroid      |
        |                       | riptionArg instance)` | BinaryDescriptionArg` |
        |                       |                       | instance into         |
        |                       |                       | builder.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `f                    | ::: block             |
        | scriptionArg.Builder` | rom​(AndroidBinaryDesc | Fill a builder with   |
        |                       | riptionArg instance)` | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `Android              |
        |                       |                       | BinaryDescriptionArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `from​(AndroidGraphEn  | ::: block             |
        | scriptionArg.Builder` | hancerArgs instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.faceb            |
        |                       |                       | ook.buck.android.Andr |
        |                       |                       | oidGraphEnhancerArgs` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `from​(H               | ::: block             |
        | scriptionArg.Builder` | asDuplicateAndroidRes | Fill a builder with   |
        |                       | ourceTypes instance)` | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook.buck    |
        |                       |                       | .android.HasDuplicate |
        |                       |                       | AndroidResourceTypes` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `from​(HasExop         | ::: block             |
        | scriptionArg.Builder` | ackageArgs instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `co                   |
        |                       |                       | m.facebook.buck.andro |
        |                       |                       | id.HasExopackageArgs` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `from​(Bu              | ::: block             |
        | scriptionArg.Builder` | ildRuleArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebo           |
        |                       |                       | ok.buck.core.descript |
        |                       |                       | ion.arg.BuildRuleArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `from​(Cons            | ::: block             |
        | scriptionArg.Builder` | tructorArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook         |
        |                       |                       | .buck.core.descriptio |
        |                       |                       | n.arg.ConstructorArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `fro                  | ::: block             |
        | scriptionArg.Builder` | m​(HasApplicationModul | Fill a builder with   |
        |                       | eBlacklist instance)` | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.fa               |
        |                       |                       | cebook.buck.core.desc |
        |                       |                       | ription.arg.HasApplic |
        |                       |                       | ationModuleBlacklist` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `from​(HasDe           | ::: block             |
        | scriptionArg.Builder` | claredDeps instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook.        |
        |                       |                       | buck.core.description |
        |                       |                       | .arg.HasDeclaredDeps` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `fro                  | ::: block             |
        | scriptionArg.Builder` | m​(HasTests instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.fa               |
        |                       |                       | cebook.buck.core.desc |
        |                       |                       | ription.arg.HasTests` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `putAllAppl           | ::: block             |
        | scriptionArg.Builder` | icationModuleConfigs​( | Put all mappings from |
        |                       | Map<String,​? extends  | the specified map as  |
        |                       | com.google.common.col | entries to            |
        |                       | lect.ImmutableList<Bu | [`applic              |
        |                       | ildTarget>> entries)` | ationModuleConfigs`]( |
        |                       |                       | AndroidBinaryDescript |
        |                       |                       | ionArg.html#getApplic |
        |                       |                       | ationModuleConfigs()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `putAllNati           | ::: block             |
        | scriptionArg.Builder` | veLibraryMergeMap​(Map | Put all mappings from |
        |                       | <String,​? extends Lis | the specified map as  |
        |                       | t<Pattern>> entries)` | entries to            |
        |                       |                       | [`                    |
        |                       |                       | nativeLibraryMergeMap |
        |                       |                       | `](AndroidBinaryDescr |
        |                       |                       | iptionArg.html#getNat |
        |                       |                       | iveLibraryMergeMap()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `p                    | ::: block             |
        | scriptionArg.Builder` | utApplicationModuleCo | Put one entry to the  |
        |                       | nfigs​(String key,     | [`applic              |
        |                       |                       | ationModuleConfigs`]( |
        |                       |    com.google.common. | AndroidBinaryDescript |
        |                       | collect.ImmutableList | ionArg.html#getApplic |
        |                       | <BuildTarget> value)` | ationModuleConfigs()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `putApplicat          | ::: block             |
        | scriptionArg.Builder` | ionModuleConfigs​(Map. | Put one entry to the  |
        |                       | Entry<String,​? extend | [`applic              |
        |                       | s com.google.common.c | ationModuleConfigs`]( |
        |                       | ollect.ImmutableList< | AndroidBinaryDescript |
        |                       | BuildTarget>> entry)` | ionArg.html#getApplic |
        |                       |                       | ationModuleConfigs()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `putNativeLibraryMer  | ::: block             |
        | scriptionArg.Builder` | geMap​(String key,     | Put one entry to the  |
        |                       |                       | [`                    |
        |                       | List<Pattern> value)` | nativeLibraryMergeMap |
        |                       |                       | `](AndroidBinaryDescr |
        |                       |                       | iptionArg.html#getNat |
        |                       |                       | iveLibraryMergeMap()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `putNativeLi          | ::: block             |
        | scriptionArg.Builder` | braryMergeMap​(Map.Ent | Put one entry to the  |
        |                       | ry<String,​? extends L | [`                    |
        |                       | ist<Pattern>> entry)` | nativeLibraryMergeMap |
        |                       |                       | `](AndroidBinaryDescr |
        |                       |                       | iptionArg.html#getNat |
        |                       |                       | iveLibraryMergeMap()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `setAapt2Loca         | ::: block             |
        | scriptionArg.Builder` | leFiltering​(boolean a | Initializes the value |
        |                       | apt2LocaleFiltering)` | for the               |
        |                       |                       | [`aapt2LocaleFilteri  |
        |                       |                       | ng`](AndroidBinaryDes |
        |                       |                       | criptionArg.html#isAa |
        |                       |                       | pt2LocaleFiltering()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `setAaptMode​(com      | ::: block             |
        | scriptionArg.Builder` | .facebook.buck.androi | Initializes the value |
        |                       | d.AaptMode aaptMode)` | for the               |
        |                       |                       | [`aaptMode`](Andro    |
        |                       |                       | idBinaryDescriptionAr |
        |                       |                       | g.html#getAaptMode()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `setAdditi            | ::: block             |
        | scriptionArg.Builder` | onalAaptParams​(Iterab | Sets or replaces all  |
        |                       | le<String> elements)` | elements for          |
        |                       |                       | [`additionalAaptParam |
        |                       |                       | s`](AndroidBinaryDesc |
        |                       |                       | riptionArg.html#getAd |
        |                       |                       | ditionalAaptParams()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `setAllowe            | ::: block             |
        | scriptionArg.Builder` | dDuplicateResourceTyp | Sets or replaces all  |
        |                       | es​(Iterable<RDotTxtEn | elements for          |
        |                       | try.RType> elements)` | [`allowedDuplicate    |
        |                       |                       | ResourceTypes`](Andro |
        |                       |                       | idBinaryDescriptionAr |
        |                       |                       | g.html#getAllowedDupl |
        |                       |                       | icateResourceTypes()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `setAl                | ::: block             |
        | scriptionArg.Builder` | lowRDotJavaInSecondar | Initializes the value |
        |                       | yDex​(boolean allowRDo | for the               |
        |                       | tJavaInSecondaryDex)` | [`allowRDotJa         |
        |                       |                       | vaInSecondaryDex`](An |
        |                       |                       | droidBinaryDescriptio |
        |                       |                       | nArg.html#isAllowRDot |
        |                       |                       | JavaInSecondaryDex()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `setAnd               | ::: block             |
        | scriptionArg.Builder` | roidAppModularityResu | Initializes the       |
        |                       | lt​(SourcePath android | optional value        |
        |                       | AppModularityResult)` | [`androidApp          |
        |                       |                       | ModularityResult`](An |
        |                       |                       | droidBinaryDescriptio |
        |                       |                       | nArg.html#getAndroidA |
        |                       |                       | ppModularityResult()) |
        |                       |                       | to                    |
        |                       |                       | androi                |
        |                       |                       | dAppModularityResult. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `setAn                | ::: block             |
        | scriptionArg.Builder` | droidAppModularityRes | Initializes the       |
        |                       | ult​(Optional<? extend | optional value        |
        |                       | s SourcePath> android | [`androidApp          |
        |                       | AppModularityResult)` | ModularityResult`](An |
        |                       |                       | droidBinaryDescriptio |
        |                       |                       | nArg.html#getAndroidA |
        |                       |                       | ppModularityResult()) |
        |                       |                       | to                    |
        |                       |                       | androi                |
        |                       |                       | dAppModularityResult. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `setAndroidSdk        | ::: block             |
        | scriptionArg.Builder` | ProguardConfig​(com.fa | Initializes the       |
        |                       | cebook.buck.android.P | optional value        |
        |                       | roGuardObfuscateStep. | [`androi              |
        |                       | SdkProguardType andro | dSdkProguardConfig`]( |
        |                       | idSdkProguardConfig)` | AndroidBinaryDescript |
        |                       |                       | ionArg.html#getAndroi |
        |                       |                       | dSdkProguardConfig()) |
        |                       |                       | to                    |
        |                       |                       | andr                  |
        |                       |                       | oidSdkProguardConfig. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `setAndroidSd         | ::: block             |
        | scriptionArg.Builder` | kProguardConfig​(Optio | Initializes the       |
        |                       | nal<? extends com.fac | optional value        |
        |                       | ebook.buck.android.Pr | [`androi              |
        |                       | oGuardObfuscateStep.S | dSdkProguardConfig`]( |
        |                       | dkProguardType> andro | AndroidBinaryDescript |
        |                       | idSdkProguardConfig)` | ionArg.html#getAndroi |
        |                       |                       | dSdkProguardConfig()) |
        |                       |                       | to                    |
        |                       |                       | andr                  |
        |                       |                       | oidSdkProguardConfig. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `setAppl              | ::: block             |
        | scriptionArg.Builder` | icationModuleBlacklis | Initializes the       |
        |                       | t​(List<Query> applica | optional value        |
        |                       | tionModuleBlacklist)` | [`applicatio          |
        |                       |                       | nModuleBlacklist`](An |
        |                       |                       | droidBinaryDescriptio |
        |                       |                       | nArg.html#getApplicat |
        |                       |                       | ionModuleBlacklist()) |
        |                       |                       | to                    |
        |                       |                       | applic                |
        |                       |                       | ationModuleBlacklist. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `setApp               | ::: block             |
        | scriptionArg.Builder` | licationModuleBlackli | Initializes the       |
        |                       | st​(Optional<? extends | optional value        |
        |                       |  List<Query>> applica | [`applicatio          |
        |                       | tionModuleBlacklist)` | nModuleBlacklist`](An |
        |                       |                       | droidBinaryDescriptio |
        |                       |                       | nArg.html#getApplicat |
        |                       |                       | ionModuleBlacklist()) |
        |                       |                       | to                    |
        |                       |                       | applic                |
        |                       |                       | ationModuleBlacklist. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `setAppl              | ::: block             |
        | scriptionArg.Builder` | icationModuleConfigs​( | Sets or replaces all  |
        |                       | Map<String,​? extends  | mappings from the     |
        |                       | com.google.common.col | specified map as      |
        |                       | lect.ImmutableList<Bu | entries for the       |
        |                       | ildTarget>> entries)` | [`applic              |
        |                       |                       | ationModuleConfigs`]( |
        |                       |                       | AndroidBinaryDescript |
        |                       |                       | ionArg.html#getApplic |
        |                       |                       | ationModuleConfigs()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `setApplicati         | ::: block             |
        | scriptionArg.Builder` | onModuleDependencies​( | Initializes the       |
        |                       | com.google.common.col | optional value        |
        |                       | lect.ImmutableMap<Str | [`applicationModul    |
        |                       | ing,​com.google.common | eDependencies`](Andro |
        |                       | .collect.ImmutableLis | idBinaryDescriptionAr |
        |                       | t<String>> applicatio | g.html#getApplication |
        |                       | nModuleDependencies)` | ModuleDependencies()) |
        |                       |                       | to                    |
        |                       |                       | applicati             |
        |                       |                       | onModuleDependencies. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `setApplicat          | ::: block             |
        | scriptionArg.Builder` | ionModuleDependencies | Initializes the       |
        |                       | ​(Optional<? extends c | optional value        |
        |                       | om.google.common.coll | [`applicationModul    |
        |                       | ect.ImmutableMap<Stri | eDependencies`](Andro |
        |                       | ng,​com.google.common. | idBinaryDescriptionAr |
        |                       | collect.ImmutableList | g.html#getApplication |
        |                       | <String>>> applicatio | ModuleDependencies()) |
        |                       | nModuleDependencies)` | to                    |
        |                       |                       | applicati             |
        |                       |                       | onModuleDependencies. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `setApplicationModul  | ::: block             |
        | scriptionArg.Builder` | esWithManifest​(Iterab | Sets or replaces all  |
        |                       | le<String> elements)` | elements for          |
        |                       |                       | [`applicationModules  |
        |                       |                       | WithManifest`](Androi |
        |                       |                       | dBinaryDescriptionArg |
        |                       |                       | .html#getApplicationM |
        |                       |                       | odulesWithManifest()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `setApplicationModule | ::: block             |
        | scriptionArg.Builder` | sWithResources​(Iterab | Sets or replaces all  |
        |                       | le<String> elements)` | elements for          |
        |                       |                       | [                     |
        |                       |                       | `applicationModulesWi |
        |                       |                       | thResources`](Android |
        |                       |                       | BinaryDescriptionArg. |
        |                       |                       | html#getApplicationMo |
        |                       |                       | dulesWithResources()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `setAppl              | ::: block             |
        | scriptionArg.Builder` | icationModuleTargets​( | Sets or replaces all  |
        |                       | Iterable<? extends Bu | elements for          |
        |                       | ildTarget> elements)` | [`applic              |
        |                       |                       | ationModuleTargets`]( |
        |                       |                       | AndroidBinaryDescript |
        |                       |                       | ionArg.html#getApplic |
        |                       |                       | ationModuleTargets()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `setAssetCompre       | ::: block             |
        | scriptionArg.Builder` | ssionAlgorithm​(Compre | Initializes the       |
        |                       | ssionAlgorithm assetC | optional value        |
        |                       | ompressionAlgorithm)` | [`assetCom            |
        |                       |                       | pressionAlgorithm`](A |
        |                       |                       | ndroidBinaryDescripti |
        |                       |                       | onArg.html#getAssetCo |
        |                       |                       | mpressionAlgorithm()) |
        |                       |                       | to                    |
        |                       |                       | asset                 |
        |                       |                       | CompressionAlgorithm. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `setAssetCompr        | ::: block             |
        | scriptionArg.Builder` | essionAlgorithm​(Optio | Initializes the       |
        |                       | nal<? extends Compres | optional value        |
        |                       | sionAlgorithm> assetC | [`assetCom            |
        |                       | ompressionAlgorithm)` | pressionAlgorithm`](A |
        |                       |                       | ndroidBinaryDescripti |
        |                       |                       | onArg.html#getAssetCo |
        |                       |                       | mpressionAlgorithm()) |
        |                       |                       | to                    |
        |                       |                       | asset                 |
        |                       |                       | CompressionAlgorithm. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `setBanne             | ::: block             |
        | scriptionArg.Builder` | dDuplicateResourceTyp | Sets or replaces all  |
        |                       | es​(Iterable<RDotTxtEn | elements for          |
        |                       | try.RType> elements)` | [`bannedDuplicat      |
        |                       |                       | eResourceTypes`](Andr |
        |                       |                       | oidBinaryDescriptionA |
        |                       |                       | rg.html#getBannedDupl |
        |                       |                       | icateResourceTypes()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `setBuildConfigVa     | ::: block             |
        | scriptionArg.Builder` | lues​(BuildConfigField | Initializes the value |
        |                       | s buildConfigValues)` | for the               |
        |                       |                       | [`buildConfigVa       |
        |                       |                       | lues`](AndroidBinaryD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tBuildConfigValues()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `setBuildConfigVal    | ::: block             |
        | scriptionArg.Builder` | uesFile​(SourcePath bu | Initializes the       |
        |                       | ildConfigValuesFile)` | optional value        |
        |                       |                       | [`                    |
        |                       |                       | buildConfigValuesFile |
        |                       |                       | `](AndroidBinaryDescr |
        |                       |                       | iptionArg.html#getBui |
        |                       |                       | ldConfigValuesFile()) |
        |                       |                       | to                    |
        |                       |                       | b                     |
        |                       |                       | uildConfigValuesFile. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `setBuildConfigVa     | ::: block             |
        | scriptionArg.Builder` | luesFile​(Optional<? e | Initializes the       |
        |                       | xtends SourcePath> bu | optional value        |
        |                       | ildConfigValuesFile)` | [`                    |
        |                       |                       | buildConfigValuesFile |
        |                       |                       | `](AndroidBinaryDescr |
        |                       |                       | iptionArg.html#getBui |
        |                       |                       | ldConfigValuesFile()) |
        |                       |                       | to                    |
        |                       |                       | b                     |
        |                       |                       | uildConfigValuesFile. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `setBuildStri         | ::: block             |
        | scriptionArg.Builder` | ngSourceMap​(boolean b | Initializes the value |
        |                       | uildStringSourceMap)` | for the               |
        |                       |                       | [`buildStringSourceM  |
        |                       |                       | ap`](AndroidBinaryDes |
        |                       |                       | criptionArg.html#isBu |
        |                       |                       | ildStringSourceMap()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `setCompat            | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Iterable<? e | Sets or replaces all  |
        |                       | xtends UnconfiguredBu | elements for          |
        |                       | ildTarget> elements)` | [`compati             |
        |                       |                       | bleWith`](AndroidBina |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `setCompressAsset     | ::: block             |
        | scriptionArg.Builder` | Libraries​(boolean com | Initializes the value |
        |                       | pressAssetLibraries)` | for the               |
        |                       |                       | [`c                   |
        |                       |                       | ompressAssetLibraries |
        |                       |                       | `](AndroidBinaryDescr |
        |                       |                       | iptionArg.html#isComp |
        |                       |                       | ressAssetLibraries()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `setCpu               | ::: block             |
        | scriptionArg.Builder` | Filters​(Iterable<Targ | Sets or replaces all  |
        |                       | etCpuType> elements)` | elements for          |
        |                       |                       | [                     |
        |                       |                       | `cpuFilters`](Android |
        |                       |                       | BinaryDescriptionArg. |
        |                       |                       | html#getCpuFilters()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `setDefaul            | ::: block             |
        | scriptionArg.Builder` | tTargetPlatform​(Uncon | Initializes the       |
        |                       | figuredBuildTarget de | optional value        |
        |                       | faultTargetPlatform)` | [`                    |
        |                       |                       | defaultTargetPlatform |
        |                       |                       | `](AndroidBinaryDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `setDefau             | ::: block             |
        | scriptionArg.Builder` | ltTargetPlatform​(Opti | Initializes the       |
        |                       | onal<? extends Unconf | optional value        |
        |                       | iguredBuildTarget> de | [`                    |
        |                       | faultTargetPlatform)` | defaultTargetPlatform |
        |                       |                       | `](AndroidBinaryDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `setDeps​(             | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Sets or replaces all  |
        |                       | ildTarget> elements)` | elements for          |
        |                       |                       | [`deps`](A            |
        |                       |                       | ndroidBinaryDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `setDex               | ::: block             |
        | scriptionArg.Builder` | Compression​(com.faceb | Initializes the       |
        |                       | ook.buck.android.DexS | optional value        |
        |                       | tore dexCompression)` | [`dexComp             |
        |                       |                       | ression`](AndroidBina |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getDexCompression()) |
        |                       |                       | to dexCompression.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `setDe                | ::: block             |
        | scriptionArg.Builder` | xCompression​(Optional | Initializes the       |
        |                       | <? extends com.facebo | optional value        |
        |                       | ok.buck.android.DexSt | [`dexComp             |
        |                       | ore> dexCompression)` | ression`](AndroidBina |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getDexCompression()) |
        |                       |                       | to dexCompression.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `                     | ::: block             |
        | scriptionArg.Builder` | setDexGroupLibLimit​(i | Initializes the value |
        |                       | nt dexGroupLibLimit)` | for the               |
        |                       |                       | [`dexGroupLib         |
        |                       |                       | Limit`](AndroidBinary |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etDexGroupLibLimit()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `setDexReorderDataDu  | ::: block             |
        | scriptionArg.Builder` | mpFile​(SourcePath dex | Initializes the       |
        |                       | ReorderDataDumpFile)` | optional value        |
        |                       |                       | [`de                  |
        |                       |                       | xReorderDataDumpFile` |
        |                       |                       | ](AndroidBinaryDescri |
        |                       |                       | ptionArg.html#getDexR |
        |                       |                       | eorderDataDumpFile()) |
        |                       |                       | to                    |
        |                       |                       | de                    |
        |                       |                       | xReorderDataDumpFile. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `setDexReorderDataD   | ::: block             |
        | scriptionArg.Builder` | umpFile​(Optional<? ex | Initializes the       |
        |                       | tends SourcePath> dex | optional value        |
        |                       | ReorderDataDumpFile)` | [`de                  |
        |                       |                       | xReorderDataDumpFile` |
        |                       |                       | ](AndroidBinaryDescri |
        |                       |                       | ptionArg.html#getDexR |
        |                       |                       | eorderDataDumpFile()) |
        |                       |                       | to                    |
        |                       |                       | de                    |
        |                       |                       | xReorderDataDumpFile. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `setDexReord          | ::: block             |
        | scriptionArg.Builder` | erToolFile​(SourcePath | Initializes the       |
        |                       |  dexReorderToolFile)` | optional value        |
        |                       |                       | [`dexReorderToolF     |
        |                       |                       | ile`](AndroidBinaryDe |
        |                       |                       | scriptionArg.html#get |
        |                       |                       | DexReorderToolFile()) |
        |                       |                       | to                    |
        |                       |                       | dexReorderToolFile.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `setDexReor           | ::: block             |
        | scriptionArg.Builder` | derToolFile​(Optional< | Initializes the       |
        |                       | ? extends SourcePath> | optional value        |
        |                       |  dexReorderToolFile)` | [`dexReorderToolF     |
        |                       |                       | ile`](AndroidBinaryDe |
        |                       |                       | scriptionArg.html#get |
        |                       |                       | DexReorderToolFile()) |
        |                       |                       | to                    |
        |                       |                       | dexReorderToolFile.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `setDex               | ::: block             |
        | scriptionArg.Builder` | Tool​(String dexTool)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`dexTool`](Andr      |
        |                       |                       | oidBinaryDescriptionA |
        |                       |                       | rg.html#getDexTool()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `setDisablePreDex​(bo  | ::: block             |
        | scriptionArg.Builder` | olean disablePreDex)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`disab               |
        |                       |                       | lePreDex`](AndroidBin |
        |                       |                       | aryDescriptionArg.htm |
        |                       |                       | l#getDisablePreDex()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `setDuplicat          | ::: block             |
        | scriptionArg.Builder` | eResourceBehavior​(Has | Initializes the value |
        |                       | DuplicateAndroidResou | for the               |
        |                       | rceTypes.DuplicateRes | [`duplicat            |
        |                       | ourceBehaviour duplic | eResourceBehavior`](A |
        |                       | ateResourceBehavior)` | ndroidBinaryDescripti |
        |                       |                       | onArg.html#getDuplica |
        |                       |                       | teResourceBehavior()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `setDup               | ::: block             |
        | scriptionArg.Builder` | licateResourceWhiteli | Initializes the       |
        |                       | st​(SourcePath duplica | optional value        |
        |                       | teResourceWhitelist)` | [`duplicateR          |
        |                       |                       | esourceWhitelist`](An |
        |                       |                       | droidBinaryDescriptio |
        |                       |                       | nArg.html#getDuplicat |
        |                       |                       | eResourceWhitelist()) |
        |                       |                       | to                    |
        |                       |                       | duplic                |
        |                       |                       | ateResourceWhitelist. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `setDu                | ::: block             |
        | scriptionArg.Builder` | plicateResourceWhitel | Initializes the       |
        |                       | ist​(Optional<? extend | optional value        |
        |                       | s SourcePath> duplica | [`duplicateR          |
        |                       | teResourceWhitelist)` | esourceWhitelist`](An |
        |                       |                       | droidBinaryDescriptio |
        |                       |                       | nArg.html#getDuplicat |
        |                       |                       | eResourceWhitelist()) |
        |                       |                       | to                    |
        |                       |                       | duplic                |
        |                       |                       | ateResourceWhitelist. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `                     | ::: block             |
        | scriptionArg.Builder` | setEnableRelinker​(boo | Initializes the value |
        |                       | lean enableRelinker)` | for the               |
        |                       |                       | [`enable              |
        |                       |                       | Relinker`](AndroidBin |
        |                       |                       | aryDescriptionArg.htm |
        |                       |                       | l#isEnableRelinker()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `setExopackage        | ::: block             |
        | scriptionArg.Builder` | ​(boolean exopackage)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`exopackage`](Androi |
        |                       |                       | dBinaryDescriptionArg |
        |                       |                       | .html#isExopackage()) |
        |                       |                       | to exopackage.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `se                   | ::: block             |
        | scriptionArg.Builder` | tExopackage​(Optional< | Initializes the       |
        |                       | Boolean> exopackage)` | optional value        |
        |                       |                       | [`exopackage`](Androi |
        |                       |                       | dBinaryDescriptionArg |
        |                       |                       | .html#isExopackage()) |
        |                       |                       | to exopackage.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `setExopackag         | ::: block             |
        | scriptionArg.Builder` | eModes​(Iterable<Exopa | Sets or replaces all  |
        |                       | ckageMode> elements)` | elements for          |
        |                       |                       | [`exopackag           |
        |                       |                       | eModes`](AndroidBinar |
        |                       |                       | yDescriptionArg.html# |
        |                       |                       | getExopackageModes()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `setExtraFil          | ::: block             |
        | scriptionArg.Builder` | teredResources​(Iterab | Sets or replaces all  |
        |                       | le<String> elements)` | elements for          |
        |                       |                       | [`ex                  |
        |                       |                       | traFilteredResources` |
        |                       |                       | ](AndroidBinaryDescri |
        |                       |                       | ptionArg.html#getExtr |
        |                       |                       | aFilteredResources()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `setIgnoreAaptProguar | ::: block             |
        | scriptionArg.Builder` | dConfig​(boolean ignor | Initializes the value |
        |                       | eAaptProguardConfig)` | for the               |
        |                       |                       | [`ignor               |
        |                       |                       | eAaptProguardConfig`] |
        |                       |                       | (AndroidBinaryDescrip |
        |                       |                       | tionArg.html#isIgnore |
        |                       |                       | AaptProguardConfig()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `setIncludesVectorD   | ::: block             |
        | scriptionArg.Builder` | rawables​(boolean incl | Initializes the value |
        |                       | udesVectorDrawables)` | for the               |
        |                       |                       | [`inc                 |
        |                       |                       | ludesVectorDrawables` |
        |                       |                       | ](AndroidBinaryDescri |
        |                       |                       | ptionArg.html#isInclu |
        |                       |                       | desVectorDrawables()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `setIsCacheable​(      | ::: block             |
        | scriptionArg.Builder` | boolean isCacheable)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`i                   |
        |                       |                       | sCacheable`](AndroidB |
        |                       |                       | inaryDescriptionArg.h |
        |                       |                       | tml#getIsCacheable()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `setKeepRe            | ::: block             |
        | scriptionArg.Builder` | sourcePattern​(String  | Initializes the       |
        |                       | keepResourcePattern)` | optional value        |
        |                       |                       | [`keepResourcePatte   |
        |                       |                       | rn`](AndroidBinaryDes |
        |                       |                       | criptionArg.html#getK |
        |                       |                       | eepResourcePattern()) |
        |                       |                       | to                    |
        |                       |                       | keepResourcePattern.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `setKeepResourcePatt  | ::: block             |
        | scriptionArg.Builder` | ern​(Optional<String>  | Initializes the       |
        |                       | keepResourcePattern)` | optional value        |
        |                       |                       | [`keepResourcePatte   |
        |                       |                       | rn`](AndroidBinaryDes |
        |                       |                       | criptionArg.html#getK |
        |                       |                       | eepResourcePattern()) |
        |                       |                       | to                    |
        |                       |                       | keepResourcePattern.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `setKeystore​(B        | ::: block             |
        | scriptionArg.Builder` | uildTarget keystore)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`keystore`](Andro    |
        |                       |                       | idBinaryDescriptionAr |
        |                       |                       | g.html#getKeystore()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `setLabels​(Iterab     | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Sets or replaces all  |
        |                       |                       | elements for          |
        |                       |                       | [`labels`](And        |
        |                       |                       | roidBinaryDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `setLicenses          | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Sets or replaces all  |
        |                       | ourcePath> elements)` | elements for          |
        |                       |                       | [`licenses`](Andro    |
        |                       |                       | idBinaryDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `setLinear            | ::: block             |
        | scriptionArg.Builder` | AllocHardLimit​(long l | Initializes the value |
        |                       | inearAllocHardLimit)` | for the               |
        |                       |                       | [`linearAllocHardLimi |
        |                       |                       | t`](AndroidBinaryDesc |
        |                       |                       | riptionArg.html#getLi |
        |                       |                       | nearAllocHardLimit()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `setLocales​(Iterab    | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Sets or replaces all  |
        |                       |                       | elements for          |
        |                       |                       | [`locales`](Andr      |
        |                       |                       | oidBinaryDescriptionA |
        |                       |                       | rg.html#getLocales()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `setLocalizedStrin    | ::: block             |
        | scriptionArg.Builder` | gFileName​(String loca | Initializes the       |
        |                       | lizedStringFileName)` | optional value        |
        |                       |                       | [`loca                |
        |                       |                       | lizedStringFileName`] |
        |                       |                       | (AndroidBinaryDescrip |
        |                       |                       | tionArg.html#getLocal |
        |                       |                       | izedStringFileName()) |
        |                       |                       | to                    |
        |                       |                       | loc                   |
        |                       |                       | alizedStringFileName. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `setLoc               | ::: block             |
        | scriptionArg.Builder` | alizedStringFileName​( | Initializes the       |
        |                       | Optional<String> loca | optional value        |
        |                       | lizedStringFileName)` | [`loca                |
        |                       |                       | lizedStringFileName`] |
        |                       |                       | (AndroidBinaryDescrip |
        |                       |                       | tionArg.html#getLocal |
        |                       |                       | izedStringFileName()) |
        |                       |                       | to                    |
        |                       |                       | loc                   |
        |                       |                       | alizedStringFileName. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `setManifest​(         | ::: block             |
        | scriptionArg.Builder` | SourcePath manifest)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`manifest`](Andro    |
        |                       |                       | idBinaryDescriptionAr |
        |                       |                       | g.html#getManifest()) |
        |                       |                       | to manifest.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `setManifest          | ::: block             |
        | scriptionArg.Builder` | ​(Optional<? extends S | Initializes the       |
        |                       | ourcePath> manifest)` | optional value        |
        |                       |                       | [`manifest`](Andro    |
        |                       |                       | idBinaryDescriptionAr |
        |                       |                       | g.html#getManifest()) |
        |                       |                       | to manifest.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `setManifes           | ::: block             |
        | scriptionArg.Builder` | tEntries​(ManifestEntr | Initializes the value |
        |                       | ies manifestEntries)` | for the               |
        |                       |                       | [`manifestE           |
        |                       |                       | ntries`](AndroidBinar |
        |                       |                       | yDescriptionArg.html# |
        |                       |                       | getManifestEntries()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `setMani              | ::: block             |
        | scriptionArg.Builder` | festSkeleton​(SourcePa | Initializes the       |
        |                       | th manifestSkeleton)` | optional value        |
        |                       |                       | [`manifestSke         |
        |                       |                       | leton`](AndroidBinary |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etManifestSkeleton()) |
        |                       |                       | to manifestSkeleton.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `setMan               | ::: block             |
        | scriptionArg.Builder` | ifestSkeleton​(Optiona | Initializes the       |
        |                       | l<? extends SourcePat | optional value        |
        |                       | h> manifestSkeleton)` | [`manifestSke         |
        |                       |                       | leton`](AndroidBinary |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etManifestSkeleton()) |
        |                       |                       | to manifestSkeleton.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `setMinimizePrima     | ::: block             |
        | scriptionArg.Builder` | ryDexSize​(boolean min | Initializes the value |
        |                       | imizePrimaryDexSize)` | for the               |
        |                       |                       | [`mi                  |
        |                       |                       | nimizePrimaryDexSize` |
        |                       |                       | ](AndroidBinaryDescri |
        |                       |                       | ptionArg.html#getMini |
        |                       |                       | mizePrimaryDexSize()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `setModuleManifestSk  | ::: block             |
        | scriptionArg.Builder` | eleton​(SourcePath mod | Initializes the       |
        |                       | uleManifestSkeleton)` | optional value        |
        |                       |                       | [`mo                  |
        |                       |                       | duleManifestSkeleton` |
        |                       |                       | ](AndroidBinaryDescri |
        |                       |                       | ptionArg.html#getModu |
        |                       |                       | leManifestSkeleton()) |
        |                       |                       | to                    |
        |                       |                       | mo                    |
        |                       |                       | duleManifestSkeleton. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `setModuleManifestS   | ::: block             |
        | scriptionArg.Builder` | keleton​(Optional<? ex | Initializes the       |
        |                       | tends SourcePath> mod | optional value        |
        |                       | uleManifestSkeleton)` | [`mo                  |
        |                       |                       | duleManifestSkeleton` |
        |                       |                       | ](AndroidBinaryDescri |
        |                       |                       | ptionArg.html#getModu |
        |                       |                       | leManifestSkeleton()) |
        |                       |                       | to                    |
        |                       |                       | mo                    |
        |                       |                       | duleManifestSkeleton. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `                     | ::: block             |
        | scriptionArg.Builder` | setName​(String name)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`name`](A            |
        |                       |                       | ndroidBinaryDescripti |
        |                       |                       | onArg.html#getName()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `setNativeLibraryM    | ::: block             |
        | scriptionArg.Builder` | ergeCodeGenerator​(Bui | Initializes the       |
        |                       | ldTarget nativeLibrar | optional value        |
        |                       | yMergeCodeGenerator)` | [                     |
        |                       |                       | `nativeLibraryMergeCo |
        |                       |                       | deGenerator`](Android |
        |                       |                       | BinaryDescriptionArg. |
        |                       |                       | html#getNativeLibrary |
        |                       |                       | MergeCodeGenerator()) |
        |                       |                       | to                    |
        |                       |                       | nativeLibra           |
        |                       |                       | ryMergeCodeGenerator. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `setNativeLibrary     | ::: block             |
        | scriptionArg.Builder` | MergeCodeGenerator​(Op | Initializes the       |
        |                       | tional<? extends Buil | optional value        |
        |                       | dTarget> nativeLibrar | [                     |
        |                       | yMergeCodeGenerator)` | `nativeLibraryMergeCo |
        |                       |                       | deGenerator`](Android |
        |                       |                       | BinaryDescriptionArg. |
        |                       |                       | html#getNativeLibrary |
        |                       |                       | MergeCodeGenerator()) |
        |                       |                       | to                    |
        |                       |                       | nativeLibra           |
        |                       |                       | ryMergeCodeGenerator. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `setNativeLibraryMerg | ::: block             |
        | scriptionArg.Builder` | eGlue​(BuildTarget nat | Initializes the       |
        |                       | iveLibraryMergeGlue)` | optional value        |
        |                       |                       | [`na                  |
        |                       |                       | tiveLibraryMergeGlue` |
        |                       |                       | ](AndroidBinaryDescri |
        |                       |                       | ptionArg.html#getNati |
        |                       |                       | veLibraryMergeGlue()) |
        |                       |                       | to                    |
        |                       |                       | na                    |
        |                       |                       | tiveLibraryMergeGlue. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `setNativeLibraryMer  | ::: block             |
        | scriptionArg.Builder` | geGlue​(Optional<? ext | Initializes the       |
        |                       | ends BuildTarget> nat | optional value        |
        |                       | iveLibraryMergeGlue)` | [`na                  |
        |                       |                       | tiveLibraryMergeGlue` |
        |                       |                       | ](AndroidBinaryDescri |
        |                       |                       | ptionArg.html#getNati |
        |                       |                       | veLibraryMergeGlue()) |
        |                       |                       | to                    |
        |                       |                       | na                    |
        |                       |                       | tiveLibraryMergeGlue. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `s                    | ::: block             |
        | scriptionArg.Builder` | etNativeLibraryMergeL | Initializes the       |
        |                       | ocalizedSymbols​(com.g | optional value        |
        |                       | oogle.common.collect. | [`nativ               |
        |                       | ImmutableSortedSet<St | eLibraryMergeLocalize |
        |                       | ring> nativeLibraryMe | dSymbols`](AndroidBin |
        |                       | rgeLocalizedSymbols)` | aryDescriptionArg.htm |
        |                       |                       | l#getNativeLibraryMer |
        |                       |                       | geLocalizedSymbols()) |
        |                       |                       | to                    |
        |                       |                       | nativeLibraryM        |
        |                       |                       | ergeLocalizedSymbols. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `                     | ::: block             |
        | scriptionArg.Builder` | setNativeLibraryMerge | Initializes the       |
        |                       | LocalizedSymbols​(Opti | optional value        |
        |                       | onal<? extends com.go | [`nativ               |
        |                       | ogle.common.collect.I | eLibraryMergeLocalize |
        |                       | mmutableSortedSet<Str | dSymbols`](AndroidBin |
        |                       | ing>> nativeLibraryMe | aryDescriptionArg.htm |
        |                       | rgeLocalizedSymbols)` | l#getNativeLibraryMer |
        |                       |                       | geLocalizedSymbols()) |
        |                       |                       | to                    |
        |                       |                       | nativeLibraryM        |
        |                       |                       | ergeLocalizedSymbols. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `setNati              | ::: block             |
        | scriptionArg.Builder` | veLibraryMergeMap​(Map | Sets or replaces all  |
        |                       | <String,​? extends Lis | mappings from the     |
        |                       | t<Pattern>> entries)` | specified map as      |
        |                       |                       | entries for the       |
        |                       |                       | [`                    |
        |                       |                       | nativeLibraryMergeMap |
        |                       |                       | `](AndroidBinaryDescr |
        |                       |                       | iptionArg.html#getNat |
        |                       |                       | iveLibraryMergeMap()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `setNat               | ::: block             |
        | scriptionArg.Builder` | iveLibraryProguardCon | Initializes the       |
        |                       | figGenerator​(BuildTar | optional value        |
        |                       | get nativeLibraryProg | [`nativeLib           |
        |                       | uardConfigGenerator)` | raryProguardConfigGen |
        |                       |                       | erator`](AndroidBinar |
        |                       |                       | yDescriptionArg.html# |
        |                       |                       | getNativeLibraryProgu |
        |                       |                       | ardConfigGenerator()) |
        |                       |                       | to                    |
        |                       |                       | nativeLibraryPro      |
        |                       |                       | guardConfigGenerator. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `setNa                | ::: block             |
        | scriptionArg.Builder` | tiveLibraryProguardCo | Initializes the       |
        |                       | nfigGenerator​(Optiona | optional value        |
        |                       | l<? extends BuildTarg | [`nativeLib           |
        |                       | et> nativeLibraryProg | raryProguardConfigGen |
        |                       | uardConfigGenerator)` | erator`](AndroidBinar |
        |                       |                       | yDescriptionArg.html# |
        |                       |                       | getNativeLibraryProgu |
        |                       |                       | ardConfigGenerator()) |
        |                       |                       | to                    |
        |                       |                       | nativeLibraryPro      |
        |                       |                       | guardConfigGenerator. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `s                    | ::: block             |
        | scriptionArg.Builder` | etNoAutoAddOverlayRes | Initializes the value |
        |                       | ources​(boolean noAuto | for the               |
        |                       | AddOverlayResources)` | [`noAutoA             |
        |                       |                       | ddOverlayResources`]( |
        |                       |                       | AndroidBinaryDescript |
        |                       |                       | ionArg.html#isNoAutoA |
        |                       |                       | ddOverlayResources()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `setNoAutoVersion     | ::: block             |
        | scriptionArg.Builder` | Resources​(boolean noA | Initializes the value |
        |                       | utoVersionResources)` | for the               |
        |                       |                       | [`n                   |
        |                       |                       | oAutoVersionResources |
        |                       |                       | `](AndroidBinaryDescr |
        |                       |                       | iptionArg.html#isNoAu |
        |                       |                       | toVersionResources()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `setNoDx​(             | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Sets or replaces all  |
        |                       | ildTarget> elements)` | elements for          |
        |                       |                       | [`noDx`](A            |
        |                       |                       | ndroidBinaryDescripti |
        |                       |                       | onArg.html#getNoDx()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `setNoVers            | ::: block             |
        | scriptionArg.Builder` | ionTransitionsResourc | Initializes the value |
        |                       | es​(boolean noVersionT | for the               |
        |                       | ransitionsResources)` | [`noVersionTransi     |
        |                       |                       | tionsResources`](Andr |
        |                       |                       | oidBinaryDescriptionA |
        |                       |                       | rg.html#isNoVersionTr |
        |                       |                       | ansitionsResources()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `setO                 | ::: block             |
        | scriptionArg.Builder` | ptimizationPasses​(int | Initializes the value |
        |                       |  optimizationPasses)` | for the               |
        |                       |                       | [`optimizationPas     |
        |                       |                       | ses`](AndroidBinaryDe |
        |                       |                       | scriptionArg.html#get |
        |                       |                       | OptimizationPasses()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `setPackageAsse       | ::: block             |
        | scriptionArg.Builder` | tLibraries​(boolean pa | Initializes the value |
        |                       | ckageAssetLibraries)` | for the               |
        |                       |                       | [                     |
        |                       |                       | `packageAssetLibrarie |
        |                       |                       | s`](AndroidBinaryDesc |
        |                       |                       | riptionArg.html#isPac |
        |                       |                       | kageAssetLibraries()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `setPackageType       | ::: block             |
        | scriptionArg.Builder` | ​(String packageType)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`p                   |
        |                       |                       | ackageType`](AndroidB |
        |                       |                       | inaryDescriptionArg.h |
        |                       |                       | tml#getPackageType()) |
        |                       |                       | to packageType.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `set                  | ::: block             |
        | scriptionArg.Builder` | PackageType​(Optional< | Initializes the       |
        |                       | String> packageType)` | optional value        |
        |                       |                       | [`p                   |
        |                       |                       | ackageType`](AndroidB |
        |                       |                       | inaryDescriptionArg.h |
        |                       |                       | tml#getPackageType()) |
        |                       |                       | to packageType.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `setP                 | ::: block             |
        | scriptionArg.Builder` | ostFilterResourcesCmd | Initializes the       |
        |                       | ​(StringWithMacros pos | optional value        |
        |                       | tFilterResourcesCmd)` | [`po                  |
        |                       |                       | stFilterResourcesCmd` |
        |                       |                       | ](AndroidBinaryDescri |
        |                       |                       | ptionArg.html#getPost |
        |                       |                       | FilterResourcesCmd()) |
        |                       |                       | to                    |
        |                       |                       | po                    |
        |                       |                       | stFilterResourcesCmd. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `set                  | ::: block             |
        | scriptionArg.Builder` | PostFilterResourcesCm | Initializes the       |
        |                       | d​(Optional<? extends  | optional value        |
        |                       | StringWithMacros> pos | [`po                  |
        |                       | tFilterResourcesCmd)` | stFilterResourcesCmd` |
        |                       |                       | ](AndroidBinaryDescri |
        |                       |                       | ptionArg.html#getPost |
        |                       |                       | FilterResourcesCmd()) |
        |                       |                       | to                    |
        |                       |                       | po                    |
        |                       |                       | stFilterResourcesCmd. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `setPreproc           | ::: block             |
        | scriptionArg.Builder` | essJavaClassesBash​(St | Initializes the       |
        |                       | ringWithMacros prepro | optional value        |
        |                       | cessJavaClassesBash)` | [`preproce            |
        |                       |                       | ssJavaClassesBash`](A |
        |                       |                       | ndroidBinaryDescripti |
        |                       |                       | onArg.html#getPreproc |
        |                       |                       | essJavaClassesBash()) |
        |                       |                       | to                    |
        |                       |                       | prepr                 |
        |                       |                       | ocessJavaClassesBash. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `setPrepro            | ::: block             |
        | scriptionArg.Builder` | cessJavaClassesBash​(O | Initializes the       |
        |                       | ptional<? extends Str | optional value        |
        |                       | ingWithMacros> prepro | [`preproce            |
        |                       | cessJavaClassesBash)` | ssJavaClassesBash`](A |
        |                       |                       | ndroidBinaryDescripti |
        |                       |                       | onArg.html#getPreproc |
        |                       |                       | essJavaClassesBash()) |
        |                       |                       | to                    |
        |                       |                       | prepr                 |
        |                       |                       | ocessJavaClassesBash. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `setPrepr             | ::: block             |
        | scriptionArg.Builder` | ocessJavaClassesDeps​( | Sets or replaces all  |
        |                       | Iterable<? extends Bu | elements for          |
        |                       | ildTarget> elements)` | [`preproce            |
        |                       |                       | ssJavaClassesDeps`](A |
        |                       |                       | ndroidBinaryDescripti |
        |                       |                       | onArg.html#getPreproc |
        |                       |                       | essJavaClassesDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `setPrimaryDexClas    | ::: block             |
        | scriptionArg.Builder` | sesFile​(SourcePath pr | Initializes the       |
        |                       | imaryDexClassesFile)` | optional value        |
        |                       |                       | [`                    |
        |                       |                       | primaryDexClassesFile |
        |                       |                       | `](AndroidBinaryDescr |
        |                       |                       | iptionArg.html#getPri |
        |                       |                       | maryDexClassesFile()) |
        |                       |                       | to                    |
        |                       |                       | p                     |
        |                       |                       | rimaryDexClassesFile. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `setPrimaryDexCla     | ::: block             |
        | scriptionArg.Builder` | ssesFile​(Optional<? e | Initializes the       |
        |                       | xtends SourcePath> pr | optional value        |
        |                       | imaryDexClassesFile)` | [`                    |
        |                       |                       | primaryDexClassesFile |
        |                       |                       | `](AndroidBinaryDescr |
        |                       |                       | iptionArg.html#getPri |
        |                       |                       | maryDexClassesFile()) |
        |                       |                       | to                    |
        |                       |                       | p                     |
        |                       |                       | rimaryDexClassesFile. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `setPrim              | ::: block             |
        | scriptionArg.Builder` | aryDexPatterns​(Iterab | Sets or replaces all  |
        |                       | le<String> elements)` | elements for          |
        |                       |                       | [`primaryDexPatte     |
        |                       |                       | rns`](AndroidBinaryDe |
        |                       |                       | scriptionArg.html#get |
        |                       |                       | PrimaryDexPatterns()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `setPrimaryDexScenar  | ::: block             |
        | scriptionArg.Builder` | ioFile​(SourcePath pri | Initializes the       |
        |                       | maryDexScenarioFile)` | optional value        |
        |                       |                       | [`pr                  |
        |                       |                       | imaryDexScenarioFile` |
        |                       |                       | ](AndroidBinaryDescri |
        |                       |                       | ptionArg.html#getPrim |
        |                       |                       | aryDexScenarioFile()) |
        |                       |                       | to                    |
        |                       |                       | pr                    |
        |                       |                       | imaryDexScenarioFile. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `setPrimaryDexScena   | ::: block             |
        | scriptionArg.Builder` | rioFile​(Optional<? ex | Initializes the       |
        |                       | tends SourcePath> pri | optional value        |
        |                       | maryDexScenarioFile)` | [`pr                  |
        |                       |                       | imaryDexScenarioFile` |
        |                       |                       | ](AndroidBinaryDescri |
        |                       |                       | ptionArg.html#getPrim |
        |                       |                       | aryDexScenarioFile()) |
        |                       |                       | to                    |
        |                       |                       | pr                    |
        |                       |                       | imaryDexScenarioFile. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `setPrimaryDexScen    | ::: block             |
        | scriptionArg.Builder` | arioOverflowAllowed​(b | Initializes the value |
        |                       | oolean primaryDexScen | for the               |
        |                       | arioOverflowAllowed)` | [`pr                  |
        |                       |                       | imaryDexScenarioOverf |
        |                       |                       | lowAllowed`](AndroidB |
        |                       |                       | inaryDescriptionArg.h |
        |                       |                       | tml#isPrimaryDexScena |
        |                       |                       | rioOverflowAllowed()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `set                  | ::: block             |
        | scriptionArg.Builder` | ProguardConfig​(Source | Initializes the       |
        |                       | Path proguardConfig)` | optional value        |
        |                       |                       | [`proguar             |
        |                       |                       | dConfig`](AndroidBina |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getProguardConfig()) |
        |                       |                       | to proguardConfig.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `se                   | ::: block             |
        | scriptionArg.Builder` | tProguardConfig​(Optio | Initializes the       |
        |                       | nal<? extends SourceP | optional value        |
        |                       | ath> proguardConfig)` | [`proguar             |
        |                       |                       | dConfig`](AndroidBina |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getProguardConfig()) |
        |                       |                       | to proguardConfig.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `setP                 | ::: block             |
        | scriptionArg.Builder` | roguardJvmArgs​(Iterab | Sets or replaces all  |
        |                       | le<String> elements)` | elements for          |
        |                       |                       | [`proguardJ           |
        |                       |                       | vmArgs`](AndroidBinar |
        |                       |                       | yDescriptionArg.html# |
        |                       |                       | getProguardJvmArgs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `set                  | ::: block             |
        | scriptionArg.Builder` | Redex​(boolean redex)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`redex`](An          |
        |                       |                       | droidBinaryDescriptio |
        |                       |                       | nArg.html#getRedex()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `setRedexConfig​(Sou   | ::: block             |
        | scriptionArg.Builder` | rcePath redexConfig)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`r                   |
        |                       |                       | edexConfig`](AndroidB |
        |                       |                       | inaryDescriptionArg.h |
        |                       |                       | tml#getRedexConfig()) |
        |                       |                       | to redexConfig.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `setRedexConfig​(Op    | ::: block             |
        | scriptionArg.Builder` | tional<? extends Sour | Initializes the       |
        |                       | cePath> redexConfig)` | optional value        |
        |                       |                       | [`r                   |
        |                       |                       | edexConfig`](AndroidB |
        |                       |                       | inaryDescriptionArg.h |
        |                       |                       | tml#getRedexConfig()) |
        |                       |                       | to redexConfig.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `se                   | ::: block             |
        | scriptionArg.Builder` | tRedexExtraArgs​(Itera | Sets or replaces all  |
        |                       | ble<? extends StringW | elements for          |
        |                       | ithMacros> elements)` | [`redexEx             |
        |                       |                       | traArgs`](AndroidBina |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getRedexExtraArgs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `setRelinkerWhitel    | ::: block             |
        | scriptionArg.Builder` | ist​(Iterable<? extend | Sets or replaces all  |
        |                       | s Pattern> elements)` | elements for          |
        |                       |                       | [`relinkerWhite       |
        |                       |                       | list`](AndroidBinaryD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tRelinkerWhitelist()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `setReorderClasse     | ::: block             |
        | scriptionArg.Builder` | sIntraDex​(boolean reo | Initializes the value |
        |                       | rderClassesIntraDex)` | for the               |
        |                       |                       | [`r                   |
        |                       |                       | eorderClassesIntraDex |
        |                       |                       | `](AndroidBinaryDescr |
        |                       |                       | iptionArg.html#isReor |
        |                       |                       | derClassesIntraDex()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `setRe                | ::: block             |
        | scriptionArg.Builder` | sourceCompression​(com | Initializes the value |
        |                       | .facebook.buck.androi | for the               |
        |                       | d.ResourcesFilter.Res | [`resourceCompressi   |
        |                       | ourceCompressionMode  | on`](AndroidBinaryDes |
        |                       | resourceCompression)` | criptionArg.html#getR |
        |                       |                       | esourceCompression()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `set                  | ::: block             |
        | scriptionArg.Builder` | ResourceFilter​(Iterab | Sets or replaces all  |
        |                       | le<String> elements)` | elements for          |
        |                       |                       | [`resourc             |
        |                       |                       | eFilter`](AndroidBina |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #getResourceFilter()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `setResource          | ::: block             |
        | scriptionArg.Builder` | UnionPackage​(String r | Initializes the       |
        |                       | esourceUnionPackage)` | optional value        |
        |                       |                       | [`resourceUnionPackag |
        |                       |                       | e`](AndroidBinaryDesc |
        |                       |                       | riptionArg.html#getRe |
        |                       |                       | sourceUnionPackage()) |
        |                       |                       | to                    |
        |                       |                       | resourceUnionPackage. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `                     | ::: block             |
        | scriptionArg.Builder` | setResourceUnionPacka | Initializes the       |
        |                       | ge​(Optional<String> r | optional value        |
        |                       | esourceUnionPackage)` | [`resourceUnionPackag |
        |                       |                       | e`](AndroidBinaryDesc |
        |                       |                       | riptionArg.html#getRe |
        |                       |                       | sourceUnionPackage()) |
        |                       |                       | to                    |
        |                       |                       | resourceUnionPackage. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `setSecon             | ::: block             |
        | scriptionArg.Builder` | daryDexHeadClassesFil | Initializes the       |
        |                       | e​(SourcePath secondar | optional value        |
        |                       | yDexHeadClassesFile)` | [`secondaryDex        |
        |                       |                       | HeadClassesFile`](And |
        |                       |                       | roidBinaryDescription |
        |                       |                       | Arg.html#getSecondary |
        |                       |                       | DexHeadClassesFile()) |
        |                       |                       | to                    |
        |                       |                       | seconda               |
        |                       |                       | ryDexHeadClassesFile. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `setSeco              | ::: block             |
        | scriptionArg.Builder` | ndaryDexHeadClassesFi | Initializes the       |
        |                       | le​(Optional<? extends | optional value        |
        |                       |  SourcePath> secondar | [`secondaryDex        |
        |                       | yDexHeadClassesFile)` | HeadClassesFile`](And |
        |                       |                       | roidBinaryDescription |
        |                       |                       | Arg.html#getSecondary |
        |                       |                       | DexHeadClassesFile()) |
        |                       |                       | to                    |
        |                       |                       | seconda               |
        |                       |                       | ryDexHeadClassesFile. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `setSecon             | ::: block             |
        | scriptionArg.Builder` | daryDexTailClassesFil | Initializes the       |
        |                       | e​(SourcePath secondar | optional value        |
        |                       | yDexTailClassesFile)` | [`secondaryDex        |
        |                       |                       | TailClassesFile`](And |
        |                       |                       | roidBinaryDescription |
        |                       |                       | Arg.html#getSecondary |
        |                       |                       | DexTailClassesFile()) |
        |                       |                       | to                    |
        |                       |                       | seconda               |
        |                       |                       | ryDexTailClassesFile. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `setSeco              | ::: block             |
        | scriptionArg.Builder` | ndaryDexTailClassesFi | Initializes the       |
        |                       | le​(Optional<? extends | optional value        |
        |                       |  SourcePath> secondar | [`secondaryDex        |
        |                       | yDexTailClassesFile)` | TailClassesFile`](And |
        |                       |                       | roidBinaryDescription |
        |                       |                       | Arg.html#getSecondary |
        |                       |                       | DexTailClassesFile()) |
        |                       |                       | to                    |
        |                       |                       | seconda               |
        |                       |                       | ryDexTailClassesFile. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `                     | ::: block             |
        | scriptionArg.Builder` | setSkipCrunchPngs​(boo | Initializes the       |
        |                       | lean skipCrunchPngs)` | optional value        |
        |                       |                       | [`skipCr              |
        |                       |                       | unchPngs`](AndroidBin |
        |                       |                       | aryDescriptionArg.htm |
        |                       |                       | l#isSkipCrunchPngs()) |
        |                       |                       | to skipCrunchPngs.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `setSkipCru           | ::: block             |
        | scriptionArg.Builder` | nchPngs​(Optional<Bool | Initializes the       |
        |                       | ean> skipCrunchPngs)` | optional value        |
        |                       |                       | [`skipCr              |
        |                       |                       | unchPngs`](AndroidBin |
        |                       |                       | aryDescriptionArg.htm |
        |                       |                       | l#isSkipCrunchPngs()) |
        |                       |                       | to skipCrunchPngs.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `setSkipProguard​(b    | ::: block             |
        | scriptionArg.Builder` | oolean skipProguard)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`sk                  |
        |                       |                       | ipProguard`](AndroidB |
        |                       |                       | inaryDescriptionArg.h |
        |                       |                       | tml#isSkipProguard()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `setTests​(            | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Sets or replaces all  |
        |                       | ildTarget> elements)` | elements for          |
        |                       |                       | [`tests`](An          |
        |                       |                       | droidBinaryDescriptio |
        |                       |                       | nArg.html#getTests()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `se                   | ::: block             |
        | scriptionArg.Builder` | tTrimResourceIds​(bool | Initializes the value |
        |                       | ean trimResourceIds)` | for the               |
        |                       |                       | [`trimReso            |
        |                       |                       | urceIds`](AndroidBina |
        |                       |                       | ryDescriptionArg.html |
        |                       |                       | #isTrimResourceIds()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `setUse               | ::: block             |
        | scriptionArg.Builder` | DynamicFeature​(boolea | Initializes the value |
        |                       | n useDynamicFeature)` | for the               |
        |                       |                       | [`useDynamicFea       |
        |                       |                       | ture`](AndroidBinaryD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tUseDynamicFeature()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `setUseSplitDex​(      | ::: block             |
        | scriptionArg.Builder` | boolean useSplitDex)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`u                   |
        |                       |                       | seSplitDex`](AndroidB |
        |                       |                       | inaryDescriptionArg.h |
        |                       |                       | tml#getUseSplitDex()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBinaryDe      | `setX                 | ::: block             |
        | scriptionArg.Builder` | zCompressionLevel​(int | Initializes the value |
        |                       |  xzCompressionLevel)` | for the               |
        |                       |                       | [`xzCompressionLe     |
        |                       |                       | vel`](AndroidBinaryDe |
        |                       |                       | scriptionArg.html#get |
        |                       |                       | XzCompressionLevel()) |
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

        []{#from(com.facebook.buck.core.description.arg.HasApplicationModuleBlacklist)}

        -   #### from

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder from​(HasApplicationModuleBlacklist instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `com.facebook.buck.core.description.arg.HasApplicationModuleBlacklist`
            instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.android.AndroidGraphEnhancerArgs)}

        -   #### from

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder from​(AndroidGraphEnhancerArgs instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `com.facebook.buck.android.AndroidGraphEnhancerArgs`
            instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.core.description.arg.HasDeclaredDeps)}

        -   #### from

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder from​(HasDeclaredDeps instance)
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
            public final AndroidBinaryDescriptionArg.Builder from​(HasTests instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `com.facebook.buck.core.description.arg.HasTests` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.android.AndroidBinaryDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder from​(AndroidBinaryDescriptionArg instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `AndroidBinaryDescriptionArg` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.android.AndroidBinaryDescription.AbstractAndroidBinaryDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder from​(com.facebook.buck.android.AndroidBinaryDescription.AbstractAndroidBinaryDescriptionArg instance)
            ```

            ::: block
            Copy abstract value type
            `AbstractAndroidBinaryDescriptionArg` instance into builder.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.android.HasExopackageArgs)}

        -   #### from

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder from​(HasExopackageArgs instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `com.facebook.buck.android.HasExopackageArgs` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.core.description.arg.BuildRuleArg)}

        -   #### from

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder from​(BuildRuleArg instance)
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

        []{#from(com.facebook.buck.android.HasDuplicateAndroidResourceTypes)}

        -   #### from

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder from​(HasDuplicateAndroidResourceTypes instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `com.facebook.buck.android.HasDuplicateAndroidResourceTypes`
            instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.core.description.arg.ConstructorArg)}

        -   #### from

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder from​(ConstructorArg instance)
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

        []{#setKeystore(com.facebook.buck.core.model.BuildTarget)}

        -   #### setKeystore

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder setKeystore​(BuildTarget keystore)
            ```

            ::: block
            Initializes the value for the
            [`keystore`](AndroidBinaryDescriptionArg.html#getKeystore())
            attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `keystore` - The value for keystore

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setUseSplitDex(boolean)}

        -   #### setUseSplitDex

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder setUseSplitDex​(boolean useSplitDex)
            ```

            ::: block
            Initializes the value for the
            [`useSplitDex`](AndroidBinaryDescriptionArg.html#getUseSplitDex())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`useSplitDex`](AndroidBinaryDescriptionArg.html#getUseSplitDex()).*
            :::

            [Parameters:]{.paramLabel}
            :   `useSplitDex` - The value for useSplitDex

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setMinimizePrimaryDexSize(boolean)}

        -   #### setMinimizePrimaryDexSize

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder setMinimizePrimaryDexSize​(boolean minimizePrimaryDexSize)
            ```

            ::: block
            Initializes the value for the
            [`minimizePrimaryDexSize`](AndroidBinaryDescriptionArg.html#getMinimizePrimaryDexSize())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`minimizePrimaryDexSize`](AndroidBinaryDescriptionArg.html#getMinimizePrimaryDexSize()).*
            :::

            [Parameters:]{.paramLabel}
            :   `minimizePrimaryDexSize` - The value for
                minimizePrimaryDexSize

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDexCompression(com.facebook.buck.android.DexStore)}

        -   #### setDexCompression

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder setDexCompression​(com.facebook.buck.android.DexStore dexCompression)
            ```

            ::: block
            Initializes the optional value
            [`dexCompression`](AndroidBinaryDescriptionArg.html#getDexCompression())
            to dexCompression.
            :::

            [Parameters:]{.paramLabel}
            :   `dexCompression` - The value for dexCompression

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setDexCompression(java.util.Optional)}

        -   #### setDexCompression

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder setDexCompression​(Optional<? extends com.facebook.buck.android.DexStore> dexCompression)
            ```

            ::: block
            Initializes the optional value
            [`dexCompression`](AndroidBinaryDescriptionArg.html#getDexCompression())
            to dexCompression.
            :::

            [Parameters:]{.paramLabel}
            :   `dexCompression` - The value for dexCompression

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addPrimaryDexPatterns(java.lang.String)}

        -   #### addPrimaryDexPatterns

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder addPrimaryDexPatterns​(String element)
            ```

            ::: block
            Adds one element to
            [`primaryDexPatterns`](AndroidBinaryDescriptionArg.html#getPrimaryDexPatterns())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A primaryDexPatterns element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addPrimaryDexPatterns(java.lang.String...)}

        -   #### addPrimaryDexPatterns

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder addPrimaryDexPatterns​(String... elements)
            ```

            ::: block
            Adds elements to
            [`primaryDexPatterns`](AndroidBinaryDescriptionArg.html#getPrimaryDexPatterns())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of primaryDexPatterns elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPrimaryDexPatterns(java.lang.Iterable)}

        -   #### setPrimaryDexPatterns

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder setPrimaryDexPatterns​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`primaryDexPatterns`](AndroidBinaryDescriptionArg.html#getPrimaryDexPatterns())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of primaryDexPatterns elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllPrimaryDexPatterns(java.lang.Iterable)}

        -   #### addAllPrimaryDexPatterns

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder addAllPrimaryDexPatterns​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`primaryDexPatterns`](AndroidBinaryDescriptionArg.html#getPrimaryDexPatterns())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of primaryDexPatterns elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPrimaryDexClassesFile(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setPrimaryDexClassesFile

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder setPrimaryDexClassesFile​(SourcePath primaryDexClassesFile)
            ```

            ::: block
            Initializes the optional value
            [`primaryDexClassesFile`](AndroidBinaryDescriptionArg.html#getPrimaryDexClassesFile())
            to primaryDexClassesFile.
            :::

            [Parameters:]{.paramLabel}
            :   `primaryDexClassesFile` - The value for
                primaryDexClassesFile

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setPrimaryDexClassesFile(java.util.Optional)}

        -   #### setPrimaryDexClassesFile

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder setPrimaryDexClassesFile​(Optional<? extends SourcePath> primaryDexClassesFile)
            ```

            ::: block
            Initializes the optional value
            [`primaryDexClassesFile`](AndroidBinaryDescriptionArg.html#getPrimaryDexClassesFile())
            to primaryDexClassesFile.
            :::

            [Parameters:]{.paramLabel}
            :   `primaryDexClassesFile` - The value for
                primaryDexClassesFile

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPrimaryDexScenarioFile(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setPrimaryDexScenarioFile

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder setPrimaryDexScenarioFile​(SourcePath primaryDexScenarioFile)
            ```

            ::: block
            Initializes the optional value
            [`primaryDexScenarioFile`](AndroidBinaryDescriptionArg.html#getPrimaryDexScenarioFile())
            to primaryDexScenarioFile.
            :::

            [Parameters:]{.paramLabel}
            :   `primaryDexScenarioFile` - The value for
                primaryDexScenarioFile

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setPrimaryDexScenarioFile(java.util.Optional)}

        -   #### setPrimaryDexScenarioFile

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder setPrimaryDexScenarioFile​(Optional<? extends SourcePath> primaryDexScenarioFile)
            ```

            ::: block
            Initializes the optional value
            [`primaryDexScenarioFile`](AndroidBinaryDescriptionArg.html#getPrimaryDexScenarioFile())
            to primaryDexScenarioFile.
            :::

            [Parameters:]{.paramLabel}
            :   `primaryDexScenarioFile` - The value for
                primaryDexScenarioFile

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPrimaryDexScenarioOverflowAllowed(boolean)}

        -   #### setPrimaryDexScenarioOverflowAllowed

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder setPrimaryDexScenarioOverflowAllowed​(boolean primaryDexScenarioOverflowAllowed)
            ```

            ::: block
            Initializes the value for the
            [`primaryDexScenarioOverflowAllowed`](AndroidBinaryDescriptionArg.html#isPrimaryDexScenarioOverflowAllowed())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`primaryDexScenarioOverflowAllowed`](AndroidBinaryDescriptionArg.html#isPrimaryDexScenarioOverflowAllowed()).*
            :::

            [Parameters:]{.paramLabel}
            :   `primaryDexScenarioOverflowAllowed` - The value for
                primaryDexScenarioOverflowAllowed

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setSecondaryDexHeadClassesFile(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setSecondaryDexHeadClassesFile

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder setSecondaryDexHeadClassesFile​(SourcePath secondaryDexHeadClassesFile)
            ```

            ::: block
            Initializes the optional value
            [`secondaryDexHeadClassesFile`](AndroidBinaryDescriptionArg.html#getSecondaryDexHeadClassesFile())
            to secondaryDexHeadClassesFile.
            :::

            [Parameters:]{.paramLabel}
            :   `secondaryDexHeadClassesFile` - The value for
                secondaryDexHeadClassesFile

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setSecondaryDexHeadClassesFile(java.util.Optional)}

        -   #### setSecondaryDexHeadClassesFile

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder setSecondaryDexHeadClassesFile​(Optional<? extends SourcePath> secondaryDexHeadClassesFile)
            ```

            ::: block
            Initializes the optional value
            [`secondaryDexHeadClassesFile`](AndroidBinaryDescriptionArg.html#getSecondaryDexHeadClassesFile())
            to secondaryDexHeadClassesFile.
            :::

            [Parameters:]{.paramLabel}
            :   `secondaryDexHeadClassesFile` - The value for
                secondaryDexHeadClassesFile

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setSecondaryDexTailClassesFile(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setSecondaryDexTailClassesFile

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder setSecondaryDexTailClassesFile​(SourcePath secondaryDexTailClassesFile)
            ```

            ::: block
            Initializes the optional value
            [`secondaryDexTailClassesFile`](AndroidBinaryDescriptionArg.html#getSecondaryDexTailClassesFile())
            to secondaryDexTailClassesFile.
            :::

            [Parameters:]{.paramLabel}
            :   `secondaryDexTailClassesFile` - The value for
                secondaryDexTailClassesFile

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setSecondaryDexTailClassesFile(java.util.Optional)}

        -   #### setSecondaryDexTailClassesFile

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder setSecondaryDexTailClassesFile​(Optional<? extends SourcePath> secondaryDexTailClassesFile)
            ```

            ::: block
            Initializes the optional value
            [`secondaryDexTailClassesFile`](AndroidBinaryDescriptionArg.html#getSecondaryDexTailClassesFile())
            to secondaryDexTailClassesFile.
            :::

            [Parameters:]{.paramLabel}
            :   `secondaryDexTailClassesFile` - The value for
                secondaryDexTailClassesFile

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setAndroidAppModularityResult(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setAndroidAppModularityResult

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder setAndroidAppModularityResult​(SourcePath androidAppModularityResult)
            ```

            ::: block
            Initializes the optional value
            [`androidAppModularityResult`](AndroidBinaryDescriptionArg.html#getAndroidAppModularityResult())
            to androidAppModularityResult.
            :::

            [Parameters:]{.paramLabel}
            :   `androidAppModularityResult` - The value for
                androidAppModularityResult

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setAndroidAppModularityResult(java.util.Optional)}

        -   #### setAndroidAppModularityResult

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder setAndroidAppModularityResult​(Optional<? extends SourcePath> androidAppModularityResult)
            ```

            ::: block
            Initializes the optional value
            [`androidAppModularityResult`](AndroidBinaryDescriptionArg.html#getAndroidAppModularityResult())
            to androidAppModularityResult.
            :::

            [Parameters:]{.paramLabel}
            :   `androidAppModularityResult` - The value for
                androidAppModularityResult

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLinearAllocHardLimit(long)}

        -   #### setLinearAllocHardLimit

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder setLinearAllocHardLimit​(long linearAllocHardLimit)
            ```

            ::: block
            Initializes the value for the
            [`linearAllocHardLimit`](AndroidBinaryDescriptionArg.html#getLinearAllocHardLimit())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`linearAllocHardLimit`](AndroidBinaryDescriptionArg.html#getLinearAllocHardLimit()).*
            :::

            [Parameters:]{.paramLabel}
            :   `linearAllocHardLimit` - The value for
                linearAllocHardLimit

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDexGroupLibLimit(int)}

        -   #### setDexGroupLibLimit

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder setDexGroupLibLimit​(int dexGroupLibLimit)
            ```

            ::: block
            Initializes the value for the
            [`dexGroupLibLimit`](AndroidBinaryDescriptionArg.html#getDexGroupLibLimit())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`dexGroupLibLimit`](AndroidBinaryDescriptionArg.html#getDexGroupLibLimit()).*
            :::

            [Parameters:]{.paramLabel}
            :   `dexGroupLibLimit` - The value for dexGroupLibLimit

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addResourceFilter(java.lang.String)}

        -   #### addResourceFilter

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder addResourceFilter​(String element)
            ```

            ::: block
            Adds one element to
            [`resourceFilter`](AndroidBinaryDescriptionArg.html#getResourceFilter())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A resourceFilter element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addResourceFilter(java.lang.String...)}

        -   #### addResourceFilter

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder addResourceFilter​(String... elements)
            ```

            ::: block
            Adds elements to
            [`resourceFilter`](AndroidBinaryDescriptionArg.html#getResourceFilter())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of resourceFilter elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setResourceFilter(java.lang.Iterable)}

        -   #### setResourceFilter

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder setResourceFilter​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`resourceFilter`](AndroidBinaryDescriptionArg.html#getResourceFilter())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of resourceFilter elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllResourceFilter(java.lang.Iterable)}

        -   #### addAllResourceFilter

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder addAllResourceFilter​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`resourceFilter`](AndroidBinaryDescriptionArg.html#getResourceFilter())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of resourceFilter elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addPreprocessJavaClassesDeps(com.facebook.buck.core.model.BuildTarget)}

        -   #### addPreprocessJavaClassesDeps

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder addPreprocessJavaClassesDeps​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`preprocessJavaClassesDeps`](AndroidBinaryDescriptionArg.html#getPreprocessJavaClassesDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A preprocessJavaClassesDeps element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addPreprocessJavaClassesDeps(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addPreprocessJavaClassesDeps

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder addPreprocessJavaClassesDeps​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`preprocessJavaClassesDeps`](AndroidBinaryDescriptionArg.html#getPreprocessJavaClassesDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of preprocessJavaClassesDeps
                elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPreprocessJavaClassesDeps(java.lang.Iterable)}

        -   #### setPreprocessJavaClassesDeps

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder setPreprocessJavaClassesDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`preprocessJavaClassesDeps`](AndroidBinaryDescriptionArg.html#getPreprocessJavaClassesDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of preprocessJavaClassesDeps
                elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllPreprocessJavaClassesDeps(java.lang.Iterable)}

        -   #### addAllPreprocessJavaClassesDeps

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder addAllPreprocessJavaClassesDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`preprocessJavaClassesDeps`](AndroidBinaryDescriptionArg.html#getPreprocessJavaClassesDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of preprocessJavaClassesDeps
                elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setXzCompressionLevel(int)}

        -   #### setXzCompressionLevel

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder setXzCompressionLevel​(int xzCompressionLevel)
            ```

            ::: block
            Initializes the value for the
            [`xzCompressionLevel`](AndroidBinaryDescriptionArg.html#getXzCompressionLevel())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`xzCompressionLevel`](AndroidBinaryDescriptionArg.html#getXzCompressionLevel()).*
            :::

            [Parameters:]{.paramLabel}
            :   `xzCompressionLevel` - The value for xzCompressionLevel

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPackageAssetLibraries(boolean)}

        -   #### setPackageAssetLibraries

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder setPackageAssetLibraries​(boolean packageAssetLibraries)
            ```

            ::: block
            Initializes the value for the
            [`packageAssetLibraries`](AndroidBinaryDescriptionArg.html#isPackageAssetLibraries())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`packageAssetLibraries`](AndroidBinaryDescriptionArg.html#isPackageAssetLibraries()).*
            :::

            [Parameters:]{.paramLabel}
            :   `packageAssetLibraries` - The value for
                packageAssetLibraries

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCompressAssetLibraries(boolean)}

        -   #### setCompressAssetLibraries

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder setCompressAssetLibraries​(boolean compressAssetLibraries)
            ```

            ::: block
            Initializes the value for the
            [`compressAssetLibraries`](AndroidBinaryDescriptionArg.html#isCompressAssetLibraries())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`compressAssetLibraries`](AndroidBinaryDescriptionArg.html#isCompressAssetLibraries()).*
            :::

            [Parameters:]{.paramLabel}
            :   `compressAssetLibraries` - The value for
                compressAssetLibraries

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setAssetCompressionAlgorithm(com.facebook.buck.android.CompressionAlgorithm)}

        -   #### setAssetCompressionAlgorithm

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder setAssetCompressionAlgorithm​(CompressionAlgorithm assetCompressionAlgorithm)
            ```

            ::: block
            Initializes the optional value
            [`assetCompressionAlgorithm`](AndroidBinaryDescriptionArg.html#getAssetCompressionAlgorithm())
            to assetCompressionAlgorithm.
            :::

            [Parameters:]{.paramLabel}
            :   `assetCompressionAlgorithm` - The value for
                assetCompressionAlgorithm

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setAssetCompressionAlgorithm(java.util.Optional)}

        -   #### setAssetCompressionAlgorithm

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder setAssetCompressionAlgorithm​(Optional<? extends CompressionAlgorithm> assetCompressionAlgorithm)
            ```

            ::: block
            Initializes the optional value
            [`assetCompressionAlgorithm`](AndroidBinaryDescriptionArg.html#getAssetCompressionAlgorithm())
            to assetCompressionAlgorithm.
            :::

            [Parameters:]{.paramLabel}
            :   `assetCompressionAlgorithm` - The value for
                assetCompressionAlgorithm

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setRedex(boolean)}

        -   #### setRedex

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder setRedex​(boolean redex)
            ```

            ::: block
            Initializes the value for the
            [`redex`](AndroidBinaryDescriptionArg.html#getRedex())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`redex`](AndroidBinaryDescriptionArg.html#getRedex()).*
            :::

            [Parameters:]{.paramLabel}
            :   `redex` - The value for redex

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setRedexConfig(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setRedexConfig

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder setRedexConfig​(SourcePath redexConfig)
            ```

            ::: block
            Initializes the optional value
            [`redexConfig`](AndroidBinaryDescriptionArg.html#getRedexConfig())
            to redexConfig.
            :::

            [Parameters:]{.paramLabel}
            :   `redexConfig` - The value for redexConfig

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setRedexConfig(java.util.Optional)}

        -   #### setRedexConfig

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder setRedexConfig​(Optional<? extends SourcePath> redexConfig)
            ```

            ::: block
            Initializes the optional value
            [`redexConfig`](AndroidBinaryDescriptionArg.html#getRedexConfig())
            to redexConfig.
            :::

            [Parameters:]{.paramLabel}
            :   `redexConfig` - The value for redexConfig

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addRedexExtraArgs(com.facebook.buck.rules.macros.StringWithMacros)}

        -   #### addRedexExtraArgs

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder addRedexExtraArgs​(StringWithMacros element)
            ```

            ::: block
            Adds one element to
            [`redexExtraArgs`](AndroidBinaryDescriptionArg.html#getRedexExtraArgs())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A redexExtraArgs element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addRedexExtraArgs(com.facebook.buck.rules.macros.StringWithMacros...)}

        -   #### addRedexExtraArgs

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder addRedexExtraArgs​(StringWithMacros... elements)
            ```

            ::: block
            Adds elements to
            [`redexExtraArgs`](AndroidBinaryDescriptionArg.html#getRedexExtraArgs())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of redexExtraArgs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setRedexExtraArgs(java.lang.Iterable)}

        -   #### setRedexExtraArgs

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder setRedexExtraArgs​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`redexExtraArgs`](AndroidBinaryDescriptionArg.html#getRedexExtraArgs())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of redexExtraArgs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllRedexExtraArgs(java.lang.Iterable)}

        -   #### addAllRedexExtraArgs

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder addAllRedexExtraArgs​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Adds elements to
            [`redexExtraArgs`](AndroidBinaryDescriptionArg.html#getRedexExtraArgs())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of redexExtraArgs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addDeps(com.facebook.buck.core.model.BuildTarget)}

        -   #### addDeps

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder addDeps​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`deps`](AndroidBinaryDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A deps element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addDeps(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addDeps

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder addDeps​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`deps`](AndroidBinaryDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDeps(java.lang.Iterable)}

        -   #### setDeps

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder setDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`deps`](AndroidBinaryDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllDeps(java.lang.Iterable)}

        -   #### addAllDeps

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder addAllDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`deps`](AndroidBinaryDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLicenses(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### addLicenses

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder addLicenses​(SourcePath element)
            ```

            ::: block
            Adds one element to
            [`licenses`](AndroidBinaryDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A licenses element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLicenses(com.facebook.buck.core.sourcepath.SourcePath...)}

        -   #### addLicenses

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder addLicenses​(SourcePath... elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](AndroidBinaryDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLicenses(java.lang.Iterable)}

        -   #### setLicenses

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder setLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`licenses`](AndroidBinaryDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLicenses(java.lang.Iterable)}

        -   #### addAllLicenses

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder addAllLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](AndroidBinaryDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLabels(java.lang.String)}

        -   #### addLabels

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder addLabels​(String element)
            ```

            ::: block
            Adds one element to
            [`labels`](AndroidBinaryDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A labels element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLabels(java.lang.String...)}

        -   #### addLabels

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder addLabels​(String... elements)
            ```

            ::: block
            Adds elements to
            [`labels`](AndroidBinaryDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLabels(java.lang.Iterable)}

        -   #### setLabels

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder setLabels​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`labels`](AndroidBinaryDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLabels(java.lang.Iterable)}

        -   #### addAllLabels

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder addAllLabels​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`labels`](AndroidBinaryDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDefaultTargetPlatform(com.facebook.buck.core.model.UnconfiguredBuildTarget)}

        -   #### setDefaultTargetPlatform

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder setDefaultTargetPlatform​(UnconfiguredBuildTarget defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](AndroidBinaryDescriptionArg.html#getDefaultTargetPlatform())
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
            public final AndroidBinaryDescriptionArg.Builder setDefaultTargetPlatform​(Optional<? extends UnconfiguredBuildTarget> defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](AndroidBinaryDescriptionArg.html#getDefaultTargetPlatform())
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
            public final AndroidBinaryDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget element)
            ```

            ::: block
            Adds one element to
            [`compatibleWith`](AndroidBinaryDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A compatibleWith element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCompatibleWith(com.facebook.buck.core.model.UnconfiguredBuildTarget...)}

        -   #### addCompatibleWith

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](AndroidBinaryDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCompatibleWith(java.lang.Iterable)}

        -   #### setCompatibleWith

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder setCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`compatibleWith`](AndroidBinaryDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllCompatibleWith(java.lang.Iterable)}

        -   #### addAllCompatibleWith

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder addAllCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](AndroidBinaryDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setName(java.lang.String)}

        -   #### setName

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder setName​(String name)
            ```

            ::: block
            Initializes the value for the
            [`name`](AndroidBinaryDescriptionArg.html#getName())
            attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `name` - The value for name

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setExopackage(boolean)}

        -   #### setExopackage

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder setExopackage​(boolean exopackage)
            ```

            ::: block
            Initializes the optional value
            [`exopackage`](AndroidBinaryDescriptionArg.html#isExopackage())
            to exopackage.
            :::

            [Parameters:]{.paramLabel}
            :   `exopackage` - The value for exopackage

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setExopackage(java.util.Optional)}

        -   #### setExopackage

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder setExopackage​(Optional<Boolean> exopackage)
            ```

            ::: block
            Initializes the optional value
            [`exopackage`](AndroidBinaryDescriptionArg.html#isExopackage())
            to exopackage.
            :::

            [Parameters:]{.paramLabel}
            :   `exopackage` - The value for exopackage

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addExopackageModes(com.facebook.buck.android.exopackage.ExopackageMode)}

        -   #### addExopackageModes

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder addExopackageModes​(ExopackageMode element)
            ```

            ::: block
            Adds one element to
            [`exopackageModes`](AndroidBinaryDescriptionArg.html#getExopackageModes())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A exopackageModes element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addExopackageModes(com.facebook.buck.android.exopackage.ExopackageMode...)}

        -   #### addExopackageModes

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder addExopackageModes​(ExopackageMode... elements)
            ```

            ::: block
            Adds elements to
            [`exopackageModes`](AndroidBinaryDescriptionArg.html#getExopackageModes())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of exopackageModes elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setExopackageModes(java.lang.Iterable)}

        -   #### setExopackageModes

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder setExopackageModes​(Iterable<ExopackageMode> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`exopackageModes`](AndroidBinaryDescriptionArg.html#getExopackageModes())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of exopackageModes elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllExopackageModes(java.lang.Iterable)}

        -   #### addAllExopackageModes

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder addAllExopackageModes​(Iterable<ExopackageMode> elements)
            ```

            ::: block
            Adds elements to
            [`exopackageModes`](AndroidBinaryDescriptionArg.html#getExopackageModes())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of exopackageModes elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addTests(com.facebook.buck.core.model.BuildTarget)}

        -   #### addTests

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder addTests​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`tests`](AndroidBinaryDescriptionArg.html#getTests())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A tests element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addTests(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addTests

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder addTests​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`tests`](AndroidBinaryDescriptionArg.html#getTests())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of tests elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setTests(java.lang.Iterable)}

        -   #### setTests

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder setTests​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`tests`](AndroidBinaryDescriptionArg.html#getTests())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of tests elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllTests(java.lang.Iterable)}

        -   #### addAllTests

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder addAllTests​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`tests`](AndroidBinaryDescriptionArg.html#getTests())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of tests elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setManifest(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setManifest

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder setManifest​(SourcePath manifest)
            ```

            ::: block
            Initializes the optional value
            [`manifest`](AndroidBinaryDescriptionArg.html#getManifest())
            to manifest.
            :::

            [Parameters:]{.paramLabel}
            :   `manifest` - The value for manifest

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setManifest(java.util.Optional)}

        -   #### setManifest

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder setManifest​(Optional<? extends SourcePath> manifest)
            ```

            ::: block
            Initializes the optional value
            [`manifest`](AndroidBinaryDescriptionArg.html#getManifest())
            to manifest.
            :::

            [Parameters:]{.paramLabel}
            :   `manifest` - The value for manifest

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setManifestSkeleton(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setManifestSkeleton

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder setManifestSkeleton​(SourcePath manifestSkeleton)
            ```

            ::: block
            Initializes the optional value
            [`manifestSkeleton`](AndroidBinaryDescriptionArg.html#getManifestSkeleton())
            to manifestSkeleton.
            :::

            [Parameters:]{.paramLabel}
            :   `manifestSkeleton` - The value for manifestSkeleton

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setManifestSkeleton(java.util.Optional)}

        -   #### setManifestSkeleton

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder setManifestSkeleton​(Optional<? extends SourcePath> manifestSkeleton)
            ```

            ::: block
            Initializes the optional value
            [`manifestSkeleton`](AndroidBinaryDescriptionArg.html#getManifestSkeleton())
            to manifestSkeleton.
            :::

            [Parameters:]{.paramLabel}
            :   `manifestSkeleton` - The value for manifestSkeleton

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setModuleManifestSkeleton(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setModuleManifestSkeleton

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder setModuleManifestSkeleton​(SourcePath moduleManifestSkeleton)
            ```

            ::: block
            Initializes the optional value
            [`moduleManifestSkeleton`](AndroidBinaryDescriptionArg.html#getModuleManifestSkeleton())
            to moduleManifestSkeleton.
            :::

            [Parameters:]{.paramLabel}
            :   `moduleManifestSkeleton` - The value for
                moduleManifestSkeleton

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setModuleManifestSkeleton(java.util.Optional)}

        -   #### setModuleManifestSkeleton

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder setModuleManifestSkeleton​(Optional<? extends SourcePath> moduleManifestSkeleton)
            ```

            ::: block
            Initializes the optional value
            [`moduleManifestSkeleton`](AndroidBinaryDescriptionArg.html#getModuleManifestSkeleton())
            to moduleManifestSkeleton.
            :::

            [Parameters:]{.paramLabel}
            :   `moduleManifestSkeleton` - The value for
                moduleManifestSkeleton

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPackageType(java.lang.String)}

        -   #### setPackageType

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder setPackageType​(String packageType)
            ```

            ::: block
            Initializes the optional value
            [`packageType`](AndroidBinaryDescriptionArg.html#getPackageType())
            to packageType.
            :::

            [Parameters:]{.paramLabel}
            :   `packageType` - The value for packageType

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setPackageType(java.util.Optional)}

        -   #### setPackageType

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder setPackageType​(Optional<String> packageType)
            ```

            ::: block
            Initializes the optional value
            [`packageType`](AndroidBinaryDescriptionArg.html#getPackageType())
            to packageType.
            :::

            [Parameters:]{.paramLabel}
            :   `packageType` - The value for packageType

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addNoDx(com.facebook.buck.core.model.BuildTarget)}

        -   #### addNoDx

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder addNoDx​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`noDx`](AndroidBinaryDescriptionArg.html#getNoDx()) set.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A noDx element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addNoDx(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addNoDx

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder addNoDx​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`noDx`](AndroidBinaryDescriptionArg.html#getNoDx()) set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of noDx elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setNoDx(java.lang.Iterable)}

        -   #### setNoDx

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder setNoDx​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`noDx`](AndroidBinaryDescriptionArg.html#getNoDx()) set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of noDx elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllNoDx(java.lang.Iterable)}

        -   #### addAllNoDx

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder addAllNoDx​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`noDx`](AndroidBinaryDescriptionArg.html#getNoDx()) set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of noDx elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDisablePreDex(boolean)}

        -   #### setDisablePreDex

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder setDisablePreDex​(boolean disablePreDex)
            ```

            ::: block
            Initializes the value for the
            [`disablePreDex`](AndroidBinaryDescriptionArg.html#getDisablePreDex())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`disablePreDex`](AndroidBinaryDescriptionArg.html#getDisablePreDex()).*
            :::

            [Parameters:]{.paramLabel}
            :   `disablePreDex` - The value for disablePreDex

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setAndroidSdkProguardConfig(com.facebook.buck.android.ProGuardObfuscateStep.SdkProguardType)}

        -   #### setAndroidSdkProguardConfig

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder setAndroidSdkProguardConfig​(com.facebook.buck.android.ProGuardObfuscateStep.SdkProguardType androidSdkProguardConfig)
            ```

            ::: block
            Initializes the optional value
            [`androidSdkProguardConfig`](AndroidBinaryDescriptionArg.html#getAndroidSdkProguardConfig())
            to androidSdkProguardConfig.
            :::

            [Parameters:]{.paramLabel}
            :   `androidSdkProguardConfig` - The value for
                androidSdkProguardConfig

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setAndroidSdkProguardConfig(java.util.Optional)}

        -   #### setAndroidSdkProguardConfig

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder setAndroidSdkProguardConfig​(Optional<? extends com.facebook.buck.android.ProGuardObfuscateStep.SdkProguardType> androidSdkProguardConfig)
            ```

            ::: block
            Initializes the optional value
            [`androidSdkProguardConfig`](AndroidBinaryDescriptionArg.html#getAndroidSdkProguardConfig())
            to androidSdkProguardConfig.
            :::

            [Parameters:]{.paramLabel}
            :   `androidSdkProguardConfig` - The value for
                androidSdkProguardConfig

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setOptimizationPasses(int)}

        -   #### setOptimizationPasses

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder setOptimizationPasses​(int optimizationPasses)
            ```

            ::: block
            Initializes the value for the
            [`optimizationPasses`](AndroidBinaryDescriptionArg.html#getOptimizationPasses())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`optimizationPasses`](AndroidBinaryDescriptionArg.html#getOptimizationPasses()).*
            :::

            [Parameters:]{.paramLabel}
            :   `optimizationPasses` - The value for optimizationPasses

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addProguardJvmArgs(java.lang.String)}

        -   #### addProguardJvmArgs

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder addProguardJvmArgs​(String element)
            ```

            ::: block
            Adds one element to
            [`proguardJvmArgs`](AndroidBinaryDescriptionArg.html#getProguardJvmArgs())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A proguardJvmArgs element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addProguardJvmArgs(java.lang.String...)}

        -   #### addProguardJvmArgs

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder addProguardJvmArgs​(String... elements)
            ```

            ::: block
            Adds elements to
            [`proguardJvmArgs`](AndroidBinaryDescriptionArg.html#getProguardJvmArgs())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of proguardJvmArgs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setProguardJvmArgs(java.lang.Iterable)}

        -   #### setProguardJvmArgs

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder setProguardJvmArgs​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`proguardJvmArgs`](AndroidBinaryDescriptionArg.html#getProguardJvmArgs())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of proguardJvmArgs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllProguardJvmArgs(java.lang.Iterable)}

        -   #### addAllProguardJvmArgs

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder addAllProguardJvmArgs​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`proguardJvmArgs`](AndroidBinaryDescriptionArg.html#getProguardJvmArgs())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of proguardJvmArgs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setProguardConfig(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setProguardConfig

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder setProguardConfig​(SourcePath proguardConfig)
            ```

            ::: block
            Initializes the optional value
            [`proguardConfig`](AndroidBinaryDescriptionArg.html#getProguardConfig())
            to proguardConfig.
            :::

            [Parameters:]{.paramLabel}
            :   `proguardConfig` - The value for proguardConfig

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setProguardConfig(java.util.Optional)}

        -   #### setProguardConfig

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder setProguardConfig​(Optional<? extends SourcePath> proguardConfig)
            ```

            ::: block
            Initializes the optional value
            [`proguardConfig`](AndroidBinaryDescriptionArg.html#getProguardConfig())
            to proguardConfig.
            :::

            [Parameters:]{.paramLabel}
            :   `proguardConfig` - The value for proguardConfig

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setResourceCompression(com.facebook.buck.android.ResourcesFilter.ResourceCompressionMode)}

        -   #### setResourceCompression

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder setResourceCompression​(com.facebook.buck.android.ResourcesFilter.ResourceCompressionMode resourceCompression)
            ```

            ::: block
            Initializes the value for the
            [`resourceCompression`](AndroidBinaryDescriptionArg.html#getResourceCompression())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`resourceCompression`](AndroidBinaryDescriptionArg.html#getResourceCompression()).*
            :::

            [Parameters:]{.paramLabel}
            :   `resourceCompression` - The value for
                resourceCompression

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setSkipCrunchPngs(boolean)}

        -   #### setSkipCrunchPngs

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder setSkipCrunchPngs​(boolean skipCrunchPngs)
            ```

            ::: block
            Initializes the optional value
            [`skipCrunchPngs`](AndroidBinaryDescriptionArg.html#isSkipCrunchPngs())
            to skipCrunchPngs.
            :::

            [Parameters:]{.paramLabel}
            :   `skipCrunchPngs` - The value for skipCrunchPngs

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setSkipCrunchPngs(java.util.Optional)}

        -   #### setSkipCrunchPngs

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder setSkipCrunchPngs​(Optional<Boolean> skipCrunchPngs)
            ```

            ::: block
            Initializes the optional value
            [`skipCrunchPngs`](AndroidBinaryDescriptionArg.html#isSkipCrunchPngs())
            to skipCrunchPngs.
            :::

            [Parameters:]{.paramLabel}
            :   `skipCrunchPngs` - The value for skipCrunchPngs

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setIncludesVectorDrawables(boolean)}

        -   #### setIncludesVectorDrawables

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder setIncludesVectorDrawables​(boolean includesVectorDrawables)
            ```

            ::: block
            Initializes the value for the
            [`includesVectorDrawables`](AndroidBinaryDescriptionArg.html#isIncludesVectorDrawables())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`includesVectorDrawables`](AndroidBinaryDescriptionArg.html#isIncludesVectorDrawables()).*
            :::

            [Parameters:]{.paramLabel}
            :   `includesVectorDrawables` - The value for
                includesVectorDrawables

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setNoAutoVersionResources(boolean)}

        -   #### setNoAutoVersionResources

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder setNoAutoVersionResources​(boolean noAutoVersionResources)
            ```

            ::: block
            Initializes the value for the
            [`noAutoVersionResources`](AndroidBinaryDescriptionArg.html#isNoAutoVersionResources())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`noAutoVersionResources`](AndroidBinaryDescriptionArg.html#isNoAutoVersionResources()).*
            :::

            [Parameters:]{.paramLabel}
            :   `noAutoVersionResources` - The value for
                noAutoVersionResources

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setNoVersionTransitionsResources(boolean)}

        -   #### setNoVersionTransitionsResources

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder setNoVersionTransitionsResources​(boolean noVersionTransitionsResources)
            ```

            ::: block
            Initializes the value for the
            [`noVersionTransitionsResources`](AndroidBinaryDescriptionArg.html#isNoVersionTransitionsResources())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`noVersionTransitionsResources`](AndroidBinaryDescriptionArg.html#isNoVersionTransitionsResources()).*
            :::

            [Parameters:]{.paramLabel}
            :   `noVersionTransitionsResources` - The value for
                noVersionTransitionsResources

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setNoAutoAddOverlayResources(boolean)}

        -   #### setNoAutoAddOverlayResources

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder setNoAutoAddOverlayResources​(boolean noAutoAddOverlayResources)
            ```

            ::: block
            Initializes the value for the
            [`noAutoAddOverlayResources`](AndroidBinaryDescriptionArg.html#isNoAutoAddOverlayResources())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`noAutoAddOverlayResources`](AndroidBinaryDescriptionArg.html#isNoAutoAddOverlayResources()).*
            :::

            [Parameters:]{.paramLabel}
            :   `noAutoAddOverlayResources` - The value for
                noAutoAddOverlayResources

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addApplicationModuleTargets(com.facebook.buck.core.model.BuildTarget)}

        -   #### addApplicationModuleTargets

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder addApplicationModuleTargets​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`applicationModuleTargets`](AndroidBinaryDescriptionArg.html#getApplicationModuleTargets())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A applicationModuleTargets element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addApplicationModuleTargets(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addApplicationModuleTargets

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder addApplicationModuleTargets​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`applicationModuleTargets`](AndroidBinaryDescriptionArg.html#getApplicationModuleTargets())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of applicationModuleTargets
                elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setApplicationModuleTargets(java.lang.Iterable)}

        -   #### setApplicationModuleTargets

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder setApplicationModuleTargets​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`applicationModuleTargets`](AndroidBinaryDescriptionArg.html#getApplicationModuleTargets())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of applicationModuleTargets
                elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllApplicationModuleTargets(java.lang.Iterable)}

        -   #### addAllApplicationModuleTargets

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder addAllApplicationModuleTargets​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`applicationModuleTargets`](AndroidBinaryDescriptionArg.html#getApplicationModuleTargets())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of applicationModuleTargets
                elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putApplicationModuleConfigs(java.lang.String,com.google.common.collect.ImmutableList)}

        -   #### putApplicationModuleConfigs

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder putApplicationModuleConfigs​(String key,
                                                                                         com.google.common.collect.ImmutableList<BuildTarget> value)
            ```

            ::: block
            Put one entry to the
            [`applicationModuleConfigs`](AndroidBinaryDescriptionArg.html#getApplicationModuleConfigs())
            map.
            :::

            [Parameters:]{.paramLabel}
            :   `key` - The key in the applicationModuleConfigs map
            :   `value` - The associated value in the
                applicationModuleConfigs map

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putApplicationModuleConfigs(java.util.Map.Entry)}

        -   #### putApplicationModuleConfigs

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder putApplicationModuleConfigs​(Map.Entry<String,​? extends com.google.common.collect.ImmutableList<BuildTarget>> entry)
            ```

            ::: block
            Put one entry to the
            [`applicationModuleConfigs`](AndroidBinaryDescriptionArg.html#getApplicationModuleConfigs())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entry` - The key and value entry

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setApplicationModuleConfigs(java.util.Map)}

        -   #### setApplicationModuleConfigs

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder setApplicationModuleConfigs​(Map<String,​? extends com.google.common.collect.ImmutableList<BuildTarget>> entries)
            ```

            ::: block
            Sets or replaces all mappings from the specified map as
            entries for the
            [`applicationModuleConfigs`](AndroidBinaryDescriptionArg.html#getApplicationModuleConfigs())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entries` - The entries that will be added to the
                applicationModuleConfigs map

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putAllApplicationModuleConfigs(java.util.Map)}

        -   #### putAllApplicationModuleConfigs

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder putAllApplicationModuleConfigs​(Map<String,​? extends com.google.common.collect.ImmutableList<BuildTarget>> entries)
            ```

            ::: block
            Put all mappings from the specified map as entries to
            [`applicationModuleConfigs`](AndroidBinaryDescriptionArg.html#getApplicationModuleConfigs())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entries` - The entries that will be added to the
                applicationModuleConfigs map

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addApplicationModulesWithResources(java.lang.String)}

        -   #### addApplicationModulesWithResources

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder addApplicationModulesWithResources​(String element)
            ```

            ::: block
            Adds one element to
            [`applicationModulesWithResources`](AndroidBinaryDescriptionArg.html#getApplicationModulesWithResources())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A applicationModulesWithResources element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addApplicationModulesWithResources(java.lang.String...)}

        -   #### addApplicationModulesWithResources

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder addApplicationModulesWithResources​(String... elements)
            ```

            ::: block
            Adds elements to
            [`applicationModulesWithResources`](AndroidBinaryDescriptionArg.html#getApplicationModulesWithResources())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of applicationModulesWithResources
                elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setApplicationModulesWithResources(java.lang.Iterable)}

        -   #### setApplicationModulesWithResources

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder setApplicationModulesWithResources​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`applicationModulesWithResources`](AndroidBinaryDescriptionArg.html#getApplicationModulesWithResources())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of
                applicationModulesWithResources elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllApplicationModulesWithResources(java.lang.Iterable)}

        -   #### addAllApplicationModulesWithResources

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder addAllApplicationModulesWithResources​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`applicationModulesWithResources`](AndroidBinaryDescriptionArg.html#getApplicationModulesWithResources())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of
                applicationModulesWithResources elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addApplicationModulesWithManifest(java.lang.String)}

        -   #### addApplicationModulesWithManifest

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder addApplicationModulesWithManifest​(String element)
            ```

            ::: block
            Adds one element to
            [`applicationModulesWithManifest`](AndroidBinaryDescriptionArg.html#getApplicationModulesWithManifest())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A applicationModulesWithManifest element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addApplicationModulesWithManifest(java.lang.String...)}

        -   #### addApplicationModulesWithManifest

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder addApplicationModulesWithManifest​(String... elements)
            ```

            ::: block
            Adds elements to
            [`applicationModulesWithManifest`](AndroidBinaryDescriptionArg.html#getApplicationModulesWithManifest())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of applicationModulesWithManifest
                elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setApplicationModulesWithManifest(java.lang.Iterable)}

        -   #### setApplicationModulesWithManifest

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder setApplicationModulesWithManifest​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`applicationModulesWithManifest`](AndroidBinaryDescriptionArg.html#getApplicationModulesWithManifest())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of
                applicationModulesWithManifest elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllApplicationModulesWithManifest(java.lang.Iterable)}

        -   #### addAllApplicationModulesWithManifest

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder addAllApplicationModulesWithManifest​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`applicationModulesWithManifest`](AndroidBinaryDescriptionArg.html#getApplicationModulesWithManifest())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of
                applicationModulesWithManifest elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setApplicationModuleDependencies(com.google.common.collect.ImmutableMap)}

        -   #### setApplicationModuleDependencies

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder setApplicationModuleDependencies​(com.google.common.collect.ImmutableMap<String,​com.google.common.collect.ImmutableList<String>> applicationModuleDependencies)
            ```

            ::: block
            Initializes the optional value
            [`applicationModuleDependencies`](AndroidBinaryDescriptionArg.html#getApplicationModuleDependencies())
            to applicationModuleDependencies.
            :::

            [Parameters:]{.paramLabel}
            :   `applicationModuleDependencies` - The value for
                applicationModuleDependencies

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setApplicationModuleDependencies(java.util.Optional)}

        -   #### setApplicationModuleDependencies

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder setApplicationModuleDependencies​(Optional<? extends com.google.common.collect.ImmutableMap<String,​com.google.common.collect.ImmutableList<String>>> applicationModuleDependencies)
            ```

            ::: block
            Initializes the optional value
            [`applicationModuleDependencies`](AndroidBinaryDescriptionArg.html#getApplicationModuleDependencies())
            to applicationModuleDependencies.
            :::

            [Parameters:]{.paramLabel}
            :   `applicationModuleDependencies` - The value for
                applicationModuleDependencies

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setIsCacheable(boolean)}

        -   #### setIsCacheable

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder setIsCacheable​(boolean isCacheable)
            ```

            ::: block
            Initializes the value for the
            [`isCacheable`](AndroidBinaryDescriptionArg.html#getIsCacheable())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`isCacheable`](AndroidBinaryDescriptionArg.html#getIsCacheable()).*
            :::

            [Parameters:]{.paramLabel}
            :   `isCacheable` - The value for isCacheable

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAdditionalAaptParams(java.lang.String)}

        -   #### addAdditionalAaptParams

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder addAdditionalAaptParams​(String element)
            ```

            ::: block
            Adds one element to
            [`additionalAaptParams`](AndroidBinaryDescriptionArg.html#getAdditionalAaptParams())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A additionalAaptParams element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAdditionalAaptParams(java.lang.String...)}

        -   #### addAdditionalAaptParams

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder addAdditionalAaptParams​(String... elements)
            ```

            ::: block
            Adds elements to
            [`additionalAaptParams`](AndroidBinaryDescriptionArg.html#getAdditionalAaptParams())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of additionalAaptParams elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setAdditionalAaptParams(java.lang.Iterable)}

        -   #### setAdditionalAaptParams

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder setAdditionalAaptParams​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`additionalAaptParams`](AndroidBinaryDescriptionArg.html#getAdditionalAaptParams())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of additionalAaptParams
                elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllAdditionalAaptParams(java.lang.Iterable)}

        -   #### addAllAdditionalAaptParams

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder addAllAdditionalAaptParams​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`additionalAaptParams`](AndroidBinaryDescriptionArg.html#getAdditionalAaptParams())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of additionalAaptParams
                elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setAaptMode(com.facebook.buck.android.AaptMode)}

        -   #### setAaptMode

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder setAaptMode​(com.facebook.buck.android.AaptMode aaptMode)
            ```

            ::: block
            Initializes the value for the
            [`aaptMode`](AndroidBinaryDescriptionArg.html#getAaptMode())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`aaptMode`](AndroidBinaryDescriptionArg.html#getAaptMode()).*
            :::

            [Parameters:]{.paramLabel}
            :   `aaptMode` - The value for aaptMode

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setTrimResourceIds(boolean)}

        -   #### setTrimResourceIds

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder setTrimResourceIds​(boolean trimResourceIds)
            ```

            ::: block
            Initializes the value for the
            [`trimResourceIds`](AndroidBinaryDescriptionArg.html#isTrimResourceIds())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`trimResourceIds`](AndroidBinaryDescriptionArg.html#isTrimResourceIds()).*
            :::

            [Parameters:]{.paramLabel}
            :   `trimResourceIds` - The value for trimResourceIds

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setAllowRDotJavaInSecondaryDex(boolean)}

        -   #### setAllowRDotJavaInSecondaryDex

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder setAllowRDotJavaInSecondaryDex​(boolean allowRDotJavaInSecondaryDex)
            ```

            ::: block
            Initializes the value for the
            [`allowRDotJavaInSecondaryDex`](AndroidBinaryDescriptionArg.html#isAllowRDotJavaInSecondaryDex())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`allowRDotJavaInSecondaryDex`](AndroidBinaryDescriptionArg.html#isAllowRDotJavaInSecondaryDex()).*
            :::

            [Parameters:]{.paramLabel}
            :   `allowRDotJavaInSecondaryDex` - The value for
                allowRDotJavaInSecondaryDex

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setKeepResourcePattern(java.lang.String)}

        -   #### setKeepResourcePattern

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder setKeepResourcePattern​(String keepResourcePattern)
            ```

            ::: block
            Initializes the optional value
            [`keepResourcePattern`](AndroidBinaryDescriptionArg.html#getKeepResourcePattern())
            to keepResourcePattern.
            :::

            [Parameters:]{.paramLabel}
            :   `keepResourcePattern` - The value for
                keepResourcePattern

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setKeepResourcePattern(java.util.Optional)}

        -   #### setKeepResourcePattern

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder setKeepResourcePattern​(Optional<String> keepResourcePattern)
            ```

            ::: block
            Initializes the optional value
            [`keepResourcePattern`](AndroidBinaryDescriptionArg.html#getKeepResourcePattern())
            to keepResourcePattern.
            :::

            [Parameters:]{.paramLabel}
            :   `keepResourcePattern` - The value for
                keepResourcePattern

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setResourceUnionPackage(java.lang.String)}

        -   #### setResourceUnionPackage

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder setResourceUnionPackage​(String resourceUnionPackage)
            ```

            ::: block
            Initializes the optional value
            [`resourceUnionPackage`](AndroidBinaryDescriptionArg.html#getResourceUnionPackage())
            to resourceUnionPackage.
            :::

            [Parameters:]{.paramLabel}
            :   `resourceUnionPackage` - The value for
                resourceUnionPackage

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setResourceUnionPackage(java.util.Optional)}

        -   #### setResourceUnionPackage

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder setResourceUnionPackage​(Optional<String> resourceUnionPackage)
            ```

            ::: block
            Initializes the optional value
            [`resourceUnionPackage`](AndroidBinaryDescriptionArg.html#getResourceUnionPackage())
            to resourceUnionPackage.
            :::

            [Parameters:]{.paramLabel}
            :   `resourceUnionPackage` - The value for
                resourceUnionPackage

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLocales(java.lang.String)}

        -   #### addLocales

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder addLocales​(String element)
            ```

            ::: block
            Adds one element to
            [`locales`](AndroidBinaryDescriptionArg.html#getLocales())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A locales element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLocales(java.lang.String...)}

        -   #### addLocales

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder addLocales​(String... elements)
            ```

            ::: block
            Adds elements to
            [`locales`](AndroidBinaryDescriptionArg.html#getLocales())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of locales elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLocales(java.lang.Iterable)}

        -   #### setLocales

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder setLocales​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`locales`](AndroidBinaryDescriptionArg.html#getLocales())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of locales elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLocales(java.lang.Iterable)}

        -   #### addAllLocales

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder addAllLocales​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`locales`](AndroidBinaryDescriptionArg.html#getLocales())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of locales elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setAapt2LocaleFiltering(boolean)}

        -   #### setAapt2LocaleFiltering

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder setAapt2LocaleFiltering​(boolean aapt2LocaleFiltering)
            ```

            ::: block
            Initializes the value for the
            [`aapt2LocaleFiltering`](AndroidBinaryDescriptionArg.html#isAapt2LocaleFiltering())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`aapt2LocaleFiltering`](AndroidBinaryDescriptionArg.html#isAapt2LocaleFiltering()).*
            :::

            [Parameters:]{.paramLabel}
            :   `aapt2LocaleFiltering` - The value for
                aapt2LocaleFiltering

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLocalizedStringFileName(java.lang.String)}

        -   #### setLocalizedStringFileName

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder setLocalizedStringFileName​(String localizedStringFileName)
            ```

            ::: block
            Initializes the optional value
            [`localizedStringFileName`](AndroidBinaryDescriptionArg.html#getLocalizedStringFileName())
            to localizedStringFileName.
            :::

            [Parameters:]{.paramLabel}
            :   `localizedStringFileName` - The value for
                localizedStringFileName

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setLocalizedStringFileName(java.util.Optional)}

        -   #### setLocalizedStringFileName

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder setLocalizedStringFileName​(Optional<String> localizedStringFileName)
            ```

            ::: block
            Initializes the optional value
            [`localizedStringFileName`](AndroidBinaryDescriptionArg.html#getLocalizedStringFileName())
            to localizedStringFileName.
            :::

            [Parameters:]{.paramLabel}
            :   `localizedStringFileName` - The value for
                localizedStringFileName

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setBuildStringSourceMap(boolean)}

        -   #### setBuildStringSourceMap

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder setBuildStringSourceMap​(boolean buildStringSourceMap)
            ```

            ::: block
            Initializes the value for the
            [`buildStringSourceMap`](AndroidBinaryDescriptionArg.html#isBuildStringSourceMap())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`buildStringSourceMap`](AndroidBinaryDescriptionArg.html#isBuildStringSourceMap()).*
            :::

            [Parameters:]{.paramLabel}
            :   `buildStringSourceMap` - The value for
                buildStringSourceMap

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setIgnoreAaptProguardConfig(boolean)}

        -   #### setIgnoreAaptProguardConfig

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder setIgnoreAaptProguardConfig​(boolean ignoreAaptProguardConfig)
            ```

            ::: block
            Initializes the value for the
            [`ignoreAaptProguardConfig`](AndroidBinaryDescriptionArg.html#isIgnoreAaptProguardConfig())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`ignoreAaptProguardConfig`](AndroidBinaryDescriptionArg.html#isIgnoreAaptProguardConfig()).*
            :::

            [Parameters:]{.paramLabel}
            :   `ignoreAaptProguardConfig` - The value for
                ignoreAaptProguardConfig

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCpuFilters(com.facebook.buck.android.toolchain.ndk.TargetCpuType)}

        -   #### addCpuFilters

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder addCpuFilters​(TargetCpuType element)
            ```

            ::: block
            Adds one element to
            [`cpuFilters`](AndroidBinaryDescriptionArg.html#getCpuFilters())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A cpuFilters element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCpuFilters(com.facebook.buck.android.toolchain.ndk.TargetCpuType...)}

        -   #### addCpuFilters

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder addCpuFilters​(TargetCpuType... elements)
            ```

            ::: block
            Adds elements to
            [`cpuFilters`](AndroidBinaryDescriptionArg.html#getCpuFilters())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of cpuFilters elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCpuFilters(java.lang.Iterable)}

        -   #### setCpuFilters

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder setCpuFilters​(Iterable<TargetCpuType> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`cpuFilters`](AndroidBinaryDescriptionArg.html#getCpuFilters())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of cpuFilters elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllCpuFilters(java.lang.Iterable)}

        -   #### addAllCpuFilters

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder addAllCpuFilters​(Iterable<TargetCpuType> elements)
            ```

            ::: block
            Adds elements to
            [`cpuFilters`](AndroidBinaryDescriptionArg.html#getCpuFilters())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of cpuFilters elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPreprocessJavaClassesBash(com.facebook.buck.rules.macros.StringWithMacros)}

        -   #### setPreprocessJavaClassesBash

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder setPreprocessJavaClassesBash​(StringWithMacros preprocessJavaClassesBash)
            ```

            ::: block
            Initializes the optional value
            [`preprocessJavaClassesBash`](AndroidBinaryDescriptionArg.html#getPreprocessJavaClassesBash())
            to preprocessJavaClassesBash.
            :::

            [Parameters:]{.paramLabel}
            :   `preprocessJavaClassesBash` - The value for
                preprocessJavaClassesBash

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setPreprocessJavaClassesBash(java.util.Optional)}

        -   #### setPreprocessJavaClassesBash

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder setPreprocessJavaClassesBash​(Optional<? extends StringWithMacros> preprocessJavaClassesBash)
            ```

            ::: block
            Initializes the optional value
            [`preprocessJavaClassesBash`](AndroidBinaryDescriptionArg.html#getPreprocessJavaClassesBash())
            to preprocessJavaClassesBash.
            :::

            [Parameters:]{.paramLabel}
            :   `preprocessJavaClassesBash` - The value for
                preprocessJavaClassesBash

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setReorderClassesIntraDex(boolean)}

        -   #### setReorderClassesIntraDex

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder setReorderClassesIntraDex​(boolean reorderClassesIntraDex)
            ```

            ::: block
            Initializes the value for the
            [`reorderClassesIntraDex`](AndroidBinaryDescriptionArg.html#isReorderClassesIntraDex())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`reorderClassesIntraDex`](AndroidBinaryDescriptionArg.html#isReorderClassesIntraDex()).*
            :::

            [Parameters:]{.paramLabel}
            :   `reorderClassesIntraDex` - The value for
                reorderClassesIntraDex

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDexTool(java.lang.String)}

        -   #### setDexTool

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder setDexTool​(String dexTool)
            ```

            ::: block
            Initializes the value for the
            [`dexTool`](AndroidBinaryDescriptionArg.html#getDexTool())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`dexTool`](AndroidBinaryDescriptionArg.html#getDexTool()).*
            :::

            [Parameters:]{.paramLabel}
            :   `dexTool` - The value for dexTool

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDexReorderToolFile(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setDexReorderToolFile

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder setDexReorderToolFile​(SourcePath dexReorderToolFile)
            ```

            ::: block
            Initializes the optional value
            [`dexReorderToolFile`](AndroidBinaryDescriptionArg.html#getDexReorderToolFile())
            to dexReorderToolFile.
            :::

            [Parameters:]{.paramLabel}
            :   `dexReorderToolFile` - The value for dexReorderToolFile

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setDexReorderToolFile(java.util.Optional)}

        -   #### setDexReorderToolFile

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder setDexReorderToolFile​(Optional<? extends SourcePath> dexReorderToolFile)
            ```

            ::: block
            Initializes the optional value
            [`dexReorderToolFile`](AndroidBinaryDescriptionArg.html#getDexReorderToolFile())
            to dexReorderToolFile.
            :::

            [Parameters:]{.paramLabel}
            :   `dexReorderToolFile` - The value for dexReorderToolFile

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDexReorderDataDumpFile(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setDexReorderDataDumpFile

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder setDexReorderDataDumpFile​(SourcePath dexReorderDataDumpFile)
            ```

            ::: block
            Initializes the optional value
            [`dexReorderDataDumpFile`](AndroidBinaryDescriptionArg.html#getDexReorderDataDumpFile())
            to dexReorderDataDumpFile.
            :::

            [Parameters:]{.paramLabel}
            :   `dexReorderDataDumpFile` - The value for
                dexReorderDataDumpFile

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setDexReorderDataDumpFile(java.util.Optional)}

        -   #### setDexReorderDataDumpFile

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder setDexReorderDataDumpFile​(Optional<? extends SourcePath> dexReorderDataDumpFile)
            ```

            ::: block
            Initializes the optional value
            [`dexReorderDataDumpFile`](AndroidBinaryDescriptionArg.html#getDexReorderDataDumpFile())
            to dexReorderDataDumpFile.
            :::

            [Parameters:]{.paramLabel}
            :   `dexReorderDataDumpFile` - The value for
                dexReorderDataDumpFile

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putNativeLibraryMergeMap(java.lang.String,java.util.List)}

        -   #### putNativeLibraryMergeMap

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder putNativeLibraryMergeMap​(String key,
                                                                                      List<Pattern> value)
            ```

            ::: block
            Put one entry to the
            [`nativeLibraryMergeMap`](AndroidBinaryDescriptionArg.html#getNativeLibraryMergeMap())
            map.
            :::

            [Parameters:]{.paramLabel}
            :   `key` - The key in the nativeLibraryMergeMap map
            :   `value` - The associated value in the
                nativeLibraryMergeMap map

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putNativeLibraryMergeMap(java.util.Map.Entry)}

        -   #### putNativeLibraryMergeMap

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder putNativeLibraryMergeMap​(Map.Entry<String,​? extends List<Pattern>> entry)
            ```

            ::: block
            Put one entry to the
            [`nativeLibraryMergeMap`](AndroidBinaryDescriptionArg.html#getNativeLibraryMergeMap())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entry` - The key and value entry

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setNativeLibraryMergeMap(java.util.Map)}

        -   #### setNativeLibraryMergeMap

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder setNativeLibraryMergeMap​(Map<String,​? extends List<Pattern>> entries)
            ```

            ::: block
            Sets or replaces all mappings from the specified map as
            entries for the
            [`nativeLibraryMergeMap`](AndroidBinaryDescriptionArg.html#getNativeLibraryMergeMap())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entries` - The entries that will be added to the
                nativeLibraryMergeMap map

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#putAllNativeLibraryMergeMap(java.util.Map)}

        -   #### putAllNativeLibraryMergeMap

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder putAllNativeLibraryMergeMap​(Map<String,​? extends List<Pattern>> entries)
            ```

            ::: block
            Put all mappings from the specified map as entries to
            [`nativeLibraryMergeMap`](AndroidBinaryDescriptionArg.html#getNativeLibraryMergeMap())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entries` - The entries that will be added to the
                nativeLibraryMergeMap map

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setNativeLibraryMergeGlue(com.facebook.buck.core.model.BuildTarget)}

        -   #### setNativeLibraryMergeGlue

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder setNativeLibraryMergeGlue​(BuildTarget nativeLibraryMergeGlue)
            ```

            ::: block
            Initializes the optional value
            [`nativeLibraryMergeGlue`](AndroidBinaryDescriptionArg.html#getNativeLibraryMergeGlue())
            to nativeLibraryMergeGlue.
            :::

            [Parameters:]{.paramLabel}
            :   `nativeLibraryMergeGlue` - The value for
                nativeLibraryMergeGlue

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setNativeLibraryMergeGlue(java.util.Optional)}

        -   #### setNativeLibraryMergeGlue

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder setNativeLibraryMergeGlue​(Optional<? extends BuildTarget> nativeLibraryMergeGlue)
            ```

            ::: block
            Initializes the optional value
            [`nativeLibraryMergeGlue`](AndroidBinaryDescriptionArg.html#getNativeLibraryMergeGlue())
            to nativeLibraryMergeGlue.
            :::

            [Parameters:]{.paramLabel}
            :   `nativeLibraryMergeGlue` - The value for
                nativeLibraryMergeGlue

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setNativeLibraryMergeCodeGenerator(com.facebook.buck.core.model.BuildTarget)}

        -   #### setNativeLibraryMergeCodeGenerator

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder setNativeLibraryMergeCodeGenerator​(BuildTarget nativeLibraryMergeCodeGenerator)
            ```

            ::: block
            Initializes the optional value
            [`nativeLibraryMergeCodeGenerator`](AndroidBinaryDescriptionArg.html#getNativeLibraryMergeCodeGenerator())
            to nativeLibraryMergeCodeGenerator.
            :::

            [Parameters:]{.paramLabel}
            :   `nativeLibraryMergeCodeGenerator` - The value for
                nativeLibraryMergeCodeGenerator

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setNativeLibraryMergeCodeGenerator(java.util.Optional)}

        -   #### setNativeLibraryMergeCodeGenerator

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder setNativeLibraryMergeCodeGenerator​(Optional<? extends BuildTarget> nativeLibraryMergeCodeGenerator)
            ```

            ::: block
            Initializes the optional value
            [`nativeLibraryMergeCodeGenerator`](AndroidBinaryDescriptionArg.html#getNativeLibraryMergeCodeGenerator())
            to nativeLibraryMergeCodeGenerator.
            :::

            [Parameters:]{.paramLabel}
            :   `nativeLibraryMergeCodeGenerator` - The value for
                nativeLibraryMergeCodeGenerator

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setNativeLibraryMergeLocalizedSymbols(com.google.common.collect.ImmutableSortedSet)}

        -   #### setNativeLibraryMergeLocalizedSymbols

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder setNativeLibraryMergeLocalizedSymbols​(com.google.common.collect.ImmutableSortedSet<String> nativeLibraryMergeLocalizedSymbols)
            ```

            ::: block
            Initializes the optional value
            [`nativeLibraryMergeLocalizedSymbols`](AndroidBinaryDescriptionArg.html#getNativeLibraryMergeLocalizedSymbols())
            to nativeLibraryMergeLocalizedSymbols.
            :::

            [Parameters:]{.paramLabel}
            :   `nativeLibraryMergeLocalizedSymbols` - The value for
                nativeLibraryMergeLocalizedSymbols

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setNativeLibraryMergeLocalizedSymbols(java.util.Optional)}

        -   #### setNativeLibraryMergeLocalizedSymbols

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder setNativeLibraryMergeLocalizedSymbols​(Optional<? extends com.google.common.collect.ImmutableSortedSet<String>> nativeLibraryMergeLocalizedSymbols)
            ```

            ::: block
            Initializes the optional value
            [`nativeLibraryMergeLocalizedSymbols`](AndroidBinaryDescriptionArg.html#getNativeLibraryMergeLocalizedSymbols())
            to nativeLibraryMergeLocalizedSymbols.
            :::

            [Parameters:]{.paramLabel}
            :   `nativeLibraryMergeLocalizedSymbols` - The value for
                nativeLibraryMergeLocalizedSymbols

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setNativeLibraryProguardConfigGenerator(com.facebook.buck.core.model.BuildTarget)}

        -   #### setNativeLibraryProguardConfigGenerator

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder setNativeLibraryProguardConfigGenerator​(BuildTarget nativeLibraryProguardConfigGenerator)
            ```

            ::: block
            Initializes the optional value
            [`nativeLibraryProguardConfigGenerator`](AndroidBinaryDescriptionArg.html#getNativeLibraryProguardConfigGenerator())
            to nativeLibraryProguardConfigGenerator.
            :::

            [Parameters:]{.paramLabel}
            :   `nativeLibraryProguardConfigGenerator` - The value for
                nativeLibraryProguardConfigGenerator

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setNativeLibraryProguardConfigGenerator(java.util.Optional)}

        -   #### setNativeLibraryProguardConfigGenerator

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder setNativeLibraryProguardConfigGenerator​(Optional<? extends BuildTarget> nativeLibraryProguardConfigGenerator)
            ```

            ::: block
            Initializes the optional value
            [`nativeLibraryProguardConfigGenerator`](AndroidBinaryDescriptionArg.html#getNativeLibraryProguardConfigGenerator())
            to nativeLibraryProguardConfigGenerator.
            :::

            [Parameters:]{.paramLabel}
            :   `nativeLibraryProguardConfigGenerator` - The value for
                nativeLibraryProguardConfigGenerator

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setEnableRelinker(boolean)}

        -   #### setEnableRelinker

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder setEnableRelinker​(boolean enableRelinker)
            ```

            ::: block
            Initializes the value for the
            [`enableRelinker`](AndroidBinaryDescriptionArg.html#isEnableRelinker())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`enableRelinker`](AndroidBinaryDescriptionArg.html#isEnableRelinker()).*
            :::

            [Parameters:]{.paramLabel}
            :   `enableRelinker` - The value for enableRelinker

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addRelinkerWhitelist(java.util.regex.Pattern)}

        -   #### addRelinkerWhitelist

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder addRelinkerWhitelist​(Pattern element)
            ```

            ::: block
            Adds one element to
            [`relinkerWhitelist`](AndroidBinaryDescriptionArg.html#getRelinkerWhitelist())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A relinkerWhitelist element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addRelinkerWhitelist(java.util.regex.Pattern...)}

        -   #### addRelinkerWhitelist

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder addRelinkerWhitelist​(Pattern... elements)
            ```

            ::: block
            Adds elements to
            [`relinkerWhitelist`](AndroidBinaryDescriptionArg.html#getRelinkerWhitelist())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of relinkerWhitelist elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setRelinkerWhitelist(java.lang.Iterable)}

        -   #### setRelinkerWhitelist

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder setRelinkerWhitelist​(Iterable<? extends Pattern> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`relinkerWhitelist`](AndroidBinaryDescriptionArg.html#getRelinkerWhitelist())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of relinkerWhitelist elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllRelinkerWhitelist(java.lang.Iterable)}

        -   #### addAllRelinkerWhitelist

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder addAllRelinkerWhitelist​(Iterable<? extends Pattern> elements)
            ```

            ::: block
            Adds elements to
            [`relinkerWhitelist`](AndroidBinaryDescriptionArg.html#getRelinkerWhitelist())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of relinkerWhitelist elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setManifestEntries(com.facebook.buck.rules.coercer.ManifestEntries)}

        -   #### setManifestEntries

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder setManifestEntries​(ManifestEntries manifestEntries)
            ```

            ::: block
            Initializes the value for the
            [`manifestEntries`](AndroidBinaryDescriptionArg.html#getManifestEntries())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`manifestEntries`](AndroidBinaryDescriptionArg.html#getManifestEntries()).*
            :::

            [Parameters:]{.paramLabel}
            :   `manifestEntries` - The value for manifestEntries

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setBuildConfigValues(com.facebook.buck.rules.coercer.BuildConfigFields)}

        -   #### setBuildConfigValues

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder setBuildConfigValues​(BuildConfigFields buildConfigValues)
            ```

            ::: block
            Initializes the value for the
            [`buildConfigValues`](AndroidBinaryDescriptionArg.html#getBuildConfigValues())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`buildConfigValues`](AndroidBinaryDescriptionArg.html#getBuildConfigValues()).*
            :::

            [Parameters:]{.paramLabel}
            :   `buildConfigValues` - The value for buildConfigValues

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPostFilterResourcesCmd(com.facebook.buck.rules.macros.StringWithMacros)}

        -   #### setPostFilterResourcesCmd

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder setPostFilterResourcesCmd​(StringWithMacros postFilterResourcesCmd)
            ```

            ::: block
            Initializes the optional value
            [`postFilterResourcesCmd`](AndroidBinaryDescriptionArg.html#getPostFilterResourcesCmd())
            to postFilterResourcesCmd.
            :::

            [Parameters:]{.paramLabel}
            :   `postFilterResourcesCmd` - The value for
                postFilterResourcesCmd

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setPostFilterResourcesCmd(java.util.Optional)}

        -   #### setPostFilterResourcesCmd

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder setPostFilterResourcesCmd​(Optional<? extends StringWithMacros> postFilterResourcesCmd)
            ```

            ::: block
            Initializes the optional value
            [`postFilterResourcesCmd`](AndroidBinaryDescriptionArg.html#getPostFilterResourcesCmd())
            to postFilterResourcesCmd.
            :::

            [Parameters:]{.paramLabel}
            :   `postFilterResourcesCmd` - The value for
                postFilterResourcesCmd

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setBuildConfigValuesFile(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setBuildConfigValuesFile

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder setBuildConfigValuesFile​(SourcePath buildConfigValuesFile)
            ```

            ::: block
            Initializes the optional value
            [`buildConfigValuesFile`](AndroidBinaryDescriptionArg.html#getBuildConfigValuesFile())
            to buildConfigValuesFile.
            :::

            [Parameters:]{.paramLabel}
            :   `buildConfigValuesFile` - The value for
                buildConfigValuesFile

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setBuildConfigValuesFile(java.util.Optional)}

        -   #### setBuildConfigValuesFile

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder setBuildConfigValuesFile​(Optional<? extends SourcePath> buildConfigValuesFile)
            ```

            ::: block
            Initializes the optional value
            [`buildConfigValuesFile`](AndroidBinaryDescriptionArg.html#getBuildConfigValuesFile())
            to buildConfigValuesFile.
            :::

            [Parameters:]{.paramLabel}
            :   `buildConfigValuesFile` - The value for
                buildConfigValuesFile

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setSkipProguard(boolean)}

        -   #### setSkipProguard

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder setSkipProguard​(boolean skipProguard)
            ```

            ::: block
            Initializes the value for the
            [`skipProguard`](AndroidBinaryDescriptionArg.html#isSkipProguard())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`skipProguard`](AndroidBinaryDescriptionArg.html#isSkipProguard()).*
            :::

            [Parameters:]{.paramLabel}
            :   `skipProguard` - The value for skipProguard

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setUseDynamicFeature(boolean)}

        -   #### setUseDynamicFeature

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder setUseDynamicFeature​(boolean useDynamicFeature)
            ```

            ::: block
            Initializes the value for the
            [`useDynamicFeature`](AndroidBinaryDescriptionArg.html#getUseDynamicFeature())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`useDynamicFeature`](AndroidBinaryDescriptionArg.html#getUseDynamicFeature()).*
            :::

            [Parameters:]{.paramLabel}
            :   `useDynamicFeature` - The value for useDynamicFeature

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addExtraFilteredResources(java.lang.String)}

        -   #### addExtraFilteredResources

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder addExtraFilteredResources​(String element)
            ```

            ::: block
            Adds one element to
            [`extraFilteredResources`](AndroidBinaryDescriptionArg.html#getExtraFilteredResources())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A extraFilteredResources element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addExtraFilteredResources(java.lang.String...)}

        -   #### addExtraFilteredResources

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder addExtraFilteredResources​(String... elements)
            ```

            ::: block
            Adds elements to
            [`extraFilteredResources`](AndroidBinaryDescriptionArg.html#getExtraFilteredResources())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of extraFilteredResources elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setExtraFilteredResources(java.lang.Iterable)}

        -   #### setExtraFilteredResources

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder setExtraFilteredResources​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`extraFilteredResources`](AndroidBinaryDescriptionArg.html#getExtraFilteredResources())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of extraFilteredResources
                elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllExtraFilteredResources(java.lang.Iterable)}

        -   #### addAllExtraFilteredResources

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder addAllExtraFilteredResources​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`extraFilteredResources`](AndroidBinaryDescriptionArg.html#getExtraFilteredResources())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of extraFilteredResources
                elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDuplicateResourceBehavior(com.facebook.buck.android.HasDuplicateAndroidResourceTypes.DuplicateResourceBehaviour)}

        -   #### setDuplicateResourceBehavior

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder setDuplicateResourceBehavior​(HasDuplicateAndroidResourceTypes.DuplicateResourceBehaviour duplicateResourceBehavior)
            ```

            ::: block
            Initializes the value for the
            [`duplicateResourceBehavior`](AndroidBinaryDescriptionArg.html#getDuplicateResourceBehavior())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`duplicateResourceBehavior`](AndroidBinaryDescriptionArg.html#getDuplicateResourceBehavior()).*
            :::

            [Parameters:]{.paramLabel}
            :   `duplicateResourceBehavior` - The value for
                duplicateResourceBehavior

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllowedDuplicateResourceTypes(com.facebook.buck.android.aapt.RDotTxtEntry.RType)}

        -   #### addAllowedDuplicateResourceTypes

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder addAllowedDuplicateResourceTypes​(RDotTxtEntry.RType element)
            ```

            ::: block
            Adds one element to
            [`allowedDuplicateResourceTypes`](AndroidBinaryDescriptionArg.html#getAllowedDuplicateResourceTypes())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A allowedDuplicateResourceTypes element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllowedDuplicateResourceTypes(com.facebook.buck.android.aapt.RDotTxtEntry.RType...)}

        -   #### addAllowedDuplicateResourceTypes

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder addAllowedDuplicateResourceTypes​(RDotTxtEntry.RType... elements)
            ```

            ::: block
            Adds elements to
            [`allowedDuplicateResourceTypes`](AndroidBinaryDescriptionArg.html#getAllowedDuplicateResourceTypes())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of allowedDuplicateResourceTypes
                elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setAllowedDuplicateResourceTypes(java.lang.Iterable)}

        -   #### setAllowedDuplicateResourceTypes

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder setAllowedDuplicateResourceTypes​(Iterable<RDotTxtEntry.RType> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`allowedDuplicateResourceTypes`](AndroidBinaryDescriptionArg.html#getAllowedDuplicateResourceTypes())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of
                allowedDuplicateResourceTypes elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllAllowedDuplicateResourceTypes(java.lang.Iterable)}

        -   #### addAllAllowedDuplicateResourceTypes

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder addAllAllowedDuplicateResourceTypes​(Iterable<RDotTxtEntry.RType> elements)
            ```

            ::: block
            Adds elements to
            [`allowedDuplicateResourceTypes`](AndroidBinaryDescriptionArg.html#getAllowedDuplicateResourceTypes())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of
                allowedDuplicateResourceTypes elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addBannedDuplicateResourceTypes(com.facebook.buck.android.aapt.RDotTxtEntry.RType)}

        -   #### addBannedDuplicateResourceTypes

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder addBannedDuplicateResourceTypes​(RDotTxtEntry.RType element)
            ```

            ::: block
            Adds one element to
            [`bannedDuplicateResourceTypes`](AndroidBinaryDescriptionArg.html#getBannedDuplicateResourceTypes())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A bannedDuplicateResourceTypes element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addBannedDuplicateResourceTypes(com.facebook.buck.android.aapt.RDotTxtEntry.RType...)}

        -   #### addBannedDuplicateResourceTypes

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder addBannedDuplicateResourceTypes​(RDotTxtEntry.RType... elements)
            ```

            ::: block
            Adds elements to
            [`bannedDuplicateResourceTypes`](AndroidBinaryDescriptionArg.html#getBannedDuplicateResourceTypes())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of bannedDuplicateResourceTypes
                elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setBannedDuplicateResourceTypes(java.lang.Iterable)}

        -   #### setBannedDuplicateResourceTypes

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder setBannedDuplicateResourceTypes​(Iterable<RDotTxtEntry.RType> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`bannedDuplicateResourceTypes`](AndroidBinaryDescriptionArg.html#getBannedDuplicateResourceTypes())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of bannedDuplicateResourceTypes
                elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllBannedDuplicateResourceTypes(java.lang.Iterable)}

        -   #### addAllBannedDuplicateResourceTypes

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder addAllBannedDuplicateResourceTypes​(Iterable<RDotTxtEntry.RType> elements)
            ```

            ::: block
            Adds elements to
            [`bannedDuplicateResourceTypes`](AndroidBinaryDescriptionArg.html#getBannedDuplicateResourceTypes())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of bannedDuplicateResourceTypes
                elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDuplicateResourceWhitelist(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setDuplicateResourceWhitelist

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder setDuplicateResourceWhitelist​(SourcePath duplicateResourceWhitelist)
            ```

            ::: block
            Initializes the optional value
            [`duplicateResourceWhitelist`](AndroidBinaryDescriptionArg.html#getDuplicateResourceWhitelist())
            to duplicateResourceWhitelist.
            :::

            [Parameters:]{.paramLabel}
            :   `duplicateResourceWhitelist` - The value for
                duplicateResourceWhitelist

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setDuplicateResourceWhitelist(java.util.Optional)}

        -   #### setDuplicateResourceWhitelist

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder setDuplicateResourceWhitelist​(Optional<? extends SourcePath> duplicateResourceWhitelist)
            ```

            ::: block
            Initializes the optional value
            [`duplicateResourceWhitelist`](AndroidBinaryDescriptionArg.html#getDuplicateResourceWhitelist())
            to duplicateResourceWhitelist.
            :::

            [Parameters:]{.paramLabel}
            :   `duplicateResourceWhitelist` - The value for
                duplicateResourceWhitelist

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setApplicationModuleBlacklist(java.util.List)}

        -   #### setApplicationModuleBlacklist

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder setApplicationModuleBlacklist​(List<Query> applicationModuleBlacklist)
            ```

            ::: block
            Initializes the optional value
            [`applicationModuleBlacklist`](AndroidBinaryDescriptionArg.html#getApplicationModuleBlacklist())
            to applicationModuleBlacklist.
            :::

            [Parameters:]{.paramLabel}
            :   `applicationModuleBlacklist` - The value for
                applicationModuleBlacklist

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setApplicationModuleBlacklist(java.util.Optional)}

        -   #### setApplicationModuleBlacklist

            ``` methodSignature
            public final AndroidBinaryDescriptionArg.Builder setApplicationModuleBlacklist​(Optional<? extends List<Query>> applicationModuleBlacklist)
            ```

            ::: block
            Initializes the optional value
            [`applicationModuleBlacklist`](AndroidBinaryDescriptionArg.html#getApplicationModuleBlacklist())
            to applicationModuleBlacklist.
            :::

            [Parameters:]{.paramLabel}
            :   `applicationModuleBlacklist` - The value for
                applicationModuleBlacklist

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#build()}

        -   #### build

            ``` methodSignature
            public AndroidBinaryDescriptionArg build()
            ```

            ::: block
            Builds a new
            [`AndroidBinaryDescriptionArg`](AndroidBinaryDescriptionArg.html "class in com.facebook.buck.android").
            :::

            [Returns:]{.returnLabel}
            :   An immutable instance of AndroidBinaryDescriptionArg

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
