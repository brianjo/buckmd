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
-   [Nested](#nested.class.summary) \| 
-   Field \| 
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   [Constr](#constructor.detail) \| 
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
[Package]{.packageLabelInType} [com.facebook.buck.rules.keys](package-summary.html)
:::

## Class DefaultDependencyFileRuleKeyFactory {#class-defaultdependencyfilerulekeyfactory .title title="Class DefaultDependencyFileRuleKeyFactory"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.rules.keys.DefaultDependencyFileRuleKeyFactory

::: description
-   

    All Implemented Interfaces:
    :   `DependencyFileRuleKeyFactory`

    ------------------------------------------------------------------------

        public final class DefaultDependencyFileRuleKeyFactory
        extends Object
        implements DependencyFileRuleKeyFactory

    ::: block
    A factory for generating dependency-file
    [`RuleKey`](../../core/rulekey/RuleKey.html "class in com.facebook.buck.core.rulekey")s.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        -   []{#nested.classes.inherited.from.class.com.facebook.buck.rules.keys.DependencyFileRuleKeyFactory}

            ### Nested classes/interfaces inherited from interface com.facebook.buck.rules.keys.[DependencyFileRuleKeyFactory](DependencyFileRuleKeyFactory.html "interface in com.facebook.buck.rules.keys")

            `DependencyFileRuleKeyFactory.RuleKeyAndInputs`
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                                      Description
          ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ -------------
          `DefaultDependencyFileRuleKeyFactory​(RuleKeyFieldLoader ruleKeyFieldLoader,                                    FileHashLoader hashLoader,                                    SourcePathRuleFinder ruleFinder)`                                                                                    
          `DefaultDependencyFileRuleKeyFactory​(RuleKeyFieldLoader ruleKeyFieldLoader,                                    FileHashLoader hashLoader,                                    SourcePathRuleFinder ruleFinder,                                    Optional<ThriftRuleKeyLogger> ruleKeyLogger)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                 Method                                                                                                                          Description
          ------------------------------------------------- ------------------------------------------------------------------------------------------------------------------------------- -------------
          `DependencyFileRuleKeyFactory.RuleKeyAndInputs`   `build​(SupportsDependencyFileRuleKey rule,      com.google.common.collect.ImmutableList<DependencyFileEntry> depFileEntries)`    
          `DependencyFileRuleKeyFactory.RuleKeyAndInputs`   `buildManifestKey​(SupportsDependencyFileRuleKey rule)`                                                                           

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
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.rules.keys.RuleKeyFieldLoader,com.facebook.buck.util.hashing.FileHashLoader,com.facebook.buck.core.rules.SourcePathRuleFinder,java.util.Optional)}

        -   #### DefaultDependencyFileRuleKeyFactory

                public DefaultDependencyFileRuleKeyFactory​(RuleKeyFieldLoader ruleKeyFieldLoader,
                                                           FileHashLoader hashLoader,
                                                           SourcePathRuleFinder ruleFinder,
                                                           Optional<ThriftRuleKeyLogger> ruleKeyLogger)

        []{#<init>(com.facebook.buck.rules.keys.RuleKeyFieldLoader,com.facebook.buck.util.hashing.FileHashLoader,com.facebook.buck.core.rules.SourcePathRuleFinder)}

        -   #### DefaultDependencyFileRuleKeyFactory

                public DefaultDependencyFileRuleKeyFactory​(RuleKeyFieldLoader ruleKeyFieldLoader,
                                                           FileHashLoader hashLoader,
                                                           SourcePathRuleFinder ruleFinder)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#build(com.facebook.buck.core.rules.attr.SupportsDependencyFileRuleKey,com.google.common.collect.ImmutableList)}

        -   #### build

            ``` methodSignature
            public DependencyFileRuleKeyFactory.RuleKeyAndInputs build​(SupportsDependencyFileRuleKey rule,
                                                                       com.google.common.collect.ImmutableList<DependencyFileEntry> depFileEntries)
                                                                throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `build` in interface `DependencyFileRuleKeyFactory`

            [Returns:]{.returnLabel}
            :   a
                [`RuleKey`](../../core/rulekey/RuleKey.html "class in com.facebook.buck.core.rulekey")
                for the given
                [`BuildRule`](../../core/rules/BuildRule.html "interface in com.facebook.buck.core.rules")
                using the given list of explicit `inputs` and an
                `ImmutableSet` of the members of
                possibleDepFileSourcePaths that were actually used in
                constructing the key.

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#buildManifestKey(com.facebook.buck.core.rules.attr.SupportsDependencyFileRuleKey)}

        -   #### buildManifestKey

            ``` methodSignature
            public DependencyFileRuleKeyFactory.RuleKeyAndInputs buildManifestKey​(SupportsDependencyFileRuleKey rule)
                                                                           throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `buildManifestKey` in
                interface `DependencyFileRuleKeyFactory`

            [Returns:]{.returnLabel}
            :   the
                [`RuleKey`](../../core/rulekey/RuleKey.html "class in com.facebook.buck.core.rulekey")
                used to index the manifest database and the list of
                inputs that should appear in the manifest (i.e., those
                that appeared in the dependency file, because all other
                inputs would be accounted for in the manifest key
                itself).

            [Throws:]{.throwsLabel}
            :   `IOException`
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
-   [Nested](#nested.class.summary) \| 
-   Field \| 
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   Field \| 
-   [Constr](#constructor.detail) \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
