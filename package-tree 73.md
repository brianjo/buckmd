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
-   Tree
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

[]{#skip.navbar.top}
:::
:::

::: navPadding
 
:::
:::

::: {role="main"}
::: header
# Hierarchy For Package com.facebook.buck.core.test.rule {#hierarchy-for-package-com.facebook.buck.core.test.rule .title}

[Package Hierarchies:]{.packageHierarchyLabel}

-   [All Packages](../../../../../../overview-tree.html)
:::

::: contentContainer
::: {.section role="region"}
## Class Hierarchy {#class-hierarchy title="Class Hierarchy"}

-   java.lang.[[Object]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}
    -   com.facebook.buck.core.test.rule.[[CoercedTestRunnerSpec]{.typeNameLink}](CoercedTestRunnerSpec.html "class in com.facebook.buck.core.test.rule")
    -   com.facebook.buck.core.test.rule.[[ExternalRunnerTestProtocol]{.typeNameLink}](ExternalRunnerTestProtocol.html "class in com.facebook.buck.core.test.rule")
        (implements
        com.facebook.buck.core.test.rule.[ExternalTestSpec](ExternalTestSpec.html "interface in com.facebook.buck.core.test.rule"))
    -   com.facebook.buck.core.test.rule.[[ExternalTestRunnerTestSpec]{.typeNameLink}](ExternalTestRunnerTestSpec.html "class in com.facebook.buck.core.test.rule")
        (implements
        com.facebook.buck.core.test.rule.[ExternalTestSpec](ExternalTestSpec.html "interface in com.facebook.buck.core.test.rule"))
    -   com.facebook.buck.core.test.rule.ImmutableExternalTestRunnerTestSpec.Builder
        -   com.facebook.buck.core.test.rule.[[ExternalTestRunnerTestSpec.Builder]{.typeNameLink}](ExternalTestRunnerTestSpec.Builder.html "class in com.facebook.buck.core.test.rule")
    -   com.facebook.buck.core.test.rule.[[TestRunnerSpec]{.typeNameLink}](TestRunnerSpec.html "class in com.facebook.buck.core.test.rule")
:::

::: {.section role="region"}
## Interface Hierarchy {#interface-hierarchy title="Interface Hierarchy"}

-   com.facebook.buck.core.rulekey.[[AllowsNonAnnotatedFields]{.typeNameLink}](../../rulekey/AllowsNonAnnotatedFields.html "interface in com.facebook.buck.core.rulekey")
    -   com.facebook.buck.core.rules.[[BuildRule]{.typeNameLink}](../../rules/BuildRule.html "interface in com.facebook.buck.core.rules")
        (also extends
        com.facebook.buck.core.build.action.[BuildEngineAction](../../build/action/BuildEngineAction.html "interface in com.facebook.buck.core.build.action"),
        java.lang.[Comparable](http://docs.oracle.com/javase/7/docs/api/java/lang/Comparable.html?is-external=true "class or interface in java.lang"){.externalLink}\<T\>,
        com.facebook.buck.core.rules.[HasNameAndType](../../rules/HasNameAndType.html "interface in com.facebook.buck.core.rules"))
        -   com.facebook.buck.core.rules.attr.[[HasSupplementaryOutputs]{.typeNameLink}](../../rules/attr/HasSupplementaryOutputs.html "interface in com.facebook.buck.core.rules.attr")
            -   com.facebook.buck.core.test.rule.[[TestXRule]{.typeNameLink}](TestXRule.html "interface in com.facebook.buck.core.test.rule")
                (also extends
                com.facebook.buck.core.test.rule.[ExternalTestRunnerRule](ExternalTestRunnerRule.html "interface in com.facebook.buck.core.test.rule"),
                com.facebook.buck.core.test.rule.[TestRule](TestRule.html "interface in com.facebook.buck.core.test.rule"))
        -   com.facebook.buck.core.test.rule.[[TestRule]{.typeNameLink}](TestRule.html "interface in com.facebook.buck.core.test.rule")
            -   com.facebook.buck.core.test.rule.[[ExternalTestRunnerRule]{.typeNameLink}](ExternalTestRunnerRule.html "interface in com.facebook.buck.core.test.rule")
                -   com.facebook.buck.core.test.rule.[[TestXRule]{.typeNameLink}](TestXRule.html "interface in com.facebook.buck.core.test.rule")
                    (also extends
                    com.facebook.buck.core.rules.attr.[HasSupplementaryOutputs](../../rules/attr/HasSupplementaryOutputs.html "interface in com.facebook.buck.core.rules.attr"),
                    com.facebook.buck.core.test.rule.[TestRule](TestRule.html "interface in com.facebook.buck.core.test.rule"))
            -   com.facebook.buck.core.test.rule.[[TestXRule]{.typeNameLink}](TestXRule.html "interface in com.facebook.buck.core.test.rule")
                (also extends
                com.facebook.buck.core.test.rule.[ExternalTestRunnerRule](ExternalTestRunnerRule.html "interface in com.facebook.buck.core.test.rule"),
                com.facebook.buck.core.rules.attr.[HasSupplementaryOutputs](../../rules/attr/HasSupplementaryOutputs.html "interface in com.facebook.buck.core.rules.attr"))
-   com.facebook.buck.core.build.action.[[BuildEngineAction]{.typeNameLink}](../../build/action/BuildEngineAction.html "interface in com.facebook.buck.core.build.action")
    -   com.facebook.buck.core.rules.[[BuildRule]{.typeNameLink}](../../rules/BuildRule.html "interface in com.facebook.buck.core.rules")
        (also extends
        com.facebook.buck.core.rulekey.[AllowsNonAnnotatedFields](../../rulekey/AllowsNonAnnotatedFields.html "interface in com.facebook.buck.core.rulekey"),
        java.lang.[Comparable](http://docs.oracle.com/javase/7/docs/api/java/lang/Comparable.html?is-external=true "class or interface in java.lang"){.externalLink}\<T\>,
        com.facebook.buck.core.rules.[HasNameAndType](../../rules/HasNameAndType.html "interface in com.facebook.buck.core.rules"))
        -   com.facebook.buck.core.rules.attr.[[HasSupplementaryOutputs]{.typeNameLink}](../../rules/attr/HasSupplementaryOutputs.html "interface in com.facebook.buck.core.rules.attr")
            -   com.facebook.buck.core.test.rule.[[TestXRule]{.typeNameLink}](TestXRule.html "interface in com.facebook.buck.core.test.rule")
                (also extends
                com.facebook.buck.core.test.rule.[ExternalTestRunnerRule](ExternalTestRunnerRule.html "interface in com.facebook.buck.core.test.rule"),
                com.facebook.buck.core.test.rule.[TestRule](TestRule.html "interface in com.facebook.buck.core.test.rule"))
        -   com.facebook.buck.core.test.rule.[[TestRule]{.typeNameLink}](TestRule.html "interface in com.facebook.buck.core.test.rule")
            -   com.facebook.buck.core.test.rule.[[ExternalTestRunnerRule]{.typeNameLink}](ExternalTestRunnerRule.html "interface in com.facebook.buck.core.test.rule")
                -   com.facebook.buck.core.test.rule.[[TestXRule]{.typeNameLink}](TestXRule.html "interface in com.facebook.buck.core.test.rule")
                    (also extends
                    com.facebook.buck.core.rules.attr.[HasSupplementaryOutputs](../../rules/attr/HasSupplementaryOutputs.html "interface in com.facebook.buck.core.rules.attr"),
                    com.facebook.buck.core.test.rule.[TestRule](TestRule.html "interface in com.facebook.buck.core.test.rule"))
            -   com.facebook.buck.core.test.rule.[[TestXRule]{.typeNameLink}](TestXRule.html "interface in com.facebook.buck.core.test.rule")
                (also extends
                com.facebook.buck.core.test.rule.[ExternalTestRunnerRule](ExternalTestRunnerRule.html "interface in com.facebook.buck.core.test.rule"),
                com.facebook.buck.core.rules.attr.[HasSupplementaryOutputs](../../rules/attr/HasSupplementaryOutputs.html "interface in com.facebook.buck.core.rules.attr"))
-   java.lang.[[Comparable]{.typeNameLink}](http://docs.oracle.com/javase/7/docs/api/java/lang/Comparable.html?is-external=true "class or interface in java.lang"){.externalLink}\<T\>
    -   com.facebook.buck.core.rules.[[BuildRule]{.typeNameLink}](../../rules/BuildRule.html "interface in com.facebook.buck.core.rules")
        (also extends
        com.facebook.buck.core.rulekey.[AllowsNonAnnotatedFields](../../rulekey/AllowsNonAnnotatedFields.html "interface in com.facebook.buck.core.rulekey"),
        com.facebook.buck.core.build.action.[BuildEngineAction](../../build/action/BuildEngineAction.html "interface in com.facebook.buck.core.build.action"),
        com.facebook.buck.core.rules.[HasNameAndType](../../rules/HasNameAndType.html "interface in com.facebook.buck.core.rules"))
        -   com.facebook.buck.core.rules.attr.[[HasSupplementaryOutputs]{.typeNameLink}](../../rules/attr/HasSupplementaryOutputs.html "interface in com.facebook.buck.core.rules.attr")
            -   com.facebook.buck.core.test.rule.[[TestXRule]{.typeNameLink}](TestXRule.html "interface in com.facebook.buck.core.test.rule")
                (also extends
                com.facebook.buck.core.test.rule.[ExternalTestRunnerRule](ExternalTestRunnerRule.html "interface in com.facebook.buck.core.test.rule"),
                com.facebook.buck.core.test.rule.[TestRule](TestRule.html "interface in com.facebook.buck.core.test.rule"))
        -   com.facebook.buck.core.test.rule.[[TestRule]{.typeNameLink}](TestRule.html "interface in com.facebook.buck.core.test.rule")
            -   com.facebook.buck.core.test.rule.[[ExternalTestRunnerRule]{.typeNameLink}](ExternalTestRunnerRule.html "interface in com.facebook.buck.core.test.rule")
                -   com.facebook.buck.core.test.rule.[[TestXRule]{.typeNameLink}](TestXRule.html "interface in com.facebook.buck.core.test.rule")
                    (also extends
                    com.facebook.buck.core.rules.attr.[HasSupplementaryOutputs](../../rules/attr/HasSupplementaryOutputs.html "interface in com.facebook.buck.core.rules.attr"),
                    com.facebook.buck.core.test.rule.[TestRule](TestRule.html "interface in com.facebook.buck.core.test.rule"))
            -   com.facebook.buck.core.test.rule.[[TestXRule]{.typeNameLink}](TestXRule.html "interface in com.facebook.buck.core.test.rule")
                (also extends
                com.facebook.buck.core.test.rule.[ExternalTestRunnerRule](ExternalTestRunnerRule.html "interface in com.facebook.buck.core.test.rule"),
                com.facebook.buck.core.rules.attr.[HasSupplementaryOutputs](../../rules/attr/HasSupplementaryOutputs.html "interface in com.facebook.buck.core.rules.attr"))
-   com.facebook.buck.core.rules.[[HasNameAndType]{.typeNameLink}](../../rules/HasNameAndType.html "interface in com.facebook.buck.core.rules")
    -   com.facebook.buck.core.rules.[[BuildRule]{.typeNameLink}](../../rules/BuildRule.html "interface in com.facebook.buck.core.rules")
        (also extends
        com.facebook.buck.core.rulekey.[AllowsNonAnnotatedFields](../../rulekey/AllowsNonAnnotatedFields.html "interface in com.facebook.buck.core.rulekey"),
        com.facebook.buck.core.build.action.[BuildEngineAction](../../build/action/BuildEngineAction.html "interface in com.facebook.buck.core.build.action"),
        java.lang.[Comparable](http://docs.oracle.com/javase/7/docs/api/java/lang/Comparable.html?is-external=true "class or interface in java.lang"){.externalLink}\<T\>)
        -   com.facebook.buck.core.rules.attr.[[HasSupplementaryOutputs]{.typeNameLink}](../../rules/attr/HasSupplementaryOutputs.html "interface in com.facebook.buck.core.rules.attr")
            -   com.facebook.buck.core.test.rule.[[TestXRule]{.typeNameLink}](TestXRule.html "interface in com.facebook.buck.core.test.rule")
                (also extends
                com.facebook.buck.core.test.rule.[ExternalTestRunnerRule](ExternalTestRunnerRule.html "interface in com.facebook.buck.core.test.rule"),
                com.facebook.buck.core.test.rule.[TestRule](TestRule.html "interface in com.facebook.buck.core.test.rule"))
        -   com.facebook.buck.core.test.rule.[[TestRule]{.typeNameLink}](TestRule.html "interface in com.facebook.buck.core.test.rule")
            -   com.facebook.buck.core.test.rule.[[ExternalTestRunnerRule]{.typeNameLink}](ExternalTestRunnerRule.html "interface in com.facebook.buck.core.test.rule")
                -   com.facebook.buck.core.test.rule.[[TestXRule]{.typeNameLink}](TestXRule.html "interface in com.facebook.buck.core.test.rule")
                    (also extends
                    com.facebook.buck.core.rules.attr.[HasSupplementaryOutputs](../../rules/attr/HasSupplementaryOutputs.html "interface in com.facebook.buck.core.rules.attr"),
                    com.facebook.buck.core.test.rule.[TestRule](TestRule.html "interface in com.facebook.buck.core.test.rule"))
            -   com.facebook.buck.core.test.rule.[[TestXRule]{.typeNameLink}](TestXRule.html "interface in com.facebook.buck.core.test.rule")
                (also extends
                com.facebook.buck.core.test.rule.[ExternalTestRunnerRule](ExternalTestRunnerRule.html "interface in com.facebook.buck.core.test.rule"),
                com.facebook.buck.core.rules.attr.[HasSupplementaryOutputs](../../rules/attr/HasSupplementaryOutputs.html "interface in com.facebook.buck.core.rules.attr"))
-   com.facebook.buck.core.test.rule.[[HasTestRunner]{.typeNameLink}](HasTestRunner.html "interface in com.facebook.buck.core.test.rule")
-   com.fasterxml.jackson.databind.JsonSerializable
    -   com.facebook.buck.core.test.rule.[[ExternalTestSpec]{.typeNameLink}](ExternalTestSpec.html "interface in com.facebook.buck.core.test.rule")
-   com.facebook.buck.core.test.rule.[[TestRule.TestReportingCallback]{.typeNameLink}](TestRule.TestReportingCallback.html "interface in com.facebook.buck.core.test.rule")
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
-   Tree
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

[]{#skip.navbar.bottom}
:::
