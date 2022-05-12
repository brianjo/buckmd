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
-   Nested \| 
-   [Field](#field.summary) \| 
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
-   [Constr](#constructor.detail) \| 
-   Method

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
[Package]{.packageLabelInType} [com.facebook.buck.features.apple.projectV2](package-summary.html)
:::

## Class XcodeNativeTargetGenerator.Result {#class-xcodenativetargetgenerator.result .title title="Class XcodeNativeTargetGenerator.Result"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.features.apple.projectV2.XcodeNativeTargetGenerator.Result

::: description
-   

    Enclosing class:
    :   [XcodeNativeTargetGenerator](XcodeNativeTargetGenerator.html "class in com.facebook.buck.features.apple.projectV2")

    ------------------------------------------------------------------------

        public static class XcodeNativeTargetGenerator.Result
        extends Object

    ::: block
    The result of materializing the build target.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#field.summary}

        ### Field Summary

          Modifier and Type                                                                   Field                          Description
          ----------------------------------------------------------------------------------- ------------------------------ -------------
          `com.google.common.collect.ImmutableList<BuildTarget>`                              `dependencies`                  
          `Optional<com.facebook.buck.features.apple.projectV2.HeaderSearchPathAttributes>`   `headerSearchPathAttributes`    
          `com.google.common.collect.ImmutableSet<BuildTarget>`                               `requiredBuildTargets`          
          `com.facebook.buck.features.apple.projectV2.XCodeNativeTargetAttributes`            `targetAttributes`              
          `com.google.common.collect.ImmutableSet<String>`                                    `targetConfigNames`             
          `TargetNode<?>`                                                                     `targetNode`                    
          `com.google.common.collect.ImmutableSet<Path>`                                      `xcconfigPaths`                 

          : Fields[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              Description
          -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- -------------
          `Result​(TargetNode<?> targetNode,       com.facebook.buck.features.apple.projectV2.XCodeNativeTargetAttributes targetAttributes)`                                                                                                                                                                                                                                                                                                                                                                                                                         
          `Result​(TargetNode<?> targetNode,       com.facebook.buck.features.apple.projectV2.XCodeNativeTargetAttributes targetAttributes,       com.google.common.collect.ImmutableList<BuildTarget> dependencies,       com.google.common.collect.ImmutableSet<BuildTarget> requiredBuildTargets,       com.google.common.collect.ImmutableSet<Path> xcconfigPaths,       com.google.common.collect.ImmutableSet<String> targetConfigNames,       Optional<com.facebook.buck.features.apple.projectV2.HeaderSearchPathAttributes> headerSearchPathAttributes)`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        -   []{#methods.inherited.from.class.java.lang.Object}

            ### Methods inherited from class java.lang.[Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

            `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`
    :::
:::

::: details
-   ::: {.section role="region"}
    -   []{#field.detail}

        ### Field Detail

        []{#targetNode}

        -   #### targetNode

                public final TargetNode<?> targetNode

        []{#targetAttributes}

        -   #### targetAttributes

                public final com.facebook.buck.features.apple.projectV2.XCodeNativeTargetAttributes targetAttributes

        []{#dependencies}

        -   #### dependencies

                public final com.google.common.collect.ImmutableList<BuildTarget> dependencies

        []{#requiredBuildTargets}

        -   #### requiredBuildTargets

                public final com.google.common.collect.ImmutableSet<BuildTarget> requiredBuildTargets

        []{#xcconfigPaths}

        -   #### xcconfigPaths

                public final com.google.common.collect.ImmutableSet<Path> xcconfigPaths

        []{#targetConfigNames}

        -   #### targetConfigNames

                public final com.google.common.collect.ImmutableSet<String> targetConfigNames

        []{#headerSearchPathAttributes}

        -   #### headerSearchPathAttributes

                public final Optional<com.facebook.buck.features.apple.projectV2.HeaderSearchPathAttributes> headerSearchPathAttributes
    :::

    ::: {.section role="region"}
    -   []{#constructor.detail}

        ### Constructor Detail

        []{#<init>(com.facebook.buck.core.model.targetgraph.TargetNode,com.facebook.buck.features.apple.projectV2.XCodeNativeTargetAttributes)}

        -   #### Result

                public Result​(TargetNode<?> targetNode,
                              com.facebook.buck.features.apple.projectV2.XCodeNativeTargetAttributes targetAttributes)

        []{#<init>(com.facebook.buck.core.model.targetgraph.TargetNode,com.facebook.buck.features.apple.projectV2.XCodeNativeTargetAttributes,com.google.common.collect.ImmutableList,com.google.common.collect.ImmutableSet,com.google.common.collect.ImmutableSet,com.google.common.collect.ImmutableSet,java.util.Optional)}

        -   #### Result

                public Result​(TargetNode<?> targetNode,
                              com.facebook.buck.features.apple.projectV2.XCodeNativeTargetAttributes targetAttributes,
                              com.google.common.collect.ImmutableList<BuildTarget> dependencies,
                              com.google.common.collect.ImmutableSet<BuildTarget> requiredBuildTargets,
                              com.google.common.collect.ImmutableSet<Path> xcconfigPaths,
                              com.google.common.collect.ImmutableSet<String> targetConfigNames,
                              Optional<com.facebook.buck.features.apple.projectV2.HeaderSearchPathAttributes> headerSearchPathAttributes)
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
-   Nested \| 
-   [Field](#field.summary) \| 
-   [Constr](#constructor.summary) \| 
-   [Method](#method.summary)

```{=html}
<!-- -->
```
-   Detail: 
-   [Field](#field.detail) \| 
-   [Constr](#constructor.detail) \| 
-   Method

</div>

[]{#skip.navbar.bottom}
:::
