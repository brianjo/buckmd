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
-   [Nested](#nested.class.summary) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.core.rules.common](package-summary.html)
:::

## Class BuildableSupport {#class-buildablesupport .title title="Class BuildableSupport"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.rules.common.BuildableSupport

::: description
-   

    ------------------------------------------------------------------------

        public final class BuildableSupport
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static class `       | `Buildable            | ::: block             |
        |                       | Support.DepsSupplier` | A build deps supplier |
        |                       |                       | that allows updating  |
        |                       |                       | of the captured rule  |
        |                       |                       | finder.               |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static Buildable     | `                     | ::: block             |
        | Support.DepsSupplier` | buildDepsSupplier​(Bui | Creates a supplier to |
        |                       | ldRule rule,          | easily implement (and |
        |                       |          SourcePathRu | cache)                |
        |                       | leFinder ruleFinder)` | Bui                   |
        |                       |                       | ldRule.getBuildDeps() |
        |                       |                       | via                   |
        |                       |                       | Buildable             |
        |                       |                       | Support.deriveDeps(). |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `deriveDeps​(          | ::: block             |
        | static java.util.stre | AddsToRuleKey rule,   | Derives dependencies  |
        | am.Stream<BuildRule>` |          SourcePathRu | based on everything   |
        |                       | leFinder ruleFinder)` | added to the rulekey. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `deriveD              | ::: block             |
        | static java.util.stre | eps​(BuildRule rule,   | Derives dependencies  |
        | am.Stream<BuildRule>` |          SourcePathRu | based on everything   |
        |                       | leFinder ruleFinder)` | added to the rulekey. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `s                    | `deriveInputs​(A       | ::: block             |
        | tatic java.util.strea | ddsToRuleKey object)` | Derives inputs based  |
        | m.Stream<SourcePath>` |                       | on everything added   |
        |                       |                       | to the rulekey.       |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `                     | `getDe                | ::: block             |
        | static java.util.stre | ps​(AddsToRuleKey tool | Streams dependencies  |
        | am.Stream<BuildRule>` | ,        SourcePathRu | based on everything   |
        |                       | leFinder ruleFinder)` | added to its rulekey. |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `s                    | `getD                 | ::: block             |
        | tatic com.google.comm | epsCollection​(AddsToR | Derives dependencies  |
        | on.collect.ImmutableC | uleKey tool,          | based on everything   |
        | ollection<BuildRule>` |          SourcePathRu | added to its rulekey. |
        |                       | leFinder ruleFinder)` | :::                   |
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

        []{#deriveDeps(com.facebook.buck.core.rulekey.AddsToRuleKey,com.facebook.buck.core.rules.SourcePathRuleFinder)}

        -   #### deriveDeps

            ``` methodSignature
            public static java.util.stream.Stream<BuildRule> deriveDeps​(AddsToRuleKey rule,
                                                                        SourcePathRuleFinder ruleFinder)
            ```

            ::: block
            Derives dependencies based on everything added to the
            rulekey.
            :::

        []{#deriveDeps(com.facebook.buck.core.rules.BuildRule,com.facebook.buck.core.rules.SourcePathRuleFinder)}

        -   #### deriveDeps

            ``` methodSignature
            public static java.util.stream.Stream<BuildRule> deriveDeps​(BuildRule rule,
                                                                        SourcePathRuleFinder ruleFinder)
            ```

            ::: block
            Derives dependencies based on everything added to the
            rulekey.
            :::

        []{#getDepsCollection(com.facebook.buck.core.rulekey.AddsToRuleKey,com.facebook.buck.core.rules.SourcePathRuleFinder)}

        -   #### getDepsCollection

            ``` methodSignature
            public static com.google.common.collect.ImmutableCollection<BuildRule> getDepsCollection​(AddsToRuleKey tool,
                                                                                                     SourcePathRuleFinder ruleFinder)
            ```

            ::: block
            Derives dependencies based on everything added to its
            rulekey.
            :::

        []{#getDeps(com.facebook.buck.core.rulekey.AddsToRuleKey,com.facebook.buck.core.rules.SourcePathRuleFinder)}

        -   #### getDeps

            ``` methodSignature
            public static java.util.stream.Stream<BuildRule> getDeps​(AddsToRuleKey tool,
                                                                     SourcePathRuleFinder ruleFinder)
            ```

            ::: block
            Streams dependencies based on everything added to its
            rulekey.
            :::

        []{#deriveInputs(com.facebook.buck.core.rulekey.AddsToRuleKey)}

        -   #### deriveInputs

            ``` methodSignature
            public static java.util.stream.Stream<SourcePath> deriveInputs​(AddsToRuleKey object)
            ```

            ::: block
            Derives inputs based on everything added to the rulekey.
            :::

        []{#buildDepsSupplier(com.facebook.buck.core.rules.BuildRule,com.facebook.buck.core.rules.SourcePathRuleFinder)}

        -   #### buildDepsSupplier

            ``` methodSignature
            public static BuildableSupport.DepsSupplier buildDepsSupplier​(BuildRule rule,
                                                                          SourcePathRuleFinder ruleFinder)
            ```

            ::: block
            Creates a supplier to easily implement (and cache)
            BuildRule.getBuildDeps() via BuildableSupport.deriveDeps().
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
-   [Nested](#nested.class.summary) \| 
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
