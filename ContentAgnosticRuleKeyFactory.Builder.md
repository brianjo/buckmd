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

## Class ContentAgnosticRuleKeyFactory.Builder\<RULE_KEY\> {#class-contentagnosticrulekeyfactory.builderrule_key .title title="Class ContentAgnosticRuleKeyFactory.Builder"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.rules.keys.AbstractRuleKeyBuilder](AbstractRuleKeyBuilder.html "class in com.facebook.buck.rules.keys")\<RULE_KEY\>

    -   -   [com.facebook.buck.rules.keys.RuleKeyBuilder](RuleKeyBuilder.html "class in com.facebook.buck.rules.keys")\<RULE_KEY\>

        -   -   com.facebook.buck.rules.keys.ContentAgnosticRuleKeyFactory.Builder\<RULE_KEY\>

::: description
-   

    Enclosing class:
    :   [ContentAgnosticRuleKeyFactory](ContentAgnosticRuleKeyFactory.html "class in com.facebook.buck.rules.keys")

    ------------------------------------------------------------------------

        public class ContentAgnosticRuleKeyFactory.Builder<RULE_KEY>
        extends RuleKeyBuilder<RULE_KEY>
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                 Description
          ------------------------------------------- -------------
          `Builder​(RuleKeyHasher<RULE_KEY> hasher)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                              Method                                             Description
          ---------------------------------------------- -------------------------------------------------- -------------
          `protected AbstractRuleKeyBuilder<RULE_KEY>`   `setAction​(Action action)`                          
          `protected RuleKeyBuilder<RULE_KEY>`           `setAddsToRuleKey​(AddsToRuleKey appendable)`        
          `protected RuleKeyBuilder<RULE_KEY>`           `setBuildRule​(BuildRule rule)`                      
          `protected RuleKeyBuilder<RULE_KEY>`           `setNonHashingSourcePath​(SourcePath sourcePath)`    
          `protected RuleKeyBuilder<RULE_KEY>`           `setSourcePath​(SourcePath sourcePath)`              

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.rules.keys.RuleKeyBuilder}

            ### Methods inherited from class com.facebook.buck.rules.keys.[RuleKeyBuilder](RuleKeyBuilder.html "class in com.facebook.buck.rules.keys")

            `build, setPath, setPath, setSingleValue`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.com.facebook.buck.rules.keys.AbstractRuleKeyBuilder}

            ### Methods inherited from class com.facebook.buck.rules.keys.[AbstractRuleKeyBuilder](AbstractRuleKeyBuilder.html "class in com.facebook.buck.rules.keys")

            `build, setReflectively, setReflectively, setReflectivelyPathKey`

        ```{=html}
        <!-- -->
        ```
        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.rules.keys.hasher.RuleKeyHasher)}

        -   #### Builder

                public Builder​(RuleKeyHasher<RULE_KEY> hasher)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#setAction(com.facebook.buck.core.rules.actions.Action)}

        -   #### setAction

            ``` methodSignature
            protected AbstractRuleKeyBuilder<RULE_KEY> setAction​(Action action)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `setAction` in class `AbstractRuleKeyBuilder<RULE_KEY>`

        []{#setBuildRule(com.facebook.buck.core.rules.BuildRule)}

        -   #### setBuildRule

            ``` methodSignature
            protected RuleKeyBuilder<RULE_KEY> setBuildRule​(BuildRule rule)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `setBuildRule` in
                class `AbstractRuleKeyBuilder<RULE_KEY>`

        []{#setAddsToRuleKey(com.facebook.buck.core.rulekey.AddsToRuleKey)}

        -   #### setAddsToRuleKey

            ``` methodSignature
            protected RuleKeyBuilder<RULE_KEY> setAddsToRuleKey​(AddsToRuleKey appendable)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `setAddsToRuleKey` in
                class `AbstractRuleKeyBuilder<RULE_KEY>`

        []{#setSourcePath(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setSourcePath

            ``` methodSignature
            protected RuleKeyBuilder<RULE_KEY> setSourcePath​(SourcePath sourcePath)
                                                      throws IOException
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `setSourcePath` in
                class `AbstractRuleKeyBuilder<RULE_KEY>`

            [Throws:]{.throwsLabel}
            :   `IOException`

        []{#setNonHashingSourcePath(com.facebook.buck.core.sourcepath.SourcePath)}

        -   #### setNonHashingSourcePath

            ``` methodSignature
            protected RuleKeyBuilder<RULE_KEY> setNonHashingSourcePath​(SourcePath sourcePath)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `setNonHashingSourcePath` in
                class `AbstractRuleKeyBuilder<RULE_KEY>`
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
