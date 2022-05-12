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
-   [Field](#field.summary) \| 
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
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

## Class AppleResources {#class-appleresources .title title="Class AppleResources"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.apple.AppleResources

::: description
-   

    ------------------------------------------------------------------------

        public class AppleResources
        extends Object
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type                                      Field                             Description
          ------------------------------------------------------ --------------------------------- -------------
          `static java.util.function.Predicate<TargetNode<?>>`   `IS_APPLE_BUNDLE_RESOURCE_NODE`    

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `static com.g         | `collectDirec         |                       |
        | oogle.common.collect. | tResources​(TargetGrap |                       |
        | ImmutableSet<AppleRes | h targetGraph,        |                       |
        | ourceDescriptionArg>` |                 Targe |                       |
        |                       | tNode<?> targetNode)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static com.g         | `collectR             | ::: block             |
        | oogle.common.collect. | ecursiveResources​(XCo | Collect resources     |
        | ImmutableSet<AppleRes | deDescriptions xcodeD | from recursive        |
        | ourceDescriptionArg>` | escriptions,          | dependencies.         |
        |                       |                  Targ | :::                   |
        |                       | etGraph targetGraph,  |                       |
        |                       |                       |                       |
        |                       |     Optional<AppleDep |                       |
        |                       | endenciesCache> cache |                       |
        |                       | ,                     |                       |
        |                       |       TargetNode<?> t |                       |
        |                       | argetNode,            |                       |
        |                       |                AppleB |                       |
        |                       | uildRules.RecursiveDe |                       |
        |                       | pendenciesMode mode)` |                       |
        +-----------------------+-----------------------+-----------------------+
        | `static <T ex         | `co                   | ::: block             |
        | tends ConstructorArg> | llectResourceDirsAndF | Collect resource dirs |
        | AppleBundleResources` | iles​(XCodeDescription | and files             |
        |                       | s xcodeDescriptions,  | :::                   |
        |                       |                       |                       |
        |                       |       TargetGraph tar |                       |
        |                       | getGraph,             |                       |
        |                       |                 Build |                       |
        |                       | RuleResolver resolver |                       |
        |                       | ,                     |                       |
        |                       |         Optional<Appl |                       |
        |                       | eDependenciesCache> c |                       |
        |                       | ache,                 |                       |
        |                       |             TargetNod |                       |
        |                       | e<T> targetNode,      |                       |
        |                       |                       |                       |
        |                       |   AppleCxxPlatform ap |                       |
        |                       | pleCxxPlatform,       |                       |
        |                       |                       |                       |
        |                       |  AppleBuildRules.Recu |                       |
        |                       | rsiveDependenciesMode |                       |
        |                       |  mode,                |                       |
        |                       |              java.uti |                       |
        |                       | l.function.Predicate< |                       |
        |                       | BuildTarget> filter)` |                       |
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
    -   []{#field.detail}

        ### Field Detail

        []{#IS_APPLE_BUNDLE_RESOURCE_NODE}

        -   #### IS_APPLE_BUNDLE_RESOURCE_NODE

                public static final java.util.function.Predicate<TargetNode<?>> IS_APPLE_BUNDLE_RESOURCE_NODE
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#collectRecursiveResources(com.facebook.buck.apple.XCodeDescriptions,com.facebook.buck.core.model.targetgraph.TargetGraph,java.util.Optional,com.facebook.buck.core.model.targetgraph.TargetNode,com.facebook.buck.apple.AppleBuildRules.RecursiveDependenciesMode)}

        -   #### collectRecursiveResources

            ``` methodSignature
            public static com.google.common.collect.ImmutableSet<AppleResourceDescriptionArg> collectRecursiveResources​(XCodeDescriptions xcodeDescriptions,
                                                                                                                        TargetGraph targetGraph,
                                                                                                                        Optional<AppleDependenciesCache> cache,
                                                                                                                        TargetNode<?> targetNode,
                                                                                                                        AppleBuildRules.RecursiveDependenciesMode mode)
            ```

            ::: block
            Collect resources from recursive dependencies.
            :::

            [Parameters:]{.paramLabel}
            :   `targetGraph` - The
                [`TargetGraph`](../core/model/targetgraph/TargetGraph.html "class in com.facebook.buck.core.model.targetgraph")
                containing the node and its dependencies.
            :   `targetNode` -
                [`TargetNode`](../core/model/targetgraph/TargetNode.html "interface in com.facebook.buck.core.model.targetgraph")
                at the tip of the traversal.

            [Returns:]{.returnLabel}
            :   The recursive resource buildables.

        []{#collectResourceDirsAndFiles(com.facebook.buck.apple.XCodeDescriptions,com.facebook.buck.core.model.targetgraph.TargetGraph,com.facebook.buck.core.rules.BuildRuleResolver,java.util.Optional,com.facebook.buck.core.model.targetgraph.TargetNode,com.facebook.buck.apple.toolchain.AppleCxxPlatform,com.facebook.buck.apple.AppleBuildRules.RecursiveDependenciesMode,java.util.function.Predicate)}

        -   #### collectResourceDirsAndFiles

            ``` methodSignature
            public static <T extends ConstructorArg> AppleBundleResources collectResourceDirsAndFiles​(XCodeDescriptions xcodeDescriptions,
                                                                                                      TargetGraph targetGraph,
                                                                                                      BuildRuleResolver resolver,
                                                                                                      Optional<AppleDependenciesCache> cache,
                                                                                                      TargetNode<T> targetNode,
                                                                                                      AppleCxxPlatform appleCxxPlatform,
                                                                                                      AppleBuildRules.RecursiveDependenciesMode mode,
                                                                                                      java.util.function.Predicate<BuildTarget> filter)
            ```

            ::: block
            Collect resource dirs and files
            :::

        []{#collectDirectResources(com.facebook.buck.core.model.targetgraph.TargetGraph,com.facebook.buck.core.model.targetgraph.TargetNode)}

        -   #### collectDirectResources

            ``` methodSignature
            public static com.google.common.collect.ImmutableSet<AppleResourceDescriptionArg> collectDirectResources​(TargetGraph targetGraph,
                                                                                                                     TargetNode<?> targetNode)
            ```
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
-   [Field](#field.summary) \| 
-   Constr \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
-   Constr \| 
-   [Method](#method.detail)

</div>

[]{#skip.navbar.bottom}
:::
