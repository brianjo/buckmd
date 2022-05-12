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
[Package]{.packageLabelInType} [com.facebook.buck.core.linkgroup](package-summary.html)
:::

## Class CxxLinkGroupMappingTarget {#class-cxxlinkgroupmappingtarget .title title="Class CxxLinkGroupMappingTarget"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.linkgroup.CxxLinkGroupMappingTarget

::: description
-   

    All Implemented Interfaces:
    :   `Comparable<CxxLinkGroupMappingTarget>`

    ------------------------------------------------------------------------

        public abstract class CxxLinkGroupMappingTarget
        extends Object
        implements Comparable<CxxLinkGroupMappingTarget>

    ::: block
    Represents how a single build target should be mapped to a link
    group.
    When used in BUCK files, it would be expressed as:

           link_group_map = [
             ("...", [("//Some:Target", "tree")]),
           ],
         

    In this case,
    [`CxxLinkGroupMappingTarget`](CxxLinkGroupMappingTarget.html "class in com.facebook.buck.core.linkgroup")
    represents the tuple `  ("//Some:Target", "tree")`.
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#nested.class.summary}

        ### Nested Class Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Class                 | Description           |
        +=======================+=======================+=======================+
        | `static class `       | `CxxLinkGroupMap      | ::: block             |
        |                       | pingTarget.Traversal` | Defines how nodes     |
        |                       |                       | should be included    |
        |                       |                       | starting from the     |
        |                       |                       | root as specified by  |
        |                       |                       | the build target.     |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+

        : Nested Classes[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                     Description
          ------------------------------- -------------
          `CxxLinkGroupMappingTarget()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                Method                                                                                                                       Description
          ------------------------------------------------ ---------------------------------------------------------------------------------------------------------------------------- -------------
          `int`                                            `compareTo​(CxxLinkGroupMappingTarget that)`                                                                                   
          `abstract BuildTarget`                           `getBuildTarget()`                                                                                                            
          `abstract Optional<Pattern>`                     `getLabelPattern()`                                                                                                           
          `abstract CxxLinkGroupMappingTarget.Traversal`   `getTraversal()`                                                                                                              
          `static CxxLinkGroupMappingTarget`               `of​(BuildTarget buildTarget,   CxxLinkGroupMappingTarget.Traversal traversal,   Optional<? extends Pattern> labelPattern)`    

          : [All Methods[ ]{.tabEnd}]{#t0 .activeTableTab}[[Static
          Methods](javascript:show(1);)[ ]{.tabEnd}]{#t1
          .tableTab}[[Instance
          Methods](javascript:show(2);)[ ]{.tabEnd}]{#t2
          .tableTab}[[Abstract
          Methods](javascript:show(4);)[ ]{.tabEnd}]{#t3
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

        []{#<init>()}

        -   #### CxxLinkGroupMappingTarget

                public CxxLinkGroupMappingTarget()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getBuildTarget()}

        -   #### getBuildTarget

            ``` methodSignature
            public abstract BuildTarget getBuildTarget()
            ```

        []{#getTraversal()}

        -   #### getTraversal

            ``` methodSignature
            public abstract CxxLinkGroupMappingTarget.Traversal getTraversal()
            ```

        []{#getLabelPattern()}

        -   #### getLabelPattern

            ``` methodSignature
            public abstract Optional<Pattern> getLabelPattern()
            ```

        []{#of(com.facebook.buck.core.model.BuildTarget,com.facebook.buck.core.linkgroup.CxxLinkGroupMappingTarget.Traversal,java.util.Optional)}

        -   #### of

            ``` methodSignature
            public static CxxLinkGroupMappingTarget of​(BuildTarget buildTarget,
                                                       CxxLinkGroupMappingTarget.Traversal traversal,
                                                       Optional<? extends Pattern> labelPattern)
            ```

        []{#compareTo(com.facebook.buck.core.linkgroup.CxxLinkGroupMappingTarget)}

        -   #### compareTo

            ``` methodSignature
            public int compareTo​(CxxLinkGroupMappingTarget that)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `compareTo` in
                interface `Comparable<CxxLinkGroupMappingTarget>`
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
