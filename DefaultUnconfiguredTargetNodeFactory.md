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
[Package]{.packageLabelInType} [com.facebook.buck.parser](package-summary.html)
:::

## Class DefaultUnconfiguredTargetNodeFactory {#class-defaultunconfiguredtargetnodefactory .title title="Class DefaultUnconfiguredTargetNodeFactory"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.parser.DefaultUnconfiguredTargetNodeFactory

::: description
-   

    All Implemented Interfaces:
    :   `UnconfiguredTargetNodeFactory`

    ------------------------------------------------------------------------

        public class DefaultUnconfiguredTargetNodeFactory
        extends Object
        implements UnconfiguredTargetNodeFactory

    ::: block
    Creates
    [`UnconfiguredTargetNode`](../core/model/targetgraph/raw/UnconfiguredTargetNode.html "interface in com.facebook.buck.core.model.targetgraph.raw")
    instances from raw data coming in form the
    [`ProjectBuildFileParser`](api/ProjectBuildFileParser.html "interface in com.facebook.buck.parser.api").
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                                                                                                                   Description
          ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `DefaultUnconfiguredTargetNodeFactory​(KnownRuleTypesProvider knownRuleTypesProvider,                                     BuiltTargetVerifier builtTargetVerifier,                                     Cells cells,                                     SelectorListFactory selectorListFactory,                                     TypeCoercerFactory typeCoercerFactory)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `Un                   | `create​(C             | ::: block             |
        | configuredTargetNode` | ell cell,       Path  | Create new            |
        |                       | buildFile,       Unco | [`UnconfiguredTarge   |
        |                       | nfiguredBuildTarget t | tNode`](../core/model |
        |                       | arget,       Dependen | /targetgraph/raw/Unco |
        |                       | cyStack dependencySta | nfiguredTargetNode.ht |
        |                       | ck,       Map<String, | ml "interface in com. |
        |                       | ​Object> rawAttributes | facebook.buck.core.mo |
        |                       | ,       Package pkg)` | del.targetgraph.raw") |
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
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.core.rules.knowntypes.provider.KnownRuleTypesProvider,com.facebook.buck.parser.BuiltTargetVerifier,com.facebook.buck.core.cell.Cells,com.facebook.buck.core.select.impl.SelectorListFactory,com.facebook.buck.rules.coercer.TypeCoercerFactory)}

        -   #### DefaultUnconfiguredTargetNodeFactory

                public DefaultUnconfiguredTargetNodeFactory​(KnownRuleTypesProvider knownRuleTypesProvider,
                                                            BuiltTargetVerifier builtTargetVerifier,
                                                            Cells cells,
                                                            SelectorListFactory selectorListFactory,
                                                            TypeCoercerFactory typeCoercerFactory)
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#create(com.facebook.buck.core.cell.Cell,java.nio.file.Path,com.facebook.buck.core.model.UnconfiguredBuildTarget,com.facebook.buck.core.exceptions.DependencyStack,java.util.Map,com.facebook.buck.core.model.targetgraph.impl.Package)}

        -   #### create

            ``` methodSignature
            public UnconfiguredTargetNode create​(Cell cell,
                                                 Path buildFile,
                                                 UnconfiguredBuildTarget target,
                                                 DependencyStack dependencyStack,
                                                 Map<String,​Object> rawAttributes,
                                                 Package pkg)
            ```

            ::: block
            [Description copied from
            interface: `UnconfiguredTargetNodeFactory`]{.descfrmTypeLabel}
            :::

            ::: block
            Create new
            [`UnconfiguredTargetNode`](../core/model/targetgraph/raw/UnconfiguredTargetNode.html "interface in com.facebook.buck.core.model.targetgraph.raw")
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `create` in interface `UnconfiguredTargetNodeFactory`

            [Parameters:]{.paramLabel}
            :   `cell` - object that current build target belongs to
            :   `buildFile` - An absolute path to a build file that has
                the corresponding build target
            :   `target` - A build target that uniquely identifies
                created
                [`UnconfiguredTargetNode`](../core/model/targetgraph/raw/UnconfiguredTargetNode.html "interface in com.facebook.buck.core.model.targetgraph.raw")
            :   `rawAttributes` - Raw attributes that forms the node, a
                Map where a key is attribute name as
            :   `pkg` - Package to apply to this node.
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
