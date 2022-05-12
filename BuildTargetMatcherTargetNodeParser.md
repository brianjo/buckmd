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
[Package]{.packageLabelInType} [com.facebook.buck.parser.spec](package-summary.html)
:::

## Class BuildTargetMatcherTargetNodeParser {#class-buildtargetmatchertargetnodeparser .title title="Class BuildTargetMatcherTargetNodeParser"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   [com.facebook.buck.core.parser.buildtargetparser.BuildTargetMatcherParser](../../core/parser/buildtargetparser/BuildTargetMatcherParser.html "class in com.facebook.buck.core.parser.buildtargetparser")\<[TargetNodeSpec](TargetNodeSpec.html "interface in com.facebook.buck.parser.spec")\>

    -   -   com.facebook.buck.parser.spec.BuildTargetMatcherTargetNodeParser

::: description
-   

    ------------------------------------------------------------------------

        public class BuildTargetMatcherTargetNodeParser
        extends BuildTargetMatcherParser<TargetNodeSpec>

    ::: block
    Parses a string to
    [`TargetNodeSpec`](TargetNodeSpec.html "interface in com.facebook.buck.parser.spec")
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                              Description
          ---------------------------------------- -------------
          `BuildTargetMatcherTargetNodeParser()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type   Method                                                                       Description
          ------------------- ---------------------------------------------------------------------------- -------------
          `TargetNodeSpec`    `createForChildren​(CellRelativePath cellRelativePath)`                        
          `TargetNodeSpec`    `createForDescendants​(CellRelativePath cellRelativePath)`                     
          `TargetNodeSpec`    `createForSingleton​(UnconfiguredBuildTargetWithOutputs targetWithOutputs)`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Concrete
          Methods](javascript:show(8);)[ ]{.tabEnd}]{#t4 .tableTab}

        -   []{#methods.inherited.from.class.com.facebook.buck.core.parser.buildtargetparser.BuildTargetMatcherParser}

            ### Methods inherited from class com.facebook.buck.core.parser.buildtargetparser.[BuildTargetMatcherParser](../../core/parser/buildtargetparser/BuildTargetMatcherParser.html "class in com.facebook.buck.core.parser.buildtargetparser")

            `forVisibilityArgument, parse`

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

        []{#<init>()}

        -   #### BuildTargetMatcherTargetNodeParser

                public BuildTargetMatcherTargetNodeParser()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#createForDescendants(com.facebook.buck.core.model.CellRelativePath)}

        -   #### createForDescendants

            ``` methodSignature
            public TargetNodeSpec createForDescendants​(CellRelativePath cellRelativePath)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `createForDescendants` in
                class `BuildTargetMatcherParser<TargetNodeSpec>`

            [Returns:]{.returnLabel}
            :   description of the target name and context being parsed
                when an error was encountered. Examples are \":azzetz in
                build file //first-party/orca/orcaapp/BUCK\" and
                \"//first-party/orca/orcaapp:mezzenger in context
                FULLY_QUALIFIED\"

        []{#createForChildren(com.facebook.buck.core.model.CellRelativePath)}

        -   #### createForChildren

            ``` methodSignature
            public TargetNodeSpec createForChildren​(CellRelativePath cellRelativePath)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `createForChildren` in
                class `BuildTargetMatcherParser<TargetNodeSpec>`

        []{#createForSingleton(com.facebook.buck.core.model.UnconfiguredBuildTargetWithOutputs)}

        -   #### createForSingleton

            ``` methodSignature
            public TargetNodeSpec createForSingleton​(UnconfiguredBuildTargetWithOutputs targetWithOutputs)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `createForSingleton` in
                class `BuildTargetMatcherParser<TargetNodeSpec>`
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
