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
-   Tree
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

[]{#skip.navbar.top}
:::
:::

::: navPadding
 
:::
:::

::: {role="main"}
::: header
# Hierarchy For Package com.facebook.buck.jvm.core {#hierarchy-for-package-com.facebook.buck.jvm.core .title}

[Package Hierarchies:]{.packageHierarchyLabel}

-   [All Packages](../../../../../overview-tree.html)
:::

::: contentContainer
::: {.section role="region"}
## Class Hierarchy {#class-hierarchy title="Class Hierarchy"}

-   java.lang.[[Object]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}
    -   com.facebook.buck.jvm.core.[[DefaultJavaAbiInfo]{.typeNameLink}](DefaultJavaAbiInfo.html "class in com.facebook.buck.jvm.core")
        (implements
        com.facebook.buck.jvm.core.[JavaAbiInfo](JavaAbiInfo.html "interface in com.facebook.buck.jvm.core"))
    -   com.facebook.buck.jvm.core.[[EmptyJavaAbiInfo]{.typeNameLink}](EmptyJavaAbiInfo.html "class in com.facebook.buck.jvm.core")
        (implements
        com.facebook.buck.jvm.core.[JavaAbiInfo](JavaAbiInfo.html "interface in com.facebook.buck.jvm.core"))
    -   com.facebook.buck.jvm.core.[[JavaAbis]{.typeNameLink}](JavaAbis.html "class in com.facebook.buck.jvm.core")
    -   com.facebook.buck.jvm.core.[[JavaLibrary.Data]{.typeNameLink}](JavaLibrary.Data.html "class in com.facebook.buck.jvm.core")
:::

::: {.section role="region"}
## Interface Hierarchy {#interface-hierarchy title="Interface Hierarchy"}

-   com.facebook.buck.core.rulekey.[[AddsToRuleKey]{.typeNameLink}](../../core/rulekey/AddsToRuleKey.html "interface in com.facebook.buck.core.rulekey")
    -   com.facebook.buck.jvm.core.[[JavaClassHashesProvider]{.typeNameLink}](JavaClassHashesProvider.html "interface in com.facebook.buck.jvm.core")
-   com.facebook.buck.core.rulekey.[[AllowsNonAnnotatedFields]{.typeNameLink}](../../core/rulekey/AllowsNonAnnotatedFields.html "interface in com.facebook.buck.core.rulekey")
    -   com.facebook.buck.core.rules.[[BuildRule]{.typeNameLink}](../../core/rules/BuildRule.html "interface in com.facebook.buck.core.rules")
        (also extends
        com.facebook.buck.core.build.action.[BuildEngineAction](../../core/build/action/BuildEngineAction.html "interface in com.facebook.buck.core.build.action"),
        java.lang.[Comparable](http://docs.oracle.com/javase/7/docs/api/java/lang/Comparable.html?is-external=true "class or interface in java.lang"){.externalLink}\<T\>,
        com.facebook.buck.core.rules.[HasNameAndType](../../core/rules/HasNameAndType.html "interface in com.facebook.buck.core.rules"))
        -   com.facebook.buck.jvm.core.[[HasJavaClassHashes]{.typeNameLink}](HasJavaClassHashes.html "interface in com.facebook.buck.jvm.core")
            -   com.facebook.buck.jvm.core.[[JavaLibrary]{.typeNameLink}](JavaLibrary.html "interface in com.facebook.buck.jvm.core")
                (also extends
                com.facebook.buck.jvm.core.[HasClasspathDeps](HasClasspathDeps.html "interface in com.facebook.buck.jvm.core"),
                com.facebook.buck.jvm.core.[HasClasspathEntries](HasClasspathEntries.html "interface in com.facebook.buck.jvm.core"),
                com.facebook.buck.jvm.core.[HasDesugarSupport](HasDesugarSupport.html "interface in com.facebook.buck.jvm.core"),
                com.facebook.buck.jvm.core.[HasJavaAbi](HasJavaAbi.html "interface in com.facebook.buck.jvm.core"),
                com.facebook.buck.jvm.core.[HasMavenCoordinates](HasMavenCoordinates.html "interface in com.facebook.buck.jvm.core"),
                com.facebook.buck.core.rules.attr.[HasRuntimeDeps](../../core/rules/attr/HasRuntimeDeps.html "interface in com.facebook.buck.core.rules.attr"),
                com.facebook.buck.jvm.core.[HasSources](HasSources.html "interface in com.facebook.buck.jvm.core"))
        -   com.facebook.buck.jvm.core.[[HasMavenCoordinates]{.typeNameLink}](HasMavenCoordinates.html "interface in com.facebook.buck.jvm.core")
            -   com.facebook.buck.jvm.core.[[JavaLibrary]{.typeNameLink}](JavaLibrary.html "interface in com.facebook.buck.jvm.core")
                (also extends
                com.facebook.buck.jvm.core.[HasClasspathDeps](HasClasspathDeps.html "interface in com.facebook.buck.jvm.core"),
                com.facebook.buck.jvm.core.[HasClasspathEntries](HasClasspathEntries.html "interface in com.facebook.buck.jvm.core"),
                com.facebook.buck.jvm.core.[HasDesugarSupport](HasDesugarSupport.html "interface in com.facebook.buck.jvm.core"),
                com.facebook.buck.jvm.core.[HasJavaAbi](HasJavaAbi.html "interface in com.facebook.buck.jvm.core"),
                com.facebook.buck.jvm.core.[HasJavaClassHashes](HasJavaClassHashes.html "interface in com.facebook.buck.jvm.core"),
                com.facebook.buck.core.rules.attr.[HasRuntimeDeps](../../core/rules/attr/HasRuntimeDeps.html "interface in com.facebook.buck.core.rules.attr"),
                com.facebook.buck.jvm.core.[HasSources](HasSources.html "interface in com.facebook.buck.jvm.core"))
        -   com.facebook.buck.core.rules.attr.[[HasRuntimeDeps]{.typeNameLink}](../../core/rules/attr/HasRuntimeDeps.html "interface in com.facebook.buck.core.rules.attr")
            -   com.facebook.buck.jvm.core.[[JavaLibrary]{.typeNameLink}](JavaLibrary.html "interface in com.facebook.buck.jvm.core")
                (also extends
                com.facebook.buck.jvm.core.[HasClasspathDeps](HasClasspathDeps.html "interface in com.facebook.buck.jvm.core"),
                com.facebook.buck.jvm.core.[HasClasspathEntries](HasClasspathEntries.html "interface in com.facebook.buck.jvm.core"),
                com.facebook.buck.jvm.core.[HasDesugarSupport](HasDesugarSupport.html "interface in com.facebook.buck.jvm.core"),
                com.facebook.buck.jvm.core.[HasJavaAbi](HasJavaAbi.html "interface in com.facebook.buck.jvm.core"),
                com.facebook.buck.jvm.core.[HasJavaClassHashes](HasJavaClassHashes.html "interface in com.facebook.buck.jvm.core"),
                com.facebook.buck.jvm.core.[HasMavenCoordinates](HasMavenCoordinates.html "interface in com.facebook.buck.jvm.core"),
                com.facebook.buck.jvm.core.[HasSources](HasSources.html "interface in com.facebook.buck.jvm.core"))
-   com.facebook.buck.core.build.action.[[BuildEngineAction]{.typeNameLink}](../../core/build/action/BuildEngineAction.html "interface in com.facebook.buck.core.build.action")
    -   com.facebook.buck.core.rules.[[BuildRule]{.typeNameLink}](../../core/rules/BuildRule.html "interface in com.facebook.buck.core.rules")
        (also extends
        com.facebook.buck.core.rulekey.[AllowsNonAnnotatedFields](../../core/rulekey/AllowsNonAnnotatedFields.html "interface in com.facebook.buck.core.rulekey"),
        java.lang.[Comparable](http://docs.oracle.com/javase/7/docs/api/java/lang/Comparable.html?is-external=true "class or interface in java.lang"){.externalLink}\<T\>,
        com.facebook.buck.core.rules.[HasNameAndType](../../core/rules/HasNameAndType.html "interface in com.facebook.buck.core.rules"))
        -   com.facebook.buck.jvm.core.[[HasJavaClassHashes]{.typeNameLink}](HasJavaClassHashes.html "interface in com.facebook.buck.jvm.core")
            -   com.facebook.buck.jvm.core.[[JavaLibrary]{.typeNameLink}](JavaLibrary.html "interface in com.facebook.buck.jvm.core")
                (also extends
                com.facebook.buck.jvm.core.[HasClasspathDeps](HasClasspathDeps.html "interface in com.facebook.buck.jvm.core"),
                com.facebook.buck.jvm.core.[HasClasspathEntries](HasClasspathEntries.html "interface in com.facebook.buck.jvm.core"),
                com.facebook.buck.jvm.core.[HasDesugarSupport](HasDesugarSupport.html "interface in com.facebook.buck.jvm.core"),
                com.facebook.buck.jvm.core.[HasJavaAbi](HasJavaAbi.html "interface in com.facebook.buck.jvm.core"),
                com.facebook.buck.jvm.core.[HasMavenCoordinates](HasMavenCoordinates.html "interface in com.facebook.buck.jvm.core"),
                com.facebook.buck.core.rules.attr.[HasRuntimeDeps](../../core/rules/attr/HasRuntimeDeps.html "interface in com.facebook.buck.core.rules.attr"),
                com.facebook.buck.jvm.core.[HasSources](HasSources.html "interface in com.facebook.buck.jvm.core"))
        -   com.facebook.buck.jvm.core.[[HasMavenCoordinates]{.typeNameLink}](HasMavenCoordinates.html "interface in com.facebook.buck.jvm.core")
            -   com.facebook.buck.jvm.core.[[JavaLibrary]{.typeNameLink}](JavaLibrary.html "interface in com.facebook.buck.jvm.core")
                (also extends
                com.facebook.buck.jvm.core.[HasClasspathDeps](HasClasspathDeps.html "interface in com.facebook.buck.jvm.core"),
                com.facebook.buck.jvm.core.[HasClasspathEntries](HasClasspathEntries.html "interface in com.facebook.buck.jvm.core"),
                com.facebook.buck.jvm.core.[HasDesugarSupport](HasDesugarSupport.html "interface in com.facebook.buck.jvm.core"),
                com.facebook.buck.jvm.core.[HasJavaAbi](HasJavaAbi.html "interface in com.facebook.buck.jvm.core"),
                com.facebook.buck.jvm.core.[HasJavaClassHashes](HasJavaClassHashes.html "interface in com.facebook.buck.jvm.core"),
                com.facebook.buck.core.rules.attr.[HasRuntimeDeps](../../core/rules/attr/HasRuntimeDeps.html "interface in com.facebook.buck.core.rules.attr"),
                com.facebook.buck.jvm.core.[HasSources](HasSources.html "interface in com.facebook.buck.jvm.core"))
        -   com.facebook.buck.core.rules.attr.[[HasRuntimeDeps]{.typeNameLink}](../../core/rules/attr/HasRuntimeDeps.html "interface in com.facebook.buck.core.rules.attr")
            -   com.facebook.buck.jvm.core.[[JavaLibrary]{.typeNameLink}](JavaLibrary.html "interface in com.facebook.buck.jvm.core")
                (also extends
                com.facebook.buck.jvm.core.[HasClasspathDeps](HasClasspathDeps.html "interface in com.facebook.buck.jvm.core"),
                com.facebook.buck.jvm.core.[HasClasspathEntries](HasClasspathEntries.html "interface in com.facebook.buck.jvm.core"),
                com.facebook.buck.jvm.core.[HasDesugarSupport](HasDesugarSupport.html "interface in com.facebook.buck.jvm.core"),
                com.facebook.buck.jvm.core.[HasJavaAbi](HasJavaAbi.html "interface in com.facebook.buck.jvm.core"),
                com.facebook.buck.jvm.core.[HasJavaClassHashes](HasJavaClassHashes.html "interface in com.facebook.buck.jvm.core"),
                com.facebook.buck.jvm.core.[HasMavenCoordinates](HasMavenCoordinates.html "interface in com.facebook.buck.jvm.core"),
                com.facebook.buck.jvm.core.[HasSources](HasSources.html "interface in com.facebook.buck.jvm.core"))
-   java.lang.[[Comparable]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/Comparable.html?is-external=true "class or interface in java.lang"){.externalLink}\<T\>
    -   com.facebook.buck.core.rules.[[BuildRule]{.typeNameLink}](../../core/rules/BuildRule.html "interface in com.facebook.buck.core.rules")
        (also extends
        com.facebook.buck.core.rulekey.[AllowsNonAnnotatedFields](../../core/rulekey/AllowsNonAnnotatedFields.html "interface in com.facebook.buck.core.rulekey"),
        com.facebook.buck.core.build.action.[BuildEngineAction](../../core/build/action/BuildEngineAction.html "interface in com.facebook.buck.core.build.action"),
        com.facebook.buck.core.rules.[HasNameAndType](../../core/rules/HasNameAndType.html "interface in com.facebook.buck.core.rules"))
        -   com.facebook.buck.jvm.core.[[HasJavaClassHashes]{.typeNameLink}](HasJavaClassHashes.html "interface in com.facebook.buck.jvm.core")
            -   com.facebook.buck.jvm.core.[[JavaLibrary]{.typeNameLink}](JavaLibrary.html "interface in com.facebook.buck.jvm.core")
                (also extends
                com.facebook.buck.jvm.core.[HasClasspathDeps](HasClasspathDeps.html "interface in com.facebook.buck.jvm.core"),
                com.facebook.buck.jvm.core.[HasClasspathEntries](HasClasspathEntries.html "interface in com.facebook.buck.jvm.core"),
                com.facebook.buck.jvm.core.[HasDesugarSupport](HasDesugarSupport.html "interface in com.facebook.buck.jvm.core"),
                com.facebook.buck.jvm.core.[HasJavaAbi](HasJavaAbi.html "interface in com.facebook.buck.jvm.core"),
                com.facebook.buck.jvm.core.[HasMavenCoordinates](HasMavenCoordinates.html "interface in com.facebook.buck.jvm.core"),
                com.facebook.buck.core.rules.attr.[HasRuntimeDeps](../../core/rules/attr/HasRuntimeDeps.html "interface in com.facebook.buck.core.rules.attr"),
                com.facebook.buck.jvm.core.[HasSources](HasSources.html "interface in com.facebook.buck.jvm.core"))
        -   com.facebook.buck.jvm.core.[[HasMavenCoordinates]{.typeNameLink}](HasMavenCoordinates.html "interface in com.facebook.buck.jvm.core")
            -   com.facebook.buck.jvm.core.[[JavaLibrary]{.typeNameLink}](JavaLibrary.html "interface in com.facebook.buck.jvm.core")
                (also extends
                com.facebook.buck.jvm.core.[HasClasspathDeps](HasClasspathDeps.html "interface in com.facebook.buck.jvm.core"),
                com.facebook.buck.jvm.core.[HasClasspathEntries](HasClasspathEntries.html "interface in com.facebook.buck.jvm.core"),
                com.facebook.buck.jvm.core.[HasDesugarSupport](HasDesugarSupport.html "interface in com.facebook.buck.jvm.core"),
                com.facebook.buck.jvm.core.[HasJavaAbi](HasJavaAbi.html "interface in com.facebook.buck.jvm.core"),
                com.facebook.buck.jvm.core.[HasJavaClassHashes](HasJavaClassHashes.html "interface in com.facebook.buck.jvm.core"),
                com.facebook.buck.core.rules.attr.[HasRuntimeDeps](../../core/rules/attr/HasRuntimeDeps.html "interface in com.facebook.buck.core.rules.attr"),
                com.facebook.buck.jvm.core.[HasSources](HasSources.html "interface in com.facebook.buck.jvm.core"))
        -   com.facebook.buck.core.rules.attr.[[HasRuntimeDeps]{.typeNameLink}](../../core/rules/attr/HasRuntimeDeps.html "interface in com.facebook.buck.core.rules.attr")
            -   com.facebook.buck.jvm.core.[[JavaLibrary]{.typeNameLink}](JavaLibrary.html "interface in com.facebook.buck.jvm.core")
                (also extends
                com.facebook.buck.jvm.core.[HasClasspathDeps](HasClasspathDeps.html "interface in com.facebook.buck.jvm.core"),
                com.facebook.buck.jvm.core.[HasClasspathEntries](HasClasspathEntries.html "interface in com.facebook.buck.jvm.core"),
                com.facebook.buck.jvm.core.[HasDesugarSupport](HasDesugarSupport.html "interface in com.facebook.buck.jvm.core"),
                com.facebook.buck.jvm.core.[HasJavaAbi](HasJavaAbi.html "interface in com.facebook.buck.jvm.core"),
                com.facebook.buck.jvm.core.[HasJavaClassHashes](HasJavaClassHashes.html "interface in com.facebook.buck.jvm.core"),
                com.facebook.buck.jvm.core.[HasMavenCoordinates](HasMavenCoordinates.html "interface in com.facebook.buck.jvm.core"),
                com.facebook.buck.jvm.core.[HasSources](HasSources.html "interface in com.facebook.buck.jvm.core"))
-   com.facebook.buck.jvm.core.[[HasClasspathDeps]{.typeNameLink}](HasClasspathDeps.html "interface in com.facebook.buck.jvm.core")
    -   com.facebook.buck.jvm.core.[[JavaLibrary]{.typeNameLink}](JavaLibrary.html "interface in com.facebook.buck.jvm.core")
        (also extends
        com.facebook.buck.jvm.core.[HasClasspathEntries](HasClasspathEntries.html "interface in com.facebook.buck.jvm.core"),
        com.facebook.buck.jvm.core.[HasDesugarSupport](HasDesugarSupport.html "interface in com.facebook.buck.jvm.core"),
        com.facebook.buck.jvm.core.[HasJavaAbi](HasJavaAbi.html "interface in com.facebook.buck.jvm.core"),
        com.facebook.buck.jvm.core.[HasJavaClassHashes](HasJavaClassHashes.html "interface in com.facebook.buck.jvm.core"),
        com.facebook.buck.jvm.core.[HasMavenCoordinates](HasMavenCoordinates.html "interface in com.facebook.buck.jvm.core"),
        com.facebook.buck.core.rules.attr.[HasRuntimeDeps](../../core/rules/attr/HasRuntimeDeps.html "interface in com.facebook.buck.core.rules.attr"),
        com.facebook.buck.jvm.core.[HasSources](HasSources.html "interface in com.facebook.buck.jvm.core"))
-   com.facebook.buck.jvm.core.[[HasClasspathEntries]{.typeNameLink}](HasClasspathEntries.html "interface in com.facebook.buck.jvm.core")
    -   com.facebook.buck.jvm.core.[[JavaLibrary]{.typeNameLink}](JavaLibrary.html "interface in com.facebook.buck.jvm.core")
        (also extends
        com.facebook.buck.jvm.core.[HasClasspathDeps](HasClasspathDeps.html "interface in com.facebook.buck.jvm.core"),
        com.facebook.buck.jvm.core.[HasDesugarSupport](HasDesugarSupport.html "interface in com.facebook.buck.jvm.core"),
        com.facebook.buck.jvm.core.[HasJavaAbi](HasJavaAbi.html "interface in com.facebook.buck.jvm.core"),
        com.facebook.buck.jvm.core.[HasJavaClassHashes](HasJavaClassHashes.html "interface in com.facebook.buck.jvm.core"),
        com.facebook.buck.jvm.core.[HasMavenCoordinates](HasMavenCoordinates.html "interface in com.facebook.buck.jvm.core"),
        com.facebook.buck.core.rules.attr.[HasRuntimeDeps](../../core/rules/attr/HasRuntimeDeps.html "interface in com.facebook.buck.core.rules.attr"),
        com.facebook.buck.jvm.core.[HasSources](HasSources.html "interface in com.facebook.buck.jvm.core"))
-   com.facebook.buck.jvm.core.[[HasDesugarSupport]{.typeNameLink}](HasDesugarSupport.html "interface in com.facebook.buck.jvm.core")
    -   com.facebook.buck.jvm.core.[[JavaLibrary]{.typeNameLink}](JavaLibrary.html "interface in com.facebook.buck.jvm.core")
        (also extends
        com.facebook.buck.jvm.core.[HasClasspathDeps](HasClasspathDeps.html "interface in com.facebook.buck.jvm.core"),
        com.facebook.buck.jvm.core.[HasClasspathEntries](HasClasspathEntries.html "interface in com.facebook.buck.jvm.core"),
        com.facebook.buck.jvm.core.[HasJavaAbi](HasJavaAbi.html "interface in com.facebook.buck.jvm.core"),
        com.facebook.buck.jvm.core.[HasJavaClassHashes](HasJavaClassHashes.html "interface in com.facebook.buck.jvm.core"),
        com.facebook.buck.jvm.core.[HasMavenCoordinates](HasMavenCoordinates.html "interface in com.facebook.buck.jvm.core"),
        com.facebook.buck.core.rules.attr.[HasRuntimeDeps](../../core/rules/attr/HasRuntimeDeps.html "interface in com.facebook.buck.core.rules.attr"),
        com.facebook.buck.jvm.core.[HasSources](HasSources.html "interface in com.facebook.buck.jvm.core"))
-   com.facebook.buck.jvm.core.[[HasJavaAbi]{.typeNameLink}](HasJavaAbi.html "interface in com.facebook.buck.jvm.core")
    -   com.facebook.buck.jvm.core.[[CalculateAbi]{.typeNameLink}](CalculateAbi.html "interface in com.facebook.buck.jvm.core")
    -   com.facebook.buck.jvm.core.[[JavaLibrary]{.typeNameLink}](JavaLibrary.html "interface in com.facebook.buck.jvm.core")
        (also extends
        com.facebook.buck.jvm.core.[HasClasspathDeps](HasClasspathDeps.html "interface in com.facebook.buck.jvm.core"),
        com.facebook.buck.jvm.core.[HasClasspathEntries](HasClasspathEntries.html "interface in com.facebook.buck.jvm.core"),
        com.facebook.buck.jvm.core.[HasDesugarSupport](HasDesugarSupport.html "interface in com.facebook.buck.jvm.core"),
        com.facebook.buck.jvm.core.[HasJavaClassHashes](HasJavaClassHashes.html "interface in com.facebook.buck.jvm.core"),
        com.facebook.buck.jvm.core.[HasMavenCoordinates](HasMavenCoordinates.html "interface in com.facebook.buck.jvm.core"),
        com.facebook.buck.core.rules.attr.[HasRuntimeDeps](../../core/rules/attr/HasRuntimeDeps.html "interface in com.facebook.buck.core.rules.attr"),
        com.facebook.buck.jvm.core.[HasSources](HasSources.html "interface in com.facebook.buck.jvm.core"))
-   com.facebook.buck.core.rules.[[HasNameAndType]{.typeNameLink}](../../core/rules/HasNameAndType.html "interface in com.facebook.buck.core.rules")
    -   com.facebook.buck.core.rules.[[BuildRule]{.typeNameLink}](../../core/rules/BuildRule.html "interface in com.facebook.buck.core.rules")
        (also extends
        com.facebook.buck.core.rulekey.[AllowsNonAnnotatedFields](../../core/rulekey/AllowsNonAnnotatedFields.html "interface in com.facebook.buck.core.rulekey"),
        com.facebook.buck.core.build.action.[BuildEngineAction](../../core/build/action/BuildEngineAction.html "interface in com.facebook.buck.core.build.action"),
        java.lang.[Comparable](http://docs.oracle.com/javase/7/docs/api/java/lang/Comparable.html?is-external=true "class or interface in java.lang"){.externalLink}\<T\>)
        -   com.facebook.buck.jvm.core.[[HasJavaClassHashes]{.typeNameLink}](HasJavaClassHashes.html "interface in com.facebook.buck.jvm.core")
            -   com.facebook.buck.jvm.core.[[JavaLibrary]{.typeNameLink}](JavaLibrary.html "interface in com.facebook.buck.jvm.core")
                (also extends
                com.facebook.buck.jvm.core.[HasClasspathDeps](HasClasspathDeps.html "interface in com.facebook.buck.jvm.core"),
                com.facebook.buck.jvm.core.[HasClasspathEntries](HasClasspathEntries.html "interface in com.facebook.buck.jvm.core"),
                com.facebook.buck.jvm.core.[HasDesugarSupport](HasDesugarSupport.html "interface in com.facebook.buck.jvm.core"),
                com.facebook.buck.jvm.core.[HasJavaAbi](HasJavaAbi.html "interface in com.facebook.buck.jvm.core"),
                com.facebook.buck.jvm.core.[HasMavenCoordinates](HasMavenCoordinates.html "interface in com.facebook.buck.jvm.core"),
                com.facebook.buck.core.rules.attr.[HasRuntimeDeps](../../core/rules/attr/HasRuntimeDeps.html "interface in com.facebook.buck.core.rules.attr"),
                com.facebook.buck.jvm.core.[HasSources](HasSources.html "interface in com.facebook.buck.jvm.core"))
        -   com.facebook.buck.jvm.core.[[HasMavenCoordinates]{.typeNameLink}](HasMavenCoordinates.html "interface in com.facebook.buck.jvm.core")
            -   com.facebook.buck.jvm.core.[[JavaLibrary]{.typeNameLink}](JavaLibrary.html "interface in com.facebook.buck.jvm.core")
                (also extends
                com.facebook.buck.jvm.core.[HasClasspathDeps](HasClasspathDeps.html "interface in com.facebook.buck.jvm.core"),
                com.facebook.buck.jvm.core.[HasClasspathEntries](HasClasspathEntries.html "interface in com.facebook.buck.jvm.core"),
                com.facebook.buck.jvm.core.[HasDesugarSupport](HasDesugarSupport.html "interface in com.facebook.buck.jvm.core"),
                com.facebook.buck.jvm.core.[HasJavaAbi](HasJavaAbi.html "interface in com.facebook.buck.jvm.core"),
                com.facebook.buck.jvm.core.[HasJavaClassHashes](HasJavaClassHashes.html "interface in com.facebook.buck.jvm.core"),
                com.facebook.buck.core.rules.attr.[HasRuntimeDeps](../../core/rules/attr/HasRuntimeDeps.html "interface in com.facebook.buck.core.rules.attr"),
                com.facebook.buck.jvm.core.[HasSources](HasSources.html "interface in com.facebook.buck.jvm.core"))
        -   com.facebook.buck.core.rules.attr.[[HasRuntimeDeps]{.typeNameLink}](../../core/rules/attr/HasRuntimeDeps.html "interface in com.facebook.buck.core.rules.attr")
            -   com.facebook.buck.jvm.core.[[JavaLibrary]{.typeNameLink}](JavaLibrary.html "interface in com.facebook.buck.jvm.core")
                (also extends
                com.facebook.buck.jvm.core.[HasClasspathDeps](HasClasspathDeps.html "interface in com.facebook.buck.jvm.core"),
                com.facebook.buck.jvm.core.[HasClasspathEntries](HasClasspathEntries.html "interface in com.facebook.buck.jvm.core"),
                com.facebook.buck.jvm.core.[HasDesugarSupport](HasDesugarSupport.html "interface in com.facebook.buck.jvm.core"),
                com.facebook.buck.jvm.core.[HasJavaAbi](HasJavaAbi.html "interface in com.facebook.buck.jvm.core"),
                com.facebook.buck.jvm.core.[HasJavaClassHashes](HasJavaClassHashes.html "interface in com.facebook.buck.jvm.core"),
                com.facebook.buck.jvm.core.[HasMavenCoordinates](HasMavenCoordinates.html "interface in com.facebook.buck.jvm.core"),
                com.facebook.buck.jvm.core.[HasSources](HasSources.html "interface in com.facebook.buck.jvm.core"))
-   com.facebook.buck.jvm.core.[[HasSources]{.typeNameLink}](HasSources.html "interface in com.facebook.buck.jvm.core")
    -   com.facebook.buck.jvm.core.[[JavaLibrary]{.typeNameLink}](JavaLibrary.html "interface in com.facebook.buck.jvm.core")
        (also extends
        com.facebook.buck.jvm.core.[HasClasspathDeps](HasClasspathDeps.html "interface in com.facebook.buck.jvm.core"),
        com.facebook.buck.jvm.core.[HasClasspathEntries](HasClasspathEntries.html "interface in com.facebook.buck.jvm.core"),
        com.facebook.buck.jvm.core.[HasDesugarSupport](HasDesugarSupport.html "interface in com.facebook.buck.jvm.core"),
        com.facebook.buck.jvm.core.[HasJavaAbi](HasJavaAbi.html "interface in com.facebook.buck.jvm.core"),
        com.facebook.buck.jvm.core.[HasJavaClassHashes](HasJavaClassHashes.html "interface in com.facebook.buck.jvm.core"),
        com.facebook.buck.jvm.core.[HasMavenCoordinates](HasMavenCoordinates.html "interface in com.facebook.buck.jvm.core"),
        com.facebook.buck.core.rules.attr.[HasRuntimeDeps](../../core/rules/attr/HasRuntimeDeps.html "interface in com.facebook.buck.core.rules.attr"))
-   com.facebook.buck.jvm.core.[[JavaAbiInfo]{.typeNameLink}](JavaAbiInfo.html "interface in com.facebook.buck.jvm.core")
-   com.facebook.buck.jvm.core.[[JavaPackageFinder]{.typeNameLink}](JavaPackageFinder.html "interface in com.facebook.buck.jvm.core")
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
-   Tree
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

[]{#skip.navbar.bottom}
:::
