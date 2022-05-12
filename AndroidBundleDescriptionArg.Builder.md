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

## Class AndroidBundleDescriptionArg.Builder {#class-androidbundledescriptionarg.builder .title title="Class AndroidBundleDescriptionArg.Builder"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.android.AndroidBundleDescriptionArg.Builder

::: description
-   

    Enclosing class:
    :   [AndroidBundleDescriptionArg](AndroidBundleDescriptionArg.html "class in com.facebook.buck.android")

    ------------------------------------------------------------------------

        @NotThreadSafe
        public static final class AndroidBundleDescriptionArg.Builder
        extends Object

    ::: block
    Builds instances of type
    [`AndroidBundleDescriptionArg`](AndroidBundleDescriptionArg.html "class in com.facebook.buck.android").
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
        | `AndroidBundleDe      | `addAdditionalAaptPa  | ::: block             |
        | scriptionArg.Builder` | rams​(String element)` | Adds one element to   |
        |                       |                       | [`additionalAaptParam |
        |                       |                       | s`](AndroidBundleDesc |
        |                       |                       | riptionArg.html#getAd |
        |                       |                       | ditionalAaptParams()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `ad                   | ::: block             |
        | scriptionArg.Builder` | dAdditionalAaptParams | Adds elements to      |
        |                       | ​(String... elements)` | [`additionalAaptParam |
        |                       |                       | s`](AndroidBundleDesc |
        |                       |                       | riptionArg.html#getAd |
        |                       |                       | ditionalAaptParams()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `addAllAdditi         | ::: block             |
        | scriptionArg.Builder` | onalAaptParams​(Iterab | Adds elements to      |
        |                       | le<String> elements)` | [`additionalAaptParam |
        |                       |                       | s`](AndroidBundleDesc |
        |                       |                       | riptionArg.html#getAd |
        |                       |                       | ditionalAaptParams()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `addAllAllowe         | ::: block             |
        | scriptionArg.Builder` | dDuplicateResourceTyp | Adds elements to      |
        |                       | es​(Iterable<RDotTxtEn | [`allowedDuplicate    |
        |                       | try.RType> elements)` | ResourceTypes`](Andro |
        |                       |                       | idBundleDescriptionAr |
        |                       |                       | g.html#getAllowedDupl |
        |                       |                       | icateResourceTypes()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `a                    | ::: block             |
        | scriptionArg.Builder` | ddAllApplicationModul | Adds elements to      |
        |                       | esWithManifest​(Iterab | [`applicationModules  |
        |                       | le<String> elements)` | WithManifest`](Androi |
        |                       |                       | dBundleDescriptionArg |
        |                       |                       | .html#getApplicationM |
        |                       |                       | odulesWithManifest()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `ad                   | ::: block             |
        | scriptionArg.Builder` | dAllApplicationModule | Adds elements to      |
        |                       | sWithResources​(Iterab | [                     |
        |                       | le<String> elements)` | `applicationModulesWi |
        |                       |                       | thResources`](Android |
        |                       |                       | BundleDescriptionArg. |
        |                       |                       | html#getApplicationMo |
        |                       |                       | dulesWithResources()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `addAllAppl           | ::: block             |
        | scriptionArg.Builder` | icationModuleTargets​( | Adds elements to      |
        |                       | Iterable<? extends Bu | [`applic              |
        |                       | ildTarget> elements)` | ationModuleTargets`]( |
        |                       |                       | AndroidBundleDescript |
        |                       |                       | ionArg.html#getApplic |
        |                       |                       | ationModuleTargets()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `addAllBanne          | ::: block             |
        | scriptionArg.Builder` | dDuplicateResourceTyp | Adds elements to      |
        |                       | es​(Iterable<RDotTxtEn | [`bannedDuplicat      |
        |                       | try.RType> elements)` | eResourceTypes`](Andr |
        |                       |                       | oidBundleDescriptionA |
        |                       |                       | rg.html#getBannedDupl |
        |                       |                       | icateResourceTypes()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `addAllCompat         | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Iterable<? e | Adds elements to      |
        |                       | xtends UnconfiguredBu | [`compati             |
        |                       | ildTarget> elements)` | bleWith`](AndroidBund |
        |                       |                       | leDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `addAllCpu            | ::: block             |
        | scriptionArg.Builder` | Filters​(Iterable<Targ | Adds elements to      |
        |                       | etCpuType> elements)` | [                     |
        |                       |                       | `cpuFilters`](Android |
        |                       |                       | BundleDescriptionArg. |
        |                       |                       | html#getCpuFilters()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `addAllDeps​(          | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Adds elements to      |
        |                       | ildTarget> elements)` | [`deps`](A            |
        |                       |                       | ndroidBundleDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `addAllExopackag      | ::: block             |
        | scriptionArg.Builder` | eModes​(Iterable<Exopa | Adds elements to      |
        |                       | ckageMode> elements)` | [`exopackag           |
        |                       |                       | eModes`](AndroidBundl |
        |                       |                       | eDescriptionArg.html# |
        |                       |                       | getExopackageModes()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `addAllExtraFil       | ::: block             |
        | scriptionArg.Builder` | teredResources​(Iterab | Adds elements to      |
        |                       | le<String> elements)` | [`ex                  |
        |                       |                       | traFilteredResources` |
        |                       |                       | ](AndroidBundleDescri |
        |                       |                       | ptionArg.html#getExtr |
        |                       |                       | aFilteredResources()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `addAllLabels​(Iterab  | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Adds elements to      |
        |                       |                       | [`labels`](And        |
        |                       |                       | roidBundleDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `addAllLicenses       | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Adds elements to      |
        |                       | ourcePath> elements)` | [`licenses`](Andro    |
        |                       |                       | idBundleDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `addAllLocales​(Iterab | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Adds elements to      |
        |                       |                       | [`locales`](Andr      |
        |                       |                       | oidBundleDescriptionA |
        |                       |                       | rg.html#getLocales()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `addAllNoDx​(          | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Adds elements to      |
        |                       | ildTarget> elements)` | [`noDx`](A            |
        |                       |                       | ndroidBundleDescripti |
        |                       |                       | onArg.html#getNoDx()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `addAllowedDuplicate  | ::: block             |
        | scriptionArg.Builder` | ResourceTypes​(RDotTxt | Adds one element to   |
        |                       | Entry.RType element)` | [`allowedDuplicate    |
        |                       |                       | ResourceTypes`](Andro |
        |                       |                       | idBundleDescriptionAr |
        |                       |                       | g.html#getAllowedDupl |
        |                       |                       | icateResourceTypes()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `ad                   | ::: block             |
        | scriptionArg.Builder` | dAllowedDuplicateReso | Adds elements to      |
        |                       | urceTypes​(RDotTxtEntr | [`allowedDuplicate    |
        |                       | y.RType... elements)` | ResourceTypes`](Andro |
        |                       |                       | idBundleDescriptionAr |
        |                       |                       | g.html#getAllowedDupl |
        |                       |                       | icateResourceTypes()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `addAllPrepr          | ::: block             |
        | scriptionArg.Builder` | ocessJavaClassesDeps​( | Adds elements to      |
        |                       | Iterable<? extends Bu | [`preproce            |
        |                       | ildTarget> elements)` | ssJavaClassesDeps`](A |
        |                       |                       | ndroidBundleDescripti |
        |                       |                       | onArg.html#getPreproc |
        |                       |                       | essJavaClassesDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `addAllPrim           | ::: block             |
        | scriptionArg.Builder` | aryDexPatterns​(Iterab | Adds elements to      |
        |                       | le<String> elements)` | [`primaryDexPatte     |
        |                       |                       | rns`](AndroidBundleDe |
        |                       |                       | scriptionArg.html#get |
        |                       |                       | PrimaryDexPatterns()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `addAllP              | ::: block             |
        | scriptionArg.Builder` | roguardJvmArgs​(Iterab | Adds elements to      |
        |                       | le<String> elements)` | [`proguardJ           |
        |                       |                       | vmArgs`](AndroidBundl |
        |                       |                       | eDescriptionArg.html# |
        |                       |                       | getProguardJvmArgs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `addAl                | ::: block             |
        | scriptionArg.Builder` | lRedexExtraArgs​(Itera | Adds elements to      |
        |                       | ble<? extends StringW | [`redexEx             |
        |                       | ithMacros> elements)` | traArgs`](AndroidBund |
        |                       |                       | leDescriptionArg.html |
        |                       |                       | #getRedexExtraArgs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `addAllRelinkerWhitel | ::: block             |
        | scriptionArg.Builder` | ist​(Iterable<? extend | Adds elements to      |
        |                       | s Pattern> elements)` | [`relinkerWhite       |
        |                       |                       | list`](AndroidBundleD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tRelinkerWhitelist()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `addAll               | ::: block             |
        | scriptionArg.Builder` | ResourceFilter​(Iterab | Adds elements to      |
        |                       | le<String> elements)` | [`resourc             |
        |                       |                       | eFilter`](AndroidBund |
        |                       |                       | leDescriptionArg.html |
        |                       |                       | #getResourceFilter()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `addAllTests​(         | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Adds elements to      |
        |                       | ildTarget> elements)` | [`tests`](An          |
        |                       |                       | droidBundleDescriptio |
        |                       |                       | nArg.html#getTests()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `addAppli             | ::: block             |
        | scriptionArg.Builder` | cationModulesWithMani | Adds one element to   |
        |                       | fest​(String element)` | [`applicationModules  |
        |                       |                       | WithManifest`](Androi |
        |                       |                       | dBundleDescriptionArg |
        |                       |                       | .html#getApplicationM |
        |                       |                       | odulesWithManifest()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `addApplicati         | ::: block             |
        | scriptionArg.Builder` | onModulesWithManifest | Adds elements to      |
        |                       | ​(String... elements)` | [`applicationModules  |
        |                       |                       | WithManifest`](Androi |
        |                       |                       | dBundleDescriptionArg |
        |                       |                       | .html#getApplicationM |
        |                       |                       | odulesWithManifest()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `addApplic            | ::: block             |
        | scriptionArg.Builder` | ationModulesWithResou | Adds one element to   |
        |                       | rces​(String element)` | [                     |
        |                       |                       | `applicationModulesWi |
        |                       |                       | thResources`](Android |
        |                       |                       | BundleDescriptionArg. |
        |                       |                       | html#getApplicationMo |
        |                       |                       | dulesWithResources()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `addApplicatio        | ::: block             |
        | scriptionArg.Builder` | nModulesWithResources | Adds elements to      |
        |                       | ​(String... elements)` | [                     |
        |                       |                       | `applicationModulesWi |
        |                       |                       | thResources`](Android |
        |                       |                       | BundleDescriptionArg. |
        |                       |                       | html#getApplicationMo |
        |                       |                       | dulesWithResources()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `addAppl              | ::: block             |
        | scriptionArg.Builder` | icationModuleTargets​( | Adds one element to   |
        |                       | BuildTarget element)` | [`applic              |
        |                       |                       | ationModuleTargets`]( |
        |                       |                       | AndroidBundleDescript |
        |                       |                       | ionArg.html#getApplic |
        |                       |                       | ationModuleTargets()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `addApplicat          | ::: block             |
        | scriptionArg.Builder` | ionModuleTargets​(Buil | Adds elements to      |
        |                       | dTarget... elements)` | [`applic              |
        |                       |                       | ationModuleTargets`]( |
        |                       |                       | AndroidBundleDescript |
        |                       |                       | ionArg.html#getApplic |
        |                       |                       | ationModuleTargets()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `addBannedDuplicate   | ::: block             |
        | scriptionArg.Builder` | ResourceTypes​(RDotTxt | Adds one element to   |
        |                       | Entry.RType element)` | [`bannedDuplicat      |
        |                       |                       | eResourceTypes`](Andr |
        |                       |                       | oidBundleDescriptionA |
        |                       |                       | rg.html#getBannedDupl |
        |                       |                       | icateResourceTypes()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `a                    | ::: block             |
        | scriptionArg.Builder` | ddBannedDuplicateReso | Adds elements to      |
        |                       | urceTypes​(RDotTxtEntr | [`bannedDuplicat      |
        |                       | y.RType... elements)` | eResourceTypes`](Andr |
        |                       |                       | oidBundleDescriptionA |
        |                       |                       | rg.html#getBannedDupl |
        |                       |                       | icateResourceTypes()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `addCompat            | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Unconfigured | Adds one element to   |
        |                       | BuildTarget element)` | [`compati             |
        |                       |                       | bleWith`](AndroidBund |
        |                       |                       | leDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `addCompatible        | ::: block             |
        | scriptionArg.Builder` | With​(UnconfiguredBuil | Adds elements to      |
        |                       | dTarget... elements)` | [`compati             |
        |                       |                       | bleWith`](AndroidBund |
        |                       |                       | leDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `addCpuFilters​(Ta     | ::: block             |
        | scriptionArg.Builder` | rgetCpuType element)` | Adds one element to   |
        |                       |                       | [                     |
        |                       |                       | `cpuFilters`](Android |
        |                       |                       | BundleDescriptionArg. |
        |                       |                       | html#getCpuFilters()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `addCpuFilters​(Target | ::: block             |
        | scriptionArg.Builder` | CpuType... elements)` | Adds elements to      |
        |                       |                       | [                     |
        |                       |                       | `cpuFilters`](Android |
        |                       |                       | BundleDescriptionArg. |
        |                       |                       | html#getCpuFilters()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `addDeps​(             | ::: block             |
        | scriptionArg.Builder` | BuildTarget element)` | Adds one element to   |
        |                       |                       | [`deps`](A            |
        |                       |                       | ndroidBundleDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `addDeps​(Buil         | ::: block             |
        | scriptionArg.Builder` | dTarget... elements)` | Adds elements to      |
        |                       |                       | [`deps`](A            |
        |                       |                       | ndroidBundleDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `a                    | ::: block             |
        | scriptionArg.Builder` | ddExopackageModes​(Exo | Adds one element to   |
        |                       | packageMode element)` | [`exopackag           |
        |                       |                       | eModes`](AndroidBundl |
        |                       |                       | eDescriptionArg.html# |
        |                       |                       | getExopackageModes()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `addEx                | ::: block             |
        | scriptionArg.Builder` | opackageModes​(Exopack | Adds elements to      |
        |                       | ageMode... elements)` | [`exopackag           |
        |                       |                       | eModes`](AndroidBundl |
        |                       |                       | eDescriptionArg.html# |
        |                       |                       | getExopackageModes()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `                     | ::: block             |
        | scriptionArg.Builder` | addExtraFilteredResou | Adds one element to   |
        |                       | rces​(String element)` | [`ex                  |
        |                       |                       | traFilteredResources` |
        |                       |                       | ](AndroidBundleDescri |
        |                       |                       | ptionArg.html#getExtr |
        |                       |                       | aFilteredResources()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `addE                 | ::: block             |
        | scriptionArg.Builder` | xtraFilteredResources | Adds elements to      |
        |                       | ​(String... elements)` | [`ex                  |
        |                       |                       | traFilteredResources` |
        |                       |                       | ](AndroidBundleDescri |
        |                       |                       | ptionArg.html#getExtr |
        |                       |                       | aFilteredResources()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `addLa                | ::: block             |
        | scriptionArg.Builder` | bels​(String element)` | Adds one element to   |
        |                       |                       | [`labels`](And        |
        |                       |                       | roidBundleDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `addLabels            | ::: block             |
        | scriptionArg.Builder` | ​(String... elements)` | Adds elements to      |
        |                       |                       | [`labels`](And        |
        |                       |                       | roidBundleDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `addLicenses          | ::: block             |
        | scriptionArg.Builder` | ​(SourcePath element)` | Adds one element to   |
        |                       |                       | [`licenses`](Andro    |
        |                       |                       | idBundleDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `addLicenses​(Sou      | ::: block             |
        | scriptionArg.Builder` | rcePath... elements)` | Adds elements to      |
        |                       |                       | [`licenses`](Andro    |
        |                       |                       | idBundleDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `addLoc               | ::: block             |
        | scriptionArg.Builder` | ales​(String element)` | Adds one element to   |
        |                       |                       | [`locales`](Andr      |
        |                       |                       | oidBundleDescriptionA |
        |                       |                       | rg.html#getLocales()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `addLocales           | ::: block             |
        | scriptionArg.Builder` | ​(String... elements)` | Adds elements to      |
        |                       |                       | [`locales`](Andr      |
        |                       |                       | oidBundleDescriptionA |
        |                       |                       | rg.html#getLocales()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `addNoDx​(             | ::: block             |
        | scriptionArg.Builder` | BuildTarget element)` | Adds one element to   |
        |                       |                       | [`noDx`](A            |
        |                       |                       | ndroidBundleDescripti |
        |                       |                       | onArg.html#getNoDx()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `addNoDx​(Buil         | ::: block             |
        | scriptionArg.Builder` | dTarget... elements)` | Adds elements to      |
        |                       |                       | [`noDx`](A            |
        |                       |                       | ndroidBundleDescripti |
        |                       |                       | onArg.html#getNoDx()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `addPrepr             | ::: block             |
        | scriptionArg.Builder` | ocessJavaClassesDeps​( | Adds one element to   |
        |                       | BuildTarget element)` | [`preproce            |
        |                       |                       | ssJavaClassesDeps`](A |
        |                       |                       | ndroidBundleDescripti |
        |                       |                       | onArg.html#getPreproc |
        |                       |                       | essJavaClassesDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `addPreproces         | ::: block             |
        | scriptionArg.Builder` | sJavaClassesDeps​(Buil | Adds elements to      |
        |                       | dTarget... elements)` | [`preproce            |
        |                       |                       | ssJavaClassesDeps`](A |
        |                       |                       | ndroidBundleDescripti |
        |                       |                       | onArg.html#getPreproc |
        |                       |                       | essJavaClassesDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `addPrimaryDexPatt    | ::: block             |
        | scriptionArg.Builder` | erns​(String element)` | Adds one element to   |
        |                       |                       | [`primaryDexPatte     |
        |                       |                       | rns`](AndroidBundleDe |
        |                       |                       | scriptionArg.html#get |
        |                       |                       | PrimaryDexPatterns()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `                     | ::: block             |
        | scriptionArg.Builder` | addPrimaryDexPatterns | Adds elements to      |
        |                       | ​(String... elements)` | [`primaryDexPatte     |
        |                       |                       | rns`](AndroidBundleDe |
        |                       |                       | scriptionArg.html#get |
        |                       |                       | PrimaryDexPatterns()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `addProguardJvm       | ::: block             |
        | scriptionArg.Builder` | Args​(String element)` | Adds one element to   |
        |                       |                       | [`proguardJ           |
        |                       |                       | vmArgs`](AndroidBundl |
        |                       |                       | eDescriptionArg.html# |
        |                       |                       | getProguardJvmArgs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `addProguardJvmArgs   | ::: block             |
        | scriptionArg.Builder` | ​(String... elements)` | Adds elements to      |
        |                       |                       | [`proguardJ           |
        |                       |                       | vmArgs`](AndroidBundl |
        |                       |                       | eDescriptionArg.html# |
        |                       |                       | getProguardJvmArgs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `ad                   | ::: block             |
        | scriptionArg.Builder` | dRedexExtraArgs​(Strin | Adds one element to   |
        |                       | gWithMacros element)` | [`redexEx             |
        |                       |                       | traArgs`](AndroidBund |
        |                       |                       | leDescriptionArg.html |
        |                       |                       | #getRedexExtraArgs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `addRed               | ::: block             |
        | scriptionArg.Builder` | exExtraArgs​(StringWit | Adds elements to      |
        |                       | hMacros... elements)` | [`redexEx             |
        |                       |                       | traArgs`](AndroidBund |
        |                       |                       | leDescriptionArg.html |
        |                       |                       | #getRedexExtraArgs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `addRelinkerWhitel    | ::: block             |
        | scriptionArg.Builder` | ist​(Pattern element)` | Adds one element to   |
        |                       |                       | [`relinkerWhite       |
        |                       |                       | list`](AndroidBundleD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tRelinkerWhitelist()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `                     | ::: block             |
        | scriptionArg.Builder` | addRelinkerWhitelist​( | Adds elements to      |
        |                       | Pattern... elements)` | [`relinkerWhite       |
        |                       |                       | list`](AndroidBundleD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tRelinkerWhitelist()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `addResourceFi        | ::: block             |
        | scriptionArg.Builder` | lter​(String element)` | Adds one element to   |
        |                       |                       | [`resourc             |
        |                       |                       | eFilter`](AndroidBund |
        |                       |                       | leDescriptionArg.html |
        |                       |                       | #getResourceFilter()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `addResourceFilter    | ::: block             |
        | scriptionArg.Builder` | ​(String... elements)` | Adds elements to      |
        |                       |                       | [`resourc             |
        |                       |                       | eFilter`](AndroidBund |
        |                       |                       | leDescriptionArg.html |
        |                       |                       | #getResourceFilter()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `addTests​(            | ::: block             |
        | scriptionArg.Builder` | BuildTarget element)` | Adds one element to   |
        |                       |                       | [`tests`](An          |
        |                       |                       | droidBundleDescriptio |
        |                       |                       | nArg.html#getTests()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `addTests​(Buil        | ::: block             |
        | scriptionArg.Builder` | dTarget... elements)` | Adds elements to      |
        |                       |                       | [`tests`](An          |
        |                       |                       | droidBundleDescriptio |
        |                       |                       | nArg.html#getTests()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `Android              | `build()`             | ::: block             |
        | BundleDescriptionArg` |                       | Builds a new          |
        |                       |                       | [`AndroidBundleDesc   |
        |                       |                       | riptionArg`](AndroidB |
        |                       |                       | undleDescriptionArg.h |
        |                       |                       | tml "class in com.fac |
        |                       |                       | ebook.buck.android"). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `from​(com.facebook.   | ::: block             |
        | scriptionArg.Builder` | buck.android.AndroidB | Copy abstract value   |
        |                       | undleDescription.Abst | type                  |
        |                       | ractAndroidBundleDesc | `AbstractAndroid      |
        |                       | riptionArg instance)` | BundleDescriptionArg` |
        |                       |                       | instance into         |
        |                       |                       | builder.              |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `f                    | ::: block             |
        | scriptionArg.Builder` | rom​(AndroidBundleDesc | Fill a builder with   |
        |                       | riptionArg instance)` | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `Android              |
        |                       |                       | BundleDescriptionArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `from​(AndroidGraphEn  | ::: block             |
        | scriptionArg.Builder` | hancerArgs instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.faceb            |
        |                       |                       | ook.buck.android.Andr |
        |                       |                       | oidGraphEnhancerArgs` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `from​(H               | ::: block             |
        | scriptionArg.Builder` | asDuplicateAndroidRes | Fill a builder with   |
        |                       | ourceTypes instance)` | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook.buck    |
        |                       |                       | .android.HasDuplicate |
        |                       |                       | AndroidResourceTypes` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `from​(HasExop         | ::: block             |
        | scriptionArg.Builder` | ackageArgs instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `co                   |
        |                       |                       | m.facebook.buck.andro |
        |                       |                       | id.HasExopackageArgs` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `from​(Bu              | ::: block             |
        | scriptionArg.Builder` | ildRuleArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebo           |
        |                       |                       | ok.buck.core.descript |
        |                       |                       | ion.arg.BuildRuleArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `from​(Cons            | ::: block             |
        | scriptionArg.Builder` | tructorArg instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook         |
        |                       |                       | .buck.core.descriptio |
        |                       |                       | n.arg.ConstructorArg` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `fro                  | ::: block             |
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
        | `AndroidBundleDe      | `from​(HasDe           | ::: block             |
        | scriptionArg.Builder` | claredDeps instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.facebook.        |
        |                       |                       | buck.core.description |
        |                       |                       | .arg.HasDeclaredDeps` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `fro                  | ::: block             |
        | scriptionArg.Builder` | m​(HasTests instance)` | Fill a builder with   |
        |                       |                       | attribute values from |
        |                       |                       | the provided          |
        |                       |                       | `com.fa               |
        |                       |                       | cebook.buck.core.desc |
        |                       |                       | ription.arg.HasTests` |
        |                       |                       | instance.             |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `putAllAppl           | ::: block             |
        | scriptionArg.Builder` | icationModuleConfigs​( | Put all mappings from |
        |                       | Map<String,​? extends  | the specified map as  |
        |                       | com.google.common.col | entries to            |
        |                       | lect.ImmutableList<Bu | [`applic              |
        |                       | ildTarget>> entries)` | ationModuleConfigs`]( |
        |                       |                       | AndroidBundleDescript |
        |                       |                       | ionArg.html#getApplic |
        |                       |                       | ationModuleConfigs()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `putAllNati           | ::: block             |
        | scriptionArg.Builder` | veLibraryMergeMap​(Map | Put all mappings from |
        |                       | <String,​? extends Lis | the specified map as  |
        |                       | t<Pattern>> entries)` | entries to            |
        |                       |                       | [`                    |
        |                       |                       | nativeLibraryMergeMap |
        |                       |                       | `](AndroidBundleDescr |
        |                       |                       | iptionArg.html#getNat |
        |                       |                       | iveLibraryMergeMap()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `p                    | ::: block             |
        | scriptionArg.Builder` | utApplicationModuleCo | Put one entry to the  |
        |                       | nfigs​(String key,     | [`applic              |
        |                       |                       | ationModuleConfigs`]( |
        |                       |    com.google.common. | AndroidBundleDescript |
        |                       | collect.ImmutableList | ionArg.html#getApplic |
        |                       | <BuildTarget> value)` | ationModuleConfigs()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `putApplicat          | ::: block             |
        | scriptionArg.Builder` | ionModuleConfigs​(Map. | Put one entry to the  |
        |                       | Entry<String,​? extend | [`applic              |
        |                       | s com.google.common.c | ationModuleConfigs`]( |
        |                       | ollect.ImmutableList< | AndroidBundleDescript |
        |                       | BuildTarget>> entry)` | ionArg.html#getApplic |
        |                       |                       | ationModuleConfigs()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `putNativeLibraryMer  | ::: block             |
        | scriptionArg.Builder` | geMap​(String key,     | Put one entry to the  |
        |                       |                       | [`                    |
        |                       | List<Pattern> value)` | nativeLibraryMergeMap |
        |                       |                       | `](AndroidBundleDescr |
        |                       |                       | iptionArg.html#getNat |
        |                       |                       | iveLibraryMergeMap()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `putNativeLi          | ::: block             |
        | scriptionArg.Builder` | braryMergeMap​(Map.Ent | Put one entry to the  |
        |                       | ry<String,​? extends L | [`                    |
        |                       | ist<Pattern>> entry)` | nativeLibraryMergeMap |
        |                       |                       | `](AndroidBundleDescr |
        |                       |                       | iptionArg.html#getNat |
        |                       |                       | iveLibraryMergeMap()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `setAapt2Loca         | ::: block             |
        | scriptionArg.Builder` | leFiltering​(boolean a | Initializes the value |
        |                       | apt2LocaleFiltering)` | for the               |
        |                       |                       | [`aapt2LocaleFilteri  |
        |                       |                       | ng`](AndroidBundleDes |
        |                       |                       | criptionArg.html#isAa |
        |                       |                       | pt2LocaleFiltering()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `setAaptMode​(com      | ::: block             |
        | scriptionArg.Builder` | .facebook.buck.androi | Initializes the value |
        |                       | d.AaptMode aaptMode)` | for the               |
        |                       |                       | [`aaptMode`](Andro    |
        |                       |                       | idBundleDescriptionAr |
        |                       |                       | g.html#getAaptMode()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `setAdditi            | ::: block             |
        | scriptionArg.Builder` | onalAaptParams​(Iterab | Sets or replaces all  |
        |                       | le<String> elements)` | elements for          |
        |                       |                       | [`additionalAaptParam |
        |                       |                       | s`](AndroidBundleDesc |
        |                       |                       | riptionArg.html#getAd |
        |                       |                       | ditionalAaptParams()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `setAllowe            | ::: block             |
        | scriptionArg.Builder` | dDuplicateResourceTyp | Sets or replaces all  |
        |                       | es​(Iterable<RDotTxtEn | elements for          |
        |                       | try.RType> elements)` | [`allowedDuplicate    |
        |                       |                       | ResourceTypes`](Andro |
        |                       |                       | idBundleDescriptionAr |
        |                       |                       | g.html#getAllowedDupl |
        |                       |                       | icateResourceTypes()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `setAl                | ::: block             |
        | scriptionArg.Builder` | lowRDotJavaInSecondar | Initializes the value |
        |                       | yDex​(boolean allowRDo | for the               |
        |                       | tJavaInSecondaryDex)` | [`allowRDotJa         |
        |                       |                       | vaInSecondaryDex`](An |
        |                       |                       | droidBundleDescriptio |
        |                       |                       | nArg.html#isAllowRDot |
        |                       |                       | JavaInSecondaryDex()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `setAnd               | ::: block             |
        | scriptionArg.Builder` | roidAppModularityResu | Initializes the       |
        |                       | lt​(SourcePath android | optional value        |
        |                       | AppModularityResult)` | [`androidApp          |
        |                       |                       | ModularityResult`](An |
        |                       |                       | droidBundleDescriptio |
        |                       |                       | nArg.html#getAndroidA |
        |                       |                       | ppModularityResult()) |
        |                       |                       | to                    |
        |                       |                       | androi                |
        |                       |                       | dAppModularityResult. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `setAn                | ::: block             |
        | scriptionArg.Builder` | droidAppModularityRes | Initializes the       |
        |                       | ult​(Optional<? extend | optional value        |
        |                       | s SourcePath> android | [`androidApp          |
        |                       | AppModularityResult)` | ModularityResult`](An |
        |                       |                       | droidBundleDescriptio |
        |                       |                       | nArg.html#getAndroidA |
        |                       |                       | ppModularityResult()) |
        |                       |                       | to                    |
        |                       |                       | androi                |
        |                       |                       | dAppModularityResult. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `setAndroidSdk        | ::: block             |
        | scriptionArg.Builder` | ProguardConfig​(com.fa | Initializes the       |
        |                       | cebook.buck.android.P | optional value        |
        |                       | roGuardObfuscateStep. | [`androi              |
        |                       | SdkProguardType andro | dSdkProguardConfig`]( |
        |                       | idSdkProguardConfig)` | AndroidBundleDescript |
        |                       |                       | ionArg.html#getAndroi |
        |                       |                       | dSdkProguardConfig()) |
        |                       |                       | to                    |
        |                       |                       | andr                  |
        |                       |                       | oidSdkProguardConfig. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `setAndroidSd         | ::: block             |
        | scriptionArg.Builder` | kProguardConfig​(Optio | Initializes the       |
        |                       | nal<? extends com.fac | optional value        |
        |                       | ebook.buck.android.Pr | [`androi              |
        |                       | oGuardObfuscateStep.S | dSdkProguardConfig`]( |
        |                       | dkProguardType> andro | AndroidBundleDescript |
        |                       | idSdkProguardConfig)` | ionArg.html#getAndroi |
        |                       |                       | dSdkProguardConfig()) |
        |                       |                       | to                    |
        |                       |                       | andr                  |
        |                       |                       | oidSdkProguardConfig. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `setAppl              | ::: block             |
        | scriptionArg.Builder` | icationModuleBlacklis | Initializes the       |
        |                       | t​(List<Query> applica | optional value        |
        |                       | tionModuleBlacklist)` | [`applicatio          |
        |                       |                       | nModuleBlacklist`](An |
        |                       |                       | droidBundleDescriptio |
        |                       |                       | nArg.html#getApplicat |
        |                       |                       | ionModuleBlacklist()) |
        |                       |                       | to                    |
        |                       |                       | applic                |
        |                       |                       | ationModuleBlacklist. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `setApp               | ::: block             |
        | scriptionArg.Builder` | licationModuleBlackli | Initializes the       |
        |                       | st​(Optional<? extends | optional value        |
        |                       |  List<Query>> applica | [`applicatio          |
        |                       | tionModuleBlacklist)` | nModuleBlacklist`](An |
        |                       |                       | droidBundleDescriptio |
        |                       |                       | nArg.html#getApplicat |
        |                       |                       | ionModuleBlacklist()) |
        |                       |                       | to                    |
        |                       |                       | applic                |
        |                       |                       | ationModuleBlacklist. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `setAppl              | ::: block             |
        | scriptionArg.Builder` | icationModuleConfigs​( | Sets or replaces all  |
        |                       | Map<String,​? extends  | mappings from the     |
        |                       | com.google.common.col | specified map as      |
        |                       | lect.ImmutableList<Bu | entries for the       |
        |                       | ildTarget>> entries)` | [`applic              |
        |                       |                       | ationModuleConfigs`]( |
        |                       |                       | AndroidBundleDescript |
        |                       |                       | ionArg.html#getApplic |
        |                       |                       | ationModuleConfigs()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `setApplicati         | ::: block             |
        | scriptionArg.Builder` | onModuleDependencies​( | Initializes the       |
        |                       | com.google.common.col | optional value        |
        |                       | lect.ImmutableMap<Str | [`applicationModul    |
        |                       | ing,​com.google.common | eDependencies`](Andro |
        |                       | .collect.ImmutableLis | idBundleDescriptionAr |
        |                       | t<String>> applicatio | g.html#getApplication |
        |                       | nModuleDependencies)` | ModuleDependencies()) |
        |                       |                       | to                    |
        |                       |                       | applicati             |
        |                       |                       | onModuleDependencies. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `setApplicat          | ::: block             |
        | scriptionArg.Builder` | ionModuleDependencies | Initializes the       |
        |                       | ​(Optional<? extends c | optional value        |
        |                       | om.google.common.coll | [`applicationModul    |
        |                       | ect.ImmutableMap<Stri | eDependencies`](Andro |
        |                       | ng,​com.google.common. | idBundleDescriptionAr |
        |                       | collect.ImmutableList | g.html#getApplication |
        |                       | <String>>> applicatio | ModuleDependencies()) |
        |                       | nModuleDependencies)` | to                    |
        |                       |                       | applicati             |
        |                       |                       | onModuleDependencies. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `setApplicationModul  | ::: block             |
        | scriptionArg.Builder` | esWithManifest​(Iterab | Sets or replaces all  |
        |                       | le<String> elements)` | elements for          |
        |                       |                       | [`applicationModules  |
        |                       |                       | WithManifest`](Androi |
        |                       |                       | dBundleDescriptionArg |
        |                       |                       | .html#getApplicationM |
        |                       |                       | odulesWithManifest()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `setApplicationModule | ::: block             |
        | scriptionArg.Builder` | sWithResources​(Iterab | Sets or replaces all  |
        |                       | le<String> elements)` | elements for          |
        |                       |                       | [                     |
        |                       |                       | `applicationModulesWi |
        |                       |                       | thResources`](Android |
        |                       |                       | BundleDescriptionArg. |
        |                       |                       | html#getApplicationMo |
        |                       |                       | dulesWithResources()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `setAppl              | ::: block             |
        | scriptionArg.Builder` | icationModuleTargets​( | Sets or replaces all  |
        |                       | Iterable<? extends Bu | elements for          |
        |                       | ildTarget> elements)` | [`applic              |
        |                       |                       | ationModuleTargets`]( |
        |                       |                       | AndroidBundleDescript |
        |                       |                       | ionArg.html#getApplic |
        |                       |                       | ationModuleTargets()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `setAssetCompre       | ::: block             |
        | scriptionArg.Builder` | ssionAlgorithm​(Compre | Initializes the       |
        |                       | ssionAlgorithm assetC | optional value        |
        |                       | ompressionAlgorithm)` | [`assetCom            |
        |                       |                       | pressionAlgorithm`](A |
        |                       |                       | ndroidBundleDescripti |
        |                       |                       | onArg.html#getAssetCo |
        |                       |                       | mpressionAlgorithm()) |
        |                       |                       | to                    |
        |                       |                       | asset                 |
        |                       |                       | CompressionAlgorithm. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `setAssetCompr        | ::: block             |
        | scriptionArg.Builder` | essionAlgorithm​(Optio | Initializes the       |
        |                       | nal<? extends Compres | optional value        |
        |                       | sionAlgorithm> assetC | [`assetCom            |
        |                       | ompressionAlgorithm)` | pressionAlgorithm`](A |
        |                       |                       | ndroidBundleDescripti |
        |                       |                       | onArg.html#getAssetCo |
        |                       |                       | mpressionAlgorithm()) |
        |                       |                       | to                    |
        |                       |                       | asset                 |
        |                       |                       | CompressionAlgorithm. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `setBanne             | ::: block             |
        | scriptionArg.Builder` | dDuplicateResourceTyp | Sets or replaces all  |
        |                       | es​(Iterable<RDotTxtEn | elements for          |
        |                       | try.RType> elements)` | [`bannedDuplicat      |
        |                       |                       | eResourceTypes`](Andr |
        |                       |                       | oidBundleDescriptionA |
        |                       |                       | rg.html#getBannedDupl |
        |                       |                       | icateResourceTypes()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `setBuildConfigVa     | ::: block             |
        | scriptionArg.Builder` | lues​(BuildConfigField | Initializes the value |
        |                       | s buildConfigValues)` | for the               |
        |                       |                       | [`buildConfigVa       |
        |                       |                       | lues`](AndroidBundleD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tBuildConfigValues()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `setBuildConfigVal    | ::: block             |
        | scriptionArg.Builder` | uesFile​(SourcePath bu | Initializes the       |
        |                       | ildConfigValuesFile)` | optional value        |
        |                       |                       | [`                    |
        |                       |                       | buildConfigValuesFile |
        |                       |                       | `](AndroidBundleDescr |
        |                       |                       | iptionArg.html#getBui |
        |                       |                       | ldConfigValuesFile()) |
        |                       |                       | to                    |
        |                       |                       | b                     |
        |                       |                       | uildConfigValuesFile. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `setBuildConfigVa     | ::: block             |
        | scriptionArg.Builder` | luesFile​(Optional<? e | Initializes the       |
        |                       | xtends SourcePath> bu | optional value        |
        |                       | ildConfigValuesFile)` | [`                    |
        |                       |                       | buildConfigValuesFile |
        |                       |                       | `](AndroidBundleDescr |
        |                       |                       | iptionArg.html#getBui |
        |                       |                       | ldConfigValuesFile()) |
        |                       |                       | to                    |
        |                       |                       | b                     |
        |                       |                       | uildConfigValuesFile. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `setBuildStri         | ::: block             |
        | scriptionArg.Builder` | ngSourceMap​(boolean b | Initializes the value |
        |                       | uildStringSourceMap)` | for the               |
        |                       |                       | [`buildStringSourceM  |
        |                       |                       | ap`](AndroidBundleDes |
        |                       |                       | criptionArg.html#isBu |
        |                       |                       | ildStringSourceMap()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `setBund              | ::: block             |
        | scriptionArg.Builder` | leConfigFile​(SourcePa | Initializes the       |
        |                       | th bundleConfigFile)` | optional value        |
        |                       |                       | [`bundleConfi         |
        |                       |                       | gFile`](AndroidBundle |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etBundleConfigFile()) |
        |                       |                       | to bundleConfigFile.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `setBun               | ::: block             |
        | scriptionArg.Builder` | dleConfigFile​(Optiona | Initializes the       |
        |                       | l<? extends SourcePat | optional value        |
        |                       | h> bundleConfigFile)` | [`bundleConfi         |
        |                       |                       | gFile`](AndroidBundle |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etBundleConfigFile()) |
        |                       |                       | to bundleConfigFile.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `setCompat            | ::: block             |
        | scriptionArg.Builder` | ibleWith​(Iterable<? e | Sets or replaces all  |
        |                       | xtends UnconfiguredBu | elements for          |
        |                       | ildTarget> elements)` | [`compati             |
        |                       |                       | bleWith`](AndroidBund |
        |                       |                       | leDescriptionArg.html |
        |                       |                       | #getCompatibleWith()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `setCompressAsset     | ::: block             |
        | scriptionArg.Builder` | Libraries​(boolean com | Initializes the value |
        |                       | pressAssetLibraries)` | for the               |
        |                       |                       | [`c                   |
        |                       |                       | ompressAssetLibraries |
        |                       |                       | `](AndroidBundleDescr |
        |                       |                       | iptionArg.html#isComp |
        |                       |                       | ressAssetLibraries()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `setCpu               | ::: block             |
        | scriptionArg.Builder` | Filters​(Iterable<Targ | Sets or replaces all  |
        |                       | etCpuType> elements)` | elements for          |
        |                       |                       | [                     |
        |                       |                       | `cpuFilters`](Android |
        |                       |                       | BundleDescriptionArg. |
        |                       |                       | html#getCpuFilters()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `setDefaul            | ::: block             |
        | scriptionArg.Builder` | tTargetPlatform​(Uncon | Initializes the       |
        |                       | figuredBuildTarget de | optional value        |
        |                       | faultTargetPlatform)` | [`                    |
        |                       |                       | defaultTargetPlatform |
        |                       |                       | `](AndroidBundleDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `setDefau             | ::: block             |
        | scriptionArg.Builder` | ltTargetPlatform​(Opti | Initializes the       |
        |                       | onal<? extends Unconf | optional value        |
        |                       | iguredBuildTarget> de | [`                    |
        |                       | faultTargetPlatform)` | defaultTargetPlatform |
        |                       |                       | `](AndroidBundleDescr |
        |                       |                       | iptionArg.html#getDef |
        |                       |                       | aultTargetPlatform()) |
        |                       |                       | to                    |
        |                       |                       | d                     |
        |                       |                       | efaultTargetPlatform. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `setDeps​(             | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Sets or replaces all  |
        |                       | ildTarget> elements)` | elements for          |
        |                       |                       | [`deps`](A            |
        |                       |                       | ndroidBundleDescripti |
        |                       |                       | onArg.html#getDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `setDex               | ::: block             |
        | scriptionArg.Builder` | Compression​(com.faceb | Initializes the       |
        |                       | ook.buck.android.DexS | optional value        |
        |                       | tore dexCompression)` | [`dexComp             |
        |                       |                       | ression`](AndroidBund |
        |                       |                       | leDescriptionArg.html |
        |                       |                       | #getDexCompression()) |
        |                       |                       | to dexCompression.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `setDe                | ::: block             |
        | scriptionArg.Builder` | xCompression​(Optional | Initializes the       |
        |                       | <? extends com.facebo | optional value        |
        |                       | ok.buck.android.DexSt | [`dexComp             |
        |                       | ore> dexCompression)` | ression`](AndroidBund |
        |                       |                       | leDescriptionArg.html |
        |                       |                       | #getDexCompression()) |
        |                       |                       | to dexCompression.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `                     | ::: block             |
        | scriptionArg.Builder` | setDexGroupLibLimit​(i | Initializes the value |
        |                       | nt dexGroupLibLimit)` | for the               |
        |                       |                       | [`dexGroupLib         |
        |                       |                       | Limit`](AndroidBundle |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etDexGroupLibLimit()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `setDexReorderDataDu  | ::: block             |
        | scriptionArg.Builder` | mpFile​(SourcePath dex | Initializes the       |
        |                       | ReorderDataDumpFile)` | optional value        |
        |                       |                       | [`de                  |
        |                       |                       | xReorderDataDumpFile` |
        |                       |                       | ](AndroidBundleDescri |
        |                       |                       | ptionArg.html#getDexR |
        |                       |                       | eorderDataDumpFile()) |
        |                       |                       | to                    |
        |                       |                       | de                    |
        |                       |                       | xReorderDataDumpFile. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `setDexReorderDataD   | ::: block             |
        | scriptionArg.Builder` | umpFile​(Optional<? ex | Initializes the       |
        |                       | tends SourcePath> dex | optional value        |
        |                       | ReorderDataDumpFile)` | [`de                  |
        |                       |                       | xReorderDataDumpFile` |
        |                       |                       | ](AndroidBundleDescri |
        |                       |                       | ptionArg.html#getDexR |
        |                       |                       | eorderDataDumpFile()) |
        |                       |                       | to                    |
        |                       |                       | de                    |
        |                       |                       | xReorderDataDumpFile. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `setDexReord          | ::: block             |
        | scriptionArg.Builder` | erToolFile​(SourcePath | Initializes the       |
        |                       |  dexReorderToolFile)` | optional value        |
        |                       |                       | [`dexReorderToolF     |
        |                       |                       | ile`](AndroidBundleDe |
        |                       |                       | scriptionArg.html#get |
        |                       |                       | DexReorderToolFile()) |
        |                       |                       | to                    |
        |                       |                       | dexReorderToolFile.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `setDexReor           | ::: block             |
        | scriptionArg.Builder` | derToolFile​(Optional< | Initializes the       |
        |                       | ? extends SourcePath> | optional value        |
        |                       |  dexReorderToolFile)` | [`dexReorderToolF     |
        |                       |                       | ile`](AndroidBundleDe |
        |                       |                       | scriptionArg.html#get |
        |                       |                       | DexReorderToolFile()) |
        |                       |                       | to                    |
        |                       |                       | dexReorderToolFile.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `setDex               | ::: block             |
        | scriptionArg.Builder` | Tool​(String dexTool)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`dexTool`](Andr      |
        |                       |                       | oidBundleDescriptionA |
        |                       |                       | rg.html#getDexTool()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `setDisablePreDex​(bo  | ::: block             |
        | scriptionArg.Builder` | olean disablePreDex)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`disab               |
        |                       |                       | lePreDex`](AndroidBun |
        |                       |                       | dleDescriptionArg.htm |
        |                       |                       | l#getDisablePreDex()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `setDuplicat          | ::: block             |
        | scriptionArg.Builder` | eResourceBehavior​(Has | Initializes the value |
        |                       | DuplicateAndroidResou | for the               |
        |                       | rceTypes.DuplicateRes | [`duplicat            |
        |                       | ourceBehaviour duplic | eResourceBehavior`](A |
        |                       | ateResourceBehavior)` | ndroidBundleDescripti |
        |                       |                       | onArg.html#getDuplica |
        |                       |                       | teResourceBehavior()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `setDup               | ::: block             |
        | scriptionArg.Builder` | licateResourceWhiteli | Initializes the       |
        |                       | st​(SourcePath duplica | optional value        |
        |                       | teResourceWhitelist)` | [`duplicateR          |
        |                       |                       | esourceWhitelist`](An |
        |                       |                       | droidBundleDescriptio |
        |                       |                       | nArg.html#getDuplicat |
        |                       |                       | eResourceWhitelist()) |
        |                       |                       | to                    |
        |                       |                       | duplic                |
        |                       |                       | ateResourceWhitelist. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `setDu                | ::: block             |
        | scriptionArg.Builder` | plicateResourceWhitel | Initializes the       |
        |                       | ist​(Optional<? extend | optional value        |
        |                       | s SourcePath> duplica | [`duplicateR          |
        |                       | teResourceWhitelist)` | esourceWhitelist`](An |
        |                       |                       | droidBundleDescriptio |
        |                       |                       | nArg.html#getDuplicat |
        |                       |                       | eResourceWhitelist()) |
        |                       |                       | to                    |
        |                       |                       | duplic                |
        |                       |                       | ateResourceWhitelist. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `                     | ::: block             |
        | scriptionArg.Builder` | setEnableRelinker​(boo | Initializes the value |
        |                       | lean enableRelinker)` | for the               |
        |                       |                       | [`enable              |
        |                       |                       | Relinker`](AndroidBun |
        |                       |                       | dleDescriptionArg.htm |
        |                       |                       | l#isEnableRelinker()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `setExopackage        | ::: block             |
        | scriptionArg.Builder` | ​(boolean exopackage)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`exopackage`](Androi |
        |                       |                       | dBundleDescriptionArg |
        |                       |                       | .html#isExopackage()) |
        |                       |                       | to exopackage.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `se                   | ::: block             |
        | scriptionArg.Builder` | tExopackage​(Optional< | Initializes the       |
        |                       | Boolean> exopackage)` | optional value        |
        |                       |                       | [`exopackage`](Androi |
        |                       |                       | dBundleDescriptionArg |
        |                       |                       | .html#isExopackage()) |
        |                       |                       | to exopackage.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `setExopackag         | ::: block             |
        | scriptionArg.Builder` | eModes​(Iterable<Exopa | Sets or replaces all  |
        |                       | ckageMode> elements)` | elements for          |
        |                       |                       | [`exopackag           |
        |                       |                       | eModes`](AndroidBundl |
        |                       |                       | eDescriptionArg.html# |
        |                       |                       | getExopackageModes()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `setExtraFil          | ::: block             |
        | scriptionArg.Builder` | teredResources​(Iterab | Sets or replaces all  |
        |                       | le<String> elements)` | elements for          |
        |                       |                       | [`ex                  |
        |                       |                       | traFilteredResources` |
        |                       |                       | ](AndroidBundleDescri |
        |                       |                       | ptionArg.html#getExtr |
        |                       |                       | aFilteredResources()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `setIgnoreAaptProguar | ::: block             |
        | scriptionArg.Builder` | dConfig​(boolean ignor | Initializes the value |
        |                       | eAaptProguardConfig)` | for the               |
        |                       |                       | [`ignor               |
        |                       |                       | eAaptProguardConfig`] |
        |                       |                       | (AndroidBundleDescrip |
        |                       |                       | tionArg.html#isIgnore |
        |                       |                       | AaptProguardConfig()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `setIncludesVectorD   | ::: block             |
        | scriptionArg.Builder` | rawables​(boolean incl | Initializes the value |
        |                       | udesVectorDrawables)` | for the               |
        |                       |                       | [`inc                 |
        |                       |                       | ludesVectorDrawables` |
        |                       |                       | ](AndroidBundleDescri |
        |                       |                       | ptionArg.html#isInclu |
        |                       |                       | desVectorDrawables()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `setIsCacheable​(      | ::: block             |
        | scriptionArg.Builder` | boolean isCacheable)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`i                   |
        |                       |                       | sCacheable`](AndroidB |
        |                       |                       | undleDescriptionArg.h |
        |                       |                       | tml#getIsCacheable()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `setKeepRe            | ::: block             |
        | scriptionArg.Builder` | sourcePattern​(String  | Initializes the       |
        |                       | keepResourcePattern)` | optional value        |
        |                       |                       | [`keepResourcePatte   |
        |                       |                       | rn`](AndroidBundleDes |
        |                       |                       | criptionArg.html#getK |
        |                       |                       | eepResourcePattern()) |
        |                       |                       | to                    |
        |                       |                       | keepResourcePattern.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `setKeepResourcePatt  | ::: block             |
        | scriptionArg.Builder` | ern​(Optional<String>  | Initializes the       |
        |                       | keepResourcePattern)` | optional value        |
        |                       |                       | [`keepResourcePatte   |
        |                       |                       | rn`](AndroidBundleDes |
        |                       |                       | criptionArg.html#getK |
        |                       |                       | eepResourcePattern()) |
        |                       |                       | to                    |
        |                       |                       | keepResourcePattern.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `setKeystore​(B        | ::: block             |
        | scriptionArg.Builder` | uildTarget keystore)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`keystore`](Andro    |
        |                       |                       | idBundleDescriptionAr |
        |                       |                       | g.html#getKeystore()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `setLabels​(Iterab     | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Sets or replaces all  |
        |                       |                       | elements for          |
        |                       |                       | [`labels`](And        |
        |                       |                       | roidBundleDescription |
        |                       |                       | Arg.html#getLabels()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `setLicenses          | ::: block             |
        | scriptionArg.Builder` | ​(Iterable<? extends S | Sets or replaces all  |
        |                       | ourcePath> elements)` | elements for          |
        |                       |                       | [`licenses`](Andro    |
        |                       |                       | idBundleDescriptionAr |
        |                       |                       | g.html#getLicenses()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `setLinear            | ::: block             |
        | scriptionArg.Builder` | AllocHardLimit​(long l | Initializes the value |
        |                       | inearAllocHardLimit)` | for the               |
        |                       |                       | [`linearAllocHardLimi |
        |                       |                       | t`](AndroidBundleDesc |
        |                       |                       | riptionArg.html#getLi |
        |                       |                       | nearAllocHardLimit()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `setLocales​(Iterab    | ::: block             |
        | scriptionArg.Builder` | le<String> elements)` | Sets or replaces all  |
        |                       |                       | elements for          |
        |                       |                       | [`locales`](Andr      |
        |                       |                       | oidBundleDescriptionA |
        |                       |                       | rg.html#getLocales()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `setLocalizedStrin    | ::: block             |
        | scriptionArg.Builder` | gFileName​(String loca | Initializes the       |
        |                       | lizedStringFileName)` | optional value        |
        |                       |                       | [`loca                |
        |                       |                       | lizedStringFileName`] |
        |                       |                       | (AndroidBundleDescrip |
        |                       |                       | tionArg.html#getLocal |
        |                       |                       | izedStringFileName()) |
        |                       |                       | to                    |
        |                       |                       | loc                   |
        |                       |                       | alizedStringFileName. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `setLoc               | ::: block             |
        | scriptionArg.Builder` | alizedStringFileName​( | Initializes the       |
        |                       | Optional<String> loca | optional value        |
        |                       | lizedStringFileName)` | [`loca                |
        |                       |                       | lizedStringFileName`] |
        |                       |                       | (AndroidBundleDescrip |
        |                       |                       | tionArg.html#getLocal |
        |                       |                       | izedStringFileName()) |
        |                       |                       | to                    |
        |                       |                       | loc                   |
        |                       |                       | alizedStringFileName. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `setManifest​(         | ::: block             |
        | scriptionArg.Builder` | SourcePath manifest)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`manifest`](Andro    |
        |                       |                       | idBundleDescriptionAr |
        |                       |                       | g.html#getManifest()) |
        |                       |                       | to manifest.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `setManifest          | ::: block             |
        | scriptionArg.Builder` | ​(Optional<? extends S | Initializes the       |
        |                       | ourcePath> manifest)` | optional value        |
        |                       |                       | [`manifest`](Andro    |
        |                       |                       | idBundleDescriptionAr |
        |                       |                       | g.html#getManifest()) |
        |                       |                       | to manifest.          |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `setManifes           | ::: block             |
        | scriptionArg.Builder` | tEntries​(ManifestEntr | Initializes the value |
        |                       | ies manifestEntries)` | for the               |
        |                       |                       | [`manifestE           |
        |                       |                       | ntries`](AndroidBundl |
        |                       |                       | eDescriptionArg.html# |
        |                       |                       | getManifestEntries()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `setMani              | ::: block             |
        | scriptionArg.Builder` | festSkeleton​(SourcePa | Initializes the       |
        |                       | th manifestSkeleton)` | optional value        |
        |                       |                       | [`manifestSke         |
        |                       |                       | leton`](AndroidBundle |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etManifestSkeleton()) |
        |                       |                       | to manifestSkeleton.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `setMan               | ::: block             |
        | scriptionArg.Builder` | ifestSkeleton​(Optiona | Initializes the       |
        |                       | l<? extends SourcePat | optional value        |
        |                       | h> manifestSkeleton)` | [`manifestSke         |
        |                       |                       | leton`](AndroidBundle |
        |                       |                       | DescriptionArg.html#g |
        |                       |                       | etManifestSkeleton()) |
        |                       |                       | to manifestSkeleton.  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `setMinimizePrima     | ::: block             |
        | scriptionArg.Builder` | ryDexSize​(boolean min | Initializes the value |
        |                       | imizePrimaryDexSize)` | for the               |
        |                       |                       | [`mi                  |
        |                       |                       | nimizePrimaryDexSize` |
        |                       |                       | ](AndroidBundleDescri |
        |                       |                       | ptionArg.html#getMini |
        |                       |                       | mizePrimaryDexSize()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `setModuleManifestSk  | ::: block             |
        | scriptionArg.Builder` | eleton​(SourcePath mod | Initializes the       |
        |                       | uleManifestSkeleton)` | optional value        |
        |                       |                       | [`mo                  |
        |                       |                       | duleManifestSkeleton` |
        |                       |                       | ](AndroidBundleDescri |
        |                       |                       | ptionArg.html#getModu |
        |                       |                       | leManifestSkeleton()) |
        |                       |                       | to                    |
        |                       |                       | mo                    |
        |                       |                       | duleManifestSkeleton. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `setModuleManifestS   | ::: block             |
        | scriptionArg.Builder` | keleton​(Optional<? ex | Initializes the       |
        |                       | tends SourcePath> mod | optional value        |
        |                       | uleManifestSkeleton)` | [`mo                  |
        |                       |                       | duleManifestSkeleton` |
        |                       |                       | ](AndroidBundleDescri |
        |                       |                       | ptionArg.html#getModu |
        |                       |                       | leManifestSkeleton()) |
        |                       |                       | to                    |
        |                       |                       | mo                    |
        |                       |                       | duleManifestSkeleton. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `                     | ::: block             |
        | scriptionArg.Builder` | setName​(String name)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`name`](A            |
        |                       |                       | ndroidBundleDescripti |
        |                       |                       | onArg.html#getName()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `setNativeLibraryM    | ::: block             |
        | scriptionArg.Builder` | ergeCodeGenerator​(Bui | Initializes the       |
        |                       | ldTarget nativeLibrar | optional value        |
        |                       | yMergeCodeGenerator)` | [                     |
        |                       |                       | `nativeLibraryMergeCo |
        |                       |                       | deGenerator`](Android |
        |                       |                       | BundleDescriptionArg. |
        |                       |                       | html#getNativeLibrary |
        |                       |                       | MergeCodeGenerator()) |
        |                       |                       | to                    |
        |                       |                       | nativeLibra           |
        |                       |                       | ryMergeCodeGenerator. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `setNativeLibrary     | ::: block             |
        | scriptionArg.Builder` | MergeCodeGenerator​(Op | Initializes the       |
        |                       | tional<? extends Buil | optional value        |
        |                       | dTarget> nativeLibrar | [                     |
        |                       | yMergeCodeGenerator)` | `nativeLibraryMergeCo |
        |                       |                       | deGenerator`](Android |
        |                       |                       | BundleDescriptionArg. |
        |                       |                       | html#getNativeLibrary |
        |                       |                       | MergeCodeGenerator()) |
        |                       |                       | to                    |
        |                       |                       | nativeLibra           |
        |                       |                       | ryMergeCodeGenerator. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `setNativeLibraryMerg | ::: block             |
        | scriptionArg.Builder` | eGlue​(BuildTarget nat | Initializes the       |
        |                       | iveLibraryMergeGlue)` | optional value        |
        |                       |                       | [`na                  |
        |                       |                       | tiveLibraryMergeGlue` |
        |                       |                       | ](AndroidBundleDescri |
        |                       |                       | ptionArg.html#getNati |
        |                       |                       | veLibraryMergeGlue()) |
        |                       |                       | to                    |
        |                       |                       | na                    |
        |                       |                       | tiveLibraryMergeGlue. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `setNativeLibraryMer  | ::: block             |
        | scriptionArg.Builder` | geGlue​(Optional<? ext | Initializes the       |
        |                       | ends BuildTarget> nat | optional value        |
        |                       | iveLibraryMergeGlue)` | [`na                  |
        |                       |                       | tiveLibraryMergeGlue` |
        |                       |                       | ](AndroidBundleDescri |
        |                       |                       | ptionArg.html#getNati |
        |                       |                       | veLibraryMergeGlue()) |
        |                       |                       | to                    |
        |                       |                       | na                    |
        |                       |                       | tiveLibraryMergeGlue. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `s                    | ::: block             |
        | scriptionArg.Builder` | etNativeLibraryMergeL | Initializes the       |
        |                       | ocalizedSymbols​(com.g | optional value        |
        |                       | oogle.common.collect. | [`nativ               |
        |                       | ImmutableSortedSet<St | eLibraryMergeLocalize |
        |                       | ring> nativeLibraryMe | dSymbols`](AndroidBun |
        |                       | rgeLocalizedSymbols)` | dleDescriptionArg.htm |
        |                       |                       | l#getNativeLibraryMer |
        |                       |                       | geLocalizedSymbols()) |
        |                       |                       | to                    |
        |                       |                       | nativeLibraryM        |
        |                       |                       | ergeLocalizedSymbols. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `                     | ::: block             |
        | scriptionArg.Builder` | setNativeLibraryMerge | Initializes the       |
        |                       | LocalizedSymbols​(Opti | optional value        |
        |                       | onal<? extends com.go | [`nativ               |
        |                       | ogle.common.collect.I | eLibraryMergeLocalize |
        |                       | mmutableSortedSet<Str | dSymbols`](AndroidBun |
        |                       | ing>> nativeLibraryMe | dleDescriptionArg.htm |
        |                       | rgeLocalizedSymbols)` | l#getNativeLibraryMer |
        |                       |                       | geLocalizedSymbols()) |
        |                       |                       | to                    |
        |                       |                       | nativeLibraryM        |
        |                       |                       | ergeLocalizedSymbols. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `setNati              | ::: block             |
        | scriptionArg.Builder` | veLibraryMergeMap​(Map | Sets or replaces all  |
        |                       | <String,​? extends Lis | mappings from the     |
        |                       | t<Pattern>> entries)` | specified map as      |
        |                       |                       | entries for the       |
        |                       |                       | [`                    |
        |                       |                       | nativeLibraryMergeMap |
        |                       |                       | `](AndroidBundleDescr |
        |                       |                       | iptionArg.html#getNat |
        |                       |                       | iveLibraryMergeMap()) |
        |                       |                       | map.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `setNat               | ::: block             |
        | scriptionArg.Builder` | iveLibraryProguardCon | Initializes the       |
        |                       | figGenerator​(BuildTar | optional value        |
        |                       | get nativeLibraryProg | [`nativeLib           |
        |                       | uardConfigGenerator)` | raryProguardConfigGen |
        |                       |                       | erator`](AndroidBundl |
        |                       |                       | eDescriptionArg.html# |
        |                       |                       | getNativeLibraryProgu |
        |                       |                       | ardConfigGenerator()) |
        |                       |                       | to                    |
        |                       |                       | nativeLibraryPro      |
        |                       |                       | guardConfigGenerator. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `setNa                | ::: block             |
        | scriptionArg.Builder` | tiveLibraryProguardCo | Initializes the       |
        |                       | nfigGenerator​(Optiona | optional value        |
        |                       | l<? extends BuildTarg | [`nativeLib           |
        |                       | et> nativeLibraryProg | raryProguardConfigGen |
        |                       | uardConfigGenerator)` | erator`](AndroidBundl |
        |                       |                       | eDescriptionArg.html# |
        |                       |                       | getNativeLibraryProgu |
        |                       |                       | ardConfigGenerator()) |
        |                       |                       | to                    |
        |                       |                       | nativeLibraryPro      |
        |                       |                       | guardConfigGenerator. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `s                    | ::: block             |
        | scriptionArg.Builder` | etNoAutoAddOverlayRes | Initializes the value |
        |                       | ources​(boolean noAuto | for the               |
        |                       | AddOverlayResources)` | [`noAutoA             |
        |                       |                       | ddOverlayResources`]( |
        |                       |                       | AndroidBundleDescript |
        |                       |                       | ionArg.html#isNoAutoA |
        |                       |                       | ddOverlayResources()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `setNoAutoVersion     | ::: block             |
        | scriptionArg.Builder` | Resources​(boolean noA | Initializes the value |
        |                       | utoVersionResources)` | for the               |
        |                       |                       | [`n                   |
        |                       |                       | oAutoVersionResources |
        |                       |                       | `](AndroidBundleDescr |
        |                       |                       | iptionArg.html#isNoAu |
        |                       |                       | toVersionResources()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `setNoDx​(             | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Sets or replaces all  |
        |                       | ildTarget> elements)` | elements for          |
        |                       |                       | [`noDx`](A            |
        |                       |                       | ndroidBundleDescripti |
        |                       |                       | onArg.html#getNoDx()) |
        |                       |                       | set.                  |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `setNoVers            | ::: block             |
        | scriptionArg.Builder` | ionTransitionsResourc | Initializes the value |
        |                       | es​(boolean noVersionT | for the               |
        |                       | ransitionsResources)` | [`noVersionTransi     |
        |                       |                       | tionsResources`](Andr |
        |                       |                       | oidBundleDescriptionA |
        |                       |                       | rg.html#isNoVersionTr |
        |                       |                       | ansitionsResources()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `setO                 | ::: block             |
        | scriptionArg.Builder` | ptimizationPasses​(int | Initializes the value |
        |                       |  optimizationPasses)` | for the               |
        |                       |                       | [`optimizationPas     |
        |                       |                       | ses`](AndroidBundleDe |
        |                       |                       | scriptionArg.html#get |
        |                       |                       | OptimizationPasses()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `setPackageAsse       | ::: block             |
        | scriptionArg.Builder` | tLibraries​(boolean pa | Initializes the value |
        |                       | ckageAssetLibraries)` | for the               |
        |                       |                       | [                     |
        |                       |                       | `packageAssetLibrarie |
        |                       |                       | s`](AndroidBundleDesc |
        |                       |                       | riptionArg.html#isPac |
        |                       |                       | kageAssetLibraries()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `setPackageType       | ::: block             |
        | scriptionArg.Builder` | ​(String packageType)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`p                   |
        |                       |                       | ackageType`](AndroidB |
        |                       |                       | undleDescriptionArg.h |
        |                       |                       | tml#getPackageType()) |
        |                       |                       | to packageType.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `set                  | ::: block             |
        | scriptionArg.Builder` | PackageType​(Optional< | Initializes the       |
        |                       | String> packageType)` | optional value        |
        |                       |                       | [`p                   |
        |                       |                       | ackageType`](AndroidB |
        |                       |                       | undleDescriptionArg.h |
        |                       |                       | tml#getPackageType()) |
        |                       |                       | to packageType.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `setP                 | ::: block             |
        | scriptionArg.Builder` | ostFilterResourcesCmd | Initializes the       |
        |                       | ​(StringWithMacros pos | optional value        |
        |                       | tFilterResourcesCmd)` | [`po                  |
        |                       |                       | stFilterResourcesCmd` |
        |                       |                       | ](AndroidBundleDescri |
        |                       |                       | ptionArg.html#getPost |
        |                       |                       | FilterResourcesCmd()) |
        |                       |                       | to                    |
        |                       |                       | po                    |
        |                       |                       | stFilterResourcesCmd. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `set                  | ::: block             |
        | scriptionArg.Builder` | PostFilterResourcesCm | Initializes the       |
        |                       | d​(Optional<? extends  | optional value        |
        |                       | StringWithMacros> pos | [`po                  |
        |                       | tFilterResourcesCmd)` | stFilterResourcesCmd` |
        |                       |                       | ](AndroidBundleDescri |
        |                       |                       | ptionArg.html#getPost |
        |                       |                       | FilterResourcesCmd()) |
        |                       |                       | to                    |
        |                       |                       | po                    |
        |                       |                       | stFilterResourcesCmd. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `setPreproc           | ::: block             |
        | scriptionArg.Builder` | essJavaClassesBash​(St | Initializes the       |
        |                       | ringWithMacros prepro | optional value        |
        |                       | cessJavaClassesBash)` | [`preproce            |
        |                       |                       | ssJavaClassesBash`](A |
        |                       |                       | ndroidBundleDescripti |
        |                       |                       | onArg.html#getPreproc |
        |                       |                       | essJavaClassesBash()) |
        |                       |                       | to                    |
        |                       |                       | prepr                 |
        |                       |                       | ocessJavaClassesBash. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `setPrepro            | ::: block             |
        | scriptionArg.Builder` | cessJavaClassesBash​(O | Initializes the       |
        |                       | ptional<? extends Str | optional value        |
        |                       | ingWithMacros> prepro | [`preproce            |
        |                       | cessJavaClassesBash)` | ssJavaClassesBash`](A |
        |                       |                       | ndroidBundleDescripti |
        |                       |                       | onArg.html#getPreproc |
        |                       |                       | essJavaClassesBash()) |
        |                       |                       | to                    |
        |                       |                       | prepr                 |
        |                       |                       | ocessJavaClassesBash. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `setPrepr             | ::: block             |
        | scriptionArg.Builder` | ocessJavaClassesDeps​( | Sets or replaces all  |
        |                       | Iterable<? extends Bu | elements for          |
        |                       | ildTarget> elements)` | [`preproce            |
        |                       |                       | ssJavaClassesDeps`](A |
        |                       |                       | ndroidBundleDescripti |
        |                       |                       | onArg.html#getPreproc |
        |                       |                       | essJavaClassesDeps()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `setPrimaryDexClas    | ::: block             |
        | scriptionArg.Builder` | sesFile​(SourcePath pr | Initializes the       |
        |                       | imaryDexClassesFile)` | optional value        |
        |                       |                       | [`                    |
        |                       |                       | primaryDexClassesFile |
        |                       |                       | `](AndroidBundleDescr |
        |                       |                       | iptionArg.html#getPri |
        |                       |                       | maryDexClassesFile()) |
        |                       |                       | to                    |
        |                       |                       | p                     |
        |                       |                       | rimaryDexClassesFile. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `setPrimaryDexCla     | ::: block             |
        | scriptionArg.Builder` | ssesFile​(Optional<? e | Initializes the       |
        |                       | xtends SourcePath> pr | optional value        |
        |                       | imaryDexClassesFile)` | [`                    |
        |                       |                       | primaryDexClassesFile |
        |                       |                       | `](AndroidBundleDescr |
        |                       |                       | iptionArg.html#getPri |
        |                       |                       | maryDexClassesFile()) |
        |                       |                       | to                    |
        |                       |                       | p                     |
        |                       |                       | rimaryDexClassesFile. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `setPrim              | ::: block             |
        | scriptionArg.Builder` | aryDexPatterns​(Iterab | Sets or replaces all  |
        |                       | le<String> elements)` | elements for          |
        |                       |                       | [`primaryDexPatte     |
        |                       |                       | rns`](AndroidBundleDe |
        |                       |                       | scriptionArg.html#get |
        |                       |                       | PrimaryDexPatterns()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `setPrimaryDexScenar  | ::: block             |
        | scriptionArg.Builder` | ioFile​(SourcePath pri | Initializes the       |
        |                       | maryDexScenarioFile)` | optional value        |
        |                       |                       | [`pr                  |
        |                       |                       | imaryDexScenarioFile` |
        |                       |                       | ](AndroidBundleDescri |
        |                       |                       | ptionArg.html#getPrim |
        |                       |                       | aryDexScenarioFile()) |
        |                       |                       | to                    |
        |                       |                       | pr                    |
        |                       |                       | imaryDexScenarioFile. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `setPrimaryDexScena   | ::: block             |
        | scriptionArg.Builder` | rioFile​(Optional<? ex | Initializes the       |
        |                       | tends SourcePath> pri | optional value        |
        |                       | maryDexScenarioFile)` | [`pr                  |
        |                       |                       | imaryDexScenarioFile` |
        |                       |                       | ](AndroidBundleDescri |
        |                       |                       | ptionArg.html#getPrim |
        |                       |                       | aryDexScenarioFile()) |
        |                       |                       | to                    |
        |                       |                       | pr                    |
        |                       |                       | imaryDexScenarioFile. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `setPrimaryDexScen    | ::: block             |
        | scriptionArg.Builder` | arioOverflowAllowed​(b | Initializes the value |
        |                       | oolean primaryDexScen | for the               |
        |                       | arioOverflowAllowed)` | [`pr                  |
        |                       |                       | imaryDexScenarioOverf |
        |                       |                       | lowAllowed`](AndroidB |
        |                       |                       | undleDescriptionArg.h |
        |                       |                       | tml#isPrimaryDexScena |
        |                       |                       | rioOverflowAllowed()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `set                  | ::: block             |
        | scriptionArg.Builder` | ProguardConfig​(Source | Initializes the       |
        |                       | Path proguardConfig)` | optional value        |
        |                       |                       | [`proguar             |
        |                       |                       | dConfig`](AndroidBund |
        |                       |                       | leDescriptionArg.html |
        |                       |                       | #getProguardConfig()) |
        |                       |                       | to proguardConfig.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `se                   | ::: block             |
        | scriptionArg.Builder` | tProguardConfig​(Optio | Initializes the       |
        |                       | nal<? extends SourceP | optional value        |
        |                       | ath> proguardConfig)` | [`proguar             |
        |                       |                       | dConfig`](AndroidBund |
        |                       |                       | leDescriptionArg.html |
        |                       |                       | #getProguardConfig()) |
        |                       |                       | to proguardConfig.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `setP                 | ::: block             |
        | scriptionArg.Builder` | roguardJvmArgs​(Iterab | Sets or replaces all  |
        |                       | le<String> elements)` | elements for          |
        |                       |                       | [`proguardJ           |
        |                       |                       | vmArgs`](AndroidBundl |
        |                       |                       | eDescriptionArg.html# |
        |                       |                       | getProguardJvmArgs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `set                  | ::: block             |
        | scriptionArg.Builder` | Redex​(boolean redex)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`redex`](An          |
        |                       |                       | droidBundleDescriptio |
        |                       |                       | nArg.html#getRedex()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `setRedexConfig​(Sou   | ::: block             |
        | scriptionArg.Builder` | rcePath redexConfig)` | Initializes the       |
        |                       |                       | optional value        |
        |                       |                       | [`r                   |
        |                       |                       | edexConfig`](AndroidB |
        |                       |                       | undleDescriptionArg.h |
        |                       |                       | tml#getRedexConfig()) |
        |                       |                       | to redexConfig.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `setRedexConfig​(Op    | ::: block             |
        | scriptionArg.Builder` | tional<? extends Sour | Initializes the       |
        |                       | cePath> redexConfig)` | optional value        |
        |                       |                       | [`r                   |
        |                       |                       | edexConfig`](AndroidB |
        |                       |                       | undleDescriptionArg.h |
        |                       |                       | tml#getRedexConfig()) |
        |                       |                       | to redexConfig.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `se                   | ::: block             |
        | scriptionArg.Builder` | tRedexExtraArgs​(Itera | Sets or replaces all  |
        |                       | ble<? extends StringW | elements for          |
        |                       | ithMacros> elements)` | [`redexEx             |
        |                       |                       | traArgs`](AndroidBund |
        |                       |                       | leDescriptionArg.html |
        |                       |                       | #getRedexExtraArgs()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `setRelinkerWhitel    | ::: block             |
        | scriptionArg.Builder` | ist​(Iterable<? extend | Sets or replaces all  |
        |                       | s Pattern> elements)` | elements for          |
        |                       |                       | [`relinkerWhite       |
        |                       |                       | list`](AndroidBundleD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tRelinkerWhitelist()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `setReorderClasse     | ::: block             |
        | scriptionArg.Builder` | sIntraDex​(boolean reo | Initializes the value |
        |                       | rderClassesIntraDex)` | for the               |
        |                       |                       | [`r                   |
        |                       |                       | eorderClassesIntraDex |
        |                       |                       | `](AndroidBundleDescr |
        |                       |                       | iptionArg.html#isReor |
        |                       |                       | derClassesIntraDex()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `setRe                | ::: block             |
        | scriptionArg.Builder` | sourceCompression​(com | Initializes the value |
        |                       | .facebook.buck.androi | for the               |
        |                       | d.ResourcesFilter.Res | [`resourceCompressi   |
        |                       | ourceCompressionMode  | on`](AndroidBundleDes |
        |                       | resourceCompression)` | criptionArg.html#getR |
        |                       |                       | esourceCompression()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `set                  | ::: block             |
        | scriptionArg.Builder` | ResourceFilter​(Iterab | Sets or replaces all  |
        |                       | le<String> elements)` | elements for          |
        |                       |                       | [`resourc             |
        |                       |                       | eFilter`](AndroidBund |
        |                       |                       | leDescriptionArg.html |
        |                       |                       | #getResourceFilter()) |
        |                       |                       | list.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `setResource          | ::: block             |
        | scriptionArg.Builder` | UnionPackage​(String r | Initializes the       |
        |                       | esourceUnionPackage)` | optional value        |
        |                       |                       | [`resourceUnionPackag |
        |                       |                       | e`](AndroidBundleDesc |
        |                       |                       | riptionArg.html#getRe |
        |                       |                       | sourceUnionPackage()) |
        |                       |                       | to                    |
        |                       |                       | resourceUnionPackage. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `                     | ::: block             |
        | scriptionArg.Builder` | setResourceUnionPacka | Initializes the       |
        |                       | ge​(Optional<String> r | optional value        |
        |                       | esourceUnionPackage)` | [`resourceUnionPackag |
        |                       |                       | e`](AndroidBundleDesc |
        |                       |                       | riptionArg.html#getRe |
        |                       |                       | sourceUnionPackage()) |
        |                       |                       | to                    |
        |                       |                       | resourceUnionPackage. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `setSecon             | ::: block             |
        | scriptionArg.Builder` | daryDexHeadClassesFil | Initializes the       |
        |                       | e​(SourcePath secondar | optional value        |
        |                       | yDexHeadClassesFile)` | [`secondaryDex        |
        |                       |                       | HeadClassesFile`](And |
        |                       |                       | roidBundleDescription |
        |                       |                       | Arg.html#getSecondary |
        |                       |                       | DexHeadClassesFile()) |
        |                       |                       | to                    |
        |                       |                       | seconda               |
        |                       |                       | ryDexHeadClassesFile. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `setSeco              | ::: block             |
        | scriptionArg.Builder` | ndaryDexHeadClassesFi | Initializes the       |
        |                       | le​(Optional<? extends | optional value        |
        |                       |  SourcePath> secondar | [`secondaryDex        |
        |                       | yDexHeadClassesFile)` | HeadClassesFile`](And |
        |                       |                       | roidBundleDescription |
        |                       |                       | Arg.html#getSecondary |
        |                       |                       | DexHeadClassesFile()) |
        |                       |                       | to                    |
        |                       |                       | seconda               |
        |                       |                       | ryDexHeadClassesFile. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `setSecon             | ::: block             |
        | scriptionArg.Builder` | daryDexTailClassesFil | Initializes the       |
        |                       | e​(SourcePath secondar | optional value        |
        |                       | yDexTailClassesFile)` | [`secondaryDex        |
        |                       |                       | TailClassesFile`](And |
        |                       |                       | roidBundleDescription |
        |                       |                       | Arg.html#getSecondary |
        |                       |                       | DexTailClassesFile()) |
        |                       |                       | to                    |
        |                       |                       | seconda               |
        |                       |                       | ryDexTailClassesFile. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `setSeco              | ::: block             |
        | scriptionArg.Builder` | ndaryDexTailClassesFi | Initializes the       |
        |                       | le​(Optional<? extends | optional value        |
        |                       |  SourcePath> secondar | [`secondaryDex        |
        |                       | yDexTailClassesFile)` | TailClassesFile`](And |
        |                       |                       | roidBundleDescription |
        |                       |                       | Arg.html#getSecondary |
        |                       |                       | DexTailClassesFile()) |
        |                       |                       | to                    |
        |                       |                       | seconda               |
        |                       |                       | ryDexTailClassesFile. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `                     | ::: block             |
        | scriptionArg.Builder` | setSkipCrunchPngs​(boo | Initializes the       |
        |                       | lean skipCrunchPngs)` | optional value        |
        |                       |                       | [`skipCr              |
        |                       |                       | unchPngs`](AndroidBun |
        |                       |                       | dleDescriptionArg.htm |
        |                       |                       | l#isSkipCrunchPngs()) |
        |                       |                       | to skipCrunchPngs.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `setSkipCru           | ::: block             |
        | scriptionArg.Builder` | nchPngs​(Optional<Bool | Initializes the       |
        |                       | ean> skipCrunchPngs)` | optional value        |
        |                       |                       | [`skipCr              |
        |                       |                       | unchPngs`](AndroidBun |
        |                       |                       | dleDescriptionArg.htm |
        |                       |                       | l#isSkipCrunchPngs()) |
        |                       |                       | to skipCrunchPngs.    |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `setSkipProguard​(b    | ::: block             |
        | scriptionArg.Builder` | oolean skipProguard)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`sk                  |
        |                       |                       | ipProguard`](AndroidB |
        |                       |                       | undleDescriptionArg.h |
        |                       |                       | tml#isSkipProguard()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `setTests​(            | ::: block             |
        | scriptionArg.Builder` | Iterable<? extends Bu | Sets or replaces all  |
        |                       | ildTarget> elements)` | elements for          |
        |                       |                       | [`tests`](An          |
        |                       |                       | droidBundleDescriptio |
        |                       |                       | nArg.html#getTests()) |
        |                       |                       | sortedSet.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `se                   | ::: block             |
        | scriptionArg.Builder` | tTrimResourceIds​(bool | Initializes the value |
        |                       | ean trimResourceIds)` | for the               |
        |                       |                       | [`trimReso            |
        |                       |                       | urceIds`](AndroidBund |
        |                       |                       | leDescriptionArg.html |
        |                       |                       | #isTrimResourceIds()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `setUse               | ::: block             |
        | scriptionArg.Builder` | DynamicFeature​(boolea | Initializes the value |
        |                       | n useDynamicFeature)` | for the               |
        |                       |                       | [`useDynamicFea       |
        |                       |                       | ture`](AndroidBundleD |
        |                       |                       | escriptionArg.html#ge |
        |                       |                       | tUseDynamicFeature()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `setUseSplitDex​(      | ::: block             |
        | scriptionArg.Builder` | boolean useSplitDex)` | Initializes the value |
        |                       |                       | for the               |
        |                       |                       | [`u                   |
        |                       |                       | seSplitDex`](AndroidB |
        |                       |                       | undleDescriptionArg.h |
        |                       |                       | tml#getUseSplitDex()) |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `AndroidBundleDe      | `setX                 | ::: block             |
        | scriptionArg.Builder` | zCompressionLevel​(int | Initializes the value |
        |                       |  xzCompressionLevel)` | for the               |
        |                       |                       | [`xzCompressionLe     |
        |                       |                       | vel`](AndroidBundleDe |
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
            public final AndroidBundleDescriptionArg.Builder from​(HasApplicationModuleBlacklist instance)
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
            public final AndroidBundleDescriptionArg.Builder from​(AndroidGraphEnhancerArgs instance)
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
            public final AndroidBundleDescriptionArg.Builder from​(HasDeclaredDeps instance)
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
            public final AndroidBundleDescriptionArg.Builder from​(HasTests instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `com.facebook.buck.core.description.arg.HasTests` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.android.AndroidBundleDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder from​(AndroidBundleDescriptionArg instance)
            ```

            ::: block
            Fill a builder with attribute values from the provided
            `AndroidBundleDescriptionArg` instance.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.android.AndroidBundleDescription.AbstractAndroidBundleDescriptionArg)}

        -   #### from

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder from​(com.facebook.buck.android.AndroidBundleDescription.AbstractAndroidBundleDescriptionArg instance)
            ```

            ::: block
            Copy abstract value type
            `AbstractAndroidBundleDescriptionArg` instance into builder.
            :::

            [Parameters:]{.paramLabel}
            :   `instance` - The instance from which to copy values

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#from(com.facebook.buck.android.HasExopackageArgs)}

        -   #### from

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder from​(HasExopackageArgs instance)
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
            public final AndroidBundleDescriptionArg.Builder from​(BuildRuleArg instance)
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
            public final AndroidBundleDescriptionArg.Builder from​(HasDuplicateAndroidResourceTypes instance)
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
            public final AndroidBundleDescriptionArg.Builder from​(ConstructorArg instance)
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
            public final AndroidBundleDescriptionArg.Builder setKeystore​(BuildTarget keystore)
            ```

            ::: block
            Initializes the value for the
            [`keystore`](AndroidBundleDescriptionArg.html#getKeystore())
            attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `keystore` - The value for keystore

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setUseSplitDex(boolean)}

        -   #### setUseSplitDex

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder setUseSplitDex​(boolean useSplitDex)
            ```

            ::: block
            Initializes the value for the
            [`useSplitDex`](AndroidBundleDescriptionArg.html#getUseSplitDex())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`useSplitDex`](AndroidBundleDescriptionArg.html#getUseSplitDex()).*
            :::

            [Parameters:]{.paramLabel}
            :   `useSplitDex` - The value for useSplitDex

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setMinimizePrimaryDexSize(boolean)}

        -   #### setMinimizePrimaryDexSize

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder setMinimizePrimaryDexSize​(boolean minimizePrimaryDexSize)
            ```

            ::: block
            Initializes the value for the
            [`minimizePrimaryDexSize`](AndroidBundleDescriptionArg.html#getMinimizePrimaryDexSize())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`minimizePrimaryDexSize`](AndroidBundleDescriptionArg.html#getMinimizePrimaryDexSize()).*
            :::

            [Parameters:]{.paramLabel}
            :   `minimizePrimaryDexSize` - The value for
                minimizePrimaryDexSize

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDexCompression(com.facebook.buck.android.DexStore)}

        -   #### setDexCompression

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder setDexCompression​(com.facebook.buck.android.DexStore dexCompression)
            ```

            ::: block
            Initializes the optional value
            [`dexCompression`](AndroidBundleDescriptionArg.html#getDexCompression())
            to dexCompression.
            :::

            [Parameters:]{.paramLabel}
            :   `dexCompression` - The value for dexCompression

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setDexCompression(java.util.Optional)}

        -   #### setDexCompression

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder setDexCompression​(Optional<? extends com.facebook.buck.android.DexStore> dexCompression)
            ```

            ::: block
            Initializes the optional value
            [`dexCompression`](AndroidBundleDescriptionArg.html#getDexCompression())
            to dexCompression.
            :::

            [Parameters:]{.paramLabel}
            :   `dexCompression` - The value for dexCompression

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addPrimaryDexPatterns(java.lang.String)}

        -   #### addPrimaryDexPatterns

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder addPrimaryDexPatterns​(String element)
            ```

            ::: block
            Adds one element to
            [`primaryDexPatterns`](AndroidBundleDescriptionArg.html#getPrimaryDexPatterns())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A primaryDexPatterns element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addPrimaryDexPatterns(java.lang.String...)}

        -   #### addPrimaryDexPatterns

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder addPrimaryDexPatterns​(String... elements)
            ```

            ::: block
            Adds elements to
            [`primaryDexPatterns`](AndroidBundleDescriptionArg.html#getPrimaryDexPatterns())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of primaryDexPatterns elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPrimaryDexPatterns(java.lang.Iterable)}

        -   #### setPrimaryDexPatterns

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder setPrimaryDexPatterns​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`primaryDexPatterns`](AndroidBundleDescriptionArg.html#getPrimaryDexPatterns())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of primaryDexPatterns elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllPrimaryDexPatterns(java.lang.Iterable)}

        -   #### addAllPrimaryDexPatterns

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder addAllPrimaryDexPatterns​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`primaryDexPatterns`](AndroidBundleDescriptionArg.html#getPrimaryDexPatterns())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of primaryDexPatterns elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPrimaryDexClassesFile(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setPrimaryDexClassesFile

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder setPrimaryDexClassesFile​(SourcePath primaryDexClassesFile)
            ```

            ::: block
            Initializes the optional value
            [`primaryDexClassesFile`](AndroidBundleDescriptionArg.html#getPrimaryDexClassesFile())
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
            public final AndroidBundleDescriptionArg.Builder setPrimaryDexClassesFile​(Optional<? extends SourcePath> primaryDexClassesFile)
            ```

            ::: block
            Initializes the optional value
            [`primaryDexClassesFile`](AndroidBundleDescriptionArg.html#getPrimaryDexClassesFile())
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
            public final AndroidBundleDescriptionArg.Builder setPrimaryDexScenarioFile​(SourcePath primaryDexScenarioFile)
            ```

            ::: block
            Initializes the optional value
            [`primaryDexScenarioFile`](AndroidBundleDescriptionArg.html#getPrimaryDexScenarioFile())
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
            public final AndroidBundleDescriptionArg.Builder setPrimaryDexScenarioFile​(Optional<? extends SourcePath> primaryDexScenarioFile)
            ```

            ::: block
            Initializes the optional value
            [`primaryDexScenarioFile`](AndroidBundleDescriptionArg.html#getPrimaryDexScenarioFile())
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
            public final AndroidBundleDescriptionArg.Builder setPrimaryDexScenarioOverflowAllowed​(boolean primaryDexScenarioOverflowAllowed)
            ```

            ::: block
            Initializes the value for the
            [`primaryDexScenarioOverflowAllowed`](AndroidBundleDescriptionArg.html#isPrimaryDexScenarioOverflowAllowed())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`primaryDexScenarioOverflowAllowed`](AndroidBundleDescriptionArg.html#isPrimaryDexScenarioOverflowAllowed()).*
            :::

            [Parameters:]{.paramLabel}
            :   `primaryDexScenarioOverflowAllowed` - The value for
                primaryDexScenarioOverflowAllowed

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setSecondaryDexHeadClassesFile(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setSecondaryDexHeadClassesFile

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder setSecondaryDexHeadClassesFile​(SourcePath secondaryDexHeadClassesFile)
            ```

            ::: block
            Initializes the optional value
            [`secondaryDexHeadClassesFile`](AndroidBundleDescriptionArg.html#getSecondaryDexHeadClassesFile())
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
            public final AndroidBundleDescriptionArg.Builder setSecondaryDexHeadClassesFile​(Optional<? extends SourcePath> secondaryDexHeadClassesFile)
            ```

            ::: block
            Initializes the optional value
            [`secondaryDexHeadClassesFile`](AndroidBundleDescriptionArg.html#getSecondaryDexHeadClassesFile())
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
            public final AndroidBundleDescriptionArg.Builder setSecondaryDexTailClassesFile​(SourcePath secondaryDexTailClassesFile)
            ```

            ::: block
            Initializes the optional value
            [`secondaryDexTailClassesFile`](AndroidBundleDescriptionArg.html#getSecondaryDexTailClassesFile())
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
            public final AndroidBundleDescriptionArg.Builder setSecondaryDexTailClassesFile​(Optional<? extends SourcePath> secondaryDexTailClassesFile)
            ```

            ::: block
            Initializes the optional value
            [`secondaryDexTailClassesFile`](AndroidBundleDescriptionArg.html#getSecondaryDexTailClassesFile())
            to secondaryDexTailClassesFile.
            :::

            [Parameters:]{.paramLabel}
            :   `secondaryDexTailClassesFile` - The value for
                secondaryDexTailClassesFile

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setBundleConfigFile(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setBundleConfigFile

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder setBundleConfigFile​(SourcePath bundleConfigFile)
            ```

            ::: block
            Initializes the optional value
            [`bundleConfigFile`](AndroidBundleDescriptionArg.html#getBundleConfigFile())
            to bundleConfigFile.
            :::

            [Parameters:]{.paramLabel}
            :   `bundleConfigFile` - The value for bundleConfigFile

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setBundleConfigFile(java.util.Optional)}

        -   #### setBundleConfigFile

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder setBundleConfigFile​(Optional<? extends SourcePath> bundleConfigFile)
            ```

            ::: block
            Initializes the optional value
            [`bundleConfigFile`](AndroidBundleDescriptionArg.html#getBundleConfigFile())
            to bundleConfigFile.
            :::

            [Parameters:]{.paramLabel}
            :   `bundleConfigFile` - The value for bundleConfigFile

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setAndroidAppModularityResult(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setAndroidAppModularityResult

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder setAndroidAppModularityResult​(SourcePath androidAppModularityResult)
            ```

            ::: block
            Initializes the optional value
            [`androidAppModularityResult`](AndroidBundleDescriptionArg.html#getAndroidAppModularityResult())
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
            public final AndroidBundleDescriptionArg.Builder setAndroidAppModularityResult​(Optional<? extends SourcePath> androidAppModularityResult)
            ```

            ::: block
            Initializes the optional value
            [`androidAppModularityResult`](AndroidBundleDescriptionArg.html#getAndroidAppModularityResult())
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
            public final AndroidBundleDescriptionArg.Builder setLinearAllocHardLimit​(long linearAllocHardLimit)
            ```

            ::: block
            Initializes the value for the
            [`linearAllocHardLimit`](AndroidBundleDescriptionArg.html#getLinearAllocHardLimit())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`linearAllocHardLimit`](AndroidBundleDescriptionArg.html#getLinearAllocHardLimit()).*
            :::

            [Parameters:]{.paramLabel}
            :   `linearAllocHardLimit` - The value for
                linearAllocHardLimit

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDexGroupLibLimit(int)}

        -   #### setDexGroupLibLimit

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder setDexGroupLibLimit​(int dexGroupLibLimit)
            ```

            ::: block
            Initializes the value for the
            [`dexGroupLibLimit`](AndroidBundleDescriptionArg.html#getDexGroupLibLimit())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`dexGroupLibLimit`](AndroidBundleDescriptionArg.html#getDexGroupLibLimit()).*
            :::

            [Parameters:]{.paramLabel}
            :   `dexGroupLibLimit` - The value for dexGroupLibLimit

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addResourceFilter(java.lang.String)}

        -   #### addResourceFilter

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder addResourceFilter​(String element)
            ```

            ::: block
            Adds one element to
            [`resourceFilter`](AndroidBundleDescriptionArg.html#getResourceFilter())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A resourceFilter element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addResourceFilter(java.lang.String...)}

        -   #### addResourceFilter

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder addResourceFilter​(String... elements)
            ```

            ::: block
            Adds elements to
            [`resourceFilter`](AndroidBundleDescriptionArg.html#getResourceFilter())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of resourceFilter elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setResourceFilter(java.lang.Iterable)}

        -   #### setResourceFilter

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder setResourceFilter​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`resourceFilter`](AndroidBundleDescriptionArg.html#getResourceFilter())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of resourceFilter elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllResourceFilter(java.lang.Iterable)}

        -   #### addAllResourceFilter

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder addAllResourceFilter​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`resourceFilter`](AndroidBundleDescriptionArg.html#getResourceFilter())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of resourceFilter elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addPreprocessJavaClassesDeps(com.facebook.buck.core.model.BuildTarget)}

        -   #### addPreprocessJavaClassesDeps

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder addPreprocessJavaClassesDeps​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`preprocessJavaClassesDeps`](AndroidBundleDescriptionArg.html#getPreprocessJavaClassesDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A preprocessJavaClassesDeps element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addPreprocessJavaClassesDeps(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addPreprocessJavaClassesDeps

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder addPreprocessJavaClassesDeps​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`preprocessJavaClassesDeps`](AndroidBundleDescriptionArg.html#getPreprocessJavaClassesDeps())
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
            public final AndroidBundleDescriptionArg.Builder setPreprocessJavaClassesDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`preprocessJavaClassesDeps`](AndroidBundleDescriptionArg.html#getPreprocessJavaClassesDeps())
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
            public final AndroidBundleDescriptionArg.Builder addAllPreprocessJavaClassesDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`preprocessJavaClassesDeps`](AndroidBundleDescriptionArg.html#getPreprocessJavaClassesDeps())
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
            public final AndroidBundleDescriptionArg.Builder setXzCompressionLevel​(int xzCompressionLevel)
            ```

            ::: block
            Initializes the value for the
            [`xzCompressionLevel`](AndroidBundleDescriptionArg.html#getXzCompressionLevel())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`xzCompressionLevel`](AndroidBundleDescriptionArg.html#getXzCompressionLevel()).*
            :::

            [Parameters:]{.paramLabel}
            :   `xzCompressionLevel` - The value for xzCompressionLevel

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPackageAssetLibraries(boolean)}

        -   #### setPackageAssetLibraries

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder setPackageAssetLibraries​(boolean packageAssetLibraries)
            ```

            ::: block
            Initializes the value for the
            [`packageAssetLibraries`](AndroidBundleDescriptionArg.html#isPackageAssetLibraries())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`packageAssetLibraries`](AndroidBundleDescriptionArg.html#isPackageAssetLibraries()).*
            :::

            [Parameters:]{.paramLabel}
            :   `packageAssetLibraries` - The value for
                packageAssetLibraries

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCompressAssetLibraries(boolean)}

        -   #### setCompressAssetLibraries

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder setCompressAssetLibraries​(boolean compressAssetLibraries)
            ```

            ::: block
            Initializes the value for the
            [`compressAssetLibraries`](AndroidBundleDescriptionArg.html#isCompressAssetLibraries())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`compressAssetLibraries`](AndroidBundleDescriptionArg.html#isCompressAssetLibraries()).*
            :::

            [Parameters:]{.paramLabel}
            :   `compressAssetLibraries` - The value for
                compressAssetLibraries

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setAssetCompressionAlgorithm(com.facebook.buck.android.CompressionAlgorithm)}

        -   #### setAssetCompressionAlgorithm

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder setAssetCompressionAlgorithm​(CompressionAlgorithm assetCompressionAlgorithm)
            ```

            ::: block
            Initializes the optional value
            [`assetCompressionAlgorithm`](AndroidBundleDescriptionArg.html#getAssetCompressionAlgorithm())
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
            public final AndroidBundleDescriptionArg.Builder setAssetCompressionAlgorithm​(Optional<? extends CompressionAlgorithm> assetCompressionAlgorithm)
            ```

            ::: block
            Initializes the optional value
            [`assetCompressionAlgorithm`](AndroidBundleDescriptionArg.html#getAssetCompressionAlgorithm())
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
            public final AndroidBundleDescriptionArg.Builder setRedex​(boolean redex)
            ```

            ::: block
            Initializes the value for the
            [`redex`](AndroidBundleDescriptionArg.html#getRedex())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`redex`](AndroidBundleDescriptionArg.html#getRedex()).*
            :::

            [Parameters:]{.paramLabel}
            :   `redex` - The value for redex

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setRedexConfig(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setRedexConfig

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder setRedexConfig​(SourcePath redexConfig)
            ```

            ::: block
            Initializes the optional value
            [`redexConfig`](AndroidBundleDescriptionArg.html#getRedexConfig())
            to redexConfig.
            :::

            [Parameters:]{.paramLabel}
            :   `redexConfig` - The value for redexConfig

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setRedexConfig(java.util.Optional)}

        -   #### setRedexConfig

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder setRedexConfig​(Optional<? extends SourcePath> redexConfig)
            ```

            ::: block
            Initializes the optional value
            [`redexConfig`](AndroidBundleDescriptionArg.html#getRedexConfig())
            to redexConfig.
            :::

            [Parameters:]{.paramLabel}
            :   `redexConfig` - The value for redexConfig

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addRedexExtraArgs(com.facebook.buck.rules.macros.StringWithMacros)}

        -   #### addRedexExtraArgs

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder addRedexExtraArgs​(StringWithMacros element)
            ```

            ::: block
            Adds one element to
            [`redexExtraArgs`](AndroidBundleDescriptionArg.html#getRedexExtraArgs())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A redexExtraArgs element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addRedexExtraArgs(com.facebook.buck.rules.macros.StringWithMacros...)}

        -   #### addRedexExtraArgs

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder addRedexExtraArgs​(StringWithMacros... elements)
            ```

            ::: block
            Adds elements to
            [`redexExtraArgs`](AndroidBundleDescriptionArg.html#getRedexExtraArgs())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of redexExtraArgs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setRedexExtraArgs(java.lang.Iterable)}

        -   #### setRedexExtraArgs

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder setRedexExtraArgs​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`redexExtraArgs`](AndroidBundleDescriptionArg.html#getRedexExtraArgs())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of redexExtraArgs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllRedexExtraArgs(java.lang.Iterable)}

        -   #### addAllRedexExtraArgs

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder addAllRedexExtraArgs​(Iterable<? extends StringWithMacros> elements)
            ```

            ::: block
            Adds elements to
            [`redexExtraArgs`](AndroidBundleDescriptionArg.html#getRedexExtraArgs())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of redexExtraArgs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setAaptMode(com.facebook.buck.android.AaptMode)}

        -   #### setAaptMode

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder setAaptMode​(com.facebook.buck.android.AaptMode aaptMode)
            ```

            ::: block
            Initializes the value for the
            [`aaptMode`](AndroidBundleDescriptionArg.html#getAaptMode())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`aaptMode`](AndroidBundleDescriptionArg.html#getAaptMode()).*
            :::

            [Parameters:]{.paramLabel}
            :   `aaptMode` - The value for aaptMode

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLicenses(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### addLicenses

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder addLicenses​(SourcePath element)
            ```

            ::: block
            Adds one element to
            [`licenses`](AndroidBundleDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A licenses element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLicenses(com.facebook.buck.core.sourcepath.SourcePath...)}

        -   #### addLicenses

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder addLicenses​(SourcePath... elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](AndroidBundleDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLicenses(java.lang.Iterable)}

        -   #### setLicenses

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder setLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`licenses`](AndroidBundleDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLicenses(java.lang.Iterable)}

        -   #### addAllLicenses

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder addAllLicenses​(Iterable<? extends SourcePath> elements)
            ```

            ::: block
            Adds elements to
            [`licenses`](AndroidBundleDescriptionArg.html#getLicenses())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of licenses elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLabels(java.lang.String)}

        -   #### addLabels

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder addLabels​(String element)
            ```

            ::: block
            Adds one element to
            [`labels`](AndroidBundleDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A labels element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLabels(java.lang.String...)}

        -   #### addLabels

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder addLabels​(String... elements)
            ```

            ::: block
            Adds elements to
            [`labels`](AndroidBundleDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLabels(java.lang.Iterable)}

        -   #### setLabels

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder setLabels​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`labels`](AndroidBundleDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLabels(java.lang.Iterable)}

        -   #### addAllLabels

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder addAllLabels​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`labels`](AndroidBundleDescriptionArg.html#getLabels())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of labels elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDefaultTargetPlatform(com.facebook.buck.core.model.UnconfiguredBuildTarget)}

        -   #### setDefaultTargetPlatform

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder setDefaultTargetPlatform​(UnconfiguredBuildTarget defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](AndroidBundleDescriptionArg.html#getDefaultTargetPlatform())
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
            public final AndroidBundleDescriptionArg.Builder setDefaultTargetPlatform​(Optional<? extends UnconfiguredBuildTarget> defaultTargetPlatform)
            ```

            ::: block
            Initializes the optional value
            [`defaultTargetPlatform`](AndroidBundleDescriptionArg.html#getDefaultTargetPlatform())
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
            public final AndroidBundleDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget element)
            ```

            ::: block
            Adds one element to
            [`compatibleWith`](AndroidBundleDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A compatibleWith element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCompatibleWith(com.facebook.buck.core.model.UnconfiguredBuildTarget...)}

        -   #### addCompatibleWith

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder addCompatibleWith​(UnconfiguredBuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](AndroidBundleDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCompatibleWith(java.lang.Iterable)}

        -   #### setCompatibleWith

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder setCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`compatibleWith`](AndroidBundleDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllCompatibleWith(java.lang.Iterable)}

        -   #### addAllCompatibleWith

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder addAllCompatibleWith​(Iterable<? extends UnconfiguredBuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`compatibleWith`](AndroidBundleDescriptionArg.html#getCompatibleWith())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of compatibleWith elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setName(java.lang.String)}

        -   #### setName

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder setName​(String name)
            ```

            ::: block
            Initializes the value for the
            [`name`](AndroidBundleDescriptionArg.html#getName())
            attribute.
            :::

            [Parameters:]{.paramLabel}
            :   `name` - The value for name

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addDeps(com.facebook.buck.core.model.BuildTarget)}

        -   #### addDeps

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder addDeps​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`deps`](AndroidBundleDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A deps element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addDeps(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addDeps

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder addDeps​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`deps`](AndroidBundleDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDeps(java.lang.Iterable)}

        -   #### setDeps

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder setDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`deps`](AndroidBundleDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllDeps(java.lang.Iterable)}

        -   #### addAllDeps

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder addAllDeps​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`deps`](AndroidBundleDescriptionArg.html#getDeps())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of deps elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setExopackage(boolean)}

        -   #### setExopackage

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder setExopackage​(boolean exopackage)
            ```

            ::: block
            Initializes the optional value
            [`exopackage`](AndroidBundleDescriptionArg.html#isExopackage())
            to exopackage.
            :::

            [Parameters:]{.paramLabel}
            :   `exopackage` - The value for exopackage

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setExopackage(java.util.Optional)}

        -   #### setExopackage

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder setExopackage​(Optional<Boolean> exopackage)
            ```

            ::: block
            Initializes the optional value
            [`exopackage`](AndroidBundleDescriptionArg.html#isExopackage())
            to exopackage.
            :::

            [Parameters:]{.paramLabel}
            :   `exopackage` - The value for exopackage

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addExopackageModes(com.facebook.buck.android.exopackage.ExopackageMode)}

        -   #### addExopackageModes

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder addExopackageModes​(ExopackageMode element)
            ```

            ::: block
            Adds one element to
            [`exopackageModes`](AndroidBundleDescriptionArg.html#getExopackageModes())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A exopackageModes element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addExopackageModes(com.facebook.buck.android.exopackage.ExopackageMode...)}

        -   #### addExopackageModes

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder addExopackageModes​(ExopackageMode... elements)
            ```

            ::: block
            Adds elements to
            [`exopackageModes`](AndroidBundleDescriptionArg.html#getExopackageModes())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of exopackageModes elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setExopackageModes(java.lang.Iterable)}

        -   #### setExopackageModes

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder setExopackageModes​(Iterable<ExopackageMode> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`exopackageModes`](AndroidBundleDescriptionArg.html#getExopackageModes())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of exopackageModes elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllExopackageModes(java.lang.Iterable)}

        -   #### addAllExopackageModes

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder addAllExopackageModes​(Iterable<ExopackageMode> elements)
            ```

            ::: block
            Adds elements to
            [`exopackageModes`](AndroidBundleDescriptionArg.html#getExopackageModes())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of exopackageModes elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addTests(com.facebook.buck.core.model.BuildTarget)}

        -   #### addTests

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder addTests​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`tests`](AndroidBundleDescriptionArg.html#getTests())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A tests element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addTests(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addTests

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder addTests​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`tests`](AndroidBundleDescriptionArg.html#getTests())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of tests elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setTests(java.lang.Iterable)}

        -   #### setTests

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder setTests​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`tests`](AndroidBundleDescriptionArg.html#getTests())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of tests elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllTests(java.lang.Iterable)}

        -   #### addAllTests

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder addAllTests​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`tests`](AndroidBundleDescriptionArg.html#getTests())
            sortedSet.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of tests elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setManifest(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setManifest

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder setManifest​(SourcePath manifest)
            ```

            ::: block
            Initializes the optional value
            [`manifest`](AndroidBundleDescriptionArg.html#getManifest())
            to manifest.
            :::

            [Parameters:]{.paramLabel}
            :   `manifest` - The value for manifest

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setManifest(java.util.Optional)}

        -   #### setManifest

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder setManifest​(Optional<? extends SourcePath> manifest)
            ```

            ::: block
            Initializes the optional value
            [`manifest`](AndroidBundleDescriptionArg.html#getManifest())
            to manifest.
            :::

            [Parameters:]{.paramLabel}
            :   `manifest` - The value for manifest

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setManifestSkeleton(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setManifestSkeleton

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder setManifestSkeleton​(SourcePath manifestSkeleton)
            ```

            ::: block
            Initializes the optional value
            [`manifestSkeleton`](AndroidBundleDescriptionArg.html#getManifestSkeleton())
            to manifestSkeleton.
            :::

            [Parameters:]{.paramLabel}
            :   `manifestSkeleton` - The value for manifestSkeleton

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setManifestSkeleton(java.util.Optional)}

        -   #### setManifestSkeleton

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder setManifestSkeleton​(Optional<? extends SourcePath> manifestSkeleton)
            ```

            ::: block
            Initializes the optional value
            [`manifestSkeleton`](AndroidBundleDescriptionArg.html#getManifestSkeleton())
            to manifestSkeleton.
            :::

            [Parameters:]{.paramLabel}
            :   `manifestSkeleton` - The value for manifestSkeleton

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setModuleManifestSkeleton(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setModuleManifestSkeleton

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder setModuleManifestSkeleton​(SourcePath moduleManifestSkeleton)
            ```

            ::: block
            Initializes the optional value
            [`moduleManifestSkeleton`](AndroidBundleDescriptionArg.html#getModuleManifestSkeleton())
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
            public final AndroidBundleDescriptionArg.Builder setModuleManifestSkeleton​(Optional<? extends SourcePath> moduleManifestSkeleton)
            ```

            ::: block
            Initializes the optional value
            [`moduleManifestSkeleton`](AndroidBundleDescriptionArg.html#getModuleManifestSkeleton())
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
            public final AndroidBundleDescriptionArg.Builder setPackageType​(String packageType)
            ```

            ::: block
            Initializes the optional value
            [`packageType`](AndroidBundleDescriptionArg.html#getPackageType())
            to packageType.
            :::

            [Parameters:]{.paramLabel}
            :   `packageType` - The value for packageType

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setPackageType(java.util.Optional)}

        -   #### setPackageType

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder setPackageType​(Optional<String> packageType)
            ```

            ::: block
            Initializes the optional value
            [`packageType`](AndroidBundleDescriptionArg.html#getPackageType())
            to packageType.
            :::

            [Parameters:]{.paramLabel}
            :   `packageType` - The value for packageType

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addNoDx(com.facebook.buck.core.model.BuildTarget)}

        -   #### addNoDx

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder addNoDx​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`noDx`](AndroidBundleDescriptionArg.html#getNoDx()) set.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A noDx element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addNoDx(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addNoDx

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder addNoDx​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`noDx`](AndroidBundleDescriptionArg.html#getNoDx()) set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of noDx elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setNoDx(java.lang.Iterable)}

        -   #### setNoDx

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder setNoDx​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`noDx`](AndroidBundleDescriptionArg.html#getNoDx()) set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of noDx elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllNoDx(java.lang.Iterable)}

        -   #### addAllNoDx

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder addAllNoDx​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`noDx`](AndroidBundleDescriptionArg.html#getNoDx()) set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of noDx elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDisablePreDex(boolean)}

        -   #### setDisablePreDex

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder setDisablePreDex​(boolean disablePreDex)
            ```

            ::: block
            Initializes the value for the
            [`disablePreDex`](AndroidBundleDescriptionArg.html#getDisablePreDex())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`disablePreDex`](AndroidBundleDescriptionArg.html#getDisablePreDex()).*
            :::

            [Parameters:]{.paramLabel}
            :   `disablePreDex` - The value for disablePreDex

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setAndroidSdkProguardConfig(com.facebook.buck.android.ProGuardObfuscateStep.SdkProguardType)}

        -   #### setAndroidSdkProguardConfig

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder setAndroidSdkProguardConfig​(com.facebook.buck.android.ProGuardObfuscateStep.SdkProguardType androidSdkProguardConfig)
            ```

            ::: block
            Initializes the optional value
            [`androidSdkProguardConfig`](AndroidBundleDescriptionArg.html#getAndroidSdkProguardConfig())
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
            public final AndroidBundleDescriptionArg.Builder setAndroidSdkProguardConfig​(Optional<? extends com.facebook.buck.android.ProGuardObfuscateStep.SdkProguardType> androidSdkProguardConfig)
            ```

            ::: block
            Initializes the optional value
            [`androidSdkProguardConfig`](AndroidBundleDescriptionArg.html#getAndroidSdkProguardConfig())
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
            public final AndroidBundleDescriptionArg.Builder setOptimizationPasses​(int optimizationPasses)
            ```

            ::: block
            Initializes the value for the
            [`optimizationPasses`](AndroidBundleDescriptionArg.html#getOptimizationPasses())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`optimizationPasses`](AndroidBundleDescriptionArg.html#getOptimizationPasses()).*
            :::

            [Parameters:]{.paramLabel}
            :   `optimizationPasses` - The value for optimizationPasses

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addProguardJvmArgs(java.lang.String)}

        -   #### addProguardJvmArgs

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder addProguardJvmArgs​(String element)
            ```

            ::: block
            Adds one element to
            [`proguardJvmArgs`](AndroidBundleDescriptionArg.html#getProguardJvmArgs())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A proguardJvmArgs element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addProguardJvmArgs(java.lang.String...)}

        -   #### addProguardJvmArgs

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder addProguardJvmArgs​(String... elements)
            ```

            ::: block
            Adds elements to
            [`proguardJvmArgs`](AndroidBundleDescriptionArg.html#getProguardJvmArgs())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of proguardJvmArgs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setProguardJvmArgs(java.lang.Iterable)}

        -   #### setProguardJvmArgs

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder setProguardJvmArgs​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`proguardJvmArgs`](AndroidBundleDescriptionArg.html#getProguardJvmArgs())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of proguardJvmArgs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllProguardJvmArgs(java.lang.Iterable)}

        -   #### addAllProguardJvmArgs

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder addAllProguardJvmArgs​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`proguardJvmArgs`](AndroidBundleDescriptionArg.html#getProguardJvmArgs())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of proguardJvmArgs elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setProguardConfig(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setProguardConfig

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder setProguardConfig​(SourcePath proguardConfig)
            ```

            ::: block
            Initializes the optional value
            [`proguardConfig`](AndroidBundleDescriptionArg.html#getProguardConfig())
            to proguardConfig.
            :::

            [Parameters:]{.paramLabel}
            :   `proguardConfig` - The value for proguardConfig

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setProguardConfig(java.util.Optional)}

        -   #### setProguardConfig

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder setProguardConfig​(Optional<? extends SourcePath> proguardConfig)
            ```

            ::: block
            Initializes the optional value
            [`proguardConfig`](AndroidBundleDescriptionArg.html#getProguardConfig())
            to proguardConfig.
            :::

            [Parameters:]{.paramLabel}
            :   `proguardConfig` - The value for proguardConfig

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setResourceCompression(com.facebook.buck.android.ResourcesFilter.ResourceCompressionMode)}

        -   #### setResourceCompression

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder setResourceCompression​(com.facebook.buck.android.ResourcesFilter.ResourceCompressionMode resourceCompression)
            ```

            ::: block
            Initializes the value for the
            [`resourceCompression`](AndroidBundleDescriptionArg.html#getResourceCompression())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`resourceCompression`](AndroidBundleDescriptionArg.html#getResourceCompression()).*
            :::

            [Parameters:]{.paramLabel}
            :   `resourceCompression` - The value for
                resourceCompression

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setSkipCrunchPngs(boolean)}

        -   #### setSkipCrunchPngs

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder setSkipCrunchPngs​(boolean skipCrunchPngs)
            ```

            ::: block
            Initializes the optional value
            [`skipCrunchPngs`](AndroidBundleDescriptionArg.html#isSkipCrunchPngs())
            to skipCrunchPngs.
            :::

            [Parameters:]{.paramLabel}
            :   `skipCrunchPngs` - The value for skipCrunchPngs

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setSkipCrunchPngs(java.util.Optional)}

        -   #### setSkipCrunchPngs

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder setSkipCrunchPngs​(Optional<Boolean> skipCrunchPngs)
            ```

            ::: block
            Initializes the optional value
            [`skipCrunchPngs`](AndroidBundleDescriptionArg.html#isSkipCrunchPngs())
            to skipCrunchPngs.
            :::

            [Parameters:]{.paramLabel}
            :   `skipCrunchPngs` - The value for skipCrunchPngs

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setIncludesVectorDrawables(boolean)}

        -   #### setIncludesVectorDrawables

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder setIncludesVectorDrawables​(boolean includesVectorDrawables)
            ```

            ::: block
            Initializes the value for the
            [`includesVectorDrawables`](AndroidBundleDescriptionArg.html#isIncludesVectorDrawables())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`includesVectorDrawables`](AndroidBundleDescriptionArg.html#isIncludesVectorDrawables()).*
            :::

            [Parameters:]{.paramLabel}
            :   `includesVectorDrawables` - The value for
                includesVectorDrawables

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setNoAutoVersionResources(boolean)}

        -   #### setNoAutoVersionResources

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder setNoAutoVersionResources​(boolean noAutoVersionResources)
            ```

            ::: block
            Initializes the value for the
            [`noAutoVersionResources`](AndroidBundleDescriptionArg.html#isNoAutoVersionResources())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`noAutoVersionResources`](AndroidBundleDescriptionArg.html#isNoAutoVersionResources()).*
            :::

            [Parameters:]{.paramLabel}
            :   `noAutoVersionResources` - The value for
                noAutoVersionResources

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setNoVersionTransitionsResources(boolean)}

        -   #### setNoVersionTransitionsResources

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder setNoVersionTransitionsResources​(boolean noVersionTransitionsResources)
            ```

            ::: block
            Initializes the value for the
            [`noVersionTransitionsResources`](AndroidBundleDescriptionArg.html#isNoVersionTransitionsResources())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`noVersionTransitionsResources`](AndroidBundleDescriptionArg.html#isNoVersionTransitionsResources()).*
            :::

            [Parameters:]{.paramLabel}
            :   `noVersionTransitionsResources` - The value for
                noVersionTransitionsResources

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setNoAutoAddOverlayResources(boolean)}

        -   #### setNoAutoAddOverlayResources

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder setNoAutoAddOverlayResources​(boolean noAutoAddOverlayResources)
            ```

            ::: block
            Initializes the value for the
            [`noAutoAddOverlayResources`](AndroidBundleDescriptionArg.html#isNoAutoAddOverlayResources())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`noAutoAddOverlayResources`](AndroidBundleDescriptionArg.html#isNoAutoAddOverlayResources()).*
            :::

            [Parameters:]{.paramLabel}
            :   `noAutoAddOverlayResources` - The value for
                noAutoAddOverlayResources

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addApplicationModuleTargets(com.facebook.buck.core.model.BuildTarget)}

        -   #### addApplicationModuleTargets

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder addApplicationModuleTargets​(BuildTarget element)
            ```

            ::: block
            Adds one element to
            [`applicationModuleTargets`](AndroidBundleDescriptionArg.html#getApplicationModuleTargets())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A applicationModuleTargets element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addApplicationModuleTargets(com.facebook.buck.core.model.BuildTarget...)}

        -   #### addApplicationModuleTargets

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder addApplicationModuleTargets​(BuildTarget... elements)
            ```

            ::: block
            Adds elements to
            [`applicationModuleTargets`](AndroidBundleDescriptionArg.html#getApplicationModuleTargets())
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
            public final AndroidBundleDescriptionArg.Builder setApplicationModuleTargets​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`applicationModuleTargets`](AndroidBundleDescriptionArg.html#getApplicationModuleTargets())
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
            public final AndroidBundleDescriptionArg.Builder addAllApplicationModuleTargets​(Iterable<? extends BuildTarget> elements)
            ```

            ::: block
            Adds elements to
            [`applicationModuleTargets`](AndroidBundleDescriptionArg.html#getApplicationModuleTargets())
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
            public final AndroidBundleDescriptionArg.Builder putApplicationModuleConfigs​(String key,
                                                                                         com.google.common.collect.ImmutableList<BuildTarget> value)
            ```

            ::: block
            Put one entry to the
            [`applicationModuleConfigs`](AndroidBundleDescriptionArg.html#getApplicationModuleConfigs())
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
            public final AndroidBundleDescriptionArg.Builder putApplicationModuleConfigs​(Map.Entry<String,​? extends com.google.common.collect.ImmutableList<BuildTarget>> entry)
            ```

            ::: block
            Put one entry to the
            [`applicationModuleConfigs`](AndroidBundleDescriptionArg.html#getApplicationModuleConfigs())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entry` - The key and value entry

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setApplicationModuleConfigs(java.util.Map)}

        -   #### setApplicationModuleConfigs

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder setApplicationModuleConfigs​(Map<String,​? extends com.google.common.collect.ImmutableList<BuildTarget>> entries)
            ```

            ::: block
            Sets or replaces all mappings from the specified map as
            entries for the
            [`applicationModuleConfigs`](AndroidBundleDescriptionArg.html#getApplicationModuleConfigs())
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
            public final AndroidBundleDescriptionArg.Builder putAllApplicationModuleConfigs​(Map<String,​? extends com.google.common.collect.ImmutableList<BuildTarget>> entries)
            ```

            ::: block
            Put all mappings from the specified map as entries to
            [`applicationModuleConfigs`](AndroidBundleDescriptionArg.html#getApplicationModuleConfigs())
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
            public final AndroidBundleDescriptionArg.Builder addApplicationModulesWithResources​(String element)
            ```

            ::: block
            Adds one element to
            [`applicationModulesWithResources`](AndroidBundleDescriptionArg.html#getApplicationModulesWithResources())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A applicationModulesWithResources element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addApplicationModulesWithResources(java.lang.String...)}

        -   #### addApplicationModulesWithResources

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder addApplicationModulesWithResources​(String... elements)
            ```

            ::: block
            Adds elements to
            [`applicationModulesWithResources`](AndroidBundleDescriptionArg.html#getApplicationModulesWithResources())
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
            public final AndroidBundleDescriptionArg.Builder setApplicationModulesWithResources​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`applicationModulesWithResources`](AndroidBundleDescriptionArg.html#getApplicationModulesWithResources())
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
            public final AndroidBundleDescriptionArg.Builder addAllApplicationModulesWithResources​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`applicationModulesWithResources`](AndroidBundleDescriptionArg.html#getApplicationModulesWithResources())
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
            public final AndroidBundleDescriptionArg.Builder addApplicationModulesWithManifest​(String element)
            ```

            ::: block
            Adds one element to
            [`applicationModulesWithManifest`](AndroidBundleDescriptionArg.html#getApplicationModulesWithManifest())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A applicationModulesWithManifest element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addApplicationModulesWithManifest(java.lang.String...)}

        -   #### addApplicationModulesWithManifest

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder addApplicationModulesWithManifest​(String... elements)
            ```

            ::: block
            Adds elements to
            [`applicationModulesWithManifest`](AndroidBundleDescriptionArg.html#getApplicationModulesWithManifest())
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
            public final AndroidBundleDescriptionArg.Builder setApplicationModulesWithManifest​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`applicationModulesWithManifest`](AndroidBundleDescriptionArg.html#getApplicationModulesWithManifest())
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
            public final AndroidBundleDescriptionArg.Builder addAllApplicationModulesWithManifest​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`applicationModulesWithManifest`](AndroidBundleDescriptionArg.html#getApplicationModulesWithManifest())
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
            public final AndroidBundleDescriptionArg.Builder setApplicationModuleDependencies​(com.google.common.collect.ImmutableMap<String,​com.google.common.collect.ImmutableList<String>> applicationModuleDependencies)
            ```

            ::: block
            Initializes the optional value
            [`applicationModuleDependencies`](AndroidBundleDescriptionArg.html#getApplicationModuleDependencies())
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
            public final AndroidBundleDescriptionArg.Builder setApplicationModuleDependencies​(Optional<? extends com.google.common.collect.ImmutableMap<String,​com.google.common.collect.ImmutableList<String>>> applicationModuleDependencies)
            ```

            ::: block
            Initializes the optional value
            [`applicationModuleDependencies`](AndroidBundleDescriptionArg.html#getApplicationModuleDependencies())
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
            public final AndroidBundleDescriptionArg.Builder setIsCacheable​(boolean isCacheable)
            ```

            ::: block
            Initializes the value for the
            [`isCacheable`](AndroidBundleDescriptionArg.html#getIsCacheable())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`isCacheable`](AndroidBundleDescriptionArg.html#getIsCacheable()).*
            :::

            [Parameters:]{.paramLabel}
            :   `isCacheable` - The value for isCacheable

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAdditionalAaptParams(java.lang.String)}

        -   #### addAdditionalAaptParams

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder addAdditionalAaptParams​(String element)
            ```

            ::: block
            Adds one element to
            [`additionalAaptParams`](AndroidBundleDescriptionArg.html#getAdditionalAaptParams())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A additionalAaptParams element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAdditionalAaptParams(java.lang.String...)}

        -   #### addAdditionalAaptParams

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder addAdditionalAaptParams​(String... elements)
            ```

            ::: block
            Adds elements to
            [`additionalAaptParams`](AndroidBundleDescriptionArg.html#getAdditionalAaptParams())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of additionalAaptParams elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setAdditionalAaptParams(java.lang.Iterable)}

        -   #### setAdditionalAaptParams

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder setAdditionalAaptParams​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`additionalAaptParams`](AndroidBundleDescriptionArg.html#getAdditionalAaptParams())
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
            public final AndroidBundleDescriptionArg.Builder addAllAdditionalAaptParams​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`additionalAaptParams`](AndroidBundleDescriptionArg.html#getAdditionalAaptParams())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of additionalAaptParams
                elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setTrimResourceIds(boolean)}

        -   #### setTrimResourceIds

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder setTrimResourceIds​(boolean trimResourceIds)
            ```

            ::: block
            Initializes the value for the
            [`trimResourceIds`](AndroidBundleDescriptionArg.html#isTrimResourceIds())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`trimResourceIds`](AndroidBundleDescriptionArg.html#isTrimResourceIds()).*
            :::

            [Parameters:]{.paramLabel}
            :   `trimResourceIds` - The value for trimResourceIds

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setAllowRDotJavaInSecondaryDex(boolean)}

        -   #### setAllowRDotJavaInSecondaryDex

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder setAllowRDotJavaInSecondaryDex​(boolean allowRDotJavaInSecondaryDex)
            ```

            ::: block
            Initializes the value for the
            [`allowRDotJavaInSecondaryDex`](AndroidBundleDescriptionArg.html#isAllowRDotJavaInSecondaryDex())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`allowRDotJavaInSecondaryDex`](AndroidBundleDescriptionArg.html#isAllowRDotJavaInSecondaryDex()).*
            :::

            [Parameters:]{.paramLabel}
            :   `allowRDotJavaInSecondaryDex` - The value for
                allowRDotJavaInSecondaryDex

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setKeepResourcePattern(java.lang.String)}

        -   #### setKeepResourcePattern

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder setKeepResourcePattern​(String keepResourcePattern)
            ```

            ::: block
            Initializes the optional value
            [`keepResourcePattern`](AndroidBundleDescriptionArg.html#getKeepResourcePattern())
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
            public final AndroidBundleDescriptionArg.Builder setKeepResourcePattern​(Optional<String> keepResourcePattern)
            ```

            ::: block
            Initializes the optional value
            [`keepResourcePattern`](AndroidBundleDescriptionArg.html#getKeepResourcePattern())
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
            public final AndroidBundleDescriptionArg.Builder setResourceUnionPackage​(String resourceUnionPackage)
            ```

            ::: block
            Initializes the optional value
            [`resourceUnionPackage`](AndroidBundleDescriptionArg.html#getResourceUnionPackage())
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
            public final AndroidBundleDescriptionArg.Builder setResourceUnionPackage​(Optional<String> resourceUnionPackage)
            ```

            ::: block
            Initializes the optional value
            [`resourceUnionPackage`](AndroidBundleDescriptionArg.html#getResourceUnionPackage())
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
            public final AndroidBundleDescriptionArg.Builder addLocales​(String element)
            ```

            ::: block
            Adds one element to
            [`locales`](AndroidBundleDescriptionArg.html#getLocales())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A locales element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addLocales(java.lang.String...)}

        -   #### addLocales

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder addLocales​(String... elements)
            ```

            ::: block
            Adds elements to
            [`locales`](AndroidBundleDescriptionArg.html#getLocales())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of locales elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLocales(java.lang.Iterable)}

        -   #### setLocales

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder setLocales​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`locales`](AndroidBundleDescriptionArg.html#getLocales())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of locales elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllLocales(java.lang.Iterable)}

        -   #### addAllLocales

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder addAllLocales​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`locales`](AndroidBundleDescriptionArg.html#getLocales())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of locales elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setAapt2LocaleFiltering(boolean)}

        -   #### setAapt2LocaleFiltering

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder setAapt2LocaleFiltering​(boolean aapt2LocaleFiltering)
            ```

            ::: block
            Initializes the value for the
            [`aapt2LocaleFiltering`](AndroidBundleDescriptionArg.html#isAapt2LocaleFiltering())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`aapt2LocaleFiltering`](AndroidBundleDescriptionArg.html#isAapt2LocaleFiltering()).*
            :::

            [Parameters:]{.paramLabel}
            :   `aapt2LocaleFiltering` - The value for
                aapt2LocaleFiltering

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setLocalizedStringFileName(java.lang.String)}

        -   #### setLocalizedStringFileName

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder setLocalizedStringFileName​(String localizedStringFileName)
            ```

            ::: block
            Initializes the optional value
            [`localizedStringFileName`](AndroidBundleDescriptionArg.html#getLocalizedStringFileName())
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
            public final AndroidBundleDescriptionArg.Builder setLocalizedStringFileName​(Optional<String> localizedStringFileName)
            ```

            ::: block
            Initializes the optional value
            [`localizedStringFileName`](AndroidBundleDescriptionArg.html#getLocalizedStringFileName())
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
            public final AndroidBundleDescriptionArg.Builder setBuildStringSourceMap​(boolean buildStringSourceMap)
            ```

            ::: block
            Initializes the value for the
            [`buildStringSourceMap`](AndroidBundleDescriptionArg.html#isBuildStringSourceMap())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`buildStringSourceMap`](AndroidBundleDescriptionArg.html#isBuildStringSourceMap()).*
            :::

            [Parameters:]{.paramLabel}
            :   `buildStringSourceMap` - The value for
                buildStringSourceMap

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setIgnoreAaptProguardConfig(boolean)}

        -   #### setIgnoreAaptProguardConfig

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder setIgnoreAaptProguardConfig​(boolean ignoreAaptProguardConfig)
            ```

            ::: block
            Initializes the value for the
            [`ignoreAaptProguardConfig`](AndroidBundleDescriptionArg.html#isIgnoreAaptProguardConfig())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`ignoreAaptProguardConfig`](AndroidBundleDescriptionArg.html#isIgnoreAaptProguardConfig()).*
            :::

            [Parameters:]{.paramLabel}
            :   `ignoreAaptProguardConfig` - The value for
                ignoreAaptProguardConfig

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCpuFilters(com.facebook.buck.android.toolchain.ndk.TargetCpuType)}

        -   #### addCpuFilters

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder addCpuFilters​(TargetCpuType element)
            ```

            ::: block
            Adds one element to
            [`cpuFilters`](AndroidBundleDescriptionArg.html#getCpuFilters())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A cpuFilters element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addCpuFilters(com.facebook.buck.android.toolchain.ndk.TargetCpuType...)}

        -   #### addCpuFilters

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder addCpuFilters​(TargetCpuType... elements)
            ```

            ::: block
            Adds elements to
            [`cpuFilters`](AndroidBundleDescriptionArg.html#getCpuFilters())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of cpuFilters elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setCpuFilters(java.lang.Iterable)}

        -   #### setCpuFilters

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder setCpuFilters​(Iterable<TargetCpuType> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`cpuFilters`](AndroidBundleDescriptionArg.html#getCpuFilters())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of cpuFilters elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllCpuFilters(java.lang.Iterable)}

        -   #### addAllCpuFilters

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder addAllCpuFilters​(Iterable<TargetCpuType> elements)
            ```

            ::: block
            Adds elements to
            [`cpuFilters`](AndroidBundleDescriptionArg.html#getCpuFilters())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of cpuFilters elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPreprocessJavaClassesBash(com.facebook.buck.rules.macros.StringWithMacros)}

        -   #### setPreprocessJavaClassesBash

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder setPreprocessJavaClassesBash​(StringWithMacros preprocessJavaClassesBash)
            ```

            ::: block
            Initializes the optional value
            [`preprocessJavaClassesBash`](AndroidBundleDescriptionArg.html#getPreprocessJavaClassesBash())
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
            public final AndroidBundleDescriptionArg.Builder setPreprocessJavaClassesBash​(Optional<? extends StringWithMacros> preprocessJavaClassesBash)
            ```

            ::: block
            Initializes the optional value
            [`preprocessJavaClassesBash`](AndroidBundleDescriptionArg.html#getPreprocessJavaClassesBash())
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
            public final AndroidBundleDescriptionArg.Builder setReorderClassesIntraDex​(boolean reorderClassesIntraDex)
            ```

            ::: block
            Initializes the value for the
            [`reorderClassesIntraDex`](AndroidBundleDescriptionArg.html#isReorderClassesIntraDex())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`reorderClassesIntraDex`](AndroidBundleDescriptionArg.html#isReorderClassesIntraDex()).*
            :::

            [Parameters:]{.paramLabel}
            :   `reorderClassesIntraDex` - The value for
                reorderClassesIntraDex

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDexTool(java.lang.String)}

        -   #### setDexTool

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder setDexTool​(String dexTool)
            ```

            ::: block
            Initializes the value for the
            [`dexTool`](AndroidBundleDescriptionArg.html#getDexTool())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`dexTool`](AndroidBundleDescriptionArg.html#getDexTool()).*
            :::

            [Parameters:]{.paramLabel}
            :   `dexTool` - The value for dexTool

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDexReorderToolFile(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setDexReorderToolFile

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder setDexReorderToolFile​(SourcePath dexReorderToolFile)
            ```

            ::: block
            Initializes the optional value
            [`dexReorderToolFile`](AndroidBundleDescriptionArg.html#getDexReorderToolFile())
            to dexReorderToolFile.
            :::

            [Parameters:]{.paramLabel}
            :   `dexReorderToolFile` - The value for dexReorderToolFile

            [Returns:]{.returnLabel}
            :   `this` builder for chained invocation

        []{#setDexReorderToolFile(java.util.Optional)}

        -   #### setDexReorderToolFile

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder setDexReorderToolFile​(Optional<? extends SourcePath> dexReorderToolFile)
            ```

            ::: block
            Initializes the optional value
            [`dexReorderToolFile`](AndroidBundleDescriptionArg.html#getDexReorderToolFile())
            to dexReorderToolFile.
            :::

            [Parameters:]{.paramLabel}
            :   `dexReorderToolFile` - The value for dexReorderToolFile

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setDexReorderDataDumpFile(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setDexReorderDataDumpFile

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder setDexReorderDataDumpFile​(SourcePath dexReorderDataDumpFile)
            ```

            ::: block
            Initializes the optional value
            [`dexReorderDataDumpFile`](AndroidBundleDescriptionArg.html#getDexReorderDataDumpFile())
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
            public final AndroidBundleDescriptionArg.Builder setDexReorderDataDumpFile​(Optional<? extends SourcePath> dexReorderDataDumpFile)
            ```

            ::: block
            Initializes the optional value
            [`dexReorderDataDumpFile`](AndroidBundleDescriptionArg.html#getDexReorderDataDumpFile())
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
            public final AndroidBundleDescriptionArg.Builder putNativeLibraryMergeMap​(String key,
                                                                                      List<Pattern> value)
            ```

            ::: block
            Put one entry to the
            [`nativeLibraryMergeMap`](AndroidBundleDescriptionArg.html#getNativeLibraryMergeMap())
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
            public final AndroidBundleDescriptionArg.Builder putNativeLibraryMergeMap​(Map.Entry<String,​? extends List<Pattern>> entry)
            ```

            ::: block
            Put one entry to the
            [`nativeLibraryMergeMap`](AndroidBundleDescriptionArg.html#getNativeLibraryMergeMap())
            map. Nulls are not permitted
            :::

            [Parameters:]{.paramLabel}
            :   `entry` - The key and value entry

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setNativeLibraryMergeMap(java.util.Map)}

        -   #### setNativeLibraryMergeMap

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder setNativeLibraryMergeMap​(Map<String,​? extends List<Pattern>> entries)
            ```

            ::: block
            Sets or replaces all mappings from the specified map as
            entries for the
            [`nativeLibraryMergeMap`](AndroidBundleDescriptionArg.html#getNativeLibraryMergeMap())
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
            public final AndroidBundleDescriptionArg.Builder putAllNativeLibraryMergeMap​(Map<String,​? extends List<Pattern>> entries)
            ```

            ::: block
            Put all mappings from the specified map as entries to
            [`nativeLibraryMergeMap`](AndroidBundleDescriptionArg.html#getNativeLibraryMergeMap())
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
            public final AndroidBundleDescriptionArg.Builder setNativeLibraryMergeGlue​(BuildTarget nativeLibraryMergeGlue)
            ```

            ::: block
            Initializes the optional value
            [`nativeLibraryMergeGlue`](AndroidBundleDescriptionArg.html#getNativeLibraryMergeGlue())
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
            public final AndroidBundleDescriptionArg.Builder setNativeLibraryMergeGlue​(Optional<? extends BuildTarget> nativeLibraryMergeGlue)
            ```

            ::: block
            Initializes the optional value
            [`nativeLibraryMergeGlue`](AndroidBundleDescriptionArg.html#getNativeLibraryMergeGlue())
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
            public final AndroidBundleDescriptionArg.Builder setNativeLibraryMergeCodeGenerator​(BuildTarget nativeLibraryMergeCodeGenerator)
            ```

            ::: block
            Initializes the optional value
            [`nativeLibraryMergeCodeGenerator`](AndroidBundleDescriptionArg.html#getNativeLibraryMergeCodeGenerator())
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
            public final AndroidBundleDescriptionArg.Builder setNativeLibraryMergeCodeGenerator​(Optional<? extends BuildTarget> nativeLibraryMergeCodeGenerator)
            ```

            ::: block
            Initializes the optional value
            [`nativeLibraryMergeCodeGenerator`](AndroidBundleDescriptionArg.html#getNativeLibraryMergeCodeGenerator())
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
            public final AndroidBundleDescriptionArg.Builder setNativeLibraryMergeLocalizedSymbols​(com.google.common.collect.ImmutableSortedSet<String> nativeLibraryMergeLocalizedSymbols)
            ```

            ::: block
            Initializes the optional value
            [`nativeLibraryMergeLocalizedSymbols`](AndroidBundleDescriptionArg.html#getNativeLibraryMergeLocalizedSymbols())
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
            public final AndroidBundleDescriptionArg.Builder setNativeLibraryMergeLocalizedSymbols​(Optional<? extends com.google.common.collect.ImmutableSortedSet<String>> nativeLibraryMergeLocalizedSymbols)
            ```

            ::: block
            Initializes the optional value
            [`nativeLibraryMergeLocalizedSymbols`](AndroidBundleDescriptionArg.html#getNativeLibraryMergeLocalizedSymbols())
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
            public final AndroidBundleDescriptionArg.Builder setNativeLibraryProguardConfigGenerator​(BuildTarget nativeLibraryProguardConfigGenerator)
            ```

            ::: block
            Initializes the optional value
            [`nativeLibraryProguardConfigGenerator`](AndroidBundleDescriptionArg.html#getNativeLibraryProguardConfigGenerator())
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
            public final AndroidBundleDescriptionArg.Builder setNativeLibraryProguardConfigGenerator​(Optional<? extends BuildTarget> nativeLibraryProguardConfigGenerator)
            ```

            ::: block
            Initializes the optional value
            [`nativeLibraryProguardConfigGenerator`](AndroidBundleDescriptionArg.html#getNativeLibraryProguardConfigGenerator())
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
            public final AndroidBundleDescriptionArg.Builder setEnableRelinker​(boolean enableRelinker)
            ```

            ::: block
            Initializes the value for the
            [`enableRelinker`](AndroidBundleDescriptionArg.html#isEnableRelinker())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`enableRelinker`](AndroidBundleDescriptionArg.html#isEnableRelinker()).*
            :::

            [Parameters:]{.paramLabel}
            :   `enableRelinker` - The value for enableRelinker

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addRelinkerWhitelist(java.util.regex.Pattern)}

        -   #### addRelinkerWhitelist

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder addRelinkerWhitelist​(Pattern element)
            ```

            ::: block
            Adds one element to
            [`relinkerWhitelist`](AndroidBundleDescriptionArg.html#getRelinkerWhitelist())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A relinkerWhitelist element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addRelinkerWhitelist(java.util.regex.Pattern...)}

        -   #### addRelinkerWhitelist

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder addRelinkerWhitelist​(Pattern... elements)
            ```

            ::: block
            Adds elements to
            [`relinkerWhitelist`](AndroidBundleDescriptionArg.html#getRelinkerWhitelist())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of relinkerWhitelist elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setRelinkerWhitelist(java.lang.Iterable)}

        -   #### setRelinkerWhitelist

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder setRelinkerWhitelist​(Iterable<? extends Pattern> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`relinkerWhitelist`](AndroidBundleDescriptionArg.html#getRelinkerWhitelist())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of relinkerWhitelist elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllRelinkerWhitelist(java.lang.Iterable)}

        -   #### addAllRelinkerWhitelist

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder addAllRelinkerWhitelist​(Iterable<? extends Pattern> elements)
            ```

            ::: block
            Adds elements to
            [`relinkerWhitelist`](AndroidBundleDescriptionArg.html#getRelinkerWhitelist())
            list.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An iterable of relinkerWhitelist elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setManifestEntries(com.facebook.buck.rules.coercer.ManifestEntries)}

        -   #### setManifestEntries

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder setManifestEntries​(ManifestEntries manifestEntries)
            ```

            ::: block
            Initializes the value for the
            [`manifestEntries`](AndroidBundleDescriptionArg.html#getManifestEntries())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`manifestEntries`](AndroidBundleDescriptionArg.html#getManifestEntries()).*
            :::

            [Parameters:]{.paramLabel}
            :   `manifestEntries` - The value for manifestEntries

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setBuildConfigValues(com.facebook.buck.rules.coercer.BuildConfigFields)}

        -   #### setBuildConfigValues

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder setBuildConfigValues​(BuildConfigFields buildConfigValues)
            ```

            ::: block
            Initializes the value for the
            [`buildConfigValues`](AndroidBundleDescriptionArg.html#getBuildConfigValues())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`buildConfigValues`](AndroidBundleDescriptionArg.html#getBuildConfigValues()).*
            :::

            [Parameters:]{.paramLabel}
            :   `buildConfigValues` - The value for buildConfigValues

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setPostFilterResourcesCmd(com.facebook.buck.rules.macros.StringWithMacros)}

        -   #### setPostFilterResourcesCmd

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder setPostFilterResourcesCmd​(StringWithMacros postFilterResourcesCmd)
            ```

            ::: block
            Initializes the optional value
            [`postFilterResourcesCmd`](AndroidBundleDescriptionArg.html#getPostFilterResourcesCmd())
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
            public final AndroidBundleDescriptionArg.Builder setPostFilterResourcesCmd​(Optional<? extends StringWithMacros> postFilterResourcesCmd)
            ```

            ::: block
            Initializes the optional value
            [`postFilterResourcesCmd`](AndroidBundleDescriptionArg.html#getPostFilterResourcesCmd())
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
            public final AndroidBundleDescriptionArg.Builder setBuildConfigValuesFile​(SourcePath buildConfigValuesFile)
            ```

            ::: block
            Initializes the optional value
            [`buildConfigValuesFile`](AndroidBundleDescriptionArg.html#getBuildConfigValuesFile())
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
            public final AndroidBundleDescriptionArg.Builder setBuildConfigValuesFile​(Optional<? extends SourcePath> buildConfigValuesFile)
            ```

            ::: block
            Initializes the optional value
            [`buildConfigValuesFile`](AndroidBundleDescriptionArg.html#getBuildConfigValuesFile())
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
            public final AndroidBundleDescriptionArg.Builder setSkipProguard​(boolean skipProguard)
            ```

            ::: block
            Initializes the value for the
            [`skipProguard`](AndroidBundleDescriptionArg.html#isSkipProguard())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`skipProguard`](AndroidBundleDescriptionArg.html#isSkipProguard()).*
            :::

            [Parameters:]{.paramLabel}
            :   `skipProguard` - The value for skipProguard

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setUseDynamicFeature(boolean)}

        -   #### setUseDynamicFeature

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder setUseDynamicFeature​(boolean useDynamicFeature)
            ```

            ::: block
            Initializes the value for the
            [`useDynamicFeature`](AndroidBundleDescriptionArg.html#getUseDynamicFeature())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`useDynamicFeature`](AndroidBundleDescriptionArg.html#getUseDynamicFeature()).*
            :::

            [Parameters:]{.paramLabel}
            :   `useDynamicFeature` - The value for useDynamicFeature

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addExtraFilteredResources(java.lang.String)}

        -   #### addExtraFilteredResources

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder addExtraFilteredResources​(String element)
            ```

            ::: block
            Adds one element to
            [`extraFilteredResources`](AndroidBundleDescriptionArg.html#getExtraFilteredResources())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A extraFilteredResources element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addExtraFilteredResources(java.lang.String...)}

        -   #### addExtraFilteredResources

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder addExtraFilteredResources​(String... elements)
            ```

            ::: block
            Adds elements to
            [`extraFilteredResources`](AndroidBundleDescriptionArg.html#getExtraFilteredResources())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `elements` - An array of extraFilteredResources elements

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#setExtraFilteredResources(java.lang.Iterable)}

        -   #### setExtraFilteredResources

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder setExtraFilteredResources​(Iterable<String> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`extraFilteredResources`](AndroidBundleDescriptionArg.html#getExtraFilteredResources())
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
            public final AndroidBundleDescriptionArg.Builder addAllExtraFilteredResources​(Iterable<String> elements)
            ```

            ::: block
            Adds elements to
            [`extraFilteredResources`](AndroidBundleDescriptionArg.html#getExtraFilteredResources())
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
            public final AndroidBundleDescriptionArg.Builder setDuplicateResourceBehavior​(HasDuplicateAndroidResourceTypes.DuplicateResourceBehaviour duplicateResourceBehavior)
            ```

            ::: block
            Initializes the value for the
            [`duplicateResourceBehavior`](AndroidBundleDescriptionArg.html#getDuplicateResourceBehavior())
            attribute.
            *If not set, this attribute will have a default value as
            returned by the initializer of
            [`duplicateResourceBehavior`](AndroidBundleDescriptionArg.html#getDuplicateResourceBehavior()).*
            :::

            [Parameters:]{.paramLabel}
            :   `duplicateResourceBehavior` - The value for
                duplicateResourceBehavior

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllowedDuplicateResourceTypes(com.facebook.buck.android.aapt.RDotTxtEntry.RType)}

        -   #### addAllowedDuplicateResourceTypes

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder addAllowedDuplicateResourceTypes​(RDotTxtEntry.RType element)
            ```

            ::: block
            Adds one element to
            [`allowedDuplicateResourceTypes`](AndroidBundleDescriptionArg.html#getAllowedDuplicateResourceTypes())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A allowedDuplicateResourceTypes element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addAllowedDuplicateResourceTypes(com.facebook.buck.android.aapt.RDotTxtEntry.RType...)}

        -   #### addAllowedDuplicateResourceTypes

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder addAllowedDuplicateResourceTypes​(RDotTxtEntry.RType... elements)
            ```

            ::: block
            Adds elements to
            [`allowedDuplicateResourceTypes`](AndroidBundleDescriptionArg.html#getAllowedDuplicateResourceTypes())
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
            public final AndroidBundleDescriptionArg.Builder setAllowedDuplicateResourceTypes​(Iterable<RDotTxtEntry.RType> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`allowedDuplicateResourceTypes`](AndroidBundleDescriptionArg.html#getAllowedDuplicateResourceTypes())
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
            public final AndroidBundleDescriptionArg.Builder addAllAllowedDuplicateResourceTypes​(Iterable<RDotTxtEntry.RType> elements)
            ```

            ::: block
            Adds elements to
            [`allowedDuplicateResourceTypes`](AndroidBundleDescriptionArg.html#getAllowedDuplicateResourceTypes())
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
            public final AndroidBundleDescriptionArg.Builder addBannedDuplicateResourceTypes​(RDotTxtEntry.RType element)
            ```

            ::: block
            Adds one element to
            [`bannedDuplicateResourceTypes`](AndroidBundleDescriptionArg.html#getBannedDuplicateResourceTypes())
            set.
            :::

            [Parameters:]{.paramLabel}
            :   `element` - A bannedDuplicateResourceTypes element

            [Returns:]{.returnLabel}
            :   `this` builder for use in a chained invocation

        []{#addBannedDuplicateResourceTypes(com.facebook.buck.android.aapt.RDotTxtEntry.RType...)}

        -   #### addBannedDuplicateResourceTypes

            ``` methodSignature
            public final AndroidBundleDescriptionArg.Builder addBannedDuplicateResourceTypes​(RDotTxtEntry.RType... elements)
            ```

            ::: block
            Adds elements to
            [`bannedDuplicateResourceTypes`](AndroidBundleDescriptionArg.html#getBannedDuplicateResourceTypes())
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
            public final AndroidBundleDescriptionArg.Builder setBannedDuplicateResourceTypes​(Iterable<RDotTxtEntry.RType> elements)
            ```

            ::: block
            Sets or replaces all elements for
            [`bannedDuplicateResourceTypes`](AndroidBundleDescriptionArg.html#getBannedDuplicateResourceTypes())
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
            public final AndroidBundleDescriptionArg.Builder addAllBannedDuplicateResourceTypes​(Iterable<RDotTxtEntry.RType> elements)
            ```

            ::: block
            Adds elements to
            [`bannedDuplicateResourceTypes`](AndroidBundleDescriptionArg.html#getBannedDuplicateResourceTypes())
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
            public final AndroidBundleDescriptionArg.Builder setDuplicateResourceWhitelist​(SourcePath duplicateResourceWhitelist)
            ```

            ::: block
            Initializes the optional value
            [`duplicateResourceWhitelist`](AndroidBundleDescriptionArg.html#getDuplicateResourceWhitelist())
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
            public final AndroidBundleDescriptionArg.Builder setDuplicateResourceWhitelist​(Optional<? extends SourcePath> duplicateResourceWhitelist)
            ```

            ::: block
            Initializes the optional value
            [`duplicateResourceWhitelist`](AndroidBundleDescriptionArg.html#getDuplicateResourceWhitelist())
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
            public final AndroidBundleDescriptionArg.Builder setApplicationModuleBlacklist​(List<Query> applicationModuleBlacklist)
            ```

            ::: block
            Initializes the optional value
            [`applicationModuleBlacklist`](AndroidBundleDescriptionArg.html#getApplicationModuleBlacklist())
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
            public final AndroidBundleDescriptionArg.Builder setApplicationModuleBlacklist​(Optional<? extends List<Query>> applicationModuleBlacklist)
            ```

            ::: block
            Initializes the optional value
            [`applicationModuleBlacklist`](AndroidBundleDescriptionArg.html#getApplicationModuleBlacklist())
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
            public AndroidBundleDescriptionArg build()
            ```

            ::: block
            Builds a new
            [`AndroidBundleDescriptionArg`](AndroidBundleDescriptionArg.html "class in com.facebook.buck.android").
            :::

            [Returns:]{.returnLabel}
            :   An immutable instance of AndroidBundleDescriptionArg

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
