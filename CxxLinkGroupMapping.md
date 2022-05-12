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
[Package]{.packageLabelInType} [com.facebook.buck.core.linkgroup](package-summary.html)
:::

## Class CxxLinkGroupMapping {#class-cxxlinkgroupmapping .title title="Class CxxLinkGroupMapping"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.linkgroup.CxxLinkGroupMapping

::: description
-   

    All Implemented Interfaces:
    :   `Comparable<CxxLinkGroupMapping>`

    ------------------------------------------------------------------------

        public abstract class CxxLinkGroupMapping
        extends Object
        implements Comparable<CxxLinkGroupMapping>

    ::: block
    Represents a single mapping which specifies which targets belong to
    a link group.
    When used in BUCK files, it would be expressed as:

           link_group_map = [
             ("group_name", [mapping1, mapping2]),
           ],
         

    In this case,
    [`CxxLinkGroupMapping`](CxxLinkGroupMapping.html "class in com.facebook.buck.core.linkgroup")
    represents the tuple `  ("group_name", [mapping1, mapping2])`. Each
    mapping (e.g., `mapping1`) is represented by
    [`CxxLinkGroupMappingTarget`](CxxLinkGroupMappingTarget.html "class in com.facebook.buck.core.linkgroup").
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor               Description
          ------------------------- -------------
          `CxxLinkGroupMapping()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

          Modifier and Type                                                               Method                                                                                                        Description
          ------------------------------------------------------------------------------- ------------------------------------------------------------------------------------------------------------- -------------
          `int`                                                                           `compareTo​(CxxLinkGroupMapping that)`                                                                          
          `abstract String`                                                               `getLinkGroup()`                                                                                               
          `abstract com.google.common.collect.ImmutableList<CxxLinkGroupMappingTarget>`   `getMappingTargets()`                                                                                          
          `static CxxLinkGroupMapping`                                                    `of​(String linkGroup,   com.google.common.collect.ImmutableList<CxxLinkGroupMappingTarget> mappingTargets)`    

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

        -   #### CxxLinkGroupMapping

                public CxxLinkGroupMapping()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getLinkGroup()}

        -   #### getLinkGroup

            ``` methodSignature
            public abstract String getLinkGroup()
            ```

        []{#getMappingTargets()}

        -   #### getMappingTargets

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableList<CxxLinkGroupMappingTarget> getMappingTargets()
            ```

        []{#of(java.lang.String,com.google.common.collect.ImmutableList)}

        -   #### of

            ``` methodSignature
            public static CxxLinkGroupMapping of​(String linkGroup,
                                                 com.google.common.collect.ImmutableList<CxxLinkGroupMappingTarget> mappingTargets)
            ```

        []{#compareTo(com.facebook.buck.core.linkgroup.CxxLinkGroupMapping)}

        -   #### compareTo

            ``` methodSignature
            public int compareTo​(CxxLinkGroupMapping that)
            ```

            [Specified by:]{.overrideSpecifyLabel}
            :   `compareTo` in
                interface `Comparable<CxxLinkGroupMapping>`
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