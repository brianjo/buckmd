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

-   [Overview](../../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../index-all.html)
-   [Help](../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../allclasses.html)

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
[Package]{.packageLabelInType} [com.facebook.buck.core.model.targetgraph.impl](package-summary.html)
:::

## Class ImmutableUnconfiguredTargetNode {#class-immutableunconfiguredtargetnode .title title="Class ImmutableUnconfiguredTargetNode"}
:::

::: contentContainer
-   [java.lang.Object](http://docs.oracle.com/javase/7/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang"){.externalLink}

-   -   com.facebook.buck.core.model.targetgraph.impl.ImmutableUnconfiguredTargetNode

::: description
-   

    All Implemented Interfaces:
    :   `ComputeResult`, `UnconfiguredTargetNode`

    ------------------------------------------------------------------------

        public abstract class ImmutableUnconfiguredTargetNode
        extends Object
        implements UnconfiguredTargetNode

    ::: block
    Immutable implementation of
    [`UnconfiguredTargetNode`](../raw/UnconfiguredTargetNode.html "interface in com.facebook.buck.core.model.targetgraph.raw").
    :::
:::

::: summary
-   ::: {.section role="region"}
    -   []{#constructor.summary}

        ### Constructor Summary

          Constructor                           Description
          ------------------------------------- -------------
          `ImmutableUnconfiguredTargetNode()`    

          : Constructors[ ]{.tabEnd}
    :::

    ::: {.section role="region"}
    -   []{#method.summary}

        ### Method Summary

        +-----------------------+-----------------------+-----------------------+
        | Modifier and Type     | Method                | Description           |
        +=======================+=======================+=======================+
        | `                     | `getAttributes()`     | ::: block             |
        | abstract com.google.c |                       | Attributes of this    |
        | ommon.collect.Immutab |                       | node coerced to the   |
        | leMap<String,​Object>` |                       | types declared in     |
        |                       |                       | constructor           |
        |                       |                       | arguments.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `abstract Unc         | `getBuildTarget()`    | ::: block             |
        | onfiguredBuildTarget` |                       | Build target of this  |
        |                       |                       | node.                 |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `abstract co          | `getCompatibleWith()` | ::: block             |
        | m.google.common.colle |                       | List of targets from  |
        | ct.ImmutableList<Unco |                       | `compatible_with`     |
        | nfiguredBuildTarget>` |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `a                    | `getDef               | ::: block             |
        | bstract Optional<Unco | aultTargetPlatform()` | Value of              |
        | nfiguredBuildTarget>` |                       | `def                  |
        |                       |                       | ault_target_platform` |
        |                       |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `abstract RuleType`   | `getRuleType()`       | ::: block             |
        |                       |                       | The type of a rule.   |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `abst                 | `get                  | ::: block             |
        | ract com.google.commo | VisibilityPatterns()` | List of patterns from |
        | n.collect.ImmutableSe |                       | `visibility`          |
        | t<VisibilityPattern>` |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `abst                 | `get                  | ::: block             |
        | ract com.google.commo | WithinViewPatterns()` | List of patterns from |
        | n.collect.ImmutableSe |                       | `within_view`         |
        | t<VisibilityPattern>` |                       | attribute.            |
        |                       |                       | :::                   |
        +-----------------------+-----------------------+-----------------------+
        | `static Un            | `of​(Unconfig          |                       |
        | configuredTargetNode` | uredBuildTarget build |                       |
        |                       | Target,   RuleType ru |                       |
        |                       | leType,   com.google. |                       |
        |                       | common.collect.Immuta |                       |
        |                       | bleMap<String,​Object> |                       |
        |                       |  attributes,   com.go |                       |
        |                       | ogle.common.collect.I |                       |
        |                       | mmutableSet<Visibilit |                       |
        |                       | yPattern> visibilityP |                       |
        |                       | atterns,   com.google |                       |
        |                       | .common.collect.Immut |                       |
        |                       | ableSet<VisibilityPat |                       |
        |                       | tern> withinViewPatte |                       |
        |                       | rns,   Optional<Uncon |                       |
        |                       | figuredBuildTarget> d |                       |
        |                       | efaultTargetPlatform, |                       |
        |                       |    com.google.common. |                       |
        |                       | collect.ImmutableList |                       |
        |                       | <UnconfiguredBuildTar |                       |
        |                       | get> compatibleWith)` |                       |
        +-----------------------+-----------------------+-----------------------+

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

        -   #### ImmutableUnconfiguredTargetNode

                public ImmutableUnconfiguredTargetNode()
    :::

    ::: {.section role="region"}
    -   []{#method.detail}

        ### Method Detail

        []{#getBuildTarget()}

        -   #### getBuildTarget

            ``` methodSignature
            public abstract UnconfiguredBuildTarget getBuildTarget()
            ```

            ::: block
            [Description copied from
            interface: `UnconfiguredTargetNode`]{.descfrmTypeLabel}
            :::

            ::: block
            Build target of this node.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getBuildTarget` in interface `UnconfiguredTargetNode`

        []{#getRuleType()}

        -   #### getRuleType

            ``` methodSignature
            public abstract RuleType getRuleType()
            ```

            ::: block
            [Description copied from
            interface: `UnconfiguredTargetNode`]{.descfrmTypeLabel}
            :::

            ::: block
            The type of a rule.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getRuleType` in interface `UnconfiguredTargetNode`

        []{#getAttributes()}

        -   #### getAttributes

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableMap<String,​Object> getAttributes()
            ```

            ::: block
            [Description copied from
            interface: `UnconfiguredTargetNode`]{.descfrmTypeLabel}
            :::

            ::: block
            Attributes of this node coerced to the types declared in
            constructor arguments.
            Note that some of these attributes may require additional
            processing before they can be stored in a constructor
            argument. For example, selectable arguments need to be
            resolved first.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getAttributes` in interface `UnconfiguredTargetNode`

        []{#getVisibilityPatterns()}

        -   #### getVisibilityPatterns

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableSet<VisibilityPattern> getVisibilityPatterns()
            ```

            ::: block
            [Description copied from
            interface: `UnconfiguredTargetNode`]{.descfrmTypeLabel}
            :::

            ::: block
            List of patterns from `visibility` attribute.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getVisibilityPatterns` in
                interface `UnconfiguredTargetNode`

        []{#getWithinViewPatterns()}

        -   #### getWithinViewPatterns

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableSet<VisibilityPattern> getWithinViewPatterns()
            ```

            ::: block
            [Description copied from
            interface: `UnconfiguredTargetNode`]{.descfrmTypeLabel}
            :::

            ::: block
            List of patterns from `within_view` attribute.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getWithinViewPatterns` in
                interface `UnconfiguredTargetNode`

        []{#getDefaultTargetPlatform()}

        -   #### getDefaultTargetPlatform

            ``` methodSignature
            public abstract Optional<UnconfiguredBuildTarget> getDefaultTargetPlatform()
            ```

            ::: block
            [Description copied from
            interface: `UnconfiguredTargetNode`]{.descfrmTypeLabel}
            :::

            ::: block
            Value of `default_target_platform` attribute. Note this
            attribute only exists for build targets.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getDefaultTargetPlatform` in
                interface `UnconfiguredTargetNode`

        []{#getCompatibleWith()}

        -   #### getCompatibleWith

            ``` methodSignature
            public abstract com.google.common.collect.ImmutableList<UnconfiguredBuildTarget> getCompatibleWith()
            ```

            ::: block
            [Description copied from
            interface: `UnconfiguredTargetNode`]{.descfrmTypeLabel}
            :::

            ::: block
            List of targets from `compatible_with` attribute. Note
            method exists for all rules, while `compatible_with` can be
            defined only for build rules.
            :::

            [Specified by:]{.overrideSpecifyLabel}
            :   `getCompatibleWith` in
                interface `UnconfiguredTargetNode`

        []{#of(com.facebook.buck.core.model.UnconfiguredBuildTarget,com.facebook.buck.core.model.RuleType,com.google.common.collect.ImmutableMap,com.google.common.collect.ImmutableSet,com.google.common.collect.ImmutableSet,java.util.Optional,com.google.common.collect.ImmutableList)}

        -   #### of

            ``` methodSignature
            public static UnconfiguredTargetNode of​(UnconfiguredBuildTarget buildTarget,
                                                    RuleType ruleType,
                                                    com.google.common.collect.ImmutableMap<String,​Object> attributes,
                                                    com.google.common.collect.ImmutableSet<VisibilityPattern> visibilityPatterns,
                                                    com.google.common.collect.ImmutableSet<VisibilityPattern> withinViewPatterns,
                                                    Optional<UnconfiguredBuildTarget> defaultTargetPlatform,
                                                    com.google.common.collect.ImmutableList<UnconfiguredBuildTarget> compatibleWith)
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

-   [Overview](../../../../../../../index.html)
-   [Package](package-summary.html)
-   Class
-   [Tree](package-tree.html)
-   [Deprecated](../../../../../../../deprecated-list.html)
-   [Index](../../../../../../../index-all.html)
-   [Help](../../../../../../../help-doc.html)
:::

::: subNav
-   [All Classes](../../../../../../../allclasses.html)

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
