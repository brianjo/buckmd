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

## Class MultiarchFileInfos {#class-multiarchfileinfos .title title="Class MultiarchFileInfos"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.apple.MultiarchFileInfos

::: description
-   

    ------------------------------------------------------------------------

        public class MultiarchFileInfos
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static void`         | `checkTa              | ::: block             |
        |                       | rgetSupportsMultiarch | Assert that target    |
        |                       | ​(BuildTarget target)` | supports multiple     |
        |                       |                       | architectures.        |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static Optional<c    | `create​(Fl            | ::: block             |
        | om.facebook.buck.appl | avorDomain<Unresolved | Inspect the given     |
        | e.MultiarchFileInfo>` | AppleCxxPlatform> app | build target and      |
        |                       | leCxxPlatforms,       | return information    |
        |                       |  BuildTarget target)` | about it if its a fat |
        |                       |                       | binary.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static com.google    | `gener                | ::: block             |
        | .common.collect.Immut | ateThinFlavors​(Sorted | Expand flavors        |
        | ableList<com.google.c | Set<Flavor> flavors)` | representing a fat    |
        | ommon.collect.Immutab |                       | binary into its thin  |
        | leSortedSet<Flavor>>` |                       | binary equivalents.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static BuildRule`    | `requireMultia        | ::: block             |
        |                       | rchRule​(BuildTarget b | Generate a fat rule   |
        |                       | uildTarget,           | from thin rules.      |
        |                       |            ProjectFil | :::                   |
        |                       | esystem projectFilesy |                       |
        |                       | stem,                 |                       |
        |                       |      BuildRuleParams  |                       |
        |                       | params,               |                       |
        |                       |        ActionGraphBui |                       |
        |                       | lder graphBuilder,    |                       |
        |                       |                   com |                       |
        |                       | .facebook.buck.apple. |                       |
        |                       | MultiarchFileInfo inf |                       |
        |                       | o,                    |                       |
        |                       |   com.google.common.c |                       |
        |                       | ollect.ImmutableSorte |                       |
        |                       | dSet<BuildRule> thinR |                       |
        |                       | ules,                 |                       |
        |                       |      CxxBuckConfig cx |                       |
        |                       | xBuckConfig,          |                       |
        |                       |             FlavorDom |                       |
        |                       | ain<UnresolvedAppleCx |                       |
        |                       | xPlatform> appleCxxPl |                       |
        |                       | atformsFlavorDomain)` |                       |
        +-----------------------+-----------------------+-----------------------+

        : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
        Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
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

        []{#create(com.facebook.buck.core.model.FlavorDomain,com.facebook.buck.core.model.BuildTarget)}

        -   #### create

            ``` methodSignature
            public static Optional<com.facebook.buck.apple.MultiarchFileInfo> create​(FlavorDomain<UnresolvedAppleCxxPlatform> appleCxxPlatforms,
                                                                                     BuildTarget target)
            ```

            ::: block
            Inspect the given build target and return information about
            it if its a fat binary.
            :::

            [Returns:]{.returnLabel}
            :   non-empty when the target represents a fat binary.

            [Throws:]{.throwsLabel}
            :   `HumanReadableException` - when the target is a fat
                binary but has incompatible flavors.

        []{#checkTargetSupportsMultiarch(com.facebook.buck.core.model.BuildTarget)}

        -   #### checkTargetSupportsMultiarch

            ``` methodSignature
            public static void checkTargetSupportsMultiarch​(BuildTarget target)
            ```

            ::: block
            Assert that target supports multiple architectures.
            :::

        []{#generateThinFlavors(java.util.SortedSet)}

        -   #### generateThinFlavors

            ``` methodSignature
            public static com.google.common.collect.ImmutableList<com.google.common.collect.ImmutableSortedSet<Flavor>> generateThinFlavors​(SortedSet<Flavor> flavors)
            ```

            ::: block
            Expand flavors representing a fat binary into its thin
            binary equivalents.
            Useful when dealing with functions unaware of fat binaries.

            This does not actually check that the particular flavor set
            is valid.
            :::

        []{#requireMultiarchRule(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.io.filesystem.ProjectFilesystem,com.facebook.buck.core.rules.BuildRuleParams,com.facebook.buck.core.rules.ActionGraphBuilder,com.facebook.buck.apple.MultiarchFileInfo,com.google.common.collect.ImmutableSortedSet,com.facebook.buck.cxx.config.CxxBuckConfig,com.facebook.buck.core.model.FlavorDomain)}

        -   #### requireMultiarchRule

            ``` methodSignature
            public static BuildRule requireMultiarchRule​(BuildTarget buildTarget,
                                                         ProjectFilesystem projectFilesystem,
                                                         BuildRuleParams params,
                                                         ActionGraphBuilder graphBuilder,
                                                         com.facebook.buck.apple.MultiarchFileInfo info,
                                                         com.google.common.collect.ImmutableSortedSet<BuildRule> thinRules,
                                                         CxxBuckConfig cxxBuckConfig,
                                                         FlavorDomain<UnresolvedAppleCxxPlatform> appleCxxPlatformsFlavorDomain)
            ```

            ::: block
            Generate a fat rule from thin rules.
            Invariant: thinRules contain all the thin rules listed in
            info.getThinTargets().
            :::
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
